# Comparing `tmp/libro-0.1.1.tar.gz` & `tmp/libro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libro-0.1.1.tar", max compression
+gzip compressed data, was "libro-0.1.2.tar", max compression
```

## Comparing `libro-0.1.1.tar` & `libro-0.1.2.tar`

### file list

```diff
@@ -1,100 +1,81 @@
--rw-r--r--   0        0        0      556 2024-01-24 11:00:49.902070 libro-0.1.1/README.md
--rw-r--r--   0        0        0        6 2024-01-11 03:02:15.929110 libro-0.1.1/libro_server/.gitignore
--rw-r--r--   0        0        0      719 2024-01-31 10:42:21.612526 libro-0.1.1/libro_server/__init__.py
--rw-r--r--   0        0        0       46 2024-01-24 11:00:49.903994 libro-0.1.1/libro_server/_version.py
--rw-r--r--   0        0        0     2927 2024-03-25 08:07:10.912494 libro-0.1.1/libro_server/app.py
--rwxr-xr-x   0        0        0      502 2024-01-24 11:00:49.904234 libro-0.1.1/libro_server/chat/__init__.py
--rw-r--r--   0        0        0     1604 2024-01-24 11:00:49.904426 libro-0.1.1/libro_server/chat/executor.py
--rw-r--r--   0        0        0      752 2024-01-24 11:00:49.904503 libro-0.1.1/libro_server/chat/item.py
--rw-r--r--   0        0        0      999 2024-01-24 11:00:49.904596 libro-0.1.1/libro_server/chat/langchain_variable.py
--rw-r--r--   0        0        0     1465 2024-01-24 11:00:49.904759 libro-0.1.1/libro_server/chat/langchain_variable_executor.py
--rw-r--r--   0        0        0     2222 2024-01-24 11:00:49.904967 libro-0.1.1/libro_server/chat/openai.py
--rw-r--r--   0        0        0     2722 2024-01-24 11:00:49.905171 libro-0.1.1/libro_server/chat/openai_chat_executor.py
--rw-r--r--   0        0        0     1618 2024-01-24 11:00:49.905249 libro-0.1.1/libro_server/chat/provider.py
--rw-r--r--   0        0        0      130 2024-01-24 11:00:49.905311 libro-0.1.1/libro_server/chat/source.py
--rw-r--r--   0        0        0       81 2024-01-31 10:42:21.612727 libro-0.1.1/libro_server/flow/__init__.py
--rw-r--r--   0        0        0     2503 2024-01-31 10:42:21.612896 libro-0.1.1/libro_server/flow/libro_client.py
--rw-r--r--   0        0        0     2425 2024-01-31 10:42:21.613060 libro-0.1.1/libro_server/flow/nb_args.py
--rw-r--r--   0        0        0     1933 2024-03-25 08:23:49.658205 libro-0.1.1/libro_server/handler.py
--rw-r--r--   0        0        0      324 2024-01-24 11:00:49.905424 libro-0.1.1/libro_server/magics/__init__.py
--rw-r--r--   0        0        0     1277 2024-01-24 11:00:49.905498 libro-0.1.1/libro_server/magics/exception.py
--rw-r--r--   0        0        0     3550 2024-01-24 11:00:49.905665 libro-0.1.1/libro_server/magics/prompt_magic.py
--rw-r--r--   0        0        0        0 2024-01-11 03:02:15.929786 libro-0.1.1/libro_server/static/.gitkeep
--rw-r--r--   0        0        0     4817 2024-03-26 11:56:02.080685 libro-0.1.1/libro_server/static/1330.async.js
--rw-r--r--   0        0        0     6234 2024-03-26 11:56:02.081326 libro-0.1.1/libro_server/static/1438.async.js
--rw-r--r--   0        0        0     4800 2024-03-26 11:56:02.082057 libro-0.1.1/libro_server/static/161.async.js
--rw-r--r--   0        0        0     6175 2024-03-26 11:56:02.082574 libro-0.1.1/libro_server/static/1639.async.js
--rw-r--r--   0        0        0     5813 2024-03-26 11:56:02.082928 libro-0.1.1/libro_server/static/1772.async.js
--rw-r--r--   0        0        0     5091 2024-03-26 11:56:02.083598 libro-0.1.1/libro_server/static/1838.async.js
--rw-r--r--   0        0        0     6197 2024-03-26 11:56:02.083819 libro-0.1.1/libro_server/static/2048.async.js
--rw-r--r--   0        0        0     5473 2024-03-26 11:56:02.084133 libro-0.1.1/libro_server/static/2118.async.js
--rw-r--r--   0        0        0     6218 2024-03-26 11:56:02.084415 libro-0.1.1/libro_server/static/2130.async.js
--rw-r--r--   0        0        0     6224 2024-03-26 11:56:02.084663 libro-0.1.1/libro_server/static/2999.async.js
--rw-r--r--   0        0        0     4818 2024-03-26 11:56:02.084817 libro-0.1.1/libro_server/static/3572.async.js
--rw-r--r--   0        0        0     6232 2024-03-26 11:56:02.085001 libro-0.1.1/libro_server/static/405.async.js
--rw-r--r--   0        0        0      213 2024-03-26 11:56:02.085319 libro-0.1.1/libro_server/static/4113.async.js
--rw-r--r--   0        0        0     6242 2024-03-26 11:56:02.085475 libro-0.1.1/libro_server/static/4116.async.js
--rw-r--r--   0        0        0     6177 2024-03-26 11:56:02.085624 libro-0.1.1/libro_server/static/4123.async.js
--rw-r--r--   0        0        0     6231 2024-03-26 11:56:02.085891 libro-0.1.1/libro_server/static/417.async.js
--rw-r--r--   0        0        0     5190 2024-03-26 11:56:02.086041 libro-0.1.1/libro_server/static/4266.async.js
--rw-r--r--   0        0        0     6230 2024-03-26 11:56:02.086242 libro-0.1.1/libro_server/static/4343.async.js
--rw-r--r--   0        0        0     5114 2024-03-26 11:56:02.086436 libro-0.1.1/libro_server/static/4541.async.js
--rw-r--r--   0        0        0     5419 2024-03-26 11:56:02.086829 libro-0.1.1/libro_server/static/4621.async.js
--rw-r--r--   0        0        0     5741 2024-03-26 11:56:02.086971 libro-0.1.1/libro_server/static/4658.async.js
--rw-r--r--   0        0        0     6090 2024-03-26 11:56:02.087122 libro-0.1.1/libro_server/static/4849.async.js
--rw-r--r--   0        0        0     6238 2024-03-26 11:56:02.087264 libro-0.1.1/libro_server/static/4887.async.js
--rw-r--r--   0        0        0     5066 2024-03-26 11:56:02.087409 libro-0.1.1/libro_server/static/5250.async.js
--rw-r--r--   0        0        0  9350375 2024-03-26 11:56:02.097081 libro-0.1.1/libro_server/static/5332.async.js
--rw-r--r--   0        0        0     6174 2024-03-26 11:56:02.100272 libro-0.1.1/libro_server/static/610.async.js
--rw-r--r--   0        0        0     5310 2024-03-26 11:56:02.100440 libro-0.1.1/libro_server/static/628.async.js
--rw-r--r--   0        0        0     5113 2024-03-26 11:56:02.100588 libro-0.1.1/libro_server/static/6357.async.js
--rw-r--r--   0        0        0     5001 2024-03-26 11:56:02.100745 libro-0.1.1/libro_server/static/6404.async.js
--rw-r--r--   0        0        0     6235 2024-03-26 11:56:02.100886 libro-0.1.1/libro_server/static/6486.async.js
--rw-r--r--   0        0        0     7189 2024-03-26 11:56:02.101034 libro-0.1.1/libro_server/static/6730.async.js
--rw-r--r--   0        0        0     5089 2024-03-26 11:56:02.101173 libro-0.1.1/libro_server/static/6962.async.js
--rw-r--r--   0        0        0     5811 2024-03-26 11:56:02.101310 libro-0.1.1/libro_server/static/6999.async.js
--rw-r--r--   0        0        0     3130 2024-03-26 11:56:02.101417 libro-0.1.1/libro_server/static/7162.async.js
--rw-r--r--   0        0        0     5118 2024-03-26 11:56:02.101550 libro-0.1.1/libro_server/static/7715.async.js
--rw-r--r--   0        0        0     6232 2024-03-26 11:56:02.101688 libro-0.1.1/libro_server/static/7851.async.js
--rw-r--r--   0        0        0     5162 2024-03-26 11:56:02.101894 libro-0.1.1/libro_server/static/79.async.js
--rw-r--r--   0        0        0     6237 2024-03-26 11:56:02.102031 libro-0.1.1/libro_server/static/8227.async.js
--rw-r--r--   0        0        0     6233 2024-03-26 11:56:02.102165 libro-0.1.1/libro_server/static/8305.async.js
--rw-r--r--   0        0        0     5172 2024-03-26 11:56:02.102302 libro-0.1.1/libro_server/static/8370.async.js
--rw-r--r--   0        0        0     6175 2024-03-26 11:56:02.102459 libro-0.1.1/libro_server/static/8525.async.js
--rw-r--r--   0        0        0    74158 2024-03-26 11:56:02.102653 libro-0.1.1/libro_server/static/8945.chunk.css
--rw-r--r--   0        0        0     5082 2024-03-26 11:56:02.102830 libro-0.1.1/libro_server/static/9095.async.js
--rw-r--r--   0        0        0     6238 2024-03-26 11:56:02.102972 libro-0.1.1/libro_server/static/9150.async.js
--rw-r--r--   0        0        0     5392 2024-03-26 11:56:02.103116 libro-0.1.1/libro_server/static/9402.async.js
--rw-r--r--   0        0        0     6222 2024-03-26 11:56:02.103238 libro-0.1.1/libro_server/static/9669.async.js
--rw-r--r--   0        0        0     4995 2024-03-26 11:56:02.103368 libro-0.1.1/libro_server/static/9674.async.js
--rw-r--r--   0        0        0 28118062 2024-03-26 11:56:02.129294 libro-0.1.1/libro_server/static/9709.async.js
--rw-r--r--   0        0        0   255768 2024-03-26 11:56:02.131609 libro-0.1.1/libro_server/static/9709.chunk.css
--rw-r--r--   0        0        0     6233 2024-03-26 11:56:02.132523 libro-0.1.1/libro_server/static/9749.async.js
--rw-r--r--   0        0        0     5189 2024-03-26 11:56:02.133398 libro-0.1.1/libro_server/static/9905.async.js
--rw-r--r--   0        0        0     1427 2024-03-26 11:56:02.134286 libro-0.1.1/libro_server/static/index.html
--rw-r--r--   0        0        0     8432 2024-03-26 11:56:02.135146 libro-0.1.1/libro_server/static/p__libro__index.async.js
--rw-r--r--   0        0        0      105 2024-03-26 11:56:02.136081 libro-0.1.1/libro_server/static/p__libro__index.chunk.css
--rw-r--r--   0        0        0    73464 2024-03-26 11:56:02.298196 libro-0.1.1/libro_server/static/static/codicon.589e0820.ttf
--rw-r--r--   0        0        0    49764 2024-03-26 11:56:02.298780 libro-0.1.1/libro_server/static/static/devopicons.3c46801a.woff2
--rw-r--r--   0        0        0    90680 2024-03-26 11:56:02.299757 libro-0.1.1/libro_server/static/static/file-icons.2cbb51ef.woff2
--rw-r--r--   0        0        0   165742 2024-03-26 11:56:02.300960 libro-0.1.1/libro_server/static/static/fontawesome-webfont.2b13baa7.eot
--rw-r--r--   0        0        0   165548 2024-03-26 11:56:02.301487 libro-0.1.1/libro_server/static/static/fontawesome-webfont.8a7cb27d.ttf
--rw-r--r--   0        0        0    98024 2024-03-26 11:56:02.302067 libro-0.1.1/libro_server/static/static/fontawesome-webfont.cf011583.woff
--rw-r--r--   0        0        0    77160 2024-03-26 11:56:02.302313 libro-0.1.1/libro_server/static/static/fontawesome-webfont.e9955780.woff2
--rw-r--r--   0        0        0   387787 2024-03-26 11:56:02.302788 libro-0.1.1/libro_server/static/static/fontawesome-webfont.f05dad85.svg
--rw-r--r--   0        0        0    77160 2024-03-26 11:56:02.303031 libro-0.1.1/libro_server/static/static/fontawesome.e9955780.woff2
--rw-r--r--   0        0        0    24412 2024-03-26 11:56:02.303213 libro-0.1.1/libro_server/static/static/mfixx.8e0807ce.woff2
--rw-r--r--   0        0        0    20248 2024-03-26 11:56:02.303386 libro-0.1.1/libro_server/static/static/octicons.c982f59d.woff2
--rw-r--r--   0        0        0   466610 2024-03-26 11:56:02.303904 libro-0.1.1/libro_server/static/static/onig.25dd2e6f.wasm
--rw-r--r--   0        0        0      741 2024-03-26 11:56:02.304426 libro-0.1.1/libro_server/static/static/plotly.eb7b9072.svg
--rw-r--r--   0        0        0   847831 2024-03-26 11:56:02.137638 libro-0.1.1/libro_server/static/umi.js
--rw-r--r--   0        0        0      457 2024-01-11 03:02:15.930077 libro-0.1.1/libro_server/templates/error.html
--rw-r--r--   0        0        0     1050 2024-01-11 03:02:15.930239 libro-0.1.1/libro_server/templates/libro.html
--rw-r--r--   0        0        0      591 2024-01-11 03:02:15.930395 libro-0.1.1/libro_server/templates/page.html
--rwxr-xr-x   0        0        0      174 2024-01-24 11:00:49.905792 libro-0.1.1/libro_server/utils/__init__.py
--rw-r--r--   0        0        0      553 2024-01-24 11:00:49.905875 libro-0.1.1/libro_server/utils/base.py
--rw-r--r--   0        0        0      689 2024-01-24 11:00:49.905962 libro-0.1.1/libro_server/utils/inspector.py
--rw-r--r--   0        0        0     1111 2024-01-24 11:00:49.906046 libro-0.1.1/libro_server/utils/langchain.py
--rw-r--r--   0        0        0     1290 2024-03-26 11:44:20.042389 libro-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       33 2024-01-11 03:02:15.930969 libro-0.1.1/setup.py
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 libro-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      556 2024-01-24 11:00:49.902070 libro-0.1.2/README.md
+-rw-r--r--   0        0        0        6 2024-04-03 06:18:16.905512 libro-0.1.2/libro_server/.gitignore
+-rw-r--r--   0        0        0      348 2024-04-03 06:20:34.869920 libro-0.1.2/libro_server/__init__.py
+-rw-r--r--   0        0        0       46 2024-04-03 06:20:44.616869 libro-0.1.2/libro_server/_version.py
+-rw-r--r--   0        0        0     2927 2024-04-03 06:18:16.906606 libro-0.1.2/libro_server/app.py
+-rw-r--r--   0        0        0     1933 2024-04-03 06:18:16.910291 libro-0.1.2/libro_server/handler.py
+-rw-r--r--   0        0        0        0 2024-04-03 06:18:16.910853 libro-0.1.2/libro_server/static/.gitkeep
+-rw-r--r--   0        0        0     4817 2024-04-03 06:25:37.869451 libro-0.1.2/libro_server/static/1330.async.js
+-rw-r--r--   0        0        0     6234 2024-04-03 06:25:37.870047 libro-0.1.2/libro_server/static/1438.async.js
+-rw-r--r--   0        0        0     4800 2024-04-03 06:25:37.870780 libro-0.1.2/libro_server/static/161.async.js
+-rw-r--r--   0        0        0     6175 2024-04-03 06:25:37.871284 libro-0.1.2/libro_server/static/1639.async.js
+-rw-r--r--   0        0        0     5813 2024-04-03 06:25:37.871633 libro-0.1.2/libro_server/static/1772.async.js
+-rw-r--r--   0        0        0     5091 2024-04-03 06:25:37.872295 libro-0.1.2/libro_server/static/1838.async.js
+-rw-r--r--   0        0        0     6197 2024-04-03 06:25:37.872471 libro-0.1.2/libro_server/static/2048.async.js
+-rw-r--r--   0        0        0     5473 2024-04-03 06:25:37.872754 libro-0.1.2/libro_server/static/2118.async.js
+-rw-r--r--   0        0        0     6218 2024-04-03 06:25:37.872983 libro-0.1.2/libro_server/static/2130.async.js
+-rw-r--r--   0        0        0     6224 2024-04-03 06:25:37.873126 libro-0.1.2/libro_server/static/2999.async.js
+-rw-r--r--   0        0        0     4818 2024-04-03 06:25:37.873245 libro-0.1.2/libro_server/static/3572.async.js
+-rw-r--r--   0        0        0     6232 2024-04-03 06:25:37.873363 libro-0.1.2/libro_server/static/405.async.js
+-rw-r--r--   0        0        0      213 2024-04-03 06:25:37.873510 libro-0.1.2/libro_server/static/4113.async.js
+-rw-r--r--   0        0        0     6242 2024-04-03 06:25:37.873714 libro-0.1.2/libro_server/static/4116.async.js
+-rw-r--r--   0        0        0     6177 2024-04-03 06:25:37.873844 libro-0.1.2/libro_server/static/4123.async.js
+-rw-r--r--   0        0        0     6231 2024-04-03 06:25:37.873967 libro-0.1.2/libro_server/static/417.async.js
+-rw-r--r--   0        0        0     5190 2024-04-03 06:25:37.874179 libro-0.1.2/libro_server/static/4266.async.js
+-rw-r--r--   0        0        0     6230 2024-04-03 06:25:37.874440 libro-0.1.2/libro_server/static/4343.async.js
+-rw-r--r--   0        0        0     5114 2024-04-03 06:25:37.874578 libro-0.1.2/libro_server/static/4541.async.js
+-rw-r--r--   0        0        0     5419 2024-04-03 06:25:37.874718 libro-0.1.2/libro_server/static/4621.async.js
+-rw-r--r--   0        0        0     5741 2024-04-03 06:25:37.874985 libro-0.1.2/libro_server/static/4658.async.js
+-rw-r--r--   0        0        0     6090 2024-04-03 06:25:37.875123 libro-0.1.2/libro_server/static/4849.async.js
+-rw-r--r--   0        0        0     6238 2024-04-03 06:25:37.875300 libro-0.1.2/libro_server/static/4887.async.js
+-rw-r--r--   0        0        0     5066 2024-04-03 06:25:37.875421 libro-0.1.2/libro_server/static/5250.async.js
+-rw-r--r--   0        0        0  9350375 2024-04-03 06:25:37.884122 libro-0.1.2/libro_server/static/5332.async.js
+-rw-r--r--   0        0        0     6174 2024-04-03 06:25:37.888836 libro-0.1.2/libro_server/static/610.async.js
+-rw-r--r--   0        0        0     5310 2024-04-03 06:25:37.888955 libro-0.1.2/libro_server/static/628.async.js
+-rw-r--r--   0        0        0     5113 2024-04-03 06:25:37.889086 libro-0.1.2/libro_server/static/6357.async.js
+-rw-r--r--   0        0        0     5001 2024-04-03 06:25:37.889206 libro-0.1.2/libro_server/static/6404.async.js
+-rw-r--r--   0        0        0     6235 2024-04-03 06:25:37.889341 libro-0.1.2/libro_server/static/6486.async.js
+-rw-r--r--   0        0        0     7189 2024-04-03 06:25:37.889472 libro-0.1.2/libro_server/static/6730.async.js
+-rw-r--r--   0        0        0     5089 2024-04-03 06:25:37.889604 libro-0.1.2/libro_server/static/6962.async.js
+-rw-r--r--   0        0        0     5811 2024-04-03 06:25:37.889729 libro-0.1.2/libro_server/static/6999.async.js
+-rw-r--r--   0        0        0     3130 2024-04-03 06:25:37.889836 libro-0.1.2/libro_server/static/7162.async.js
+-rw-r--r--   0        0        0     5118 2024-04-03 06:25:37.889950 libro-0.1.2/libro_server/static/7715.async.js
+-rw-r--r--   0        0        0     6232 2024-04-03 06:25:37.890063 libro-0.1.2/libro_server/static/7851.async.js
+-rw-r--r--   0        0        0     5162 2024-04-03 06:25:37.890173 libro-0.1.2/libro_server/static/79.async.js
+-rw-r--r--   0        0        0     6237 2024-04-03 06:25:37.890287 libro-0.1.2/libro_server/static/8227.async.js
+-rw-r--r--   0        0        0     6233 2024-04-03 06:25:37.890401 libro-0.1.2/libro_server/static/8305.async.js
+-rw-r--r--   0        0        0     5172 2024-04-03 06:25:37.890520 libro-0.1.2/libro_server/static/8370.async.js
+-rw-r--r--   0        0        0     6175 2024-04-03 06:25:37.890661 libro-0.1.2/libro_server/static/8525.async.js
+-rw-r--r--   0        0        0    74158 2024-04-03 06:25:37.890816 libro-0.1.2/libro_server/static/8945.chunk.css
+-rw-r--r--   0        0        0     5082 2024-04-03 06:25:37.890962 libro-0.1.2/libro_server/static/9095.async.js
+-rw-r--r--   0        0        0     6238 2024-04-03 06:25:37.891102 libro-0.1.2/libro_server/static/9150.async.js
+-rw-r--r--   0        0        0     5392 2024-04-03 06:25:37.891232 libro-0.1.2/libro_server/static/9402.async.js
+-rw-r--r--   0        0        0     6222 2024-04-03 06:25:37.891354 libro-0.1.2/libro_server/static/9669.async.js
+-rw-r--r--   0        0        0     4995 2024-04-03 06:25:37.891471 libro-0.1.2/libro_server/static/9674.async.js
+-rw-r--r--   0        0        0 28118062 2024-04-03 06:25:37.918458 libro-0.1.2/libro_server/static/9709.async.js
+-rw-r--r--   0        0        0   255768 2024-04-03 06:25:37.919473 libro-0.1.2/libro_server/static/9709.chunk.css
+-rw-r--r--   0        0        0     6233 2024-04-03 06:25:37.919621 libro-0.1.2/libro_server/static/9749.async.js
+-rw-r--r--   0        0        0     5189 2024-04-03 06:25:37.919737 libro-0.1.2/libro_server/static/9905.async.js
+-rw-r--r--   0        0        0     1427 2024-04-03 06:25:37.919857 libro-0.1.2/libro_server/static/index.html
+-rw-r--r--   0        0        0     8432 2024-04-03 06:25:37.920009 libro-0.1.2/libro_server/static/p__libro__index.async.js
+-rw-r--r--   0        0        0      105 2024-04-03 06:25:37.921425 libro-0.1.2/libro_server/static/p__libro__index.chunk.css
+-rw-r--r--   0        0        0    73464 2024-04-03 06:25:38.000456 libro-0.1.2/libro_server/static/static/codicon.589e0820.ttf
+-rw-r--r--   0        0        0    49764 2024-04-03 06:25:38.001172 libro-0.1.2/libro_server/static/static/devopicons.3c46801a.woff2
+-rw-r--r--   0        0        0    90680 2024-04-03 06:25:38.001953 libro-0.1.2/libro_server/static/static/file-icons.2cbb51ef.woff2
+-rw-r--r--   0        0        0   165742 2024-04-03 06:25:38.002323 libro-0.1.2/libro_server/static/static/fontawesome-webfont.2b13baa7.eot
+-rw-r--r--   0        0        0   165548 2024-04-03 06:25:38.002933 libro-0.1.2/libro_server/static/static/fontawesome-webfont.8a7cb27d.ttf
+-rw-r--r--   0        0        0    98024 2024-04-03 06:25:38.003194 libro-0.1.2/libro_server/static/static/fontawesome-webfont.cf011583.woff
+-rw-r--r--   0        0        0    77160 2024-04-03 06:25:38.003418 libro-0.1.2/libro_server/static/static/fontawesome-webfont.e9955780.woff2
+-rw-r--r--   0        0        0   387787 2024-04-03 06:25:38.003996 libro-0.1.2/libro_server/static/static/fontawesome-webfont.f05dad85.svg
+-rw-r--r--   0        0        0    77160 2024-04-03 06:25:38.004227 libro-0.1.2/libro_server/static/static/fontawesome.e9955780.woff2
+-rw-r--r--   0        0        0    24412 2024-04-03 06:25:38.004378 libro-0.1.2/libro_server/static/static/mfixx.8e0807ce.woff2
+-rw-r--r--   0        0        0    20248 2024-04-03 06:25:38.004542 libro-0.1.2/libro_server/static/static/octicons.c982f59d.woff2
+-rw-r--r--   0        0        0   466610 2024-04-03 06:25:38.005022 libro-0.1.2/libro_server/static/static/onig.25dd2e6f.wasm
+-rw-r--r--   0        0        0      741 2024-04-03 06:25:38.005176 libro-0.1.2/libro_server/static/static/plotly.eb7b9072.svg
+-rw-r--r--   0        0        0   847831 2024-04-03 06:25:37.922235 libro-0.1.2/libro_server/static/umi.js
+-rw-r--r--   0        0        0      457 2024-04-03 06:18:16.910976 libro-0.1.2/libro_server/templates/error.html
+-rw-r--r--   0        0        0     1050 2024-04-03 06:18:16.911049 libro-0.1.2/libro_server/templates/libro.html
+-rw-r--r--   0        0        0      591 2024-04-03 06:18:16.911305 libro-0.1.2/libro_server/templates/page.html
+-rw-r--r--   0        0        0     1115 2024-04-03 06:23:02.581456 libro-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       33 2024-01-11 03:02:15.930969 libro-0.1.2/setup.py
+-rw-r--r--   0        0        0     1183 1970-01-01 00:00:00.000000 libro-0.1.2/PKG-INFO
```

### Comparing `libro-0.1.1/README.md` & `libro-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/app.py` & `libro-0.1.2/libro_server/app.py`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/handler.py` & `libro-0.1.2/libro_server/handler.py`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/1330.async.js` & `libro-0.1.2/libro_server/static/1330.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/1438.async.js` & `libro-0.1.2/libro_server/static/1438.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/161.async.js` & `libro-0.1.2/libro_server/static/161.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/1639.async.js` & `libro-0.1.2/libro_server/static/1639.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/1772.async.js` & `libro-0.1.2/libro_server/static/1772.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/1838.async.js` & `libro-0.1.2/libro_server/static/1838.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/2048.async.js` & `libro-0.1.2/libro_server/static/2048.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/2118.async.js` & `libro-0.1.2/libro_server/static/2118.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/2130.async.js` & `libro-0.1.2/libro_server/static/2130.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/2999.async.js` & `libro-0.1.2/libro_server/static/2999.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/3572.async.js` & `libro-0.1.2/libro_server/static/3572.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/405.async.js` & `libro-0.1.2/libro_server/static/405.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/4116.async.js` & `libro-0.1.2/libro_server/static/4116.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/4123.async.js` & `libro-0.1.2/libro_server/static/4123.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/417.async.js` & `libro-0.1.2/libro_server/static/417.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/4266.async.js` & `libro-0.1.2/libro_server/static/4266.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/4343.async.js` & `libro-0.1.2/libro_server/static/4343.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/4541.async.js` & `libro-0.1.2/libro_server/static/4541.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/4621.async.js` & `libro-0.1.2/libro_server/static/4621.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/4658.async.js` & `libro-0.1.2/libro_server/static/4658.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/4849.async.js` & `libro-0.1.2/libro_server/static/4849.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/4887.async.js` & `libro-0.1.2/libro_server/static/4887.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/5250.async.js` & `libro-0.1.2/libro_server/static/5250.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/5332.async.js` & `libro-0.1.2/libro_server/static/5332.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/610.async.js` & `libro-0.1.2/libro_server/static/610.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/628.async.js` & `libro-0.1.2/libro_server/static/628.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/6357.async.js` & `libro-0.1.2/libro_server/static/6357.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/6404.async.js` & `libro-0.1.2/libro_server/static/6404.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/6486.async.js` & `libro-0.1.2/libro_server/static/6486.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/6730.async.js` & `libro-0.1.2/libro_server/static/6730.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/6962.async.js` & `libro-0.1.2/libro_server/static/6962.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/6999.async.js` & `libro-0.1.2/libro_server/static/6999.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/7162.async.js` & `libro-0.1.2/libro_server/static/7162.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/7715.async.js` & `libro-0.1.2/libro_server/static/7715.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/7851.async.js` & `libro-0.1.2/libro_server/static/7851.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/79.async.js` & `libro-0.1.2/libro_server/static/79.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/8227.async.js` & `libro-0.1.2/libro_server/static/8227.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/8305.async.js` & `libro-0.1.2/libro_server/static/8305.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/8370.async.js` & `libro-0.1.2/libro_server/static/8370.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/8525.async.js` & `libro-0.1.2/libro_server/static/8525.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/8945.chunk.css` & `libro-0.1.2/libro_server/static/8945.chunk.css`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/9095.async.js` & `libro-0.1.2/libro_server/static/9095.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/9150.async.js` & `libro-0.1.2/libro_server/static/9150.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/9402.async.js` & `libro-0.1.2/libro_server/static/9402.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/9669.async.js` & `libro-0.1.2/libro_server/static/9669.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/9674.async.js` & `libro-0.1.2/libro_server/static/9674.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/9709.async.js` & `libro-0.1.2/libro_server/static/9709.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/9709.chunk.css` & `libro-0.1.2/libro_server/static/9709.chunk.css`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/9749.async.js` & `libro-0.1.2/libro_server/static/9749.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/9905.async.js` & `libro-0.1.2/libro_server/static/9905.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/index.html` & `libro-0.1.2/libro_server/static/index.html`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/p__libro__index.async.js` & `libro-0.1.2/libro_server/static/p__libro__index.async.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/codicon.589e0820.ttf` & `libro-0.1.2/libro_server/static/static/codicon.589e0820.ttf`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/devopicons.3c46801a.woff2` & `libro-0.1.2/libro_server/static/static/devopicons.3c46801a.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/file-icons.2cbb51ef.woff2` & `libro-0.1.2/libro_server/static/static/file-icons.2cbb51ef.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/fontawesome-webfont.2b13baa7.eot` & `libro-0.1.2/libro_server/static/static/fontawesome-webfont.2b13baa7.eot`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/fontawesome-webfont.8a7cb27d.ttf` & `libro-0.1.2/libro_server/static/static/fontawesome-webfont.8a7cb27d.ttf`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/fontawesome-webfont.cf011583.woff` & `libro-0.1.2/libro_server/static/static/fontawesome-webfont.cf011583.woff`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/fontawesome-webfont.e9955780.woff2` & `libro-0.1.2/libro_server/static/static/fontawesome-webfont.e9955780.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/fontawesome-webfont.f05dad85.svg` & `libro-0.1.2/libro_server/static/static/fontawesome-webfont.f05dad85.svg`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/fontawesome.e9955780.woff2` & `libro-0.1.2/libro_server/static/static/fontawesome.e9955780.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/mfixx.8e0807ce.woff2` & `libro-0.1.2/libro_server/static/static/mfixx.8e0807ce.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/octicons.c982f59d.woff2` & `libro-0.1.2/libro_server/static/static/octicons.c982f59d.woff2`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/onig.25dd2e6f.wasm` & `libro-0.1.2/libro_server/static/static/onig.25dd2e6f.wasm`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/static/plotly.eb7b9072.svg` & `libro-0.1.2/libro_server/static/static/plotly.eb7b9072.svg`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/static/umi.js` & `libro-0.1.2/libro_server/static/umi.js`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/templates/libro.html` & `libro-0.1.2/libro_server/templates/libro.html`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/libro_server/templates/page.html` & `libro-0.1.2/libro_server/templates/page.html`

 * *Files identical despite different names*

### Comparing `libro-0.1.1/pyproject.toml` & `libro-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libro"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["zhanba <c5e1856@gmail.com>", "brokun <brokun0128@gmail.com>"]
 readme = "README.md"
 packages = [{include = "libro_server"}]
 include = ['README.md', 'setup.py', 'jupyter-config', 'libro_server/static/**/*', 'libro_server/template', 'libro_server/*.py']
 exclude = ['lab/**/*']
 
@@ -22,25 +22,17 @@
 python = ">=3.8.1,<3.12"
 jupyter-server = ">=2.10.0"
 jupyterlab-server = "^2.24.0"
 ipykernel = "^6.16.2"
 ipython = ">=7.34.0"
 jupyter-lsp = "^2.2.0"
 ruff-lsp = ">=0.0.50"
-langchain = "^0.1.0"
-nbclient = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
-pandas = "^1.5.1"
-transformers = "^4.31.0"
-matplotlib = "^3.7.2"
-pandas-stubs = "^1.5.3"
 poethepoet = "^0.21.1"
 twine = "^4.0.2"
 jupyterlab = "^3.6.5"
-yapf = "^0.40.2"
-langchain_openai = "^0.0.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `libro-0.1.1/PKG-INFO` & `libro-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: libro
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: zhanba
 Author-email: c5e1856@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipykernel (>=6.16.2,<7.0.0)
 Requires-Dist: ipython (>=7.34.0)
 Requires-Dist: jupyter-lsp (>=2.2.0,<3.0.0)
 Requires-Dist: jupyter-server (>=2.10.0)
 Requires-Dist: jupyterlab-server (>=2.24.0,<3.0.0)
-Requires-Dist: langchain (>=0.1.0,<0.2.0)
-Requires-Dist: nbclient (>=0.9.0,<0.10.0)
 Requires-Dist: ruff-lsp (>=0.0.50)
 Description-Content-Type: text/markdown
 
 # libro server
 
 ## env setup
```

