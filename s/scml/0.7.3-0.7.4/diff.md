# Comparing `tmp/scml-0.7.3.tar.gz` & `tmp/scml-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scml-0.7.3.tar", last modified: Sun Mar 17 09:05:10 2024, max compression
+gzip compressed data, was "scml-0.7.4.tar", last modified: Wed Apr  3 06:18:11 2024, max compression
```

## Comparing `scml-0.7.3.tar` & `scml-0.7.4.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.422693 scml-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-17 09:05:01.000000 scml-0.7.3/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-17 09:05:01.000000 scml-0.7.3/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-17 09:05:01.000000 scml-0.7.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-17 09:05:01.000000 scml-0.7.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-17 09:05:01.000000 scml-0.7.3/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-17 09:05:01.000000 scml-0.7.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-03-17 09:05:01.000000 scml-0.7.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-17 09:05:01.000000 scml-0.7.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-17 09:05:01.000000 scml-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-17 09:05:01.000000 scml-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-03-17 09:05:10.422693 scml-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-17 09:05:01.000000 scml-0.7.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-17 09:05:10.422693 scml-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-03-17 09:05:01.000000 scml-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.390693 scml-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.398693 scml-0.7.3/src/scml/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   132032 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    69113 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/cliadv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.402693 scml-0.7.3/src/scml/oneshot/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    21685 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.402693 scml-0.7.3/src/scml/oneshot/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/agents/aspiration.py
--rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/agents/greedy.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/agents/nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/agents/rand.py
--rw-r--r--   0 runner    (1001) docker     (127)    40670 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/awi.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    81738 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.402693 scml-0.7.3/src/scml/oneshot/rl/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/rl/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/rl/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/rl/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/rl/env.py
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/rl/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12062 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/rl/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/rl/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/rl/reward.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/sysagents.py
--rw-r--r--   0 runner    (1001) docker     (127)    47513 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/ufun.py
--rw-r--r--   0 runner    (1001) docker     (127)   127473 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/oneshot/world.py
--rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.406693 scml-0.7.3/src/scml/scml2019/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6793 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14656 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20378 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/awi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11734 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/bank.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57559 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23625 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/consumers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.406693 scml-0.7.3/src/scml/scml2019/factory_managers/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/factory_managers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    38211 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/factory_managers/builtins.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1027 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7189 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/insurance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8296 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/miners.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29292 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/schedulers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46519 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/simulators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    59623 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/utils19.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2257 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/visualizers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   106736 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2019/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.410693 scml-0.7.3/src/scml/scml2020/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.410693 scml-0.7.3/src/scml/scml2020/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/agents/bcse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/agents/decentralizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/agents/do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/agents/indneg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/agents/moving.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/agents/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/agents/reactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/agents/satisficer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29681 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/awi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.410693 scml-0.7.3/src/scml/scml2020/components/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32704 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/components/negotiation.py
--rw-r--r--   0 runner    (1001) docker     (127)    20521 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/components/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    13477 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/components/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/components/signing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/components/trading.py
--rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.410693 scml-0.7.3/src/scml/scml2020/services/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/services/controllers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27113 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/services/simulators.py
--rw-r--r--   0 runner    (1001) docker     (127)   133308 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/scml2020/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.414693 scml-0.7.3/src/scml/std/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.414693 scml-0.7.3/src/scml/std/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/agents/aspiration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/agents/greedy.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/agents/nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/agents/rand.py
--rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/awi.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.414693 scml-0.7.3/src/scml/std/rl/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/rl/action.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/rl/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/rl/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/rl/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/rl/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/rl/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/rl/reward.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/sysagents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/ufun.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/std/world.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   148769 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.414693 scml-0.7.3/src/scml/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.418693 scml-0.7.3/src/scml/vendor/quick/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/vendor/quick/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/vendor/quick/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/vendor/quick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29361 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/vendor/quick/quick.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-17 09:05:01.000000 scml-0.7.3/src/scml/vendor/quick/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.422693 scml-0.7.3/src/scml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-03-17 09:05:10.000000 scml-0.7.3/src/scml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-03-17 09:05:10.000000 scml-0.7.3/src/scml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 09:05:10.000000 scml-0.7.3/src/scml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-17 09:05:10.000000 scml-0.7.3/src/scml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 09:05:10.000000 scml-0.7.3/src/scml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-17 09:05:10.000000 scml-0.7.3/src/scml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-17 09:05:10.000000 scml-0.7.3/src/scml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.418693 scml-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:01.000000 scml-0.7.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.418693 scml-0.7.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:01.000000 scml-0.7.3/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.418693 scml-0.7.3/tests/etc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:01.000000 scml-0.7.3/tests/etc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-03-17 09:05:01.000000 scml-0.7.3/tests/etc/test_can_run_tutorial2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-17 09:05:01.000000 scml-0.7.3/tests/etc/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-17 09:05:01.000000 scml-0.7.3/tests/etc/test_jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.418693 scml-0.7.3/tests/old/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:01.000000 scml-0.7.3/tests/old/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17345 2024-03-17 09:05:01.000000 scml-0.7.3/tests/old/test_factory2019.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20339 2024-03-17 09:05:01.000000 scml-0.7.3/tests/old/test_scheduler2019.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      553 2024-03-17 09:05:01.000000 scml-0.7.3/tests/old/test_scml2019.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12090 2024-03-17 09:05:01.000000 scml-0.7.3/tests/old/test_scml2019factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2606 2024-03-17 09:05:01.000000 scml-0.7.3/tests/old/test_scml2019tournaments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.418693 scml-0.7.3/tests/oneshot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:01.000000 scml-0.7.3/tests/oneshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-17 09:05:01.000000 scml-0.7.3/tests/oneshot/test_oneshot_do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-03-17 09:05:01.000000 scml-0.7.3/tests/oneshot/test_oneshot_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-03-17 09:05:01.000000 scml-0.7.3/tests/oneshot/test_oneshot_ufun.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-03-17 09:05:01.000000 scml-0.7.3/tests/oneshot/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    34929 2024-03-17 09:05:01.000000 scml-0.7.3/tests/oneshot/test_scml2021oneshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-03-17 09:05:01.000000 scml-0.7.3/tests/oneshot/test_scml2023oneshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-03-17 09:05:01.000000 scml-0.7.3/tests/oneshot/test_scml2024oneshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-03-17 09:05:01.000000 scml-0.7.3/tests/oneshot/test_sync_jackson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.418693 scml-0.7.3/tests/rl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:01.000000 scml-0.7.3/tests/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-17 09:05:01.000000 scml-0.7.3/tests/rl/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29750 2024-03-17 09:05:01.000000 scml-0.7.3/tests/rl/test_rl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.422693 scml-0.7.3/tests/std/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:01.000000 scml-0.7.3/tests/std/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-03-17 09:05:01.000000 scml-0.7.3/tests/std/test_std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:10.422693 scml-0.7.3/tests/std2020design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:01.000000 scml-0.7.3/tests/std2020design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-03-17 09:05:01.000000 scml-0.7.3/tests/std2020design/test_scml2020.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-03-17 09:05:01.000000 scml-0.7.3/tests/std2020design/test_scml2020factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3960 2024-03-17 09:05:01.000000 scml-0.7.3/tests/std2020design/test_scml2020tournaments.py
--rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-03-17 09:05:01.000000 scml-0.7.3/tests/std2020design/test_scml2021.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8392 2024-03-17 09:05:01.000000 scml-0.7.3/tests/std2020design/test_scml2021tournaments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-17 09:05:01.000000 scml-0.7.3/tests/std2020design/test_scml2023.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-17 09:05:01.000000 scml-0.7.3/tests/switches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-17 09:05:01.000000 scml-0.7.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.810520 scml-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 06:18:02.000000 scml-0.7.4/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-03 06:18:02.000000 scml-0.7.4/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 06:18:02.000000 scml-0.7.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 06:18:02.000000 scml-0.7.4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 06:18:02.000000 scml-0.7.4/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 06:18:02.000000 scml-0.7.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19223 2024-04-03 06:18:02.000000 scml-0.7.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-03 06:18:02.000000 scml-0.7.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-03 06:18:02.000000 scml-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-03 06:18:02.000000 scml-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21741 2024-04-03 06:18:11.810520 scml-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-03 06:18:02.000000 scml-0.7.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-03 06:18:11.810520 scml-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-03 06:18:02.000000 scml-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.778519 scml-0.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.786519 scml-0.7.4/src/scml/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132032 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69113 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/cliadv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.786519 scml-0.7.4/src/scml/oneshot/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21685 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.790519 scml-0.7.4/src/scml/oneshot/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agents/aspiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agents/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agents/nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agents/rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40941 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/awi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84620 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.790519 scml-0.7.4/src/scml/oneshot/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/sysagents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47513 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/ufun.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127475 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/world.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.794520 scml-0.7.4/src/scml/scml2019/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6793 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14656 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20378 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/awi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11734 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/bank.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57559 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23625 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/consumers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.794520 scml-0.7.4/src/scml/scml2019/factory_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/factory_managers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38211 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/factory_managers/builtins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1027 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7189 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/insurance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8296 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/miners.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29292 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/schedulers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46519 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/simulators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59623 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/utils19.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2257 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/visualizers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   106736 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.794520 scml-0.7.4/src/scml/scml2020/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.798519 scml-0.7.4/src/scml/scml2020/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/bcse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/decentralizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/do_nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/indneg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/moving.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/reactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/satisficer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29681 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/awi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.798519 scml-0.7.4/src/scml/scml2020/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32704 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20521 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13477 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/signing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.798519 scml-0.7.4/src/scml/scml2020/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/services/controllers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27113 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/services/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133308 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.798519 scml-0.7.4/src/scml/std/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/src/scml/std/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agents/aspiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agents/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agents/nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agents/rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/awi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/src/scml/std/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/sysagents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/ufun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   148769 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/src/scml/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/src/scml/vendor/quick/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/quick/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/quick/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/quick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29361 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/quick/quick.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/quick/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.810520 scml-0.7.4/src/scml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21741 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.806520 scml-0.7.4/tests/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/etc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-03 06:18:02.000000 scml-0.7.4/tests/etc/test_can_run_tutorial2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-03 06:18:02.000000 scml-0.7.4/tests/etc/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 06:18:02.000000 scml-0.7.4/tests/etc/test_jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.806520 scml-0.7.4/tests/old/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17345 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/test_factory2019.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20339 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/test_scheduler2019.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      553 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/test_scml2019.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12090 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/test_scml2019factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2606 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/test_scml2019tournaments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.806520 scml-0.7.4/tests/oneshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_oneshot_do_nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_oneshot_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_oneshot_ufun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34929 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_scml2021oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_scml2023oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_scml2024oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_sync_jackson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.806520 scml-0.7.4/tests/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-03 06:18:02.000000 scml-0.7.4/tests/rl/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29750 2024-04-03 06:18:02.000000 scml-0.7.4/tests/rl/test_rl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.806520 scml-0.7.4/tests/std/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std/test_std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.810520 scml-0.7.4/tests/std2020design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2020.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2020factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3960 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2020tournaments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2021.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8392 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2021tournaments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-03 06:18:02.000000 scml-0.7.4/tests/switches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-03 06:18:02.000000 scml-0.7.4/tox.ini
```

### Comparing `scml-0.7.3/.cookiecutterrc` & `scml-0.7.4/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/.travis.yml` & `scml-0.7.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/CHANGELOG.rst` & `scml-0.7.4/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Changelog
 =========
 
+0.7.4 (2024.04.03)
+------------------
+
+* AWI: Correcting n_competitors and adding my_competitors
+* slightly faster random oneshot
+* bugfix in builtin_std_agents
+* Adding more contexts
+* Adding loading sklearn to FAQ
+
+0.7.3 (2024.03.15)
+------------------
+
+* Requiring negmas 0.10.18
+
 0.7.2 (2024.03.02)
 ------------------
 
 * requiring negmas >=0.10.17
 * minor bugfix correcting method name in 2022 version
 * correcting NMI type in some agents
 * bugfix CLI failed because "method" is not in World
```

### Comparing `scml-0.7.3/CONTRIBUTING.rst` & `scml-0.7.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/LICENSE` & `scml-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/MANIFEST.in` & `scml-0.7.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/PKG-INFO` & `scml-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scml
-Version: 0.7.3
+Version: 0.7.4
 Summary: ANAC Supply Chain Management League Platform
 Home-page: https://github.com/yasserfarouk/scml
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Project-URL: Documentation, https://scml.readthedocs.io/
 Project-URL: Changelog, https://scml.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/yasserfarouk/scml/issues
@@ -23,15 +23,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: click
 Requires-Dist: pytest
 Requires-Dist: hypothesis
-Requires-Dist: negmas>=0.10.18
+Requires-Dist: negmas>=0.10.20
 Requires-Dist: joblib
 Requires-Dist: jupyter
 Requires-Dist: gif
 Requires-Dist: gymnasium
 Provides-Extra: gui
 Requires-Dist: pyqt5; extra == "gui"
 
@@ -97,14 +97,28 @@
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 Changelog
 =========
 
+0.7.4 (2024.04.03)
+------------------
+
+* AWI: Correcting n_competitors and adding my_competitors
+* slightly faster random oneshot
+* bugfix in builtin_std_agents
+* Adding more contexts
+* Adding loading sklearn to FAQ
+
+0.7.3 (2024.03.15)
+------------------
+
+* Requiring negmas 0.10.18
+
 0.7.2 (2024.03.02)
 ------------------
 
 * requiring negmas >=0.10.17
 * minor bugfix correcting method name in 2022 version
 * correcting NMI type in some agents
 * bugfix CLI failed because "method" is not in World
```

### Comparing `scml-0.7.3/README.rst` & `scml-0.7.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/scml
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/scml.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/scml
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/yasserfarouk/scml/v0.7.3.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/yasserfarouk/scml/v0.7.4.svg
     :alt: Commits since latest release
-    :target: https://github.com/yasserfarouk/scml/compare/v0.7.3...master
+    :target: https://github.com/yasserfarouk/scml/compare/v0.7.4...master
 
 .. |CI| image:: https://github.com/yasserfarouk/scml/workflows/CI/badge.svg
     :target: https://www.github.com/yasserfarouk/scml
     :alt: Build Status
 
 .. |PyPiPublished| image:: https://github.com/yasserfarouk/scml/workflows/PyPI/badge.svg
     :target: https://pypi.python.org/pypi/scml
```

### Comparing `scml-0.7.3/setup.cfg` & `scml-0.7.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/setup.py` & `scml-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="scml",
-    version="0.7.3",
+    version="0.7.4",
     description="ANAC Supply Chain Management League Platform",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
@@ -59,15 +59,15 @@
         # eg: 'keyword1', 'keyword2', 'keyword3',
     ],
     python_requires=">=3.10",
     install_requires=[
         "click",
         "pytest",
         "hypothesis",
-        "negmas>=0.10.18",
+        "negmas>=0.10.20",
         "joblib",
         "jupyter",
         "gif",
         "gymnasium",
         # "python-constraint",
         # "prettytable",
         # "pulp",
```

### Comparing `scml-0.7.3/src/scml/cli.py` & `scml-0.7.4/src/scml/cli.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/cliadv.py` & `scml-0.7.4/src/scml/cliadv.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/common.py` & `scml-0.7.4/src/scml/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/experiment.py` & `scml-0.7.4/src/scml/experiment.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/__init__.py` & `scml-0.7.4/src/scml/oneshot/__init__.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/adapter.py` & `scml-0.7.4/src/scml/oneshot/adapter.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/agent.py` & `scml-0.7.4/src/scml/oneshot/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/agents/aspiration.py` & `scml-0.7.4/src/scml/oneshot/agents/aspiration.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/agents/greedy.py` & `scml-0.7.4/src/scml/oneshot/agents/greedy.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/agents/nothing.py` & `scml-0.7.4/src/scml/oneshot/agents/nothing.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/agents/rand.py` & `scml-0.7.4/src/scml/oneshot/agents/rand.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,34 +36,45 @@
     def __init__(
         self,
         *args,
         p_accept=PROB_ACCEPTANCE,
         p_end=PROB_END,
         **kwargs,
     ):
-        self.p_accept, self.p_end = p_accept, p_end
+        self.p_accept, self.p_end = p_accept + p_end, p_end
         super().__init__(*args, **kwargs)
 
     def _random_offer(self, negotiator_id: str):
         nmi = self.get_nmi(negotiator_id)
         if not nmi:
             return None  # will end the negotiation
         return nmi.random_outcome()
 
     def propose(self, negotiator_id, state) -> Outcome | None:
         return self._random_offer(negotiator_id)
 
     def respond(self, negotiator_id, state, source=None) -> ResponseType:
-        if random.random() < self.p_end:
+        r = random.random()
+        if r < self.p_end:
             return ResponseType.END_NEGOTIATION
-        if random.random() < self.p_accept:
+        if r < self.p_accept:
             return ResponseType.ACCEPT_OFFER
         return ResponseType.REJECT_OFFER
 
 
+class NiceAgent(RandomOneShotAgent):
+    """An agent that offers randomly and accepts anything"""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, p_accept=0, p_end=0, **kwargs)
+
+    def respond(self, negotiator_id, state, source=None) -> ResponseType:
+        return ResponseType.ACCEPT_OFFER
+
+
 class SyncRandomOneShotAgent(OneShotSyncAgent):
     """
     An agent that distributes its needs over its partners randomly.
 
     Args:
         equal: If given, it tries to equally distribute its needs over as many of its
                suppliers/consumers as possible
```

### Comparing `scml-0.7.3/src/scml/oneshot/awi.py` & `scml-0.7.4/src/scml/oneshot/awi.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     def n_products(self) -> int:
         """Returns the number of products in the system"""
         return len(self._world.catalog_prices)
 
     @property
     def n_competitors(self) -> int:
         """Returns the number of factories/agents in the same production level"""
-        return len(self._world.consumers[self.my_output_product]) - 1
+        return len(self._world.consumers[self.my_input_product]) - 1
 
     @property
     def n_processes(self) -> int:
         """Returns the number of processes in the system"""
         return self.n_products - 1
 
     @property
@@ -383,14 +383,23 @@
 
     @property
     def my_output_product(self) -> int:
         """the product I need to sell"""
         return self.profile.output_product if self.profile else -10
 
     @property
+    def my_competitors(self) -> list[str]:
+        """Returns the names of all factories in the same level as me"""
+        return [
+            _
+            for _ in self._world.consumers[self.my_input_product]
+            if _ != self.agent.id
+        ]
+
+    @property
     def my_suppliers(self) -> list[str]:
         """Returns a list of IDs for all of the agent's suppliers
         (agents that can supply the product I need).
         """
         return self.all_suppliers[self.level]
 
     @property
```

### Comparing `scml-0.7.3/src/scml/oneshot/common.py` & `scml-0.7.4/src/scml/oneshot/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/context.py` & `scml-0.7.4/src/scml/oneshot/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from collections import defaultdict
 from enum import Enum
 from typing import Any, Iterable, Union, Sequence
 
 import numpy as np
 from attr import define, field
 from scml.oneshot.agents.greedy import GreedyOneShotAgent
-from scml.oneshot.agents.rand import EqualDistOneShotAgent, RandDistOneShotAgent
+from scml.oneshot.agents.rand import (
+    EqualDistOneShotAgent,
+    NiceAgent,
+    RandDistOneShotAgent,
+)
 from negmas.helpers.strings import unique_name
 
 from scml.common import intin, isin, isinclass, isinfloat, isinobject, make_array
 from scml.oneshot.agent import OneShotAgent
 from scml.oneshot.agents import Placeholder
 from scml.oneshot.awi import OneShotAWI
 from scml.oneshot.common import is_system_agent
@@ -41,14 +45,19 @@
     "StrongConsumerContext",
     "WeakSupplierContext",
     "WeakConsumerContext",
     "BalancedSupplierContext",
     "BalancedConsumerContext",
     "RepeatingContext",
     "ContextParams",
+    "MonopolicContext",
+    "SingleAgentPerLevelSupplierContext",
+    "EutopiaContext",
+    "EutopiaConsumerContext",
+    "EutopiaSupplierContext",
 ]
 
 
 DefaultAgentsOneShot = (
     GreedyOneShotAgent,
     RandDistOneShotAgent,
     EqualDistOneShotAgent,
@@ -1005,14 +1014,22 @@
     exogenous_sales_predictability: tuple[float, float] | float = (0.6, 0.9)
     exogenous_control: tuple[float, float] | float = -1
     exogenous_price_dev: tuple[float, float] | float = (0.1, 0.2)
     equal_exogenous_supply = False
     equal_exogenous_sales = False
     cap_exogenous_quantities: bool = True
 
+    def __attrs_post_init__(self):
+        from scml.std.world import StdWorld
+
+        if self.perishable:
+            assert not issubclass(self.world_type, StdWorld)
+        else:
+            assert issubclass(self.world_type, StdWorld)
+
     def extract_context_params(
         self, min_values: bool, level: int | None = None
     ) -> ContextParams:
         nlines = safemin(self.n_lines) if min_values else safemax(self.n_lines)
         app = self.n_agents_per_process
         if not isinstance(app, Iterable):
             nsuppliers = nconsumers = app
@@ -1040,22 +1057,14 @@
             level == -1
             or not isinstance(self.n_processes, Iterable)
             and level == self.n_processes - 1
         ):
             nconsumers = 0
         return ContextParams(self.perishable, nlines, nsuppliers, nconsumers)
 
-    def __attrs_post_init__(self):
-        from scml.std.world import StdWorld
-
-        if self.perishable:
-            assert not issubclass(self.world_type, StdWorld)
-        else:
-            assert issubclass(self.world_type, StdWorld)
-
     def make_predefined_config(
         self,
         agent_types: list[type[OneShotAgent]],
         agent_processes: list[int],
         agent_params: list[dict[str, Any]],
         n_agents_per_process: list[int],
     ) -> dict[str, Any]:
@@ -1900,14 +1909,90 @@
         nlines = safemin(self.n_lines) if min_values else safemax(self.n_lines)
         nsuppliers = self.n_suppliers
         nconsumers = self.n_consumers
         return ContextParams(self.perishable, nlines, int(nsuppliers), int(nconsumers))
 
 
 @define
+class MonopolicContext(LimitedPartnerNumbersContext):
+    """An agent that has no competitors in the same level as themselves"""
+
+    # n_competitors: tuple[int, int] = field(default=(0, 0), converter=lambda _: (0, 0))
+    n_competitors: tuple[int, int] = (0, 0)
+    n_agents_per_process: np.ndarray | list[int] | tuple[int, int] | int = field(
+        default=(1, max(N_CONSUMERS[-1], N_SUPPLIERS[-1])),
+        converter=lambda _: (1, max(N_CONSUMERS[-1], N_SUPPLIERS[-1])),
+    )
+
+    def __attrs_post_init__(self):
+        npp = self.n_agents_per_process
+        if isinstance(npp, int):
+            assert (
+                npp == 1
+            ), f"You passed {self.n_agents_per_process=} to a MonopolicContext but this MUST be one in this case"
+        elif isinstance(npp, tuple):
+            npp = (min(1, npp[0]), npp[1])
+        else:
+            npp = list(set(list(npp) + [1]))
+        object.__setattr__(self, "n_agents_per_process", npp)
+        return super().__attrs_post_init__()
+
+
+@define
+class SingleAgentPerLevelConsumerContext(MonopolicContext):
+    """A world in which every level has exactly one factory and the agent is a consumer"""
+
+    level: int = -1
+    n_consumers: tuple[int, int] = (0, 0)
+    n_suppliers: tuple[int, int] = (1, 1)
+    n_agents_per_process: np.ndarray | list[int] | tuple[int, int] | int = field(
+        default=1, converter=lambda _: 1
+    )
+
+
+@define
+class SingleAgentPerLevelSupplierContext(MonopolicContext):
+    """A world in which every level has exactly one factory and the agent is a supplier"""
+
+    level: int = 0
+    n_consumers: tuple[int, int] = (1, 1)
+    n_suppliers: tuple[int, int] = (0, 0)
+    n_agents_per_process: np.ndarray | list[int] | tuple[int, int] | int = field(
+        default=1, converter=lambda _: 1
+    )
+
+
+@define
+class EutopiaContext(MonopolicContext):
+    """An unrealistic context in which the agent is the only one in its level and all other agents are nice."""
+
+    non_competitors: tuple[str | type[OneShotAgent], ...] = field(
+        default=(NiceAgent,), converter=lambda _: (NiceAgent,)
+    )
+
+
+@define
+class EutopiaSupplierContext(EutopiaContext):
+    """An unrealistic context in which the agent is the only supplier and all consumers are nice."""
+
+    level: int = field(default=0, converter=lambda _: 0)
+    n_consumers: tuple[int, int] = N_CONSUMERS
+    n_suppliers: tuple[int, int] = (0, 0)
+
+
+@define
+class EutopiaConsumerContext(EutopiaContext):
+    """An unrealistic context in which the agent is the only consumer and all suppliers are nice."""
+
+    level: int = field(default=-1, converter=lambda _: -1)
+    n_consumers: tuple[int, int] = (0, 0)
+    n_suppliers: tuple[int, int] = N_SUPPLIERS
+
+
+@define
 class FixedPartnerNumbersOneShotContext(FixedPartnerNumbersContext):
     ...
 
 
 @define
 class ANACContext(GeneralContext):
     """Generates a oneshot world with no constraints except compatibility with a specific ANAC competition year."""
```

### Comparing `scml-0.7.3/src/scml/oneshot/helper.py` & `scml-0.7.4/src/scml/oneshot/helper.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/mixins.py` & `scml-0.7.4/src/scml/oneshot/mixins.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/policy.py` & `scml-0.7.4/src/scml/oneshot/policy.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/rl/action.py` & `scml-0.7.4/src/scml/oneshot/rl/action.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/rl/agent.py` & `scml-0.7.4/src/scml/oneshot/rl/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/rl/common.py` & `scml-0.7.4/src/scml/oneshot/rl/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/rl/env.py` & `scml-0.7.4/src/scml/oneshot/rl/env.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/rl/helpers.py` & `scml-0.7.4/src/scml/oneshot/rl/helpers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/rl/observation.py` & `scml-0.7.4/src/scml/oneshot/rl/observation.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
                 assert all(
                     0 <= a < b for a, b in zip(v, space.nvec)
                 ), f"{offers=}\n{extra=}\n{v=}\n{space.nvec=}\n{space.nvec - v =}\n{ (awi.current_exogenous_input_quantity , awi.total_supplies , awi.total_sales , awi.current_exogenous_output_quantity) }"  # type: ignore
 
         return v
 
     def extra_obs(self, awi: OneShotAWI) -> list[tuple[float, int] | float]:
-        """ "
+        """
         The observation values other than offers and previous offers.
 
         Returns:
             A list of tuples. Each is some observation variable as a
             real number between zero and one and a number of bins to
             use for discrediting this variable. If a single value, the
             number of bins will be self.n_bin
```

### Comparing `scml-0.7.3/src/scml/oneshot/rl/policies.py` & `scml-0.7.4/src/scml/oneshot/rl/policies.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/rl/reward.py` & `scml-0.7.4/src/scml/oneshot/rl/reward.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/sysagents.py` & `scml-0.7.4/src/scml/oneshot/sysagents.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/ufun.py` & `scml-0.7.4/src/scml/oneshot/ufun.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/oneshot/world.py` & `scml-0.7.4/src/scml/oneshot/world.py`

 * *Files 0% similar despite different names*

```diff
@@ -926,16 +926,16 @@
             shortfall_penalty: A range to sample mean-shortfall penalty for all factories from
             storage_cost: A range to sample mean-storage costs fro all factories from (only used if perishable is False)
             disposal_cost_dev: A range to sample std. dev of disposal costs for all factories from
             shortfall_penalty_dev: A range to sample std. dev of shortfall penalty for all factories from
             storage_cost_dev: The standard deviation of storage cost relative to the mean price
             exogenous_price_dev: The standard deviation of exogenous contract prices relative to the mean price
             price_multiplier: A value to multiply with trading/catalog price to get the upper limit on prices for all negotiations
-            random_agent_types: If True, the final agent types used by the generato wil always be sampled from the given types.
-                                If False, this random sampling will only happin if len(agent_types) != n_agents.
+            random_agent_types: If True, the final agent types used by the generator will always be sampled from the given types.
+                                If False, this random sampling will only happen if len(agent_types) != n_agents.
             penalties_scale: What are `disposal_cost` and `shortfall_penalty` relative to.
                             There are four options: `trading`, `catalog` mean trading
                             and catalog prices of the product. `unit` means the unit
                             price in the contract and `none` means the `storage-cost`
                             and `shortfall_penalty` are absolute values (in money unit).
                             If not given will be read through the AWI
             exogenous_generation_method: the generation method. This is only for compatibility with SCML2020World and is not used.
```

### Comparing `scml-0.7.3/src/scml/runner.py` & `scml-0.7.4/src/scml/runner.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/__init__.py` & `scml-0.7.4/src/scml/scml2019/__init__.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/agent.py` & `scml-0.7.4/src/scml/scml2019/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/awi.py` & `scml-0.7.4/src/scml/scml2019/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/bank.py` & `scml-0.7.4/src/scml/scml2019/bank.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/common.py` & `scml-0.7.4/src/scml/scml2019/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/consumers.py` & `scml-0.7.4/src/scml/scml2019/consumers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/factory_managers/builtins.py` & `scml-0.7.4/src/scml/scml2019/factory_managers/builtins.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/helpers.py` & `scml-0.7.4/src/scml/scml2019/helpers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/insurance.py` & `scml-0.7.4/src/scml/scml2019/insurance.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/miners.py` & `scml-0.7.4/src/scml/scml2019/miners.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/schedulers.py` & `scml-0.7.4/src/scml/scml2019/schedulers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/simulators.py` & `scml-0.7.4/src/scml/scml2019/simulators.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/utils19.py` & `scml-0.7.4/src/scml/scml2019/utils19.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/visualizers.py` & `scml-0.7.4/src/scml/scml2019/visualizers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2019/world.py` & `scml-0.7.4/src/scml/scml2019/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/__init__.py` & `scml-0.7.4/src/scml/scml2020/__init__.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/agent.py` & `scml-0.7.4/src/scml/scml2020/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/agents/bcse.py` & `scml-0.7.4/src/scml/scml2020/agents/bcse.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/agents/decentralizing.py` & `scml-0.7.4/src/scml/scml2020/agents/decentralizing.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/agents/do_nothing.py` & `scml-0.7.4/src/scml/scml2020/agents/do_nothing.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/agents/indneg.py` & `scml-0.7.4/src/scml/scml2020/agents/indneg.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/agents/moving.py` & `scml-0.7.4/src/scml/scml2020/agents/moving.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/agents/random.py` & `scml-0.7.4/src/scml/scml2020/agents/random.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/agents/reactive.py` & `scml-0.7.4/src/scml/scml2020/agents/reactive.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/agents/satisficer.py` & `scml-0.7.4/src/scml/scml2020/agents/satisficer.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/awi.py` & `scml-0.7.4/src/scml/scml2020/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/common.py` & `scml-0.7.4/src/scml/scml2020/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/components/negotiation.py` & `scml-0.7.4/src/scml/scml2020/components/negotiation.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/components/prediction.py` & `scml-0.7.4/src/scml/scml2020/components/prediction.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/components/production.py` & `scml-0.7.4/src/scml/scml2020/components/production.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/components/signing.py` & `scml-0.7.4/src/scml/scml2020/components/signing.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/components/simulation.py` & `scml-0.7.4/src/scml/scml2020/components/simulation.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/components/trading.py` & `scml-0.7.4/src/scml/scml2020/components/trading.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/factory.py` & `scml-0.7.4/src/scml/scml2020/factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/services/controllers.py` & `scml-0.7.4/src/scml/scml2020/services/controllers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/services/simulators.py` & `scml-0.7.4/src/scml/scml2020/services/simulators.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/scml2020/world.py` & `scml-0.7.4/src/scml/scml2020/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/std/__init__.py` & `scml-0.7.4/src/scml/std/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Args:
         as_str: If true, the full type name will be returned otherwise the
                 type object itself.
     """
     from negmas.helpers import get_class
 
     types = [
-        f"scml.oneshot.agents.{_}"
+        f"scml.std.agents.{_}"
         for _ in agents.__all__
         if _ not in ("StdPlaceholder", "Placeholder", "OneShotDummyAgent")
     ]
     if as_str:
         return types
     return [get_class(_) for _ in types]
```

### Comparing `scml-0.7.3/src/scml/std/agent.py` & `scml-0.7.4/src/scml/std/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/std/agents/greedy.py` & `scml-0.7.4/src/scml/std/agents/greedy.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/std/agents/rand.py` & `scml-0.7.4/src/scml/std/agents/rand.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/std/awi.py` & `scml-0.7.4/src/scml/std/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/std/common.py` & `scml-0.7.4/src/scml/std/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/std/context.py` & `scml-0.7.4/src/scml/std/context.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/std/policy.py` & `scml-0.7.4/src/scml/std/policy.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/std/rl/env.py` & `scml-0.7.4/src/scml/std/rl/env.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/std/ufun.py` & `scml-0.7.4/src/scml/std/ufun.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/std/world.py` & `scml-0.7.4/src/scml/std/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/utils.py` & `scml-0.7.4/src/scml/utils.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/vendor/quick/LICENSE` & `scml-0.7.4/src/scml/vendor/quick/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/vendor/quick/README.md` & `scml-0.7.4/src/scml/vendor/quick/README.md`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml/vendor/quick/quick.py` & `scml-0.7.4/src/scml/vendor/quick/quick.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/src/scml.egg-info/PKG-INFO` & `scml-0.7.4/src/scml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scml
-Version: 0.7.3
+Version: 0.7.4
 Summary: ANAC Supply Chain Management League Platform
 Home-page: https://github.com/yasserfarouk/scml
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Project-URL: Documentation, https://scml.readthedocs.io/
 Project-URL: Changelog, https://scml.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/yasserfarouk/scml/issues
@@ -23,15 +23,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: click
 Requires-Dist: pytest
 Requires-Dist: hypothesis
-Requires-Dist: negmas>=0.10.18
+Requires-Dist: negmas>=0.10.20
 Requires-Dist: joblib
 Requires-Dist: jupyter
 Requires-Dist: gif
 Requires-Dist: gymnasium
 Provides-Extra: gui
 Requires-Dist: pyqt5; extra == "gui"
 
@@ -97,14 +97,28 @@
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 Changelog
 =========
 
+0.7.4 (2024.04.03)
+------------------
+
+* AWI: Correcting n_competitors and adding my_competitors
+* slightly faster random oneshot
+* bugfix in builtin_std_agents
+* Adding more contexts
+* Adding loading sklearn to FAQ
+
+0.7.3 (2024.03.15)
+------------------
+
+* Requiring negmas 0.10.18
+
 0.7.2 (2024.03.02)
 ------------------
 
 * requiring negmas >=0.10.17
 * minor bugfix correcting method name in 2022 version
 * correcting NMI type in some agents
 * bugfix CLI failed because "method" is not in World
```

### Comparing `scml-0.7.3/src/scml.egg-info/SOURCES.txt` & `scml-0.7.4/src/scml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/etc/test_can_run_tutorial2.py` & `scml-0.7.4/tests/etc/test_can_run_tutorial2.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/etc/test_cli.py` & `scml-0.7.4/tests/etc/test_cli.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/etc/test_jupyter.py` & `scml-0.7.4/tests/etc/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/old/test_factory2019.py` & `scml-0.7.4/tests/old/test_factory2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/old/test_scheduler2019.py` & `scml-0.7.4/tests/old/test_scheduler2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/old/test_scml2019.py` & `scml-0.7.4/tests/old/test_scml2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/old/test_scml2019factory.py` & `scml-0.7.4/tests/old/test_scml2019factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/old/test_scml2019tournaments.py` & `scml-0.7.4/tests/old/test_scml2019tournaments.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/oneshot/test_oneshot_do_nothing.py` & `scml-0.7.4/tests/oneshot/test_oneshot_do_nothing.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/oneshot/test_oneshot_sync.py` & `scml-0.7.4/tests/oneshot/test_oneshot_sync.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/oneshot/test_oneshot_ufun.py` & `scml-0.7.4/tests/oneshot/test_oneshot_ufun.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/oneshot/test_runner.py` & `scml-0.7.4/tests/oneshot/test_runner.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/oneshot/test_scml2021oneshot.py` & `scml-0.7.4/tests/oneshot/test_scml2021oneshot.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/oneshot/test_scml2023oneshot.py` & `scml-0.7.4/tests/oneshot/test_scml2023oneshot.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/oneshot/test_scml2024oneshot.py` & `scml-0.7.4/tests/oneshot/test_scml2024oneshot.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/oneshot/test_sync_jackson.py` & `scml-0.7.4/tests/oneshot/test_sync_jackson.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/rl/test_rl.py` & `scml-0.7.4/tests/rl/test_rl.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/std/test_std.py` & `scml-0.7.4/tests/std/test_std.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/std2020design/test_scml2020.py` & `scml-0.7.4/tests/std2020design/test_scml2020.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/std2020design/test_scml2020factory.py` & `scml-0.7.4/tests/std2020design/test_scml2020factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/std2020design/test_scml2020tournaments.py` & `scml-0.7.4/tests/std2020design/test_scml2020tournaments.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/std2020design/test_scml2021.py` & `scml-0.7.4/tests/std2020design/test_scml2021.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/std2020design/test_scml2021tournaments.py` & `scml-0.7.4/tests/std2020design/test_scml2021tournaments.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/std2020design/test_scml2023.py` & `scml-0.7.4/tests/std2020design/test_scml2023.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tests/switches.py` & `scml-0.7.4/tests/switches.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.3/tox.ini` & `scml-0.7.4/tox.ini`

 * *Files identical despite different names*

