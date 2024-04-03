# Comparing `tmp/linktools-0.8.2rc0.tar.gz` & `tmp/linktools-0.8.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktools-0.8.2rc0.tar", last modified: Sat Mar 30 15:13:58 2024, max compression
+gzip compressed data, was "linktools-0.8.3rc0.tar", last modified: Wed Apr  3 08:10:39 2024, max compression
```

## Comparing `linktools-0.8.2rc0.tar` & `linktools-0.8.3rc0.tar`

### file list

```diff
@@ -1,131 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.952578 linktools-0.8.2rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34580 2024-03-30 15:13:58.952578 linktools-0.8.2rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32666 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 15:13:58.952578 linktools-0.8.2rc0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4274 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.928578 linktools-0.8.2rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.932578 linktools-0.8.2rc0/src/linktools/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21195 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.936578 linktools-0.8.2rc0/src/linktools/android/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/android/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23927 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/android/adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/android/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.936578 linktools-0.8.2rc0/src/linktools/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-03-30 15:13:53.000000 linktools-0.8.2rc0/src/linktools/assets/android-tools.apk
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-30 15:13:53.000000 linktools-0.8.2rc0/src/linktools/assets/android-tools.json
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/chrome-driver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.928578 linktools-0.8.2rc0/src/linktools/assets/containers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.936578 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/http.conf
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/https.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.936578 linktools-0.8.2rc0/src/linktools/assets/containers/110-portainer/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/110-portainer/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/110-portainer/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/110-portainer/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/fake_useragent.json
--rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-03-30 15:12:01.000000 linktools-0.8.2rc0/src/linktools/assets/frida.js
--rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-03-30 15:12:01.000000 linktools-0.8.2rc0/src/linktools/assets/frida.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.928578 linktools-0.8.2rc0/src/linktools/assets/objection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/assets/objection/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/objection/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools/assets/tools.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    29492 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/cli/commands/android/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/adb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2637 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/objection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/pidcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/top.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/cli/commands/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/cntr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/grep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/shell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.944578 linktools-0.8.2rc0/src/linktools/cli/commands/ios/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/objection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.944578 linktools-0.8.2rc0/src/linktools/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/container/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21236 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/container/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/container/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.944578 linktools-0.8.2rc0/src/linktools/frida/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/android.py
--rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.944578 linktools-0.8.2rc0/src/linktools/ida/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ida/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.944578 linktools-0.8.2rc0/src/linktools/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ios/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.948578 linktools-0.8.2rc0/src/linktools/references/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.948578 linktools-0.8.2rc0/src/linktools/references/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.948578 linktools-0.8.2rc0/src/linktools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/utils/_lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/utils/_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/utils/_subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17177 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.948578 linktools-0.8.2rc0/src/linktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34580 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.478895 linktools-0.8.3rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34580 2024-04-03 08:10:39.478895 linktools-0.8.3rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32666 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:10:39.478895 linktools-0.8.3rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.454895 linktools-0.8.3rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.458895 linktools-0.8.3rc0/src/linktools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21599 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18049 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.458895 linktools-0.8.3rc0/src/linktools/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/android/adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/android/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.462895 linktools-0.8.3rc0/src/linktools/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-03 08:10:23.000000 linktools-0.8.3rc0/src/linktools/assets/android-tools.apk
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-03 08:10:23.000000 linktools-0.8.3rc0/src/linktools/assets/android-tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/chrome-driver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.454895 linktools-0.8.3rc0/src/linktools/assets/containers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.462895 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/http.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/https.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.462895 linktools-0.8.3rc0/src/linktools/assets/containers/110-portainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/110-portainer/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/110-portainer/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/110-portainer/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.462895 linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/fake_useragent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-04-03 08:08:17.000000 linktools-0.8.3rc0/src/linktools/assets/frida.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-03 08:08:17.000000 linktools-0.8.3rc0/src/linktools/assets/frida.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.454895 linktools-0.8.3rc0/src/linktools/assets/objection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.462895 linktools-0.8.3rc0/src/linktools/assets/objection/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/objection/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools/assets/tools.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.466895 linktools-0.8.3rc0/src/linktools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30240 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.466895 linktools-0.8.3rc0/src/linktools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.466895 linktools-0.8.3rc0/src/linktools/cli/commands/android/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/adb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/objection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/pidcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/top.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.466895 linktools-0.8.3rc0/src/linktools/cli/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/cntr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/grep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/cli/commands/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/objection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21272 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/container/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/container/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/frida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ida/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.474895 linktools-0.8.3rc0/src/linktools/references/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.474895 linktools-0.8.3rc0/src/linktools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/utils/_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/utils/_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/utils/_subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17283 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.474895 linktools-0.8.3rc0/src/linktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34580 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/top_level.txt
```

### Comparing `linktools-0.8.2rc0/LICENSE` & `linktools-0.8.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/PKG-INFO` & `linktools-0.8.3rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.2rc0
+Version: 0.8.3rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `linktools-0.8.2rc0/README.md` & `linktools-0.8.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/pyproject.toml` & `linktools-0.8.3rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/setup.py` & `linktools-0.8.3rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,16 +82,16 @@
         fd_out.write(
             template.render(
                 release="True" if release else "False",
                 version=version,
             )
         )
 
-    with open(get_path("dependencies.json"), "rt", encoding="utf-8") as fd:
-        data = json.load(fd)
+    with open(get_path("requirements.yml"), "rt", encoding="utf-8") as fd:
+        data = yaml.safe_load(fd)
         # install_requires = dependencies + dev-dependencies
         install_requires = data.get("dependencies")
         if not release:
             install_requires.extend(data.get("dev-dependencies"))
         # extras_require = optional-dependencies
         extras_require = data.get("optional-dependencies")
         all_requires = []
```

### Comparing `linktools-0.8.2rc0/src/linktools/__init__.py` & `linktools-0.8.3rc0/src/linktools/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/_config.py` & `linktools-0.8.3rc0/src/linktools/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,18 +109,19 @@
 
     def optionxform(self, optionstr: str):
         return optionstr
 
 
 class ConfigCacheParser:
 
-    def __init__(self, path: str, namespace: str):
+    def __init__(self, config: "Config"):
         self._parser = ConfigParser(default_section="ENV")  # 兼容老版本，默认ENV作为默认节
-        self._path = path
-        self._section = f"{namespace}.CACHE".upper()
+        self._path = config.cache_path
+        self._section = f"{config._namespace}.CACHE".upper()
+        self.load()
 
     def load(self):
         if self._path and os.path.exists(self._path):
             self._parser.read(self._path)
         if not self._parser.has_section(self._section):
             self._parser.add_section(self._section)
 
@@ -161,15 +162,15 @@
 
         if self._data != __missing__:
             return self._data
 
         type = type or self._type
         if self._cached:
             # load cache from config file
-            config_parser = config._get_cache_parser()
+            config_parser = ConfigCacheParser(config)
             config_cache = cache
             if config_cache == __missing__:
                 config_cache = config_parser.get(key, __missing__)
 
             # load config value
             result = self._load(config, key, config_cache)
             if isinstance(result, ConfigProperty):
@@ -265,26 +266,30 @@
         :param prefix: 环境变量前缀
         :param share: 是否共享配置
         """
         self._environ = environ
         self._config = config if share else pickle.loads(pickle.dumps(config))
         self._namespace = namespace if namespace != __missing__ else "MAIN"
         self._prefix = prefix.upper() if prefix != __missing__ else ""
-        self._cache = dict()
         self._reload = None
+        self._cache = dict()
         self._cache_path = self._environ.get_data_path(f"{self._environ.name}.cfg", create_parent=True)
         self.load_cache()
 
     @property
     def reload(self) -> bool:
         """
         是否重新加载配置
         """
         if self._reload is None:
-            self._reload = self.get("RELOAD_CONFIG", type=bool, default=False)
+            value = False
+            key = f"{self._prefix}RELOAD_CONFIG"
+            if key in os.environ:
+                value = self.cast(os.environ[key], type=bool)
+            self._reload = value
         return self._reload
 
     @reload.setter
     def reload(self, value: bool):
         """
         是否重新加载配置
         """
@@ -314,29 +319,32 @@
             if env_key in os.environ:
                 value = os.environ.get(env_key)
                 return self.cast(value, type=type)
 
             if key in self._cache:
                 value = self._cache.get(key)
                 prop = self._config.get(key, None)
-                if isinstance(prop, ConfigProperty) and prop.reloadable and self.reload:
-                    with self.__lock__:
-                        value = self._cache[key] = prop.load(self, key, type=type, cache=value)
-                else:
-                    value = self.cast(value, type=type)
-                return value
+                if self.reload:
+                    if isinstance(prop, ConfigProperty) and prop.reloadable:
+                        with self.__lock__:
+                            value = self._cache[key] = prop.load(self, key, type=type, cache=value)
+                            return value
+                    if isinstance(default, ConfigProperty) and default.reloadable:
+                        with self.__lock__:
+                            value = self._cache[key] = default.load(self, key, type=type, cache=value)
+                            return value
+                return self.cast(value, type=type)
 
             if key in self._config:
                 value = self._config.get(key)
                 if isinstance(value, ConfigProperty):
                     with self.__lock__:
                         value = self._cache[key] = value.load(self, key, type=type)
-                else:
-                    value = self.cast(value, type=type)
-                return value
+                        return value
+                return self.cast(value, type=type)
 
         except Exception as e:
             last_error = e
 
         if default == __missing__:
             if last_error != __missing__:
                 raise last_error
@@ -425,41 +433,48 @@
             return True
         # 剩下的就是需要递归读取所有文件的情况了
         for root, dirs, files in os.walk(path, topdown=False):
             for name in files:
                 self.update_from_file(os.path.join(root, name))
         return True
 
+    @property
+    def cache_path(self) -> str:
+        """
+        缓存文件路径
+        """
+        return self._cache_path
+
     def load_cache(self) -> None:
         """
         从缓存中加载配置
         """
-        parser = self._get_cache_parser()
+        parser = ConfigCacheParser(self)
         with self.__lock__:
             self._cache.clear()
             self._cache.update(parser.items())
 
     def save_cache(self, **kwargs: Any) -> None:
         """
         保存配置到缓存
         :param kwargs: 需要保存的配置
         """
-        parser = self._get_cache_parser()
+        parser = ConfigCacheParser(self)
         with self.__lock__:
             for key, value in kwargs.items():
                 self._cache[key] = value
                 parser.set(key, self.cast(value, type=str))
         parser.dump()
 
     def remove_cache(self, *keys: str) -> None:
         """
         删除缓存
         :param keys: 需要删除的缓存键
         """
-        parser = self._get_cache_parser()
+        parser = ConfigCacheParser(self)
         with self.__lock__:
             for key in keys:
                 self._cache.pop(key, None)
                 parser.remove(key)
         parser.dump()
 
     def __contains__(self, key) -> bool:
@@ -469,19 +484,14 @@
 
     def __getitem__(self, key: str) -> Any:
         return self.get(key)
 
     def __setitem__(self, key: str, value: Any):
         self.set(key, value)
 
-    def _get_cache_parser(self) -> ConfigCacheParser:
-        parser = ConfigCacheParser(self._cache_path, self._namespace)
-        parser.load()
-        return parser
-
     class Prompt(ConfigProperty):
 
         def __init__(
                 self,
                 prompt: str = None,
                 password: bool = False,
                 choices: Optional[List[str]] = None,
@@ -623,18 +633,18 @@
 
         def __init__(self, message: str = None):
             super().__init__()
             self.message = message
 
         def _load(self, config: "Config", key: str, cache: Any):
             message = self.message or \
-                f"Cannot find config \"{key}\". {os.linesep}" \
-                f"You can use any of the following methods to fix it: {os.linesep}" \
-                f"1. set \"{config._prefix}{key}\" as an environment variable, {os.linesep}" \
-                f"2. call config.save_cache method to save the value to file. {os.linesep}"
+                      f"Cannot find config \"{key}\". {os.linesep}" \
+                      f"You can use any of the following methods to fix it: {os.linesep}" \
+                      f"1. set \"{config._prefix}{key}\" as an environment variable, {os.linesep}" \
+                      f"2. call config.save_cache method to save the value to file. {os.linesep}"
             raise ConfigError(message)
 
 
 class ConfigWrapper(Config):
 
     def __init__(
             self,
```

### Comparing `linktools-0.8.2rc0/src/linktools/_environ.py` & `linktools-0.8.3rc0/src/linktools/_environ.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import abc
 import json
 import logging
 import os
 import pathlib
+import shutil
+import time
 from typing import TYPE_CHECKING, TypeVar, Type, Any
 
 from . import utils, metadata
 from .decorator import cached_property, cached_classproperty
 
 if TYPE_CHECKING:
     from ._config import ConfigDict, Config
@@ -107,30 +109,30 @@
         self.set_config("DEBUG", value)
 
     @cached_property
     def data_path(self) -> str:
         """
         存放文件目录
         """
-        prefix = f"{metadata.__name__}_".upper()
+        prefix = f"{metadata.__name__}".upper()
         path = os.environ.get(f"{prefix}_DATA_PATH", None)
         if path:  # 优先使用环境变量中的${DATA_PATH}
             return path
         path = os.environ.get(f"{prefix}_STORAGE_PATH", None)
         if path:  # 其次使用环境变量中的${STORAGE_PATH}/data
             return os.path.join(path, "data")
         # 最后使用默认路径${HOME}/.linktools/data
         return os.path.join(str(pathlib.Path.home()), f".{metadata.__name__}", "data")
 
     @cached_property
     def temp_path(self) -> str:
         """
         存放临时文件目录
         """
-        prefix = f"{metadata.__name__}_".upper()
+        prefix = f"{metadata.__name__}".upper()
         path = os.environ.get(f"{prefix}_TEMP_PATH", None)
         if path:  # 优先使用环境变量中的${TEMP_PATH}
             return path
         path = os.environ.get(f"{prefix}_STORAGE_PATH", None)
         if path:  # 其次使用环境变量中的${STORAGE_PATH}/temp
             return os.path.join(path, "temp")
         # 最后使用默认路径${HOME}/.linktools/temp
@@ -164,14 +166,43 @@
 
     def get_temp_dir(self, *paths: str, create: bool = False) -> str:
         """
         获取临时文件目录下的子目录
         """
         return utils.get_path(self.temp_path, *paths, create=create, create_parent=False)
 
+    def clean_temp_files(self, expire_days: int = 7) -> None:
+        """
+        清理临时文件
+        """
+        current_time = time.time()
+        target_time = current_time - expire_days * 24 * 60 * 60
+        for root, dirs, files in os.walk(self.temp_path, topdown=False):
+            for name in files:
+                path = os.path.join(root, name)
+                last_time = max(
+                    os.path.getatime(path),
+                    os.path.getctime(path),
+                    os.path.getmtime(path),
+                )
+                if last_time < target_time:
+                    self.logger.info(f"Remove expired temp file: {path}")
+                    os.remove(path)
+            for name in dirs:
+                path = os.path.join(root, name)
+                if os.path.exists(path) and not os.listdir(path):
+                    last_time = max(
+                        os.path.getatime(path),
+                        os.path.getctime(path),
+                        os.path.getmtime(path),
+                    )
+                    if last_time < target_time:
+                        self.logger.info(f"Remove empty temp directory: {path}")
+                        shutil.rmtree(path, ignore_errors=True)
+
     @cached_classproperty
     def _log_manager(self) -> logging.Manager:
 
         empty_args = tuple()
 
         class Logger(logging.Logger):
```

### Comparing `linktools-0.8.2rc0/src/linktools/_tools.py` & `linktools-0.8.3rc0/src/linktools/_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,25 +358,25 @@
         if not utils.is_empty(self.unpack_path):
             self._container.logger.debug(f"Delete {self.root_path}")
             shutil.rmtree(self.root_path, ignore_errors=True)
         elif self.absolute_path.startswith(self.root_path):
             self._container.logger.debug(f"Delete {self.absolute_path}")
             os.remove(self.absolute_path)
 
-    def popen(self, *args: [Any], **kwargs) -> utils.Popen:
+    def popen(self, *args: [Any], **kwargs) -> utils.Process:
         self.prepare()
 
         # java or other
         executable_cmdline = self.executable_cmdline
         if executable_cmdline[0] in self._container.items:
             args = [*executable_cmdline[1:], *args]
             tool = self._container.items[executable_cmdline[0]]
             return tool.popen(*args, **kwargs)
 
-        return utils.Popen(*[*executable_cmdline, *args], **kwargs)
+        return utils.Process(*[*executable_cmdline, *args], **kwargs)
 
     @utils.timeoutable
     def exec(
             self,
             *args: [Any],
             timeout: utils.Timeout = None,
             ignore_errors: bool = False,
```

### Comparing `linktools-0.8.2rc0/src/linktools/_url.py` & `linktools-0.8.3rc0/src/linktools/_url.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/android/__init__.py` & `linktools-0.8.3rc0/src/linktools/android/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/android/adb.py` & `linktools-0.8.3rc0/src/linktools/android/adb.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     def uid(self) -> int:
         """
         获取shell的uid
         :return: uid
         """
         return self.get_uid()
 
-    def popen(self, *args: [Any], **kwargs) -> utils.Popen:
+    def popen(self, *args: [Any], **kwargs) -> utils.Process:
         """
         执行命令
         :param args: 命令行参数
         :return: 打开的进程
         """
         args = ["-s", self.id, *args]
         return self._adb.popen(*args, **kwargs)
```

### Comparing `linktools-0.8.2rc0/src/linktools/android/struct.py` & `linktools-0.8.3rc0/src/linktools/android/struct.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/android-tools.apk` & `linktools-0.8.3rc0/src/linktools/assets/android-tools.apk`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/android-tools.json` & `linktools-0.8.3rc0/src/linktools/assets/android-tools.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'ANDROID_TOOL_BRIDGE_APK'": "{'time': '2024-04-03 16:10:23'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "ANDROID_TOOL_BRIDGE_APK": {
         "main": "android.tools.Main",
         "md5": "6a8c9cfb8555846bee1b972b63331027",
         "name": "android-tools.apk",
         "size": 82987,
-        "time": "2024-03-30 23:13:53"
+        "time": "2024-04-03 16:10:23"
     },
     "ANDROID_TOOL_FRIDA_SERVER": [
         {
             "min_version": "15.1.8",
             "name": "strong-frida-server-{version}-android-{abi}",
             "url": "https://github.com/hzzheyang/strongR-frida-android/releases/download/{version}/hluda-server-{version}-android-{abi}.xz"
         },
```

### Comparing `linktools-0.8.2rc0/src/linktools/assets/chrome-driver.json` & `linktools-0.8.3rc0/src/linktools/assets/chrome-driver.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/Dockerfile` & `linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/Dockerfile`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/container.py` & `linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt` & `linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/containers/110-portainer/container.py` & `linktools-0.8.3rc0/src/linktools/assets/containers/110-portainer/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/compose.yml` & `linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/compose.yml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/container.py` & `linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/nginx.conf` & `linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/nginx.conf`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/fake_useragent.json` & `linktools-0.8.3rc0/src/linktools/assets/fake_useragent.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/frida.js` & `linktools-0.8.3rc0/src/linktools/assets/frida.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/frida.min.js` & `linktools-0.8.3rc0/src/linktools/assets/frida.min.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/objection/plugins/__init__.py` & `linktools-0.8.3rc0/src/linktools/assets/objection/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/assets/tools.json` & `linktools-0.8.3rc0/src/linktools/assets/tools.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/__init__.py` & `linktools-0.8.3rc0/src/linktools/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,14 @@
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 from . import argparse
 
 from .command import \
-    BaseCommand, CommandError, \
+    BaseCommand, BaseCommandGroup, CommandError, \
     SubCommand, SubCommandGroup, SubCommandWrapper, \
     subcommand, subcommand_argument, SubCommandError
 
 from .device import \
     DeviceCommandMixin, AndroidCommandMixin, IOSCommandMixin, \
     AndroidCommand, IOSCommand
```

### Comparing `linktools-0.8.2rc0/src/linktools/cli/argparse.py` & `linktools-0.8.3rc0/src/linktools/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/command.py` & `linktools-0.8.3rc0/src/linktools/cli/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,65 +60,14 @@
     pass
 
 
 class SubCommandError(CommandError):
     pass
 
 
-class LogCommandMixin:
-
-    def add_log_options(self: "BaseCommand", parser: ArgumentParser = None):
-
-        environ = self.environ
-        parser = parser or self._argument_parser
-
-        class VerboseAction(Action):
-
-            def __call__(self, parser, namespace, values, option_string=None):
-                logging.root.setLevel(logging.DEBUG)
-
-        class DebugAction(Action):
-
-            def __call__(self, parser, namespace, values, option_string=None):
-                environ.debug = True
-                environ.logger.setLevel(logging.DEBUG)
-
-        class LogTimeAction(BooleanOptionalAction):
-
-            def __call__(self, parser, namespace, values, option_string=None):
-                if option_string in self.option_strings:
-                    value = not option_string.startswith("--no-")
-                    handler = LogHandler.get_instance()
-                    if handler:
-                        handler.show_time = value
-                    environ.set_config("SHOW_LOG_TIME", value)
-
-        class LogLevelAction(BooleanOptionalAction):
-
-            def __call__(self, parser, namespace, values, option_string=None):
-                if option_string in self.option_strings:
-                    value = not option_string.startswith("--no-")
-                    handler = LogHandler.get_instance()
-                    if handler:
-                        handler.show_level = value
-                    environ.set_config("SHOW_LOG_LEVEL", value)
-
-        group = parser.add_argument_group(title="log options")
-        group.add_argument("--verbose", action=VerboseAction, nargs=0, const=True, dest=SUPPRESS,
-                           help="increase log verbosity")
-        group.add_argument("--debug", action=DebugAction, nargs=0, const=True, dest=SUPPRESS,
-                           help=f"increase {self.environ.name}'s log verbosity, and enable debug mode")
-
-        if LogHandler.get_instance():
-            group.add_argument("--time", action=LogTimeAction, dest=SUPPRESS,
-                               help="show log time")
-            group.add_argument("--level", action=LogLevelAction, dest=SUPPRESS,
-                               help="show log level")
-
-
 def _filter_kwargs(kwargs):
     return {k: v for k, v in kwargs.items() if v != __missing__}
 
 
 _subcommand_index: int = 0
 _subcommand_map: Dict[str, Set[str]] = {}
 
@@ -174,14 +123,15 @@
         conflict_handler: str = __missing__,
         add_help: bool = __missing__,
         allow_abbrev: bool = __missing__,
         pass_args: bool = False):
     """
     子命令装饰器
     """
+
     def decorator(func):
         if not hasattr(func, "__subcommand_info__"):
             setattr(func, "__subcommand_info__", _SubCommandMethodInfo())
 
         subcommand_info = func.__subcommand_info__
         subcommand_info.func = func
         subcommand_info.pass_args = pass_args
@@ -236,14 +186,15 @@
         nargs: Union[int, str] = __missing__,
         required: bool = __missing__,
         type: "Union[Type[Union[int, float, str]], Callable[[str], T], FileType]" = __missing__,
         **kwargs: Any):
     """
     子命令参数装饰器，与@subcommand配合使用
     """
+
     def decorator(func):
         subcommand_argument_info = _SubCommandMethodArgumentInfo()
         subcommand_argument_info.set_args(
             *[name_or_flag, *name_or_flags],
             action=action,
             nargs=nargs,
             const=const,
@@ -543,14 +494,15 @@
             if subcommand.has_parent:
                 parent_subparsers = subparsers_map.get(subcommand.parent_id, None)
                 if not parent_subparsers:
                     raise SubCommandError(f"Subcommand {subcommand} has no parent subparser")
 
             parser = subcommand.create_parser(type=parent_subparsers.add_parser)
             parser.set_defaults(**{f"__subcommand_{id(self):x}__": subcommand})
+            self.init_common_arguments(parser)
 
             if subcommand.is_group:
                 _subparsers = parser.add_subparsers(metavar="COMMAND", help="Command Help")
                 _subparsers.required = False
                 subparsers_map[subcommand.id] = _subparsers
 
             # BaseCommand 类型单独处理，因为有可能在init_arguments中添加了子命令
@@ -656,15 +608,15 @@
             if info.children:
                 current_max_level = max_level - current_node_level if max_level is not None else None
                 self._make_subcommand_tree(current_node, info.children, SubCommand.ROOT_ID, current_max_level)
 
         return tree
 
 
-class BaseCommand(LogCommandMixin, SubCommandMixin, metaclass=abc.ABCMeta):
+class BaseCommand(SubCommandMixin, metaclass=abc.ABCMeta):
 
     @property
     def name(self):
         """
         命令名
         """
         name = self.__module__
@@ -697,14 +649,28 @@
     @property
     def known_errors(self) -> List[Type[BaseException]]:
         """
         已知错误类型
         """
         return [CommandError]
 
+    @abc.abstractmethod
+    def init_arguments(self, parser: ArgumentParser) -> None:
+        """
+        初始化参数，在调用create_parser时执行
+        """
+        pass
+
+    @abc.abstractmethod
+    def run(self, args: Namespace) -> Optional[int]:
+        """
+        业务逻辑入口
+        """
+        pass
+
     def create_parser(
             self,
             *args: Any,
             type: Callable[..., ArgumentParser] = ArgumentParser,
             formatter_class: Type[HelpFormatter] = RawDescriptionHelpFormatter,
             conflict_handler="resolve",
             **kwargs: Any
@@ -727,35 +693,78 @@
         )
         self.init_base_arguments(parser)
         self.init_arguments(parser)
         return parser
 
     @cached_property
     def _argument_parser(self) -> ArgumentParser:
-        return self.create_parser()
+        parser = self.create_parser()
+        self.init_common_arguments(parser)
+        return parser
 
     def init_base_arguments(self, parser: ArgumentParser) -> None:
         """
         初始化基础参数，在调用create_parser时执行
         """
         pass
 
-    @abc.abstractmethod
-    def init_arguments(self, parser: ArgumentParser) -> None:
+    def init_common_arguments(self, parser: ArgumentParser) -> None:
         """
-        初始化参数，在调用create_parser时执行
+        初始化公共参数，会在命令本身和所有子命令中调用
         """
-        pass
+        environ = self.environ
+        prefix = parser.prefix_chars
 
-    @abc.abstractmethod
-    def run(self, args: Namespace) -> Optional[int]:
-        """
-        业务逻辑入口
-        """
-        pass
+        class VerboseAction(Action):
+
+            def __call__(self, parser, namespace, values, option_string=None):
+                logging.root.setLevel(logging.DEBUG)
+
+        class DebugAction(Action):
+
+            def __call__(self, parser, namespace, values, option_string=None):
+                environ.debug = True
+                environ.logger.setLevel(logging.DEBUG)
+
+        class LogTimeAction(BooleanOptionalAction):
+
+            def __call__(self, parser, namespace, values, option_string=None):
+                if option_string in self.option_strings:
+                    value = not option_string.startswith("--no-")
+                    handler = LogHandler.get_instance()
+                    if handler:
+                        handler.show_time = value
+                    environ.set_config("SHOW_LOG_TIME", value)
+
+        class LogLevelAction(BooleanOptionalAction):
+
+            def __call__(self, parser, namespace, values, option_string=None):
+                if option_string in self.option_strings:
+                    value = not option_string.startswith("--no-")
+                    handler = LogHandler.get_instance()
+                    if handler:
+                        handler.show_level = value
+                    environ.set_config("SHOW_LOG_LEVEL", value)
+
+        group = parser.add_argument_group(title="log options")
+        group.add_argument(f"{prefix}{prefix}verbose", action=VerboseAction, nargs=0, const=True, dest=SUPPRESS,
+                           help="increase log verbosity")
+        group.add_argument(f"{prefix}{prefix}debug", action=DebugAction, nargs=0, const=True, dest=SUPPRESS,
+                           help=f"increase {self.environ.name}'s log verbosity, and enable debug mode")
+
+        if LogHandler.get_instance():
+            group.add_argument(f"{prefix}{prefix}time", action=LogTimeAction, dest=SUPPRESS,
+                               help="show log time")
+            group.add_argument(f"{prefix}{prefix}level", action=LogLevelAction, dest=SUPPRESS,
+                               help="show log level")
+
+        if self.environ.version != NotImplemented:
+            parser.add_argument(
+                f"{prefix}{prefix}version", action="version", version=self.environ.version
+            )
 
     def main(self, *args, **kwargs) -> None:
         """
         main命令入口
         """
         if is_terminal():
             logging.basicConfig(
@@ -767,42 +776,35 @@
         else:
             logging.basicConfig(
                 level=logging.INFO,
                 format="[%(asctime)s] %(levelname)s %(module)s %(funcName)s %(message)s",
                 datefmt="%H:%M:%S"
             )
 
-        self.add_log_options()
-
-        if self.environ.version != NotImplemented:
-            self._argument_parser.add_argument(
-                "--version", action="version", version=self.environ.version
-            )
-
         try:
-            exit_code = self(*args, **kwargs)
+            result = self(*args, **kwargs)
         except SystemExit as e:
-            exit_code = e.code
+            result = e.code
 
         except (KeyboardInterrupt, EOFError) as e:
-            exit_code = 1
+            result = 1
             error_type, error_message = e.__class__.__name__, str(e).strip()
             self.logger.error(
                 f"{error_type}: {error_message}" if error_message else error_type,
             )
 
         except:
-            exit_code = 1
+            result = 1
             if environ.debug:
                 console = get_console()
                 console.print_exception(show_locals=True)
             else:
                 self.logger.error(traceback.format_exc())
 
-        exit(exit_code)
+        exit(result)
 
     def __call__(self, args: Union[List[str], Namespace] = None) -> int:
         """
         内部调用命令入口
         """
         try:
             if not isinstance(args, Namespace):
@@ -821,7 +823,25 @@
             error_type, error_message = e.__class__.__name__, str(e).strip()
             self.logger.error(
                 f"{error_type}: {error_message}" if error_message else error_type,
                 exc_info=True if environ.debug else None,
             )
 
         return exit_code
+
+
+class BaseCommandGroup(BaseCommand, metaclass=abc.ABCMeta):
+
+    def init_subcommands(self) -> Any:
+        return self
+
+    def init_arguments(self, parser: ArgumentParser) -> None:
+        self.add_subcommands(
+            parser=parser,
+            target=self.walk_subcommands(self.init_subcommands())
+        )
+
+    def run(self, args: Namespace) -> Optional[int]:
+        subcommand = self.parse_subcommand(args)
+        if not subcommand or subcommand.is_group:
+            return self.print_subcommands(args, subcommand, max_level=2)
+        return subcommand.run(args)
```

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/android/adb.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/android/agent.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/android/agent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/android/app.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/android/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/android/debug.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/android/debug.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         device.shell("am", "force-stop", args.package, log_output=True)
         device.shell("am", "start", "-D", "-n", "{}/{}".format(args.package, args.activity), log_output=True)
 
         pid = utils.int(device.shell("top", "-n", "1", "|", "grep", args.package).split()[0])
         with device.forward(f"tcp:{args.port}", f"jdwp:{pid}"):
             data = input("jdb connect? [Y/n]: ").strip()
             if data in ["", "Y", "y"]:
-                process = utils.Popen("jdb", "-connect",
-                                      "com.sun.jdi.SocketAttach:hostname=127.0.0.1,port={}".format(args.port))
+                process = utils.Process(
+                    "jdb", "-connect", f"com.sun.jdi.SocketAttach:hostname=127.0.0.1,port={args.port}")
                 return process.call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/android/frida.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/android/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/android/info.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/android/info.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/android/intent.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/android/intent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/android/objection.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/android/objection.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             if args.redirect_address or args.redirect_port:
                 # 如果需要重定向到本地端口
                 address = args.redirect_address
                 port = args.redirect_port or 8080
                 info = device.get_package(package)
                 uid = info.user_id if info else None
                 with device.redirect(address, port, uid):
-                    return utils.Popen(*objection_args).call()
+                    return utils.Process(*objection_args).call()
             else:
-                return utils.Popen(*objection_args).call()
+                return utils.Process(*objection_args).call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/android/pidcat.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/android/pidcat.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/android/top.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/android/top.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/common/cert.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/common/cert.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/common/cntr.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/common/cntr.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,44 +24,36 @@
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import Namespace, ArgumentParser
 from subprocess import SubprocessError
-from typing import Optional, List, Type, Dict, Tuple
+from typing import Optional, List, Type, Dict, Tuple, Any
 
 import yaml
 from git import GitCommandError
 
 from linktools import environ, ConfigError, utils
-from linktools.cli import BaseCommand, subcommand, SubCommandWrapper, subcommand_argument, SubCommandGroup
+from linktools.cli import BaseCommand, subcommand, SubCommandWrapper, subcommand_argument, SubCommandGroup, \
+    BaseCommandGroup
 from linktools.cli.argparse import KeyValueAction
 from linktools.container import ContainerManager, ContainerError
 from linktools.rich import confirm, choose
 
 manager = ContainerManager(environ)
 
 
-class RepoCommand(BaseCommand):
+class RepoCommand(BaseCommandGroup):
     """manage container repository"""
 
     @property
     def name(self):
         return "repo"
 
-    def init_arguments(self, parser: ArgumentParser) -> None:
-        self.add_subcommands(parser)
-
-    def run(self, args: Namespace) -> Optional[int]:
-        subcommand = self.parse_subcommand(args)
-        if not subcommand:
-            return self.print_subcommands(args)
-        return subcommand.run(args)
-
     @subcommand("list", help="list repositories")
     def on_command_list(self):
         repos = manager.get_all_repos()
         for key, value in repos.items():
             data = {key: value}
             self.logger.info(
                 yaml.dump(data, sort_keys=False).strip()
@@ -126,31 +118,36 @@
     @subcommand_argument("configs", action=KeyValueAction, nargs="+", help="container config key=value")
     def on_command_set(self, configs: Dict[str, str]):
         manager.config.save_cache(**configs)
         for key in sorted(configs.keys()):
             value = manager.config.get(key)
             self.logger.info(f"{key}: {value}")
 
-    @subcommand("remove", help="remove container configs")
-    @subcommand_argument("keys", metavar="KEY", nargs="+", help="container config keys")
-    def on_command_remove(self, keys: List[str]):
-        manager.config.remove_cache(*keys)
-        self.logger.info(f"Remove {', '.join(keys)} success")
+    @subcommand("unset", help="remove container configs")
+    @subcommand_argument("configs", action=KeyValueAction, metavar="KEY", nargs="+", help="container config keys")
+    def on_command_remove(self, configs: Dict[str, str]):
+        manager.config.remove_cache(*configs)
+        self.logger.info(f"Unset {', '.join(configs)} success")
 
     @subcommand("list", help="list container configs")
     def on_command_list(self):
         keys = set()
         for container in manager.prepare_installed_containers():
             keys.update(container.configs.keys())
-            if hasattr(container, "keys") and isinstance(container.keys, (Tuple, List)):
+            if hasattr(container, "keys") and isinstance(container.keys, (Tuple, List, Dict)):
                 keys.update([key for key in container.keys if key in manager.config])
         for key in sorted(keys):
             value = manager.config.get(key)
             self.logger.info(f"{key}: {value}")
 
+    @subcommand("edit", help="edit the config file in an editor")
+    @subcommand_argument("--editor", help="editor to use to edit the file")
+    def on_command_edit(self, editor: str):
+        return manager.create_process(editor, manager.config.cache_path).call()
+
     @subcommand("reload", help="reload container configs")
     def on_command_reload(self):
         manager.config.reload = True
         manager.prepare_installed_containers()
 
 
 class ExecCommand(BaseCommand):
@@ -191,55 +188,44 @@
         exec_args = parser.parse_args(exec_args)
         subcommand = self.parse_subcommand(exec_args)
         if not subcommand or isinstance(subcommand, SubCommandGroup):
             return self.print_subcommands(exec_args, root=subcommand, max_level=2)
         return subcommand.run(exec_args)
 
 
-class Command(BaseCommand):
+class Command(BaseCommandGroup):
     """
     Deploy docker/pod containers
     """
 
     @property
     def known_errors(self) -> List[Type[BaseException]]:
         known_errors = super().known_errors
         known_errors.extend([ContainerError, ConfigError, SubprocessError, GitCommandError, OSError])
         return known_errors
 
-    def init_arguments(self, parser: ArgumentParser) -> None:
-        subcommands = [
-            *self.walk_subcommands(self),
+    def init_subcommands(self) -> Any:
+        return [
+            self,
             SubCommandWrapper(ExecCommand()),
             SubCommandWrapper(ConfigCommand()),
             SubCommandWrapper(RepoCommand()),
         ]
 
-        self.add_subcommands(parser, target=subcommands)
-
-    def run(self, args: Namespace) -> Optional[int]:
-        subcommand = self.parse_subcommand(args)
-        if not subcommand or isinstance(subcommand, SubCommandGroup):
-            return self.print_subcommands(args, root=subcommand, max_level=2)
-        return subcommand.run(args)
-
     @subcommand("list", help="list all containers")
     def on_command_list(self):
         installed_containers = manager.get_installed_containers()
         depend_containers = manager.resolve_depend_containers(installed_containers)
         for container in sorted(manager.containers.values(), key=lambda o: o.order):
-            if container in depend_containers:
-                if not container.enable:
-                    self.logger.info(f"[ ] {container.name}", extra={"style": "dim"})
-                elif container in installed_containers:
-                    self.logger.info(f"[*] {container.name} [added]", extra={"style": "red bold"})
-                else:
-                    self.logger.info(f"[-] {container.name} [dependency]", extra={"style": "red dim"})
-            else:
+            if container not in depend_containers or not container.enable:
                 self.logger.info(f"[ ] {container.name}", extra={"style": "dim"})
+            elif container in installed_containers:
+                self.logger.info(f"[*] {container.name} [added]", extra={"style": "red bold"})
+            else:
+                self.logger.info(f"[-] {container.name} [dependency]", extra={"style": "red dim"})
 
     @subcommand("add", help="add containers to installed list")
     @subcommand_argument("names", metavar="CONTAINER", nargs="+", help="container name",
                          choices=utils.lazy_load(lambda: [o.name for o in manager.containers.values()]))
     def on_command_add(self, names: List[str]):
         containers = manager.add_installed_containers(*names)
         if not containers:
```

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/common/grep.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/common/grep.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/common/shell.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/common/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,20 +37,20 @@
                 self._shell_path = os.environ["ComSpec"]
 
     def init_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument("-c", "--command", action="store", default=None, help="shell command")
 
     def run(self, args: Namespace) -> Optional[int]:
         if args.command:
-            process = utils.Popen(args.command, shell=True)
+            process = utils.Process(args.command, shell=True)
             return process.call()
 
         if not self._shell_path or not os.path.exists(self._shell_path):
             raise NotImplementedError(f"unsupported system {environ.system}")
 
-        process = utils.Popen(self._shell_path)
+        process = utils.Process(self._shell_path)
         return process.call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/common/tools.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/common/tools.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/ios/frida.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/ios/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/ios/ipa.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/ios/objection.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/ios/objection.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,13 +82,13 @@
             if args.file_commands:
                 objection_args += ["--file-commands", args.file_commands]
             if args.startup_script:
                 objection_args += ["--startup-script", args.startup_script]
             if args.plugin_folder:
                 objection_args += ["--plugin-folder", args.plugin_folder]
 
-            return utils.Popen(*objection_args).call()
+            return utils.Process(*objection_args).call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/ios/scp.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/ios/scp.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/ios/sib.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/commands/ios/ssh.py` & `linktools-0.8.3rc0/src/linktools/cli/commands/ios/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/cli/device.py` & `linktools-0.8.3rc0/src/linktools/cli/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -120,14 +120,16 @@
 
 
 class DeviceCommandMixin:
 
     def add_device_options(self: "BaseCommand", parser: ArgumentParser):
 
         parser = parser or self._argument_parser
+        prefix = parser.prefix_chars
+
         cache = DeviceCache(
             self.environ.get_temp_path(
                 "cache", "device", "mobile",
                 create_parent=True
             )
         )
 
@@ -186,25 +188,27 @@
                 device_parser = DevicePicker.copy_on_write(namespace, self.dest)
                 device_parser.func = pick
 
         option_group = parser.add_argument_group(title="mobile device options")
         option_group.set_defaults(device_picker=DevicePicker(pick))
 
         device_group = option_group.add_mutually_exclusive_group()
-        device_group.add_argument("-i", "--id", metavar="ID", dest="device_picker", action=IDAction,
-                                  help="specify unique device identifier")
-        device_group.add_argument("-l", "--last", dest="device_picker", nargs=0, const=True, action=LastAction,
-                                  help="use last device")
+        device_group.add_argument(f"{prefix}i", f"{prefix}{prefix}id", metavar="ID", dest="device_picker",
+                                  action=IDAction, help="specify unique device identifier")
+        device_group.add_argument(f"{prefix}l", f"{prefix}{prefix}last", dest="device_picker", nargs=0, const=True,
+                                  action=LastAction, help="use last device")
 
 
 class AndroidCommandMixin:
 
     def add_android_options(self: BaseCommand, parser: ArgumentParser) -> None:
 
         parser = parser or self._argument_parser
+        prefix = parser.prefix_chars
+
         cache = DeviceCache(
             self.environ.get_temp_path(
                 "cache", "device", "android",
                 create_parent=True
             )
         )
 
@@ -302,44 +306,46 @@
                     device_parser.options.extend(values)
                 else:
                     device_parser.options.append(str(values))
 
         option_group = parser.add_argument_group(title="adb options")
         option_group.set_defaults(device_picker=AndroidPicker(pick))
 
-        option_group.add_argument("-a", "--all-interfaces", dest="device_picker", nargs=0, action=OptionAction,
+        option_group.add_argument(f"{prefix}a", f"{prefix}{prefix}all-interfaces", dest="device_picker", nargs=0, action=OptionAction,
                                   help="listen on all network interfaces, not just localhost (adb -a option)")
 
         device_group = option_group.add_mutually_exclusive_group()
-        device_group.add_argument("-d", "--device", dest="device_picker", nargs=0, action=DeviceAction,
+        device_group.add_argument(f"{prefix}d", f"{prefix}{prefix}device", dest="device_picker", nargs=0, action=DeviceAction,
                                   help="use USB device (adb -d option)")
-        device_group.add_argument("-s", "--serial", metavar="SERIAL", dest="device_picker", action=SerialAction,
+        device_group.add_argument(f"{prefix}s", f"{prefix}{prefix}serial", metavar="SERIAL", dest="device_picker", action=SerialAction,
                                   help="use device with given serial (adb -s option)")
-        device_group.add_argument("-e", "--emulator", dest="device_picker", nargs=0, action=EmulatorAction,
+        device_group.add_argument(f"{prefix}e", f"{prefix}{prefix}emulator", dest="device_picker", nargs=0, action=EmulatorAction,
                                   help="use TCP/IP device (adb -e option)")
-        device_group.add_argument("-c", "--connect", metavar="IP[:PORT]", dest="device_picker", action=ConnectAction,
+        device_group.add_argument(f"{prefix}c", f"{prefix}{prefix}connect", metavar="IP[:PORT]", dest="device_picker", action=ConnectAction,
                                   help="use device with TCP/IP")
-        device_group.add_argument("-l", "--last", dest="device_picker", nargs=0, action=LastAction,
+        device_group.add_argument(f"{prefix}l", f"{prefix}{prefix}last", dest="device_picker", nargs=0, action=LastAction,
                                   help="use last device")
 
-        option_group.add_argument("-t", "--transport", metavar="ID", dest="device_picker", action=OptionAction,
+        option_group.add_argument(f"{prefix}t", f"{prefix}{prefix}transport", metavar="ID", dest="device_picker", action=OptionAction,
                                   help="use device with given transport ID (adb -t option)")
-        option_group.add_argument("-H", metavar="HOST", dest="device_picker", action=OptionAction,
+        option_group.add_argument(f"{prefix}H", metavar="HOST", dest="device_picker", action=OptionAction,
                                   help="name of adb server host [default=localhost] (adb -H option)")
-        option_group.add_argument("-P", metavar="PORT", dest="device_picker", action=OptionAction,
+        option_group.add_argument(f"{prefix}P", metavar="PORT", dest="device_picker", action=OptionAction,
                                   help="port of adb server [default=5037] (adb -P option)")
-        option_group.add_argument("-L", metavar="SOCKET", dest="device_picker", action=OptionAction,
+        option_group.add_argument(f"{prefix}L", metavar="SOCKET", dest="device_picker", action=OptionAction,
                                   help="listen on given socket for adb server [default=tcp:localhost:5037] (adb -L option)")
 
 
 class IOSCommandMixin:
 
     def add_ios_options(self: BaseCommand, parser: ArgumentParser):
 
         parser = parser or self._argument_parser
+        prefix = parser.prefix_chars
+
         cache = DeviceCache(
             self.environ.get_temp_path(
                 "cache", "device", "ios",
                 create_parent=True
             )
         )
 
@@ -406,19 +412,19 @@
                 device_parser = IOSPicker.copy_on_write(namespace, self.dest)
                 device_parser.func = pick
 
         option_group = parser.add_argument_group(title="sib options")
         option_group.set_defaults(device_picker=IOSPicker(pick))
 
         device_group = option_group.add_mutually_exclusive_group()
-        device_group.add_argument("-u", "--udid", metavar="UDID", dest="device_picker", action=UdidAction,
+        device_group.add_argument(f"{prefix}u", f"{prefix}{prefix}udid", metavar="UDID", dest="device_picker", action=UdidAction,
                                   help="specify unique device identifier")
-        device_group.add_argument("-c", "--connect", metavar="IP:PORT", dest="device_picker", action=ConnectAction,
+        device_group.add_argument(f"{prefix}c", f"{prefix}{prefix}connect", metavar="IP:PORT", dest="device_picker", action=ConnectAction,
                                   help="use device with TCP/IP")
-        device_group.add_argument("-l", "--last", dest="device_picker", nargs=0, const=True, action=LastAction,
+        device_group.add_argument(f"{prefix}l", f"{prefix}{prefix}last", dest="device_picker", nargs=0, const=True, action=LastAction,
                                   help="use last device")
 
 
 class AndroidNamespace(Namespace):
     device_picker: AndroidPicker = None
```

### Comparing `linktools-0.8.2rc0/src/linktools/container/__init__.py` & `linktools-0.8.3rc0/src/linktools/container/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/container/container.py` & `linktools-0.8.3rc0/src/linktools/container/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/container/manager.py` & `linktools-0.8.3rc0/src/linktools/container/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,26 +352,26 @@
         )
 
     def create_process(
             self,
             *args,
             privilege: bool = None,
             **kwargs
-    ) -> utils.Popen:
+    ) -> utils.Process:
         if privilege:
             if self.system in ("darwin", "linux") and self.uid != 0:
                 args = ["sudo", *args]
-        return utils.Popen(*args, **kwargs)
+        return utils.Process(*args, **kwargs)
 
     def create_docker_process(
             self,
             *args,
             privilege: bool = None,
             **kwargs
-    ) -> utils.Popen:
+    ) -> utils.Process:
         commands = []
         if self.container_type in ("docker", "docker-rootless"):
             commands.extend(["docker"])
             if privilege is None:
                 privilege = self.container_type == "docker"
         elif self.container_type == "podman":
             commands.extend(["podman"])
@@ -381,15 +381,15 @@
 
     def create_docker_compose_process(
             self,
             containers: List[BaseContainer],
             *args: str,
             privilege: bool = None,
             **kwargs: Any
-    ) -> utils.Popen:
+    ) -> utils.Process:
         commands = []
         if self.container_type in ("docker", "docker-rootless"):
             commands.extend(["docker", "compose"])
             if privilege is None:
                 privilege = self.container_type == "docker"
         elif self.container_type == "podman":
             commands.extend(["podman", "compose"])
@@ -428,15 +428,15 @@
                 if key not in repos:
                     return
                 if not force:
                     raise ContainerError(f"Repository `{key}` already exists.")
                 self._remove_repo_file(repos.pop(key))
                 self._dump_config(self._repo_config_path, repos)
 
-            if url.startswith("http://") or url.startswith("https://") or url.startswith("git@"):
+            if url.startswith("http://") or url.startswith("https://") or url.startswith("ssh://") or url.startswith("git@"):
                 ensure_repo_not_exist(url)
                 self.logger.info(f"Add git repository: {url}")
                 repo_name = utils.guess_file_name(url)
                 repo_path = self._choose_repo_path(repo_name)
                 Repository.clone_with_progress(url, repo_path, branch)
                 repos[url] = dict(type="git", repo_path=repo_path, repo_name=repo_name)
```

### Comparing `linktools-0.8.2rc0/src/linktools/container/repository.py` & `linktools-0.8.3rc0/src/linktools/container/repository.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/decorator.py` & `linktools-0.8.3rc0/src/linktools/decorator.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/device.py` & `linktools-0.8.3rc0/src/linktools/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         from .android import Adb
         from .ios import Sib
         for device in Adb().list_devices(alive=alive):
             yield device
         for device in Sib().list_devices(alive=alive):
             yield device
 
-    def popen(self, *args: [Any], **kwargs) -> utils.Popen:
+    def popen(self, *args: [Any], **kwargs) -> utils.Process:
         if self._tool is None:
             raise self._error_type("tool not found")
         return self._tool.popen(
             *(*self._options, *args),
             **kwargs
         )
```

### Comparing `linktools-0.8.2rc0/src/linktools/frida/__init__.py` & `linktools-0.8.3rc0/src/linktools/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/frida/android.py` & `linktools-0.8.3rc0/src/linktools/frida/android.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/frida/app.py` & `linktools-0.8.3rc0/src/linktools/frida/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/frida/ios.py` & `linktools-0.8.3rc0/src/linktools/frida/ios.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/frida/script.py` & `linktools-0.8.3rc0/src/linktools/frida/script.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/frida/server.py` & `linktools-0.8.3rc0/src/linktools/frida/server.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/ida/__init__.py` & `linktools-0.8.3rc0/src/linktools/ida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/ida/ida.py` & `linktools-0.8.3rc0/src/linktools/ida/ida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/ios/ipa.py` & `linktools-0.8.3rc0/src/linktools/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/ios/sib.py` & `linktools-0.8.3rc0/src/linktools/ios/sib.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 return device.info
         raise SibError(f"device '{self.id}' not found")
 
     @cached_property
     def detail(self) -> dict:
         return self.info.get("deviceDetail")
 
-    def popen(self, *args: [Any], **kwargs) -> utils.Popen:
+    def popen(self, *args: [Any], **kwargs) -> utils.Process:
         """
         执行命令
         :param args: 命令行参数
         :return: 打开的进程
         """
         args = ["--udid", self.id, *args]
         return self._sib.popen(*args, **kwargs)
```

### Comparing `linktools-0.8.2rc0/src/linktools/metadata.py` & `linktools-0.8.3rc0/src/linktools/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 class __MissingType:
     __eq__ = lambda l, r: \
         l is r or type(l) is type(r)
 
 
 __name__ = "linktools"
 __release__ = True
-__version__ = "0.8.2rc0"
+__version__ = "0.8.3rc0"
 __missing__ = __MissingType()
 __description__ = f"""\
     ___       __   __              __
    / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.2rc0)
+  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.3rc0)
  / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
 /_/_/_/ /_/_/|_|\\__/\\____/\\____/_/____/
 """
```

### Comparing `linktools-0.8.2rc0/src/linktools/reactor.py` & `linktools-0.8.3rc0/src/linktools/reactor.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/references/fake_useragent/fake.py` & `linktools-0.8.3rc0/src/linktools/references/fake_useragent/fake.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/references/fake_useragent/utils.py` & `linktools-0.8.3rc0/src/linktools/references/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/rich.py` & `linktools-0.8.3rc0/src/linktools/rich.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/ssh.py` & `linktools-0.8.3rc0/src/linktools/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/utils/__init__.py` & `linktools-0.8.3rc0/src/linktools/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 )
 
 from ._lazy import (
     get_derived_type, lazy_load, lazy_iter, lazy_raise, lazy_import, lazy_import_file
 )
 
 from ._subprocess import (
-    Popen,
+    Process,
     list2cmdline,
 )
 
 from ._port import (
     is_port_free,
     pick_unused_port,
     NoFreePortFoundError,
```

### Comparing `linktools-0.8.2rc0/src/linktools/utils/_lazy.py` & `linktools-0.8.3rc0/src/linktools/utils/_lazy.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/utils/_port.py` & `linktools-0.8.3rc0/src/linktools/utils/_port.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2rc0/src/linktools/utils/_subprocess.py` & `linktools-0.8.3rc0/src/linktools/utils/_subprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 flag, data = self._queue.get_nowait()
                 if flag is not None:
                     yield flag, data
             except queue.Empty:
                 break
 
 
-class Popen(subprocess.Popen):
+class Process(subprocess.Popen):
 
     def __init__(self, *args, **kwargs):
         capture_output = kwargs.pop("capture_output", False)
         if capture_output is True:
             if kwargs.get("stdout") is not None or kwargs.get("stderr") is not None:
                 raise ValueError("stdout and stderr arguments may not be used "
                                  "with capture_output.")
@@ -98,17 +98,19 @@
             kwargs["stderr"] = subprocess.PIPE
         if "cwd" not in kwargs:
             try:
                 kwargs["cwd"] = os.getcwd()
             except FileNotFoundError:
                 kwargs["cwd"] = environ.get_temp_dir(create=True)
         if "append_env" in kwargs:
-            env = os.environ.copy()
-            env.update(kwargs.pop("env", {}))
+            env = kwargs.pop("env", None)
+            env = dict(env) if env else dict()
             env.update(kwargs.pop("append_env"))
+            for key, value in os.environ.items():
+                env.setdefault(key, value)
             kwargs["env"] = env
 
         args = [str(arg) for arg in args]
         environ.logger.debug(f"Exec cmdline: {list2cmdline(args)}")
 
         super().__init__(args, **kwargs)
```

### Comparing `linktools-0.8.2rc0/src/linktools/utils/_utils.py` & `linktools-0.8.3rc0/src/linktools/utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -438,29 +438,32 @@
     def read_file(path: str, text: bool, encoding=DEFAULT_ENCODING) -> Union[str, bytes]: ...
 
 
 def read_file(path: str, text: bool = False, encoding=DEFAULT_ENCODING) -> Union[str, bytes]:
     """
     读取文件数据
     """
-    with open(path, "rb") as fd:
-        data = fd.read()
     if text:
-        data = data.decode(encoding)
-    return data
+        with open(path, "rt", encoding=encoding) as fd:
+            return fd.read()
+    else:
+        with open(path, "rb") as fd:
+            return fd.read()
 
 
 def write_file(path: str, data: [str, bytes], encoding=DEFAULT_ENCODING) -> None:
     """
     写入文件数据
     """
     if isinstance(data, str):
-        data = bytes(data, DEFAULT_ENCODING)
-    with open(path, "wb") as fd:
-        fd.write(data)
+        with open(path, "wt", encoding=encoding) as fd:
+            fd.write(data)
+    else:
+        with open(path, "wb") as fd:
+            fd.write(data)
 
 
 def get_lan_ip() -> Optional[str]:
     """
     获取本地IP地址
     """
     s = None
```

### Comparing `linktools-0.8.2rc0/src/linktools.egg-info/PKG-INFO` & `linktools-0.8.3rc0/src/linktools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.2rc0
+Version: 0.8.3rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `linktools-0.8.2rc0/src/linktools.egg-info/SOURCES.txt` & `linktools-0.8.3rc0/src/linktools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 src/linktools.egg-info/PKG-INFO
 src/linktools.egg-info/SOURCES.txt
 src/linktools.egg-info/dependency_links.txt
 src/linktools.egg-info/entry_points.txt
 src/linktools.egg-info/requires.txt
 src/linktools.egg-info/top_level.txt
 src/linktools/android/__init__.py
-src/linktools/android/__main__.py
 src/linktools/android/adb.py
 src/linktools/android/struct.py
 src/linktools/assets/android-tools.apk
 src/linktools/assets/android-tools.json
 src/linktools/assets/chrome-driver.json
 src/linktools/assets/fake_useragent.json
 src/linktools/assets/frida.js
@@ -60,14 +59,15 @@
 src/linktools/cli/commands/android/intent.py
 src/linktools/cli/commands/android/objection.py
 src/linktools/cli/commands/android/pidcat.py
 src/linktools/cli/commands/android/top.py
 src/linktools/cli/commands/common/__init__.py
 src/linktools/cli/commands/common/cert.py
 src/linktools/cli/commands/common/cntr.py
+src/linktools/cli/commands/common/env.py
 src/linktools/cli/commands/common/grep.py
 src/linktools/cli/commands/common/shell.py
 src/linktools/cli/commands/common/tools.py
 src/linktools/cli/commands/ios/__init__.py
 src/linktools/cli/commands/ios/frida.py
 src/linktools/cli/commands/ios/ipa.py
 src/linktools/cli/commands/ios/objection.py
@@ -75,24 +75,22 @@
 src/linktools/cli/commands/ios/sib.py
 src/linktools/cli/commands/ios/ssh.py
 src/linktools/container/__init__.py
 src/linktools/container/container.py
 src/linktools/container/manager.py
 src/linktools/container/repository.py
 src/linktools/frida/__init__.py
-src/linktools/frida/__main__.py
 src/linktools/frida/android.py
 src/linktools/frida/app.py
 src/linktools/frida/ios.py
 src/linktools/frida/script.py
 src/linktools/frida/server.py
 src/linktools/ida/__init__.py
 src/linktools/ida/ida.py
 src/linktools/ios/__init__.py
-src/linktools/ios/__main__.py
 src/linktools/ios/ipa.py
 src/linktools/ios/sib.py
 src/linktools/references/__init__.py
 src/linktools/references/fake_useragent/__init__.py
 src/linktools/references/fake_useragent/errors.py
 src/linktools/references/fake_useragent/fake.py
 src/linktools/references/fake_useragent/log.py
```

### Comparing `linktools-0.8.2rc0/src/linktools.egg-info/entry_points.txt` & `linktools-0.8.3rc0/src/linktools.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 at-info = linktools.cli.commands.android.info:command.main
 at-intent = linktools.cli.commands.android.intent:command.main
 at-objection = linktools.cli.commands.android.objection:command.main
 at-pidcat = linktools.cli.commands.android.pidcat:command.main
 at-top = linktools.cli.commands.android.top:command.main
 ct-cert = linktools.cli.commands.common.cert:command.main
 ct-cntr = linktools.cli.commands.common.cntr:command.main
+ct-env = linktools.cli.commands.common.env:command.main
 ct-grep = linktools.cli.commands.common.grep:command.main
 ct-shell = linktools.cli.commands.common.shell:command.main
 ct-tools = linktools.cli.commands.common.tools:command.main
 it-frida = linktools.cli.commands.ios.frida:command.main
 it-ipa = linktools.cli.commands.ios.ipa:command.main
 it-objection = linktools.cli.commands.ios.objection:command.main
 it-scp = linktools.cli.commands.ios.scp:command.main
```

### Comparing `linktools-0.8.2rc0/src/linktools.egg-info/requires.txt` & `linktools-0.8.3rc0/src/linktools.egg-info/requires.txt`

 * *Files identical despite different names*

