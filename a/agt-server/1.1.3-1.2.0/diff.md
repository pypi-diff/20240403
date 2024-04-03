# Comparing `tmp/agt_server-1.1.3.tar.gz` & `tmp/agt_server-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agt_server-1.1.3.tar", last modified: Sun Mar  3 06:22:45 2024, max compression
+gzip compressed data, was "agt_server-1.2.0.tar", last modified: Wed Apr  3 02:46:09 2024, max compression
```

## Comparing `agt_server-1.1.3.tar` & `agt_server-1.2.0.tar`

### file list

```diff
@@ -1,415 +1,445 @@
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.834685 agt_server-1.1.3/
--rw-r--r--   0 johnwu     (501) staff       (20)     3537 2024-01-25 22:07:40.000000 agt_server-1.1.3/.gitignore
--rw-r--r--   0 johnwu     (501) staff       (20)     1063 2024-01-17 14:08:17.000000 agt_server-1.1.3/LICENSE
--rw-r--r--   0 johnwu     (501) staff       (20)       66 2024-01-25 21:21:35.000000 agt_server-1.1.3/MANIFEST.in
--rw-r--r--   0 johnwu     (501) staff       (20)     6482 2024-03-03 06:22:45.834529 agt_server-1.1.3/PKG-INFO
--rw-r--r--   0 johnwu     (501) staff       (20)     5853 2024-02-06 19:53:48.000000 agt_server-1.1.3/README.md
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.746002 agt_server-1.1.3/data/
--rw-r--r--   0 johnwu     (501) staff       (20)    80155 2024-01-23 17:19:42.000000 agt_server-1.1.3/data/profile.svg
--rw-r--r--   0 johnwu     (501) staff       (20)       49 2024-02-08 21:55:59.000000 agt_server-1.1.3/requirements.txt
--rw-r--r--   0 johnwu     (501) staff       (20)       38 2024-03-03 06:22:45.834739 agt_server-1.1.3/setup.cfg
--rw-r--r--   0 johnwu     (501) staff       (20)     1175 2024-03-03 06:22:38.000000 agt_server-1.1.3/setup.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.747464 agt_server-1.1.3/src/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:10.000000 agt_server-1.1.3/src/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.747568 agt_server-1.1.3/src/agt_server/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:24.000000 agt_server-1.1.3/src/agt_server/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.748453 agt_server-1.1.3/src/agt_server/agents/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.1.3/src/agt_server/agents/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.751218 agt_server-1.1.3/src/agt_server/agents/base_agents/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.1.3/src/agt_server/agents/base_agents/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     2137 2024-02-26 02:01:12.000000 agt_server-1.1.3/src/agt_server/agents/base_agents/agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1917 2024-02-26 02:01:22.000000 agt_server-1.1.3/src/agt_server/agents/base_agents/bos_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     8115 2024-02-26 02:01:35.000000 agt_server-1.1.3/src/agt_server/agents/base_agents/bosii_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1875 2024-02-26 02:01:43.000000 agt_server-1.1.3/src/agt_server/agents/base_agents/chicken_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     6043 2024-02-10 11:47:44.000000 agt_server-1.1.3/src/agt_server/agents/base_agents/cm_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3916 2024-02-15 16:06:43.000000 agt_server-1.1.3/src/agt_server/agents/base_agents/game_report.py
--rw-r--r--   0 johnwu     (501) staff       (20)     9938 2024-02-26 02:02:11.000000 agt_server-1.1.3/src/agt_server/agents/base_agents/lemonade_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1969 2024-02-26 02:02:18.000000 agt_server-1.1.3/src/agt_server/agents/base_agents/rps_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.751577 agt_server-1.1.3/src/agt_server/agents/test_agents/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.736307 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.751840 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/always_compromise/
--rw-r--r--   0 johnwu     (501) staff       (20)     1636 2024-01-25 21:04:23.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.752217 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/always_stubborn/
--rw-r--r--   0 johnwu     (501) staff       (20)     1600 2024-01-25 21:04:29.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.752471 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/anti_punitive/
--rw-r--r--   0 johnwu     (501) staff       (20)     1755 2024-01-25 21:04:34.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.752792 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/fishing_chip/
--rw-r--r--   0 johnwu     (501) staff       (20)     1996 2024-01-25 21:04:39.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.753018 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/punitive_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2211 2024-01-25 21:04:43.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.753451 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1618 2024-01-25 21:04:48.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.753716 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/reluctant_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1985 2024-01-25 21:04:54.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.753884 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1541 2024-01-25 21:05:00.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.754045 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:05:04.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.754193 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1586 2024-01-25 21:05:08.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.754410 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:05:13.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.754577 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1575 2024-01-25 21:05:17.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.754798 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1591 2024-01-25 21:05:22.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.737905 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.754949 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/always_compromise/
--rw-r--r--   0 johnwu     (501) staff       (20)     1679 2024-01-25 21:05:44.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.755236 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/always_stubborn/
--rw-r--r--   0 johnwu     (501) staff       (20)     1658 2024-01-25 21:05:47.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.755466 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/anti_punitive/
--rw-r--r--   0 johnwu     (501) staff       (20)     1813 2024-01-25 21:05:53.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.755745 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/chipping_fish/
--rw-r--r--   0 johnwu     (501) staff       (20)     3915 2024-01-25 21:05:57.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.755887 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/exponential/
--rw-r--r--   0 johnwu     (501) staff       (20)     4518 2024-01-25 21:06:03.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.756145 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/ficticious_play/
--rw-r--r--   0 johnwu     (501) staff       (20)     4667 2024-01-25 21:06:09.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.756518 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/fishing_chip/
--rw-r--r--   0 johnwu     (501) staff       (20)     2054 2024-01-25 21:06:13.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.756738 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/mystery/
--rw-r--r--   0 johnwu     (501) staff       (20)     3403 2024-01-25 21:06:17.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.757074 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/punitive_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2263 2024-01-30 22:46:02.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.757334 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2993 2024-01-25 21:06:27.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.757529 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1676 2024-01-25 21:06:31.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.757788 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/reluctant_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2041 2024-01-25 21:06:36.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.758046 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2474 2024-01-25 21:06:40.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.758306 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1604 2024-01-25 21:06:44.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.758595 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1628 2024-01-25 21:06:48.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.759060 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1649 2024-01-25 21:06:53.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.759209 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1632 2024-01-25 21:06:57.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.759369 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1693 2024-01-25 21:07:01.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.759522 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1654 2024-01-25 21:07:07.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.759674 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.759775 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/always_continue/
--rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:09:10.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.759996 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/always_swerve/
--rw-r--r--   0 johnwu     (501) staff       (20)     1605 2024-01-25 21:09:14.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.760532 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/basic_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:09:07.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/basic_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1708 2024-01-25 21:09:18.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.760719 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/exponential/
--rw-r--r--   0 johnwu     (501) staff       (20)     3331 2024-01-25 21:09:23.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.761029 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ficticious_play/
--rw-r--r--   0 johnwu     (501) staff       (20)     3252 2024-01-25 21:09:28.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.762819 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lastmove_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-05 15:59:43.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lastmove_chicken/i_fixed_policy.py
--rw-r--r--   0 johnwu     (501) staff       (20)     2890 2024-01-25 21:09:36.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:52.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py
--rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable_static.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-05 15:59:58.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lastmove_chicken/uniform_policy.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.764458 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lookback_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:24:35.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lookback_chicken/i_fixed_policy.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3075 2024-01-25 21:09:42.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:45:02.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py
--rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable_static.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:24:35.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lookback_chicken/uniform_policy.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.764798 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/mystery_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:17:17.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/mystery_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1993 2024-01-25 21:09:48.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.766300 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:30:36.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/i_fixed_policy.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3219 2024-01-25 21:09:54.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:25.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py
--rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:30:36.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/uniform_policy.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.766504 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1629 2024-01-25 21:09:59.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.766687 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:10:03.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.766988 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1587 2024-01-25 21:10:07.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.767171 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1612 2024-01-25 21:10:11.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.767347 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1648 2024-01-25 21:10:15.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.767521 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1521 2024-01-25 21:10:19.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.767803 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1613 2024-01-25 21:10:25.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.767986 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:41:39.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.768246 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/always_stay/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:09.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/always_stay/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-02-15 18:47:18.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.768546 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/best_respond_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-15 18:47:54.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.768841 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/circular_hotel/
--rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-15 18:48:36.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.769265 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/decrement_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:15.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/decrement_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-15 18:48:57.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.769564 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/del_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-15 18:49:07.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.769888 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/dumb_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)     1975 2024-02-15 18:49:21.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.770168 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     7288 2024-02-15 18:49:40.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.770438 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/etch_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     3073 2024-02-15 18:50:03.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.770721 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/eyes_out/
--rw-r--r--   0 johnwu     (501) staff       (20)     2418 2024-02-15 18:50:12.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.771009 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/good_bot/
--rw-r--r--   0 johnwu     (501) staff       (20)     2088 2024-02-15 18:50:23.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.771302 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/hi_bot/
--rw-r--r--   0 johnwu     (501) staff       (20)     2798 2024-02-15 18:50:37.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.771687 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/increment_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:22.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/increment_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1614 2024-02-15 18:50:57.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.771921 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/jimbus/
--rw-r--r--   0 johnwu     (501) staff       (20)     2284 2024-02-15 18:51:08.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.772184 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/kamen_rider/
--rw-r--r--   0 johnwu     (501) staff       (20)     2588 2024-02-15 18:51:19.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.772410 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/q_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     3798 2024-02-15 18:51:31.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.772664 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-02-15 18:51:42.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.772939 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/spinner/
--rw-r--r--   0 johnwu     (501) staff       (20)     2056 2024-02-15 18:51:51.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.773346 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1485 2024-02-15 18:52:13.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.773627 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1515 2024-02-15 18:52:23.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.773900 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:52:30.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.774278 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-15 18:52:44.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.774459 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1533 2024-02-15 18:52:57.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.774619 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1531 2024-02-15 18:53:11.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.775031 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/stick_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:20:02.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/stick_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:53:22.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.775209 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/sticky/
--rw-r--r--   0 johnwu     (501) staff       (20)     2441 2024-02-15 18:53:32.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.775378 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/team_player/
--rw-r--r--   0 johnwu     (501) staff       (20)     3659 2024-02-15 18:53:44.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.775672 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/zenly/
--rw-r--r--   0 johnwu     (501) staff       (20)     3045 2024-02-15 18:53:56.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.742025 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.775982 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/always_stay/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:10:52.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/always_stay/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-02-18 02:10:52.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.776202 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-18 02:11:06.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.776442 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/
--rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-18 02:11:20.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.776802 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:11:25.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-18 02:11:25.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.777007 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/del_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-22 06:12:46.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.777271 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-22 06:07:27.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.777543 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-22 06:12:45.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.777742 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.777864 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/exponential/
--rw-r--r--   0 johnwu     (501) staff       (20)     2954 2024-01-26 06:19:46.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/exponential/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.778111 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/ficticious_play/
--rw-r--r--   0 johnwu     (501) staff       (20)     3052 2024-01-26 05:13:48.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.778387 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1549 2024-01-25 21:15:25.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.778679 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/rock_lover/
--rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:32.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.779029 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1506 2024-01-25 21:15:38.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.779254 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:43.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.779695 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1543 2024-01-25 21:16:13.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.779937 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-01-25 21:16:18.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.780170 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1444 2024-01-25 22:02:30.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.780439 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1527 2024-01-25 21:16:28.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.780781 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/ta_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 22:14:36.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/ta_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1454 2024-01-25 21:16:33.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)      662 2023-05-31 04:43:31.000000 agt_server-1.1.3/src/agt_server/agents/test_agents/stress_test.txt
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.743176 agt_server-1.1.3/src/agt_server/configs/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.782394 agt_server-1.1.3/src/agt_server/configs/handin_configs/
--rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:28:03.000000 agt_server-1.1.3/src/agt_server/configs/handin_configs/bos_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      223 2024-02-22 04:27:55.000000 agt_server-1.1.3/src/agt_server/configs/handin_configs/bosii_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      231 2024-02-22 04:27:45.000000 agt_server-1.1.3/src/agt_server/configs/handin_configs/chicken_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      263 2024-03-02 19:44:48.000000 agt_server-1.1.3/src/agt_server/configs/handin_configs/lemonade_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:27:36.000000 agt_server-1.1.3/src/agt_server/configs/handin_configs/rps_config.json
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.783964 agt_server-1.1.3/src/agt_server/configs/server_configs/
--rw-r--r--   0 johnwu     (501) staff       (20)      603 2024-02-01 23:47:38.000000 agt_server-1.1.3/src/agt_server/configs/server_configs/bos_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      797 2024-02-06 00:46:41.000000 agt_server-1.1.3/src/agt_server/configs/server_configs/bosii_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      608 2024-02-15 16:14:51.000000 agt_server-1.1.3/src/agt_server/configs/server_configs/chicken_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      621 2024-01-30 21:38:03.000000 agt_server-1.1.3/src/agt_server/configs/server_configs/lemonade_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      604 2024-01-30 21:37:55.000000 agt_server-1.1.3/src/agt_server/configs/server_configs/rps_config.json
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.784279 agt_server-1.1.3/src/agt_server/handin/
--rw-r--r--   0 johnwu     (501) staff       (20)     3648 2024-03-01 00:46:20.000000 agt_server-1.1.3/src/agt_server/handin/handin.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.784788 agt_server-1.1.3/src/agt_server/handin/results/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:56.000000 agt_server-1.1.3/src/agt_server/handin/results/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.784900 agt_server-1.1.3/src/agt_server/handin/results/bos/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:49.000000 agt_server-1.1.3/src/agt_server/handin/results/bos/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.785018 agt_server-1.1.3/src/agt_server/handin/results/bosii/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:04.000000 agt_server-1.1.3/src/agt_server/handin/results/bosii/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.785130 agt_server-1.1.3/src/agt_server/handin/results/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:25.000000 agt_server-1.1.3/src/agt_server/handin/results/chicken/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.822242 agt_server-1.1.3/src/agt_server/handin/results/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)     2786 2024-02-22 23:10:32.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3094 2024-02-23 00:23:34.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3249 2024-02-26 03:46:11.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:12:09.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:13:49.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:14:53.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:21:10.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:23:39.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:25:31.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:26:34.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:27:17.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     1737 2024-02-26 04:27:28.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     1673 2024-02-26 04:27:55.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:28:23.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:31:07.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:32:45.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:33:29.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2631 2024-02-26 04:34:38.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2866 2024-02-26 04:55:11.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2759 2024-02-26 06:39:27.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-26 06:49:59.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2674 2024-02-26 06:59:09.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     9873 2024-02-26 23:17:30.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      526 2024-02-26 23:18:48.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2722 2024-02-26 23:36:33.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2784 2024-02-26 23:37:56.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2494 2024-02-26 23:38:30.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      219 2024-02-26 23:45:11.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-45-11_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:24.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-45-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:28.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-45-28_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:31.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-45-31_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:46:21.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-46-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3054 2024-02-26 23:47:10.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:47:41.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-47-41_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-26 23:50:39.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-50-38_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-26 23:58:51.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-58-51_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-27 00:09:44.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:09:46.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_19-09-46_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2416 2024-02-27 00:13:56.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2610 2024-02-27 00:14:32.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:19:21.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_19-19-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:21:53.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_19-21-53_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     4940 2024-02-27 20:26:21.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3215 2024-02-27 20:27:18.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     7406 2024-02-27 20:32:27.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3367 2024-02-27 20:33:47.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     7165 2024-02-27 20:36:53.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     6897 2024-02-27 20:40:29.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5795 2024-02-27 20:40:37.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     6689 2024-02-27 20:49:05.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    69971 2024-02-28 04:53:17.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    42190 2024-02-28 08:28:23.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    38084 2024-02-28 10:04:34.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    38027 2024-02-28 11:31:24.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5240 2024-02-28 11:34:41.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     1921 2024-02-28 11:35:40.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     8899 2024-02-28 11:42:21.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    39034 2024-02-28 14:22:14.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    74776 2024-02-28 19:14:37.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5920 2024-02-28 21:11:22.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5102 2024-02-28 21:13:24.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     4669 2024-02-28 21:16:32.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5107 2024-02-28 21:19:34.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    16781 2024-02-28 21:40:00.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    15945 2024-02-28 21:51:18.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    17789 2024-02-28 22:18:47.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    15831 2024-02-28 22:55:20.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3939 2024-03-01 00:34:13.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    14259 2024-03-01 00:45:25.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3812 2024-03-01 00:46:34.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3998 2024-03-01 00:48:27.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     6081 2024-03-01 01:51:10.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     9474 2024-03-01 01:52:08.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     8767 2024-03-01 01:52:36.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5900 2024-03-01 01:54:12.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    12641 2024-03-01 02:00:54.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    33503 2024-03-01 03:09:35.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    31050 2024-03-01 05:10:15.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    18142 2024-03-01 05:31:08.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    18785 2024-03-01 06:24:52.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    19642 2024-03-01 07:22:31.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3325 2024-03-01 07:22:31.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/LemonadeArena.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3900 2024-02-26 04:14:53.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/LemonadeTest.txt
--rw-r--r--   0 johnwu     (501) staff       (20)   785905 2024-03-01 23:54:21.000000 agt_server-1.1.3/src/agt_server/handin/results/lemonade/shortcut.json
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.824199 agt_server-1.1.3/src/agt_server/handin/results/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:14.000000 agt_server-1.1.3/src/agt_server/handin/results/rps/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.826125 agt_server-1.1.3/src/agt_server/local_games/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.1.3/src/agt_server/local_games/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     2318 2024-02-22 09:00:09.000000 agt_server-1.1.3/src/agt_server/local_games/base.py
--rw-r--r--   0 johnwu     (501) staff       (20)     9604 2024-02-15 18:16:30.000000 agt_server-1.1.3/src/agt_server/local_games/bos_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)    10213 2024-02-15 18:16:15.000000 agt_server-1.1.3/src/agt_server/local_games/bosii_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)     9731 2024-02-15 18:17:49.000000 agt_server-1.1.3/src/agt_server/local_games/chicken_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)    17963 2024-03-03 06:22:30.000000 agt_server-1.1.3/src/agt_server/local_games/lemonade_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)     9703 2024-02-15 18:17:04.000000 agt_server-1.1.3/src/agt_server/local_games/rps_arena.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.826496 agt_server-1.1.3/src/agt_server/server/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.1.3/src/agt_server/server/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.829138 agt_server-1.1.3/src/agt_server/server/games/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.1.3/src/agt_server/server/games/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      596 2024-01-31 02:48:39.000000 agt_server-1.1.3/src/agt_server/server/games/bos_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)    18510 2024-01-30 21:30:44.000000 agt_server-1.1.3/src/agt_server/server/games/bosii_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)      606 2024-01-25 21:17:28.000000 agt_server-1.1.3/src/agt_server/server/games/chicken_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)    16908 2024-01-30 21:34:09.000000 agt_server-1.1.3/src/agt_server/server/games/complete_2x2_matrix_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)      710 2024-01-23 13:08:08.000000 agt_server-1.1.3/src/agt_server/server/games/game.py
--rw-r--r--   0 johnwu     (501) staff       (20)    19180 2024-01-30 21:32:26.000000 agt_server-1.1.3/src/agt_server/server/games/lemonade_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)      671 2024-01-25 21:17:39.000000 agt_server-1.1.3/src/agt_server/server/games/rps_game.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.829376 agt_server-1.1.3/src/agt_server/server/results/
--rw-r--r--   0 johnwu     (501) staff       (20)       18 2024-01-25 18:51:20.000000 agt_server-1.1.3/src/agt_server/server/results/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.829981 agt_server-1.1.3/src/agt_server/server/results/bos/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:35.000000 agt_server-1.1.3/src/agt_server/server/results/bos/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.830273 agt_server-1.1.3/src/agt_server/server/results/bosii/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:39.000000 agt_server-1.1.3/src/agt_server/server/results/bosii/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.830382 agt_server-1.1.3/src/agt_server/server/results/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:43.000000 agt_server-1.1.3/src/agt_server/server/results/chicken/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.830482 agt_server-1.1.3/src/agt_server/server/results/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:49.000000 agt_server-1.1.3/src/agt_server/server/results/lemonade/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.830592 agt_server-1.1.3/src/agt_server/server/results/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:54.000000 agt_server-1.1.3/src/agt_server/server/results/rps/.gitkeep
--rw-r--r--   0 johnwu     (501) staff       (20)    23118 2024-02-15 16:20:24.000000 agt_server-1.1.3/src/agt_server/server/server.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.748314 agt_server-1.1.3/src/agt_server.egg-info/
--rw-r--r--   0 johnwu     (501) staff       (20)     6482 2024-03-03 06:22:45.000000 agt_server-1.1.3/src/agt_server.egg-info/PKG-INFO
--rw-r--r--   0 johnwu     (501) staff       (20)    16710 2024-03-03 06:22:45.000000 agt_server-1.1.3/src/agt_server.egg-info/SOURCES.txt
--rw-r--r--   0 johnwu     (501) staff       (20)        1 2024-03-03 06:22:45.000000 agt_server-1.1.3/src/agt_server.egg-info/dependency_links.txt
--rw-r--r--   0 johnwu     (501) staff       (20)       48 2024-03-03 06:22:45.000000 agt_server-1.1.3/src/agt_server.egg-info/requires.txt
--rw-r--r--   0 johnwu     (501) staff       (20)       11 2024-03-03 06:22:45.000000 agt_server-1.1.3/src/agt_server.egg-info/top_level.txt
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.744579 agt_server-1.1.3/test/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.744917 agt_server-1.1.3/test/server_test/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.831105 agt_server-1.1.3/test/server_test/bos/
--rw-r--r--   0 johnwu     (501) staff       (20)     7014 2024-01-25 21:24:06.000000 agt_server-1.1.3/test/server_test/bos/bos_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)     8015 2024-01-25 21:22:03.000000 agt_server-1.1.3/test/server_test/bos/bos_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.831884 agt_server-1.1.3/test/server_test/bosii/
--rw-r--r--   0 johnwu     (501) staff       (20)    10139 2024-01-25 21:26:19.000000 agt_server-1.1.3/test/server_test/bosii/bosii_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)    11361 2024-01-25 21:28:31.000000 agt_server-1.1.3/test/server_test/bosii/bosii_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.832545 agt_server-1.1.3/test/server_test/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)    10276 2024-01-25 21:35:28.000000 agt_server-1.1.3/test/server_test/chicken/chicken_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)    11631 2024-01-25 21:50:35.000000 agt_server-1.1.3/test/server_test/chicken/chicken_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.833419 agt_server-1.1.3/test/server_test/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)    13981 2024-01-25 21:53:38.000000 agt_server-1.1.3/test/server_test/lemonade/lemonade_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)     8108 2024-01-25 21:56:56.000000 agt_server-1.1.3/test/server_test/lemonade/lemonade_ql.sh
--rw-r--r--   0 johnwu     (501) staff       (20)    16031 2024-01-25 21:58:30.000000 agt_server-1.1.3/test/server_test/lemonade/lemonade_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-03-03 06:22:45.834055 agt_server-1.1.3/test/server_test/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)     5940 2024-01-25 22:00:19.000000 agt_server-1.1.3/test/server_test/rps/rps_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)     6884 2024-01-25 22:00:40.000000 agt_server-1.1.3/test/server_test/rps/rps_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.126889 agt_server-1.2.0/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3537 2024-01-25 22:07:40.000000 agt_server-1.2.0/.gitignore
+-rw-r--r--   0 johnwu     (501) staff       (20)     1063 2024-01-17 14:08:17.000000 agt_server-1.2.0/LICENSE
+-rw-r--r--   0 johnwu     (501) staff       (20)       66 2024-01-25 21:21:35.000000 agt_server-1.2.0/MANIFEST.in
+-rw-r--r--   0 johnwu     (501) staff       (20)     6482 2024-04-03 02:46:09.126745 agt_server-1.2.0/PKG-INFO
+-rw-r--r--   0 johnwu     (501) staff       (20)     5853 2024-02-06 19:53:48.000000 agt_server-1.2.0/README.md
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.076227 agt_server-1.2.0/data/
+-rw-r--r--   0 johnwu     (501) staff       (20)    80155 2024-01-23 17:19:42.000000 agt_server-1.2.0/data/profile.svg
+-rw-r--r--   0 johnwu     (501) staff       (20)       56 2024-04-03 02:45:51.000000 agt_server-1.2.0/requirements.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)       38 2024-04-03 02:46:09.126952 agt_server-1.2.0/setup.cfg
+-rw-r--r--   0 johnwu     (501) staff       (20)     1175 2024-04-03 02:45:59.000000 agt_server-1.2.0/setup.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.076505 agt_server-1.2.0/src/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:10.000000 agt_server-1.2.0/src/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.076665 agt_server-1.2.0/src/agt_server/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:24.000000 agt_server-1.2.0/src/agt_server/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.077597 agt_server-1.2.0/src/agt_server/agents/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.2.0/src/agt_server/agents/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.078930 agt_server-1.2.0/src/agt_server/agents/base_agents/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.2.0/src/agt_server/agents/base_agents/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     2137 2024-02-26 02:01:12.000000 agt_server-1.2.0/src/agt_server/agents/base_agents/agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1917 2024-02-26 02:01:22.000000 agt_server-1.2.0/src/agt_server/agents/base_agents/bos_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     8115 2024-02-26 02:01:35.000000 agt_server-1.2.0/src/agt_server/agents/base_agents/bosii_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1875 2024-02-26 02:01:43.000000 agt_server-1.2.0/src/agt_server/agents/base_agents/chicken_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     6043 2024-02-10 11:47:44.000000 agt_server-1.2.0/src/agt_server/agents/base_agents/cm_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3916 2024-02-15 16:06:43.000000 agt_server-1.2.0/src/agt_server/agents/base_agents/game_report.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    10046 2024-03-31 16:34:04.000000 agt_server-1.2.0/src/agt_server/agents/base_agents/lemonade_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    13055 2024-04-02 19:29:35.000000 agt_server-1.2.0/src/agt_server/agents/base_agents/lsvm_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1969 2024-02-26 02:02:18.000000 agt_server-1.2.0/src/agt_server/agents/base_agents/rps_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.079156 agt_server-1.2.0/src/agt_server/agents/test_agents/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.060270 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.082516 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/always_compromise/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1636 2024-01-25 21:04:23.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.082701 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/always_stubborn/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1600 2024-01-25 21:04:29.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.082864 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/anti_punitive/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1755 2024-01-25 21:04:34.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.083010 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/fishing_chip/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1996 2024-01-25 21:04:39.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.083156 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/punitive_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2211 2024-01-25 21:04:43.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.083301 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1618 2024-01-25 21:04:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.083439 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/reluctant_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1985 2024-01-25 21:04:54.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.083576 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1541 2024-01-25 21:05:00.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.083712 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:05:04.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.083846 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1586 2024-01-25 21:05:08.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.083984 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:05:13.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.084130 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1575 2024-01-25 21:05:17.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.084262 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1591 2024-01-25 21:05:22.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.061786 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.084411 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/always_compromise/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1679 2024-01-25 21:05:44.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.084562 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/always_stubborn/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1658 2024-01-25 21:05:47.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.084697 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/anti_punitive/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1813 2024-01-25 21:05:53.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.084832 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/chipping_fish/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3915 2024-01-25 21:05:57.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.084971 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/exponential/
+-rw-r--r--   0 johnwu     (501) staff       (20)     4518 2024-01-25 21:06:03.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.085095 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/ficticious_play/
+-rw-r--r--   0 johnwu     (501) staff       (20)     4667 2024-01-25 21:06:09.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.085225 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/fishing_chip/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2054 2024-01-25 21:06:13.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.085370 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/mystery/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3403 2024-01-25 21:06:17.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.085503 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/punitive_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2263 2024-01-30 22:46:02.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.085648 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2993 2024-01-25 21:06:27.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.085790 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1676 2024-01-25 21:06:31.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.085931 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/reluctant_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2041 2024-01-25 21:06:36.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.086064 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2474 2024-01-25 21:06:40.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.086205 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1604 2024-01-25 21:06:44.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.086337 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1628 2024-01-25 21:06:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.086471 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1649 2024-01-25 21:06:53.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.086607 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1632 2024-01-25 21:06:57.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.086763 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1693 2024-01-25 21:07:01.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.086985 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1654 2024-01-25 21:07:07.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.087134 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.087242 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/always_continue/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:09:10.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.087435 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/always_swerve/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1605 2024-01-25 21:09:14.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.087749 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/basic_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:09:07.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/basic_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1708 2024-01-25 21:09:18.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.087924 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/exponential/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3331 2024-01-25 21:09:23.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.088081 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ficticious_play/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3252 2024-01-25 21:09:28.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.089058 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lastmove_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-05 15:59:43.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lastmove_chicken/i_fixed_policy.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     2890 2024-01-25 21:09:36.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:52.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable_static.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-05 15:59:58.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lastmove_chicken/uniform_policy.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.089975 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lookback_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:24:35.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lookback_chicken/i_fixed_policy.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3075 2024-01-25 21:09:42.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:45:02.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable_static.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:24:35.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lookback_chicken/uniform_policy.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.090283 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/mystery_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:17:17.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/mystery_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1993 2024-01-25 21:09:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.091305 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:30:36.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/i_fixed_policy.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3219 2024-01-25 21:09:54.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:25.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:30:36.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/uniform_policy.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.091492 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1629 2024-01-25 21:09:59.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.091693 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:10:03.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.091863 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1587 2024-01-25 21:10:07.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.092025 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1612 2024-01-25 21:10:11.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.092192 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1648 2024-01-25 21:10:15.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.092370 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1521 2024-01-25 21:10:19.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.092537 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1613 2024-01-25 21:10:25.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.092699 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:41:39.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.092959 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/always_stay/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:09.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/always_stay/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-02-15 18:47:18.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.093139 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/best_respond_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-15 18:47:54.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.093313 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/circular_hotel/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-15 18:48:36.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.093616 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/decrement_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:15.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/decrement_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-15 18:48:57.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.093798 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/del_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-15 18:49:07.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.093976 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/dumb_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1975 2024-02-15 18:49:21.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.094133 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     7288 2024-02-15 18:49:40.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.094300 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/etch_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3073 2024-02-15 18:50:03.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.094483 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/eyes_out/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2418 2024-02-15 18:50:12.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.094653 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/good_bot/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2088 2024-02-15 18:50:23.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.094821 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/hi_bot/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2798 2024-02-15 18:50:37.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.095106 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/increment_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:22.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/increment_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1614 2024-02-15 18:50:57.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.095252 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/jimbus/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2284 2024-02-15 18:51:08.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.095418 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/kamen_rider/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2588 2024-02-15 18:51:19.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.095596 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/q_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3798 2024-02-15 18:51:31.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.095765 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-02-15 18:51:42.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.095929 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/spinner/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2056 2024-02-15 18:51:51.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.096095 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1485 2024-02-15 18:52:13.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.096266 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1515 2024-02-15 18:52:23.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.096433 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:52:30.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.096599 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-15 18:52:44.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.096770 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1533 2024-02-15 18:52:57.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.096933 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1531 2024-02-15 18:53:11.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.097232 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/stick_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:20:02.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/stick_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:53:22.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.097390 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/sticky/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2441 2024-02-15 18:53:32.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.097559 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/team_player/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3659 2024-02-15 18:53:44.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.097734 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/zenly/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3045 2024-02-15 18:53:56.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.071118 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.098028 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/always_stay/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:10:52.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/always_stay/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-04-01 18:00:21.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.098194 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-18 02:11:06.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.098371 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-18 02:11:20.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.098664 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:11:25.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-18 02:11:25.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.098814 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/del_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-22 06:12:46.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.098971 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-22 06:07:27.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.099125 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-22 06:12:45.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.099286 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:39:15.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.099661 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/jump_bidder/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:42:54.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/jump_bidder/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      191 2024-04-02 21:45:01.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/jump_bidder/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1258 2024-04-02 19:33:38.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/jump_bidder/jump_bidder.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.100072 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:42:59.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      191 2024-04-02 21:45:42.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1259 2024-04-02 19:34:13.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/jump_bidder.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.100515 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/min_bidder/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:05.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/min_bidder/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      188 2024-04-02 21:45:45.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/min_bidder/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1277 2024-04-02 19:34:47.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/min_bidder/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.100928 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/min_bidder 2/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:10.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/min_bidder 2/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      187 2024-04-02 21:41:36.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/min_bidder 2/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1275 2024-04-02 18:08:23.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/min_bidder 2/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.101335 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/truthful_bidder/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:16.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/truthful_bidder/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      202 2024-04-02 21:46:00.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/truthful_bidder/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1292 2024-04-02 19:36:57.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/truthful_bidder/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.101768 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:22.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      188 2024-04-02 21:46:05.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1293 2024-04-02 19:37:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.101903 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.102026 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/exponential/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2954 2024-01-26 06:19:46.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/exponential/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.102177 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/ficticious_play/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3052 2024-01-26 05:13:48.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.102324 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1549 2024-01-25 21:15:25.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.102491 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/rock_lover/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:32.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.102639 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1506 2024-01-25 21:15:38.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.102771 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:43.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.102926 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1543 2024-01-25 21:16:13.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.103082 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-01-25 21:16:18.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.103226 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1444 2024-01-25 22:02:30.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.103371 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1527 2024-01-25 21:16:28.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.103632 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/ta_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 22:14:36.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/ta_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1454 2024-01-25 21:16:33.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      662 2023-05-31 04:43:31.000000 agt_server-1.2.0/src/agt_server/agents/test_agents/stress_test.txt
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.073047 agt_server-1.2.0/src/agt_server/configs/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.104488 agt_server-1.2.0/src/agt_server/configs/handin_configs/
+-rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:28:03.000000 agt_server-1.2.0/src/agt_server/configs/handin_configs/bos_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      223 2024-02-22 04:27:55.000000 agt_server-1.2.0/src/agt_server/configs/handin_configs/bosii_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      231 2024-02-22 04:27:45.000000 agt_server-1.2.0/src/agt_server/configs/handin_configs/chicken_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      263 2024-03-02 19:44:48.000000 agt_server-1.2.0/src/agt_server/configs/handin_configs/lemonade_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      294 2024-04-02 18:15:54.000000 agt_server-1.2.0/src/agt_server/configs/handin_configs/lsvm_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:27:36.000000 agt_server-1.2.0/src/agt_server/configs/handin_configs/rps_config.json
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.105372 agt_server-1.2.0/src/agt_server/configs/server_configs/
+-rw-r--r--   0 johnwu     (501) staff       (20)      603 2024-02-01 23:47:38.000000 agt_server-1.2.0/src/agt_server/configs/server_configs/bos_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      797 2024-02-06 00:46:41.000000 agt_server-1.2.0/src/agt_server/configs/server_configs/bosii_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      608 2024-02-15 16:14:51.000000 agt_server-1.2.0/src/agt_server/configs/server_configs/chicken_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      621 2024-01-30 21:38:03.000000 agt_server-1.2.0/src/agt_server/configs/server_configs/lemonade_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      623 2024-03-31 16:36:02.000000 agt_server-1.2.0/src/agt_server/configs/server_configs/lsvm_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      604 2024-01-30 21:37:55.000000 agt_server-1.2.0/src/agt_server/configs/server_configs/rps_config.json
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.105520 agt_server-1.2.0/src/agt_server/handin/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3656 2024-04-03 02:38:28.000000 agt_server-1.2.0/src/agt_server/handin/handin.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.105655 agt_server-1.2.0/src/agt_server/handin/results/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:56.000000 agt_server-1.2.0/src/agt_server/handin/results/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.105765 agt_server-1.2.0/src/agt_server/handin/results/bos/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:49.000000 agt_server-1.2.0/src/agt_server/handin/results/bos/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.105886 agt_server-1.2.0/src/agt_server/handin/results/bosii/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:04.000000 agt_server-1.2.0/src/agt_server/handin/results/bosii/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.106017 agt_server-1.2.0/src/agt_server/handin/results/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:25.000000 agt_server-1.2.0/src/agt_server/handin/results/chicken/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.119020 agt_server-1.2.0/src/agt_server/handin/results/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2786 2024-02-22 23:10:32.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3094 2024-02-23 00:23:34.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3249 2024-02-26 03:46:11.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:12:09.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:13:49.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:14:53.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:21:10.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:23:39.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:25:31.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:26:34.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:27:17.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     1737 2024-02-26 04:27:28.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     1673 2024-02-26 04:27:55.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:28:23.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:31:07.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:32:45.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:33:29.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2631 2024-02-26 04:34:38.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2866 2024-02-26 04:55:11.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2759 2024-02-26 06:39:27.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-26 06:49:59.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2674 2024-02-26 06:59:09.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     9873 2024-02-26 23:17:30.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      526 2024-02-26 23:18:48.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2722 2024-02-26 23:36:33.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2784 2024-02-26 23:37:56.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2494 2024-02-26 23:38:30.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      219 2024-02-26 23:45:11.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-45-11_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:24.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-45-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:28.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-45-28_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:31.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-45-31_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:46:21.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-46-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3054 2024-02-26 23:47:10.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:47:41.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-47-41_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-26 23:50:39.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-50-38_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-26 23:58:51.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-58-51_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-27 00:09:44.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:09:46.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_19-09-46_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2416 2024-02-27 00:13:56.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2610 2024-02-27 00:14:32.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:19:21.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_19-19-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:21:53.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_19-21-53_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     4940 2024-02-27 20:26:21.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3215 2024-02-27 20:27:18.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     7406 2024-02-27 20:32:27.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3367 2024-02-27 20:33:47.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     7165 2024-02-27 20:36:53.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     6897 2024-02-27 20:40:29.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5795 2024-02-27 20:40:37.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     6689 2024-02-27 20:49:05.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    69971 2024-02-28 04:53:17.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    42190 2024-02-28 08:28:23.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    38084 2024-02-28 10:04:34.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    38027 2024-02-28 11:31:24.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5240 2024-02-28 11:34:41.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     1921 2024-02-28 11:35:40.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     8899 2024-02-28 11:42:21.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    39034 2024-02-28 14:22:14.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    74776 2024-02-28 19:14:37.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5920 2024-02-28 21:11:22.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5102 2024-02-28 21:13:24.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     4669 2024-02-28 21:16:32.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5107 2024-02-28 21:19:34.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    16781 2024-02-28 21:40:00.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    15945 2024-02-28 21:51:18.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    17789 2024-02-28 22:18:47.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    15831 2024-02-28 22:55:20.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3939 2024-03-01 00:34:13.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    14259 2024-03-01 00:45:25.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3812 2024-03-01 00:46:34.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3998 2024-03-01 00:48:27.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     6081 2024-03-01 01:51:10.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     9474 2024-03-01 01:52:08.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     8767 2024-03-01 01:52:36.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5900 2024-03-01 01:54:12.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    12641 2024-03-01 02:00:54.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    33503 2024-03-01 03:09:35.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    31050 2024-03-01 05:10:15.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    18142 2024-03-01 05:31:08.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    18785 2024-03-01 06:24:52.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    19642 2024-03-01 07:22:31.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3325 2024-03-01 07:22:31.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/LemonadeArena.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3900 2024-02-26 04:14:53.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/LemonadeTest.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)   785905 2024-03-01 23:54:21.000000 agt_server-1.2.0/src/agt_server/handin/results/lemonade/shortcut.json
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.120695 agt_server-1.2.0/src/agt_server/handin/results/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:14.000000 agt_server-1.2.0/src/agt_server/handin/results/rps/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.121845 agt_server-1.2.0/src/agt_server/local_games/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.2.0/src/agt_server/local_games/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     2318 2024-02-22 09:00:09.000000 agt_server-1.2.0/src/agt_server/local_games/base.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     9604 2024-02-15 18:16:30.000000 agt_server-1.2.0/src/agt_server/local_games/bos_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    10213 2024-02-15 18:16:15.000000 agt_server-1.2.0/src/agt_server/local_games/bosii_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     9731 2024-02-15 18:17:49.000000 agt_server-1.2.0/src/agt_server/local_games/chicken_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    17831 2024-04-02 02:32:20.000000 agt_server-1.2.0/src/agt_server/local_games/lemonade_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    23055 2024-04-02 19:30:00.000000 agt_server-1.2.0/src/agt_server/local_games/lsvm_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     9703 2024-02-15 18:17:04.000000 agt_server-1.2.0/src/agt_server/local_games/rps_arena.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.122106 agt_server-1.2.0/src/agt_server/server/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.2.0/src/agt_server/server/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.123423 agt_server-1.2.0/src/agt_server/server/games/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.2.0/src/agt_server/server/games/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      596 2024-01-31 02:48:39.000000 agt_server-1.2.0/src/agt_server/server/games/bos_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    18510 2024-01-30 21:30:44.000000 agt_server-1.2.0/src/agt_server/server/games/bosii_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      606 2024-01-25 21:17:28.000000 agt_server-1.2.0/src/agt_server/server/games/chicken_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    16908 2024-01-30 21:34:09.000000 agt_server-1.2.0/src/agt_server/server/games/complete_2x2_matrix_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      710 2024-01-23 13:08:08.000000 agt_server-1.2.0/src/agt_server/server/games/game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    19180 2024-01-30 21:32:26.000000 agt_server-1.2.0/src/agt_server/server/games/lemonade_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      671 2024-01-25 21:17:39.000000 agt_server-1.2.0/src/agt_server/server/games/rps_game.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.123569 agt_server-1.2.0/src/agt_server/server/results/
+-rw-r--r--   0 johnwu     (501) staff       (20)       18 2024-01-25 18:51:20.000000 agt_server-1.2.0/src/agt_server/server/results/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.123715 agt_server-1.2.0/src/agt_server/server/results/bos/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:35.000000 agt_server-1.2.0/src/agt_server/server/results/bos/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.123877 agt_server-1.2.0/src/agt_server/server/results/bosii/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:39.000000 agt_server-1.2.0/src/agt_server/server/results/bosii/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.124045 agt_server-1.2.0/src/agt_server/server/results/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:43.000000 agt_server-1.2.0/src/agt_server/server/results/chicken/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.124148 agt_server-1.2.0/src/agt_server/server/results/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:49.000000 agt_server-1.2.0/src/agt_server/server/results/lemonade/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.124261 agt_server-1.2.0/src/agt_server/server/results/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:54.000000 agt_server-1.2.0/src/agt_server/server/results/rps/.gitkeep
+-rw-r--r--   0 johnwu     (501) staff       (20)    23118 2024-02-15 16:20:24.000000 agt_server-1.2.0/src/agt_server/server/server.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.077445 agt_server-1.2.0/src/agt_server.egg-info/
+-rw-r--r--   0 johnwu     (501) staff       (20)     6482 2024-04-03 02:46:09.000000 agt_server-1.2.0/src/agt_server.egg-info/PKG-INFO
+-rw-r--r--   0 johnwu     (501) staff       (20)    18184 2024-04-03 02:46:09.000000 agt_server-1.2.0/src/agt_server.egg-info/SOURCES.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)        1 2024-04-03 02:46:09.000000 agt_server-1.2.0/src/agt_server.egg-info/dependency_links.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)       55 2024-04-03 02:46:09.000000 agt_server-1.2.0/src/agt_server.egg-info/requires.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)       11 2024-04-03 02:46:09.000000 agt_server-1.2.0/src/agt_server.egg-info/top_level.txt
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.074724 agt_server-1.2.0/test/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.075147 agt_server-1.2.0/test/server_test/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.124537 agt_server-1.2.0/test/server_test/bos/
+-rw-r--r--   0 johnwu     (501) staff       (20)     7014 2024-01-25 21:24:06.000000 agt_server-1.2.0/test/server_test/bos/bos_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)     8015 2024-01-25 21:22:03.000000 agt_server-1.2.0/test/server_test/bos/bos_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.124992 agt_server-1.2.0/test/server_test/bosii/
+-rw-r--r--   0 johnwu     (501) staff       (20)    10139 2024-01-25 21:26:19.000000 agt_server-1.2.0/test/server_test/bosii/bosii_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)    11361 2024-01-25 21:28:31.000000 agt_server-1.2.0/test/server_test/bosii/bosii_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.125699 agt_server-1.2.0/test/server_test/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)    10276 2024-01-25 21:35:28.000000 agt_server-1.2.0/test/server_test/chicken/chicken_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)    11631 2024-01-25 21:50:35.000000 agt_server-1.2.0/test/server_test/chicken/chicken_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.126277 agt_server-1.2.0/test/server_test/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)    13981 2024-01-25 21:53:38.000000 agt_server-1.2.0/test/server_test/lemonade/lemonade_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)     8108 2024-01-25 21:56:56.000000 agt_server-1.2.0/test/server_test/lemonade/lemonade_ql.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)    16031 2024-01-25 21:58:30.000000 agt_server-1.2.0/test/server_test/lemonade/lemonade_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-03 02:46:09.126559 agt_server-1.2.0/test/server_test/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)     5940 2024-01-25 22:00:19.000000 agt_server-1.2.0/test/server_test/rps/rps_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)     6884 2024-01-25 22:00:40.000000 agt_server-1.2.0/test/server_test/rps/rps_test.sh
```

### Comparing `agt_server-1.1.3/.gitignore` & `agt_server-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/LICENSE` & `agt_server-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/PKG-INFO` & `agt_server-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agt_server
-Version: 1.1.3
+Version: 1.2.0
 Summary: The AGT Server is a python platform designed to run and implement game environments that autonomous agents can connect to and compete in.
 Home-page: https://github.com/brown-agt/agt-server-remastered
 Author: John Wu
 Author-email: john_w_wu@brown.edu
 Project-URL: Bug Tracker, https://github.com/brown-agt/agt-server-remastered/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agt_server-1.1.3/README.md` & `agt_server-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/data/profile.svg` & `agt_server-1.2.0/data/profile.svg`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/setup.py` & `agt_server-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='agt_server', 
-    version='1.1.3',
+    version='1.2.0',
     author='John Wu', 
     author_email='john_w_wu@brown.edu', 
     description='The AGT Server is a python platform designed to run and implement game environments that autonomous agents can connect to and compete in.',  # Provide a short description
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/brown-agt/agt-server-remastered',  
     project_urls={
```

### Comparing `agt_server-1.1.3/src/agt_server/agents/base_agents/agent.py` & `agt_server-1.2.0/src/agt_server/agents/base_agents/agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/base_agents/bos_agent.py` & `agt_server-1.2.0/src/agt_server/agents/base_agents/bos_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/base_agents/bosii_agent.py` & `agt_server-1.2.0/src/agt_server/agents/base_agents/bosii_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/base_agents/chicken_agent.py` & `agt_server-1.2.0/src/agt_server/agents/base_agents/chicken_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/base_agents/cm_agent.py` & `agt_server-1.2.0/src/agt_server/agents/base_agents/cm_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/base_agents/game_report.py` & `agt_server-1.2.0/src/agt_server/agents/base_agents/game_report.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/base_agents/lemonade_agent.py` & `agt_server-1.2.0/src/agt_server/agents/base_agents/lemonade_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pkg_resources
 
 
 class LemonadeAgent(Agent):
     def __init__(self, name=None, timestamp=None):
         super().__init__(name, timestamp)
         self.valid_actions = list(range(12))
+        # TODO: Fix config so it uses the server by default but handin also sets the config to it's version
         config_path = pkg_resources.resource_filename('agt_server', 'configs/server_configs/lemonade_config.json')
         with open(config_path) as cfile:
             server_config = json.load(cfile)
         self.response_time = server_config['response_time']
 
     def timeout_handler(self):
         print(f"{self.name} has timed out")
```

### Comparing `agt_server-1.1.3/src/agt_server/agents/base_agents/rps_agent.py` & `agt_server-1.2.0/src/agt_server/agents/base_agents/rps_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/exponential/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/exponential/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py` & `agt_server-1.2.0/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/agents/test_agents/stress_test.txt` & `agt_server-1.2.0/src/agt_server/agents/test_agents/stress_test.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/configs/server_configs/bos_config.json` & `agt_server-1.2.0/src/agt_server/configs/server_configs/bos_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/configs/server_configs/bosii_config.json` & `agt_server-1.2.0/src/agt_server/configs/server_configs/bosii_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/configs/server_configs/chicken_config.json` & `agt_server-1.2.0/src/agt_server/configs/server_configs/chicken_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/configs/server_configs/lemonade_config.json` & `agt_server-1.2.0/src/agt_server/configs/server_configs/lemonade_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/configs/server_configs/rps_config.json` & `agt_server-1.2.0/src/agt_server/configs/server_configs/rps_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/handin.py` & `agt_server-1.2.0/src/agt_server/handin/handin.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 file_mod_time = os.path.getmtime(file_path)
                 if file_mod_time > folder_mod_times[root]:
                     folder_mod_times[root] = file_mod_time
             except Exception as e:
                 print(f"Failed to get modification time for {file_path}: {e}", file=sys.stderr)
         
         for file in files:
-            if file == 'my_agent.py':
+            if file == 'agent_submission.py':
                 full_path = os.path.join(root, file)
                 try:
                     agent_submission = import_agent_submission_from_path(full_path)
                     agent_submission.timestamp = folder_mod_times[root]
                     agent_submissions.append(agent_submission)
                 except Exception as e:
                     print(f"Failed to import {full_path}: {e}", file=sys.stderr)
```

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/LemonadeArena.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/LemonadeArena.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/LemonadeTest.txt` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/LemonadeTest.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/handin/results/lemonade/shortcut.json` & `agt_server-1.2.0/src/agt_server/handin/results/lemonade/shortcut.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/local_games/base.py` & `agt_server-1.2.0/src/agt_server/local_games/base.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/local_games/bos_arena.py` & `agt_server-1.2.0/src/agt_server/local_games/bos_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/local_games/bosii_arena.py` & `agt_server-1.2.0/src/agt_server/local_games/bosii_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/local_games/chicken_arena.py` & `agt_server-1.2.0/src/agt_server/local_games/chicken_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/local_games/lemonade_arena.py` & `agt_server-1.2.0/src/agt_server/local_games/lemonade_arena.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,17 +296,15 @@
             
             names = [p1.name, p2.name, p3.name]
             timestamps = [p1.timestamp, p2.timestamp, p3.timestamp]
             combined = sorted(zip(names, timestamps), key=lambda x: x[0])
             sorted_names, sorted_timestamps = zip(*combined)
             name_key = "|".join(sorted_names)
             
-            #print(name_key, sorted_timestamps, data)
             if random.random() > 0.07 and name_key in data: 
-                # and data[name_key]["timestamps"] == list(sorted_timestamps)
                 total_u = data[name_key]["util"]
                 winner = sorted_names[np.argmax(total_u)]
                 self.results.append(list(sorted_names) + total_u + [winner])
             else: 
                 self.run_helper(p1, p2, p3)
         else: 
             self.run_helper(p1, p2, p3)
```

### Comparing `agt_server-1.1.3/src/agt_server/local_games/rps_arena.py` & `agt_server-1.2.0/src/agt_server/local_games/rps_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/server/games/bos_game.py` & `agt_server-1.2.0/src/agt_server/server/games/bos_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/server/games/bosii_game.py` & `agt_server-1.2.0/src/agt_server/server/games/bosii_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/server/games/chicken_game.py` & `agt_server-1.2.0/src/agt_server/server/games/chicken_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/server/games/complete_2x2_matrix_game.py` & `agt_server-1.2.0/src/agt_server/server/games/complete_2x2_matrix_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/server/games/game.py` & `agt_server-1.2.0/src/agt_server/server/games/game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/server/games/lemonade_game.py` & `agt_server-1.2.0/src/agt_server/server/games/lemonade_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/server/games/rps_game.py` & `agt_server-1.2.0/src/agt_server/server/games/rps_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server/server/server.py` & `agt_server-1.2.0/src/agt_server/server/server.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/src/agt_server.egg-info/PKG-INFO` & `agt_server-1.2.0/src/agt_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agt-server
-Version: 1.1.3
+Version: 1.2.0
 Summary: The AGT Server is a python platform designed to run and implement game environments that autonomous agents can connect to and compete in.
 Home-page: https://github.com/brown-agt/agt-server-remastered
 Author: John Wu
 Author-email: john_w_wu@brown.edu
 Project-URL: Bug Tracker, https://github.com/brown-agt/agt-server-remastered/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agt_server-1.1.3/src/agt_server.egg-info/SOURCES.txt` & `agt_server-1.2.0/src/agt_server.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/agt_server/agents/base_agents/agent.py
 src/agt_server/agents/base_agents/bos_agent.py
 src/agt_server/agents/base_agents/bosii_agent.py
 src/agt_server/agents/base_agents/chicken_agent.py
 src/agt_server/agents/base_agents/cm_agent.py
 src/agt_server/agents/base_agents/game_report.py
 src/agt_server/agents/base_agents/lemonade_agent.py
+src/agt_server/agents/base_agents/lsvm_agent.py
 src/agt_server/agents/base_agents/rps_agent.py
 src/agt_server/agents/test_agents/__init__.py
 src/agt_server/agents/test_agents/stress_test.txt
 src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py
 src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py
 src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py
 src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py
@@ -127,14 +128,33 @@
 src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py
 src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py
 src/agt_server/agents/test_agents/lemonade_small/decrement_agent/__init__.py
 src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py
 src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py
 src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py
 src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py
+src/agt_server/agents/test_agents/lsvm/__init__.py
+src/agt_server/agents/test_agents/lsvm/jump_bidder/__init__.py
+src/agt_server/agents/test_agents/lsvm/jump_bidder/agent_submission.py
+src/agt_server/agents/test_agents/lsvm/jump_bidder/jump_bidder.py
+src/agt_server/agents/test_agents/lsvm/jump_bidder 2/__init__.py
+src/agt_server/agents/test_agents/lsvm/jump_bidder 2/agent_submission.py
+src/agt_server/agents/test_agents/lsvm/jump_bidder 2/jump_bidder.py
+src/agt_server/agents/test_agents/lsvm/min_bidder/__init__.py
+src/agt_server/agents/test_agents/lsvm/min_bidder/agent_submission.py
+src/agt_server/agents/test_agents/lsvm/min_bidder/my_agent.py
+src/agt_server/agents/test_agents/lsvm/min_bidder 2/__init__.py
+src/agt_server/agents/test_agents/lsvm/min_bidder 2/agent_submission.py
+src/agt_server/agents/test_agents/lsvm/min_bidder 2/my_agent.py
+src/agt_server/agents/test_agents/lsvm/truthful_bidder/__init__.py
+src/agt_server/agents/test_agents/lsvm/truthful_bidder/agent_submission.py
+src/agt_server/agents/test_agents/lsvm/truthful_bidder/my_agent.py
+src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/__init__.py
+src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/agent_submission.py
+src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/my_agent.py
 src/agt_server/agents/test_agents/rps/__init__.py
 src/agt_server/agents/test_agents/rps/exponential/my_agent.py
 src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py
 src/agt_server/agents/test_agents/rps/random_agent/my_agent.py
 src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py
 src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py
 src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py
@@ -144,19 +164,21 @@
 src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py
 src/agt_server/agents/test_agents/rps/ta_agent/__init__.py
 src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py
 src/agt_server/configs/handin_configs/bos_config.json
 src/agt_server/configs/handin_configs/bosii_config.json
 src/agt_server/configs/handin_configs/chicken_config.json
 src/agt_server/configs/handin_configs/lemonade_config.json
+src/agt_server/configs/handin_configs/lsvm_config.json
 src/agt_server/configs/handin_configs/rps_config.json
 src/agt_server/configs/server_configs/bos_config.json
 src/agt_server/configs/server_configs/bosii_config.json
 src/agt_server/configs/server_configs/chicken_config.json
 src/agt_server/configs/server_configs/lemonade_config.json
+src/agt_server/configs/server_configs/lsvm_config.json
 src/agt_server/configs/server_configs/rps_config.json
 src/agt_server/handin/handin.py
 src/agt_server/handin/results/__init__.py
 src/agt_server/handin/results/bos/__init__.py
 src/agt_server/handin/results/bosii/__init__.py
 src/agt_server/handin/results/chicken/__init__.py
 src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt
@@ -246,14 +268,15 @@
 src/agt_server/handin/results/rps/__init__.py
 src/agt_server/local_games/__init__.py
 src/agt_server/local_games/base.py
 src/agt_server/local_games/bos_arena.py
 src/agt_server/local_games/bosii_arena.py
 src/agt_server/local_games/chicken_arena.py
 src/agt_server/local_games/lemonade_arena.py
+src/agt_server/local_games/lsvm_arena.py
 src/agt_server/local_games/rps_arena.py
 src/agt_server/server/__init__.py
 src/agt_server/server/server.py
 src/agt_server/server/games/__init__.py
 src/agt_server/server/games/bos_game.py
 src/agt_server/server/games/bosii_game.py
 src/agt_server/server/games/chicken_game.py
```

### Comparing `agt_server-1.1.3/test/server_test/bos/bos_local_test.sh` & `agt_server-1.2.0/test/server_test/bos/bos_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/test/server_test/bos/bos_test.sh` & `agt_server-1.2.0/test/server_test/bos/bos_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/test/server_test/bosii/bosii_local_test.sh` & `agt_server-1.2.0/test/server_test/bosii/bosii_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/test/server_test/bosii/bosii_test.sh` & `agt_server-1.2.0/test/server_test/bosii/bosii_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/test/server_test/chicken/chicken_local_test.sh` & `agt_server-1.2.0/test/server_test/chicken/chicken_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/test/server_test/chicken/chicken_test.sh` & `agt_server-1.2.0/test/server_test/chicken/chicken_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/test/server_test/lemonade/lemonade_local_test.sh` & `agt_server-1.2.0/test/server_test/lemonade/lemonade_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/test/server_test/lemonade/lemonade_ql.sh` & `agt_server-1.2.0/test/server_test/lemonade/lemonade_ql.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/test/server_test/lemonade/lemonade_test.sh` & `agt_server-1.2.0/test/server_test/lemonade/lemonade_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/test/server_test/rps/rps_local_test.sh` & `agt_server-1.2.0/test/server_test/rps/rps_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.1.3/test/server_test/rps/rps_test.sh` & `agt_server-1.2.0/test/server_test/rps/rps_test.sh`

 * *Files identical despite different names*

