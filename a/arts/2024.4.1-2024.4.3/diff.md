# Comparing `tmp/arts-2024.4.1.tar.gz` & `tmp/arts-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arts-2024.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "arts-2024.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `arts-2024.4.1.tar` & `arts-2024.4.3.tar`

### file list

```diff
@@ -1,229 +1,231 @@
--rw-r--r--   0        0        0     2175 2023-12-20 10:09:43.709218 arts-2024.4.1/.gitignore
--rw-r--r--   0        0        0       46 2024-03-10 10:13:06.948005 arts-2024.4.1/README.md
--rw-r--r--   0        0        0      317 2024-02-22 12:02:36.224046 arts-2024.4.1/arts/CoolMemory-English/Copyright
--rw-r--r--   0        0        0    10294 2024-03-31 09:22:44.234618 arts-2024.4.1/arts/CoolMemory-English/README.md
--rw-r--r--   0        0        0      110 2024-03-06 00:07:28.301653 arts-2024.4.1/arts/CoolMemory-English/art.json
--rw-r--r--   0        0        0      393 2023-12-10 08:00:44.000000 arts-2024.4.1/arts/CoolMemory-English/licenses/README.md
--rw-r--r--   0        0        0     1586 2023-12-10 08:00:44.000000 arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE
--rw-r--r--   0        0        0    11550 2023-12-10 08:00:44.000000 arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE
--rw-r--r--   0        0        0    32825 2023-12-10 08:00:44.000000 arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/Python/LICENSE
--rw-r--r--   0        0        0     2987 2023-12-10 08:00:44.000000 arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE
--rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE
--rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE
--rw-r--r--   0        0        0      106 2024-03-31 10:18:29.252509 arts-2024.4.1/arts/WeChat-Art-Museum/art.json
--rw-r--r--   0        0        0    50988 2024-04-01 02:43:36.159990 arts-2024.4.1/arts/WeChat-Art-Museum/index.html
--rw-r--r--   0        0        0        0 2024-02-22 15:47:26.927352 arts-2024.4.1/arts/__init__.py
--rw-r--r--   0        0        0     3088 2023-09-24 08:08:30.000000 arts-2024.4.1/arts/articles/010-赚钱宝典/010-财富的本质/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:01:11.532367 arts-2024.4.1/arts/articles/010-赚钱宝典/010-财富的本质/art.json
--rw-r--r--   0        0        0     1681 2023-12-20 10:09:07.827303 arts-2024.4.1/arts/articles/010-赚钱宝典/020-商业价值/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:01:11.533332 arts-2024.4.1/arts/articles/010-赚钱宝典/020-商业价值/art.json
--rw-r--r--   0        0        0     3552 2023-12-22 07:27:54.636897 arts-2024.4.1/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md
--rw-r--r--   0        0        0       44 2023-12-22 07:26:00.584312 arts-2024.4.1/arts/articles/010-赚钱宝典/030-财富稳定型社会/art.json
--rw-r--r--   0        0        0     1812 2024-01-02 20:05:02.520382 arts-2024.4.1/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md
--rw-r--r--   0        0        0       44 2024-01-02 20:46:41.567445 arts-2024.4.1/arts/articles/075-追英赶美/300-产业升级与失业潮/art.json
--rw-r--r--   0        0        0     1253 2024-01-18 01:49:14.297346 arts-2024.4.1/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md
--rw-r--r--   0        0        0       44 2024-01-02 20:47:04.916014 arts-2024.4.1/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/art.json
--rw-r--r--   0        0        0     1559 2023-11-15 13:45:10.000000 arts-2024.4.1/arts/articles/150-小民参政/300-广义的民主/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:02:18.547561 arts-2024.4.1/arts/articles/150-小民参政/300-广义的民主/art.json
--rw-r--r--   0        0        0     1499 2023-10-24 11:49:00.000000 arts-2024.4.1/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:02:18.545561 arts-2024.4.1/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/art.json
--rw-r--r--   0        0        0     1450 2023-11-05 04:22:04.000000 arts-2024.4.1/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.648073 arts-2024.4.1/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/art.json
--rw-r--r--   0        0        0     3278 2024-02-25 10:11:51.363950 arts-2024.4.1/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.644190 arts-2024.4.1/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/art.json
--rw-r--r--   0        0        0     1265 2024-03-28 16:30:38.111960 arts-2024.4.1/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.645220 arts-2024.4.1/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/art.json
--rw-r--r--   0        0        0     1135 2024-03-04 05:13:36.283230 arts-2024.4.1/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.647184 arts-2024.4.1/arts/articles/300-批判那些伪文艺/800-务实与务虚/art.json
--rw-r--r--   0        0        0     2095 2024-01-18 01:48:33.751985 arts-2024.4.1/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.900873 arts-2024.4.1/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/art.json
--rw-r--r--   0        0        0     1668 2023-11-05 03:35:50.000000 arts-2024.4.1/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.909872 arts-2024.4.1/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/art.json
--rw-r--r--   0        0        0     1669 2023-11-15 13:41:24.000000 arts-2024.4.1/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.903896 arts-2024.4.1/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/art.json
--rw-r--r--   0        0        0     1906 2023-12-27 20:37:35.730568 arts-2024.4.1/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.899872 arts-2024.4.1/arts/articles/450-万象思考/200-人工智能会不会统治人类？/art.json
--rw-r--r--   0        0        0     1154 2023-11-05 02:49:06.000000 arts-2024.4.1/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.907909 arts-2024.4.1/arts/articles/450-万象思考/250-忒修斯之船悖论/art.json
--rw-r--r--   0        0        0     3155 2023-12-27 20:37:10.901781 arts-2024.4.1/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md
--rw-r--r--   0        0        0       44 2024-01-05 13:23:02.578368 arts-2024.4.1/arts/articles/450-万象思考/300-有无相生，难易相成的启发/art.json
--rw-r--r--   0        0        0     1354 2023-11-05 03:42:52.000000 arts-2024.4.1/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md
--rw-r--r--   0        0        0       44 2024-01-05 13:30:30.884939 arts-2024.4.1/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/art.json
--rw-r--r--   0        0        0     1123 2023-09-10 18:11:18.000000 arts-2024.4.1/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.906885 arts-2024.4.1/arts/articles/450-万象思考/500-人们为什么希望拥有后代/art.json
--rw-r--r--   0        0        0      708 2023-12-27 20:36:45.425482 arts-2024.4.1/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.904897 arts-2024.4.1/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/art.json
--rw-r--r--   0        0        0     5024 2023-11-15 13:32:28.000000 arts-2024.4.1/arts/articles/450-万象思考/700-堕胎自由权/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.901873 arts-2024.4.1/arts/articles/450-万象思考/700-堕胎自由权/art.json
--rw-r--r--   0        0        0     3701 2023-11-15 13:30:02.000000 arts-2024.4.1/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.910899 arts-2024.4.1/arts/articles/450-万象思考/800-人人平等是个伪概念/art.json
--rw-r--r--   0        0        0     3385 2023-12-27 20:36:19.402593 arts-2024.4.1/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.414383 arts-2024.4.1/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/art.json
--rw-r--r--   0        0        0     2466 2024-02-25 10:07:00.576902 arts-2024.4.1/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.399805 arts-2024.4.1/arts/articles/600-时空猜想/400-我们可能处在人造世界/art.json
--rw-r--r--   0        0        0     3007 2023-11-04 19:08:36.000000 arts-2024.4.1/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.412423 arts-2024.4.1/arts/articles/600-时空猜想/600-占卜真的存在吗？/art.json
--rw-r--r--   0        0        0     2630 2023-11-04 19:15:30.000000 arts-2024.4.1/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.411378 arts-2024.4.1/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/art.json
--rw-r--r--   0        0        0     2038 2023-12-28 02:10:43.748193 arts-2024.4.1/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md
--rw-r--r--   0        0        0       44 2023-12-28 02:02:17.049897 arts-2024.4.1/arts/articles/700-论时事/300-那些年，我们经历过的历史/art.json
--rw-r--r--   0        0        0     1742 2024-01-13 20:46:22.292355 arts-2024.4.1/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:35.958057 arts-2024.4.1/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/art.json
--rw-r--r--   0        0        0     7343 2023-06-23 06:29:18.000000 arts-2024.4.1/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:05:12.312457 arts-2024.4.1/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/art.json
--rw-r--r--   0        0        0     1652 2023-06-23 06:48:36.000000 arts-2024.4.1/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:05:34.053435 arts-2024.4.1/arts/articles/800-小说/600-一念天堂/050-被绑架/art.json
--rw-r--r--   0        0        0    11283 2024-02-22 12:02:36.224046 arts-2024.4.1/arts/cooltypes/LICENSE
--rw-r--r--   0        0        0      293 2024-03-22 15:18:30.564599 arts-2024.4.1/arts/cooltypes/__init__.py
--rw-r--r--   0        0        0     1542 2024-03-31 09:40:29.228723 arts-2024.4.1/arts/cooltypes/envname/README.md
--rw-r--r--   0        0        0       62 2024-02-23 04:28:30.402332 arts-2024.4.1/arts/cooltypes/envname/__init__.py
--rw-r--r--   0        0        0      409 2024-02-23 04:27:58.084752 arts-2024.4.1/arts/cooltypes/envname/_core.py
--rw-r--r--   0        0        0      865 2024-02-23 04:12:59.530774 arts-2024.4.1/arts/cooltypes/moduledb/README.md
--rw-r--r--   0        0        0       32 2024-02-23 04:03:44.487797 arts-2024.4.1/arts/cooltypes/moduledb/__init__.py
--rw-r--r--   0        0        0     3717 2024-02-23 04:15:35.883622 arts-2024.4.1/arts/cooltypes/moduledb/_core.py
--rw-r--r--   0        0        0        0 2024-03-11 20:20:36.445694 arts-2024.4.1/arts/cooltypes/modules/coolstr/__init__.py
--rw-r--r--   0        0        0     2181 2024-03-22 15:28:12.579126 arts-2024.4.1/arts/cooltypes/modules/coolstr/_core.py
--rw-r--r--   0        0        0     3316 2024-03-31 09:40:29.228723 arts-2024.4.1/arts/cooltypes/modules/cooltime/README.md
--rw-r--r--   0        0        0        0 2024-03-11 20:20:55.541076 arts-2024.4.1/arts/cooltypes/modules/cooltime/__init__.py
--rw-r--r--   0        0        0       44 2024-02-22 10:39:05.460423 arts-2024.4.1/arts/cooltypes/modules/cooltime/_art.json
--rw-r--r--   0        0        0     3665 2024-03-22 15:09:31.411034 arts-2024.4.1/arts/cooltypes/modules/cooltime/_core.py
--rw-r--r--   0        0        0     5793 2024-03-22 15:12:37.868753 arts-2024.4.1/arts/cooltypes/modules/rslice/README.md
--rw-r--r--   0        0        0        0 2024-03-11 20:26:19.316480 arts-2024.4.1/arts/cooltypes/modules/rslice/__init__.py
--rw-r--r--   0        0        0     2801 2024-03-22 15:12:37.864736 arts-2024.4.1/arts/cooltypes/modules/rslice/_core.py
--rw-r--r--   0        0        0        0 2024-03-11 20:22:01.981114 arts-2024.4.1/arts/cooltypes/modules/vtype/__init__.py
--rw-r--r--   0        0        0    10008 2024-03-22 15:22:10.216978 arts-2024.4.1/arts/cooltypes/modules/vtype/_core.py
--rw-r--r--   0        0        0      238 2024-03-22 14:31:42.101320 arts-2024.4.1/arts/cooltypes/设计.md
--rw-r--r--   0        0        0    58636 2024-04-01 02:44:13.049818 arts-2024.4.1/arts/index.html
--rw-r--r--   0        0        0       44 2024-01-16 13:04:45.523107 arts-2024.4.1/arts/life/2018/莆田学院·毕业生留影/art.json
--rw-r--r--   0        0        0      830 2024-02-12 15:02:22.123647 arts-2024.4.1/arts/life/2018/莆田学院·毕业生留影/index.html
--rw-r--r--   0        0        0       44 2024-01-17 04:28:07.076300 arts-2024.4.1/arts/life/2019/苏州市虎丘山/art.json
--rw-r--r--   0        0        0     1233 2024-03-24 16:39:19.059155 arts-2024.4.1/arts/life/2019/苏州市虎丘山/index.html
--rw-r--r--   0        0        0       44 2024-01-17 03:40:13.294365 arts-2024.4.1/arts/life/2022/泉州市丰泽区·雨后街道/art.json
--rw-r--r--   0        0        0      969 2024-03-24 16:39:36.018072 arts-2024.4.1/arts/life/2022/泉州市丰泽区·雨后街道/index.html
--rw-r--r--   0        0        0       44 2024-01-30 05:00:40.402244 arts-2024.4.1/arts/life/2023/更换微信账号了/art.json
--rw-r--r--   0        0        0      832 2024-02-12 15:02:47.979648 arts-2024.4.1/arts/life/2023/更换微信账号了/index.html
--rw-r--r--   0        0        0       44 2024-03-24 16:41:15.708702 arts-2024.4.1/arts/life/2024/泉州市承天禅寺/art.json
--rw-r--r--   0        0        0     1133 2024-03-25 03:52:07.749983 arts-2024.4.1/arts/life/2024/泉州市承天禅寺/index.html
--rw-r--r--   0        0        0    11276 2024-02-22 12:02:36.224046 arts-2024.4.1/arts/miumapp/LICENSE
--rw-r--r--   0        0        0     5762 2024-03-31 09:40:29.228723 arts-2024.4.1/arts/miumapp/README.md
--rw-r--r--   0        0        0       36 2024-02-12 15:08:38.569224 arts-2024.4.1/arts/miumapp/__init__.py
--rw-r--r--   0        0        0     7747 2024-03-25 04:09:08.267200 arts-2024.4.1/arts/miumapp/_core.py
--rw-r--r--   0        0        0      111 2024-03-05 23:26:53.659150 arts-2024.4.1/arts/miumapp/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.1/arts/miumapp/licenses/README.md
--rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.1/arts/miumapp/licenses/pyppeteer/LICENSE
--rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.1/arts/miumapp/licenses/tornado/LICENSE
--rw-r--r--   0        0        0       48 2024-02-12 15:15:42.556195 arts-2024.4.1/arts/miumapp/miumapp/__init__.py
--rw-r--r--   0        0        0     4657 2024-02-22 17:30:50.375647 arts-2024.4.1/arts/miumapp/miumapp/demo.html
--rw-r--r--   0        0        0     1241 2024-03-25 04:09:36.827762 arts-2024.4.1/arts/miumapp/miumapp/demo.py
--rw-r--r--   0        0        0      645 2024-03-12 12:18:10.837369 arts-2024.4.1/arts/miumapp/pyproject.toml
--rw-r--r--   0        0        0    11273 2024-03-02 20:20:55.781363 arts-2024.4.1/arts/oodb/LICENSE
--rw-r--r--   0        0        0    22563 2024-03-31 09:40:29.216952 arts-2024.4.1/arts/oodb/README.md
--rw-r--r--   0        0        0       44 2024-03-06 00:36:04.879589 arts-2024.4.1/arts/oodb/__init__.py
--rw-r--r--   0        0        0    19029 2024-03-06 09:46:30.072966 arts-2024.4.1/arts/oodb/_core.py
--rw-r--r--   0        0        0       99 2024-03-06 01:01:05.433633 arts-2024.4.1/arts/oodb/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.1/arts/oodb/licenses/README.md
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.1/arts/oodb/licenses/pymongo/LICENSE
--rw-r--r--   0        0        0       53 2024-03-06 00:36:04.879589 arts-2024.4.1/arts/oodb/oodb.py
--rw-r--r--   0        0        0      626 2024-03-06 09:57:01.274330 arts-2024.4.1/arts/oodb/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-03-03 07:09:08.518004 arts-2024.4.1/arts/oomongo/LICENSE
--rw-r--r--   0        0        0    17439 2024-03-31 09:40:29.227707 arts-2024.4.1/arts/oomongo/README.md
--rw-r--r--   0        0        0       49 2024-03-05 08:01:41.054010 arts-2024.4.1/arts/oomongo/__init__.py
--rw-r--r--   0        0        0    27613 2024-03-06 00:34:47.221863 arts-2024.4.1/arts/oomongo/_core.py
--rw-r--r--   0        0        0       92 2024-03-06 00:50:10.273786 arts-2024.4.1/arts/oomongo/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.1/arts/oomongo/licenses/README.md
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 arts-2024.4.1/arts/oomongo/licenses/motor/LICENSE
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.1/arts/oomongo/licenses/pymongo/LICENSE
--rw-r--r--   0        0        0       61 2024-03-05 08:01:41.059008 arts-2024.4.1/arts/oomongo/oomongo.py
--rw-r--r--   0        0        0      563 2024-03-06 00:09:25.377118 arts-2024.4.1/arts/oomongo/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-03-03 07:10:17.933453 arts-2024.4.1/arts/oomysql/LICENSE
--rw-r--r--   0        0        0    17139 2024-03-31 09:40:29.228723 arts-2024.4.1/arts/oomysql/README.md
--rw-r--r--   0        0        0       45 2024-03-05 08:02:05.322948 arts-2024.4.1/arts/oomysql/__init__.py
--rw-r--r--   0        0        0    35301 2024-03-24 00:57:24.021318 arts-2024.4.1/arts/oomysql/_core.py
--rw-r--r--   0        0        0       90 2024-03-06 00:10:16.490984 arts-2024.4.1/arts/oomysql/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.1/arts/oomysql/licenses/README.md
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:56.000000 arts-2024.4.1/arts/oomysql/licenses/aiomysql/LICENSE
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 arts-2024.4.1/arts/oomysql/licenses/pymysql/LICENSE
--rw-r--r--   0        0        0       57 2024-03-05 08:02:05.335929 arts-2024.4.1/arts/oomysql/oomysql.py
--rw-r--r--   0        0        0      641 2024-03-06 00:09:38.203916 arts-2024.4.1/arts/oomysql/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 arts-2024.4.1/arts/openai2/LICENSE
--rw-r--r--   0        0        0    13971 2024-03-31 09:40:29.216952 arts-2024.4.1/arts/openai2/README.md
--rw-r--r--   0        0        0      167 2023-12-19 12:18:48.792856 arts-2024.4.1/arts/openai2/__init__.py
--rw-r--r--   0        0        0     6923 2023-11-15 22:45:46.000000 arts-2024.4.1/arts/openai2/_core/GroupChat.py
--rw-r--r--   0        0        0     9258 2023-12-17 18:34:22.000000 arts-2024.4.1/arts/openai2/_core/chat.py
--rw-r--r--   0        0        0     2279 2024-02-23 04:06:51.826269 arts-2024.4.1/arts/openai2/_core/chat_in_cmd.py
--rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 arts-2024.4.1/arts/openai2/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.1/arts/openai2/licenses/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 arts-2024.4.1/arts/openai2/licenses/openai/LICENSE
--rw-r--r--   0        0        0      203 2024-03-03 10:11:45.701543 arts-2024.4.1/arts/openai2/openai2.py
--rw-r--r--   0        0        0      801 2024-03-06 00:09:43.494818 arts-2024.4.1/arts/openai2/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.1/arts/skybox/Copyright
--rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 arts-2024.4.1/arts/skybox/README.md
--rw-r--r--   0        0        0      321 2024-03-31 11:04:55.600521 arts-2024.4.1/arts/skybox/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.1/arts/skybox/skybox/Copyright
--rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 arts-2024.4.1/arts/skybox/skybox/__init__.py
--rw-r--r--   0        0        0    12001 2024-04-01 02:53:11.002626 arts-2024.4.1/arts/skybox/skybox/files_hashes
--rw-r--r--   0        0        0       44 2023-12-19 10:10:36.391618 arts-2024.4.1/arts/thoughts/2022/现代工人的螺丝钉处境/art.json
--rw-r--r--   0        0        0     1374 2024-01-16 22:36:30.326371 arts-2024.4.1/arts/thoughts/2022/现代工人的螺丝钉处境/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.542208 arts-2024.4.1/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/art.json
--rw-r--r--   0        0        0     1346 2024-01-30 04:04:01.359662 arts-2024.4.1/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.562268 arts-2024.4.1/arts/thoughts/2023/专利是个公平的赛道/art.json
--rw-r--r--   0        0        0     1340 2024-03-27 02:41:37.370555 arts-2024.4.1/arts/thoughts/2023/专利是个公平的赛道/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.547209 arts-2024.4.1/arts/thoughts/2023/事情的真实性是由度的/art.json
--rw-r--r--   0        0        0     1001 2024-01-16 22:36:30.329386 arts-2024.4.1/arts/thoughts/2023/事情的真实性是由度的/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.556244 arts-2024.4.1/arts/thoughts/2023/人无法摆脱兽性/art.json
--rw-r--r--   0        0        0     1659 2024-01-16 22:36:30.330406 arts-2024.4.1/arts/thoughts/2023/人无法摆脱兽性/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.551211 arts-2024.4.1/arts/thoughts/2023/什么是极端？/art.json
--rw-r--r--   0        0        0      884 2024-01-16 22:36:30.330406 arts-2024.4.1/arts/thoughts/2023/什么是极端？/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.541243 arts-2024.4.1/arts/thoughts/2023/保护好人/art.json
--rw-r--r--   0        0        0      802 2024-01-16 22:36:30.331373 arts-2024.4.1/arts/thoughts/2023/保护好人/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.554209 arts-2024.4.1/arts/thoughts/2023/只筛选，不教化/art.json
--rw-r--r--   0        0        0      853 2024-01-16 22:36:30.331373 arts-2024.4.1/arts/thoughts/2023/只筛选，不教化/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.549209 arts-2024.4.1/arts/thoughts/2023/喊高考加油是刷存在感/art.json
--rw-r--r--   0        0        0     1047 2024-01-16 22:36:30.332406 arts-2024.4.1/arts/thoughts/2023/喊高考加油是刷存在感/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.552210 arts-2024.4.1/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/art.json
--rw-r--r--   0        0        0     1630 2024-01-16 22:36:30.333372 arts-2024.4.1/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.553243 arts-2024.4.1/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/art.json
--rw-r--r--   0        0        0     2475 2024-01-30 04:03:34.796607 arts-2024.4.1/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.561243 arts-2024.4.1/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/art.json
--rw-r--r--   0        0        0      833 2024-01-18 01:51:26.994040 arts-2024.4.1/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.545246 arts-2024.4.1/arts/thoughts/2023/想去国外了解自己/art.json
--rw-r--r--   0        0        0      966 2024-01-16 22:36:30.335371 arts-2024.4.1/arts/thoughts/2023/想去国外了解自己/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.548245 arts-2024.4.1/arts/thoughts/2023/现代化的分工合作机制/art.json
--rw-r--r--   0        0        0     1668 2024-01-16 22:36:30.335371 arts-2024.4.1/arts/thoughts/2023/现代化的分工合作机制/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.544210 arts-2024.4.1/arts/thoughts/2023/用理性处理简单的事情/art.json
--rw-r--r--   0        0        0     1587 2024-01-16 22:36:30.336371 arts-2024.4.1/arts/thoughts/2023/用理性处理简单的事情/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.557226 arts-2024.4.1/arts/thoughts/2023/真正的问题无法通过花招解决/art.json
--rw-r--r--   0        0        0      977 2024-01-16 22:36:30.336371 arts-2024.4.1/arts/thoughts/2023/真正的问题无法通过花招解决/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.560208 arts-2024.4.1/arts/thoughts/2023/艺术本天成，媒介偶显之/art.json
--rw-r--r--   0        0        0      629 2024-01-16 22:36:30.337410 arts-2024.4.1/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.558244 arts-2024.4.1/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/art.json
--rw-r--r--   0        0        0     1168 2024-01-16 22:36:30.338372 arts-2024.4.1/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html
--rw-r--r--   0        0        0       44 2024-01-13 21:13:40.122707 arts-2024.4.1/arts/thoughts/2024/不要害怕犯错/art.json
--rw-r--r--   0        0        0      698 2024-01-16 22:36:30.339373 arts-2024.4.1/arts/thoughts/2024/不要害怕犯错/index.html
--rw-r--r--   0        0        0       44 2024-01-01 14:23:12.130009 arts-2024.4.1/arts/thoughts/2024/新年题诗/art.json
--rw-r--r--   0        0        0     1152 2024-01-18 06:19:08.705581 arts-2024.4.1/arts/thoughts/2024/新年题诗/index.html
--rw-r--r--   0        0        0       44 2024-01-03 04:10:15.709103 arts-2024.4.1/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/art.json
--rw-r--r--   0        0        0     1270 2024-01-16 22:36:30.341372 arts-2024.4.1/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html
--rw-r--r--   0        0        0       44 2024-03-24 15:35:39.622105 arts-2024.4.1/arts/thoughts/2024/编程语言的进化/art.json
--rw-r--r--   0        0        0     1022 2024-03-24 16:22:12.389078 arts-2024.4.1/arts/thoughts/2024/编程语言的进化/example.html
--rw-r--r--   0        0        0     1520 2024-03-25 03:53:51.266590 arts-2024.4.1/arts/thoughts/2024/编程语言的进化/index.html
--rw-r--r--   0        0        0       44 2024-01-30 04:08:51.850343 arts-2024.4.1/arts/thoughts/2024/萝莉岛事件引发的信任危机/art.json
--rw-r--r--   0        0        0     1077 2024-01-30 04:15:45.681734 arts-2024.4.1/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html
--rw-r--r--   0        0        0       44 2024-01-18 06:20:18.873404 arts-2024.4.1/arts/thoughts/2024/霍金去萝莉岛干嘛了/art.json
--rw-r--r--   0        0        0     1174 2024-01-18 06:24:05.339876 arts-2024.4.1/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html
--rw-r--r--   0        0        0      103 2024-03-03 07:12:46.987154 arts-2024.4.1/arts/tutorials/150-操作MySQL/art.json
--rw-r--r--   0        0        0      103 2024-03-06 00:50:30.486267 arts-2024.4.1/arts/tutorials/225-操作MongoDB/art.json
--rw-r--r--   0        0        0      146 2024-02-25 14:11:14.480558 arts-2024.4.1/arts/tutorials/300-开发桌面GUI应用/art.json
--rw-r--r--   0        0        0      103 2024-02-18 14:43:25.042841 arts-2024.4.1/arts/tutorials/450-对接ChatGPT/art.json
--rw-r--r--   0        0        0      122 2024-03-22 15:10:08.573597 arts-2024.4.1/arts/tutorials/525-时间模块/art.json
--rw-r--r--   0        0        0      100 2024-03-06 01:01:25.689741 arts-2024.4.1/arts/tutorials/562-面向对象数据库/art.json
--rw-r--r--   0        0        0     3415 2023-12-20 10:09:07.822297 arts-2024.4.1/arts/tutorials/600-用37行代码实现AI五子棋/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:14:03.255370 arts-2024.4.1/arts/tutorials/600-用37行代码实现AI五子棋/art.json
--rw-r--r--   0        0        0     8070 2024-02-25 05:45:21.624081 arts-2024.4.1/arts/tutorials/750-正则表达式/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:13:55.412792 arts-2024.4.1/arts/tutorials/750-正则表达式/art.json
--rw-r--r--   0        0        0       44 2024-01-30 03:46:52.790397 arts-2024.4.1/arts/videos/200-秦时明月[项羽]·谪居/art.json
--rw-r--r--   0        0        0       44 2023-12-19 10:07:05.944886 arts-2024.4.1/arts/videos/400-李连杰[霍元甲]·兰亭序/art.json
--rw-r--r--   0        0        0       44 2023-12-19 10:07:05.933448 arts-2024.4.1/arts/videos/600-楚门的世界·五月雨/art.json
--rw-r--r--   0        0        0       44 2024-01-05 13:31:13.729378 arts-2024.4.1/arts/videos/800-AI是这样画包拯的/art.json
--rw-r--r--   0        0        0      524 2024-04-01 02:45:51.624753 arts-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 arts-2024.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2175 2023-12-20 10:09:43.709218 arts-2024.4.3/.gitignore
+-rw-r--r--   0        0        0       46 2024-03-10 10:13:06.948005 arts-2024.4.3/README.md
+-rw-r--r--   0        0        0      317 2024-02-22 12:02:36.224046 arts-2024.4.3/arts/CoolMemory-English/Copyright
+-rw-r--r--   0        0        0    10294 2024-03-31 09:22:44.234618 arts-2024.4.3/arts/CoolMemory-English/README.md
+-rw-r--r--   0        0        0      110 2024-03-06 00:07:28.301653 arts-2024.4.3/arts/CoolMemory-English/art.json
+-rw-r--r--   0        0        0      393 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/README.md
+-rw-r--r--   0        0        0     1586 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE
+-rw-r--r--   0        0        0    11550 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE
+-rw-r--r--   0        0        0    32825 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Python/LICENSE
+-rw-r--r--   0        0        0     2987 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE
+-rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE
+-rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE
+-rw-r--r--   0        0        0      106 2024-03-31 10:18:29.252509 arts-2024.4.3/arts/WeChat-Art-Museum/art.json
+-rw-r--r--   0        0        0    52542 2024-04-03 06:13:33.904082 arts-2024.4.3/arts/WeChat-Art-Museum/index.html
+-rw-r--r--   0        0        0        0 2024-02-22 15:47:26.927352 arts-2024.4.3/arts/__init__.py
+-rw-r--r--   0        0        0     3088 2023-09-24 08:08:30.000000 arts-2024.4.3/arts/articles/010-赚钱宝典/010-财富的本质/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:01:11.532367 arts-2024.4.3/arts/articles/010-赚钱宝典/010-财富的本质/art.json
+-rw-r--r--   0        0        0     1681 2023-12-20 10:09:07.827303 arts-2024.4.3/arts/articles/010-赚钱宝典/020-商业价值/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:01:11.533332 arts-2024.4.3/arts/articles/010-赚钱宝典/020-商业价值/art.json
+-rw-r--r--   0        0        0     3552 2023-12-22 07:27:54.636897 arts-2024.4.3/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md
+-rw-r--r--   0        0        0       44 2023-12-22 07:26:00.584312 arts-2024.4.3/arts/articles/010-赚钱宝典/030-财富稳定型社会/art.json
+-rw-r--r--   0        0        0     1812 2024-01-02 20:05:02.520382 arts-2024.4.3/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md
+-rw-r--r--   0        0        0       44 2024-01-02 20:46:41.567445 arts-2024.4.3/arts/articles/075-追英赶美/300-产业升级与失业潮/art.json
+-rw-r--r--   0        0        0     1253 2024-01-18 01:49:14.297346 arts-2024.4.3/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md
+-rw-r--r--   0        0        0       44 2024-01-02 20:47:04.916014 arts-2024.4.3/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/art.json
+-rw-r--r--   0        0        0     1559 2023-11-15 13:45:10.000000 arts-2024.4.3/arts/articles/150-小民参政/300-广义的民主/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:02:18.547561 arts-2024.4.3/arts/articles/150-小民参政/300-广义的民主/art.json
+-rw-r--r--   0        0        0     1499 2023-10-24 11:49:00.000000 arts-2024.4.3/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:02:18.545561 arts-2024.4.3/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/art.json
+-rw-r--r--   0        0        0     1450 2023-11-05 04:22:04.000000 arts-2024.4.3/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.648073 arts-2024.4.3/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/art.json
+-rw-r--r--   0        0        0     3278 2024-02-25 10:11:51.363950 arts-2024.4.3/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.644190 arts-2024.4.3/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/art.json
+-rw-r--r--   0        0        0     1265 2024-03-28 16:30:38.111960 arts-2024.4.3/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.645220 arts-2024.4.3/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/art.json
+-rw-r--r--   0        0        0     1135 2024-03-04 05:13:36.283230 arts-2024.4.3/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.647184 arts-2024.4.3/arts/articles/300-批判那些伪文艺/800-务实与务虚/art.json
+-rw-r--r--   0        0        0     2095 2024-01-18 01:48:33.751985 arts-2024.4.3/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.900873 arts-2024.4.3/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/art.json
+-rw-r--r--   0        0        0     1668 2023-11-05 03:35:50.000000 arts-2024.4.3/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.909872 arts-2024.4.3/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/art.json
+-rw-r--r--   0        0        0     1669 2023-11-15 13:41:24.000000 arts-2024.4.3/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.903896 arts-2024.4.3/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/art.json
+-rw-r--r--   0        0        0     1906 2023-12-27 20:37:35.730568 arts-2024.4.3/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.899872 arts-2024.4.3/arts/articles/450-万象思考/200-人工智能会不会统治人类？/art.json
+-rw-r--r--   0        0        0     1154 2023-11-05 02:49:06.000000 arts-2024.4.3/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.907909 arts-2024.4.3/arts/articles/450-万象思考/250-忒修斯之船悖论/art.json
+-rw-r--r--   0        0        0     3155 2023-12-27 20:37:10.901781 arts-2024.4.3/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md
+-rw-r--r--   0        0        0       44 2024-01-05 13:23:02.578368 arts-2024.4.3/arts/articles/450-万象思考/300-有无相生，难易相成的启发/art.json
+-rw-r--r--   0        0        0     1354 2023-11-05 03:42:52.000000 arts-2024.4.3/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md
+-rw-r--r--   0        0        0       44 2024-01-05 13:30:30.884939 arts-2024.4.3/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/art.json
+-rw-r--r--   0        0        0     1123 2023-09-10 18:11:18.000000 arts-2024.4.3/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.906885 arts-2024.4.3/arts/articles/450-万象思考/500-人们为什么希望拥有后代/art.json
+-rw-r--r--   0        0        0      708 2023-12-27 20:36:45.425482 arts-2024.4.3/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.904897 arts-2024.4.3/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/art.json
+-rw-r--r--   0        0        0     5024 2023-11-15 13:32:28.000000 arts-2024.4.3/arts/articles/450-万象思考/700-堕胎自由权/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.901873 arts-2024.4.3/arts/articles/450-万象思考/700-堕胎自由权/art.json
+-rw-r--r--   0        0        0     3701 2023-11-15 13:30:02.000000 arts-2024.4.3/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.910899 arts-2024.4.3/arts/articles/450-万象思考/800-人人平等是个伪概念/art.json
+-rw-r--r--   0        0        0     3385 2023-12-27 20:36:19.402593 arts-2024.4.3/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.414383 arts-2024.4.3/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/art.json
+-rw-r--r--   0        0        0     2466 2024-02-25 10:07:00.576902 arts-2024.4.3/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.399805 arts-2024.4.3/arts/articles/600-时空猜想/400-我们可能处在人造世界/art.json
+-rw-r--r--   0        0        0     3007 2023-11-04 19:08:36.000000 arts-2024.4.3/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.412423 arts-2024.4.3/arts/articles/600-时空猜想/600-占卜真的存在吗？/art.json
+-rw-r--r--   0        0        0     2630 2023-11-04 19:15:30.000000 arts-2024.4.3/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.411378 arts-2024.4.3/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/art.json
+-rw-r--r--   0        0        0     2038 2023-12-28 02:10:43.748193 arts-2024.4.3/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md
+-rw-r--r--   0        0        0       44 2023-12-28 02:02:17.049897 arts-2024.4.3/arts/articles/700-论时事/300-那些年，我们经历过的历史/art.json
+-rw-r--r--   0        0        0     1742 2024-01-13 20:46:22.292355 arts-2024.4.3/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:35.958057 arts-2024.4.3/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/art.json
+-rw-r--r--   0        0        0     7343 2023-06-23 06:29:18.000000 arts-2024.4.3/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:05:12.312457 arts-2024.4.3/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/art.json
+-rw-r--r--   0        0        0     1652 2023-06-23 06:48:36.000000 arts-2024.4.3/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:05:34.053435 arts-2024.4.3/arts/articles/800-小说/600-一念天堂/050-被绑架/art.json
+-rw-r--r--   0        0        0    11283 2024-02-22 12:02:36.224046 arts-2024.4.3/arts/cooltypes/LICENSE
+-rw-r--r--   0        0        0      293 2024-03-22 15:18:30.564599 arts-2024.4.3/arts/cooltypes/__init__.py
+-rw-r--r--   0        0        0     1542 2024-03-31 09:40:29.228723 arts-2024.4.3/arts/cooltypes/envname/README.md
+-rw-r--r--   0        0        0       62 2024-02-23 04:28:30.402332 arts-2024.4.3/arts/cooltypes/envname/__init__.py
+-rw-r--r--   0        0        0      409 2024-02-23 04:27:58.084752 arts-2024.4.3/arts/cooltypes/envname/_core.py
+-rw-r--r--   0        0        0      865 2024-02-23 04:12:59.530774 arts-2024.4.3/arts/cooltypes/moduledb/README.md
+-rw-r--r--   0        0        0       32 2024-02-23 04:03:44.487797 arts-2024.4.3/arts/cooltypes/moduledb/__init__.py
+-rw-r--r--   0        0        0     3717 2024-02-23 04:15:35.883622 arts-2024.4.3/arts/cooltypes/moduledb/_core.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:20:36.445694 arts-2024.4.3/arts/cooltypes/modules/coolstr/__init__.py
+-rw-r--r--   0        0        0     2181 2024-03-22 15:28:12.579126 arts-2024.4.3/arts/cooltypes/modules/coolstr/_core.py
+-rw-r--r--   0        0        0     3316 2024-03-31 09:40:29.228723 arts-2024.4.3/arts/cooltypes/modules/cooltime/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 20:20:55.541076 arts-2024.4.3/arts/cooltypes/modules/cooltime/__init__.py
+-rw-r--r--   0        0        0       44 2024-02-22 10:39:05.460423 arts-2024.4.3/arts/cooltypes/modules/cooltime/_art.json
+-rw-r--r--   0        0        0     3665 2024-03-22 15:09:31.411034 arts-2024.4.3/arts/cooltypes/modules/cooltime/_core.py
+-rw-r--r--   0        0        0     5793 2024-03-22 15:12:37.868753 arts-2024.4.3/arts/cooltypes/modules/rslice/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 20:26:19.316480 arts-2024.4.3/arts/cooltypes/modules/rslice/__init__.py
+-rw-r--r--   0        0        0     2801 2024-03-22 15:12:37.864736 arts-2024.4.3/arts/cooltypes/modules/rslice/_core.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:22:01.981114 arts-2024.4.3/arts/cooltypes/modules/vtype/__init__.py
+-rw-r--r--   0        0        0    10008 2024-03-22 15:22:10.216978 arts-2024.4.3/arts/cooltypes/modules/vtype/_core.py
+-rw-r--r--   0        0        0      238 2024-03-22 14:31:42.101320 arts-2024.4.3/arts/cooltypes/设计.md
+-rw-r--r--   0        0        0    60426 2024-04-03 06:13:25.657966 arts-2024.4.3/arts/index.html
+-rw-r--r--   0        0        0       44 2024-01-16 13:04:45.523107 arts-2024.4.3/arts/life/2018/莆田学院·毕业生留影/art.json
+-rw-r--r--   0        0        0      830 2024-02-12 15:02:22.123647 arts-2024.4.3/arts/life/2018/莆田学院·毕业生留影/index.html
+-rw-r--r--   0        0        0       44 2024-01-17 04:28:07.076300 arts-2024.4.3/arts/life/2019/苏州市虎丘山/art.json
+-rw-r--r--   0        0        0     1233 2024-03-24 16:39:19.059155 arts-2024.4.3/arts/life/2019/苏州市虎丘山/index.html
+-rw-r--r--   0        0        0       44 2024-01-17 03:40:13.294365 arts-2024.4.3/arts/life/2022/泉州市丰泽区·雨后街道/art.json
+-rw-r--r--   0        0        0      969 2024-03-24 16:39:36.018072 arts-2024.4.3/arts/life/2022/泉州市丰泽区·雨后街道/index.html
+-rw-r--r--   0        0        0       44 2024-01-30 05:00:40.402244 arts-2024.4.3/arts/life/2023/更换微信账号了/art.json
+-rw-r--r--   0        0        0      898 2024-04-03 03:17:39.386427 arts-2024.4.3/arts/life/2023/更换微信账号了/index.html
+-rw-r--r--   0        0        0       44 2024-03-24 16:41:15.708702 arts-2024.4.3/arts/life/2024/泉州市承天禅寺/art.json
+-rw-r--r--   0        0        0     1133 2024-03-25 03:52:07.749983 arts-2024.4.3/arts/life/2024/泉州市承天禅寺/index.html
+-rw-r--r--   0        0        0    11276 2024-02-22 12:02:36.224046 arts-2024.4.3/arts/miumapp/LICENSE
+-rw-r--r--   0        0        0     5762 2024-03-31 09:40:29.228723 arts-2024.4.3/arts/miumapp/README.md
+-rw-r--r--   0        0        0       36 2024-02-12 15:08:38.569224 arts-2024.4.3/arts/miumapp/__init__.py
+-rw-r--r--   0        0        0     7747 2024-03-25 04:09:08.267200 arts-2024.4.3/arts/miumapp/_core.py
+-rw-r--r--   0        0        0      111 2024-03-05 23:26:53.659150 arts-2024.4.3/arts/miumapp/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3/arts/miumapp/licenses/README.md
+-rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/miumapp/licenses/pyppeteer/LICENSE
+-rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/miumapp/licenses/tornado/LICENSE
+-rw-r--r--   0        0        0       48 2024-02-12 15:15:42.556195 arts-2024.4.3/arts/miumapp/miumapp/__init__.py
+-rw-r--r--   0        0        0     4657 2024-02-22 17:30:50.375647 arts-2024.4.3/arts/miumapp/miumapp/demo.html
+-rw-r--r--   0        0        0     1241 2024-03-25 04:09:36.827762 arts-2024.4.3/arts/miumapp/miumapp/demo.py
+-rw-r--r--   0        0        0      645 2024-03-12 12:18:10.837369 arts-2024.4.3/arts/miumapp/pyproject.toml
+-rw-r--r--   0        0        0    11273 2024-03-02 20:20:55.781363 arts-2024.4.3/arts/oodb/LICENSE
+-rw-r--r--   0        0        0    22563 2024-03-31 09:40:29.216952 arts-2024.4.3/arts/oodb/README.md
+-rw-r--r--   0        0        0       44 2024-03-06 00:36:04.879589 arts-2024.4.3/arts/oodb/__init__.py
+-rw-r--r--   0        0        0    19029 2024-03-06 09:46:30.072966 arts-2024.4.3/arts/oodb/_core.py
+-rw-r--r--   0        0        0       99 2024-03-06 01:01:05.433633 arts-2024.4.3/arts/oodb/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3/arts/oodb/licenses/README.md
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.3/arts/oodb/licenses/pymongo/LICENSE
+-rw-r--r--   0        0        0       53 2024-03-06 00:36:04.879589 arts-2024.4.3/arts/oodb/oodb.py
+-rw-r--r--   0        0        0      626 2024-03-06 09:57:01.274330 arts-2024.4.3/arts/oodb/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-03-03 07:09:08.518004 arts-2024.4.3/arts/oomongo/LICENSE
+-rw-r--r--   0        0        0    17439 2024-03-31 09:40:29.227707 arts-2024.4.3/arts/oomongo/README.md
+-rw-r--r--   0        0        0       49 2024-03-05 08:01:41.054010 arts-2024.4.3/arts/oomongo/__init__.py
+-rw-r--r--   0        0        0    27613 2024-03-06 00:34:47.221863 arts-2024.4.3/arts/oomongo/_core.py
+-rw-r--r--   0        0        0       92 2024-03-06 00:50:10.273786 arts-2024.4.3/arts/oomongo/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3/arts/oomongo/licenses/README.md
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 arts-2024.4.3/arts/oomongo/licenses/motor/LICENSE
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.3/arts/oomongo/licenses/pymongo/LICENSE
+-rw-r--r--   0        0        0       61 2024-03-05 08:01:41.059008 arts-2024.4.3/arts/oomongo/oomongo.py
+-rw-r--r--   0        0        0      563 2024-03-06 00:09:25.377118 arts-2024.4.3/arts/oomongo/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-03-03 07:10:17.933453 arts-2024.4.3/arts/oomysql/LICENSE
+-rw-r--r--   0        0        0    17139 2024-03-31 09:40:29.228723 arts-2024.4.3/arts/oomysql/README.md
+-rw-r--r--   0        0        0       45 2024-03-05 08:02:05.322948 arts-2024.4.3/arts/oomysql/__init__.py
+-rw-r--r--   0        0        0    35301 2024-03-24 00:57:24.021318 arts-2024.4.3/arts/oomysql/_core.py
+-rw-r--r--   0        0        0       90 2024-03-06 00:10:16.490984 arts-2024.4.3/arts/oomysql/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3/arts/oomysql/licenses/README.md
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:56.000000 arts-2024.4.3/arts/oomysql/licenses/aiomysql/LICENSE
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 arts-2024.4.3/arts/oomysql/licenses/pymysql/LICENSE
+-rw-r--r--   0        0        0       57 2024-03-05 08:02:05.335929 arts-2024.4.3/arts/oomysql/oomysql.py
+-rw-r--r--   0        0        0      641 2024-03-06 00:09:38.203916 arts-2024.4.3/arts/oomysql/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 arts-2024.4.3/arts/openai2/LICENSE
+-rw-r--r--   0        0        0    13971 2024-03-31 09:40:29.216952 arts-2024.4.3/arts/openai2/README.md
+-rw-r--r--   0        0        0      167 2023-12-19 12:18:48.792856 arts-2024.4.3/arts/openai2/__init__.py
+-rw-r--r--   0        0        0     6923 2023-11-15 22:45:46.000000 arts-2024.4.3/arts/openai2/_core/GroupChat.py
+-rw-r--r--   0        0        0     9258 2023-12-17 18:34:22.000000 arts-2024.4.3/arts/openai2/_core/chat.py
+-rw-r--r--   0        0        0     2279 2024-02-23 04:06:51.826269 arts-2024.4.3/arts/openai2/_core/chat_in_cmd.py
+-rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 arts-2024.4.3/arts/openai2/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3/arts/openai2/licenses/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 arts-2024.4.3/arts/openai2/licenses/openai/LICENSE
+-rw-r--r--   0        0        0      203 2024-03-03 10:11:45.701543 arts-2024.4.3/arts/openai2/openai2.py
+-rw-r--r--   0        0        0      801 2024-03-06 00:09:43.494818 arts-2024.4.3/arts/openai2/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.3/arts/skybox/Copyright
+-rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 arts-2024.4.3/arts/skybox/README.md
+-rw-r--r--   0        0        0      321 2024-03-31 11:04:55.600521 arts-2024.4.3/arts/skybox/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.3/arts/skybox/skybox/Copyright
+-rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 arts-2024.4.3/arts/skybox/skybox/__init__.py
+-rw-r--r--   0        0        0    12001 2024-04-01 02:53:11.002626 arts-2024.4.3/arts/skybox/skybox/files_hashes
+-rw-r--r--   0        0        0       44 2023-12-19 10:10:36.391618 arts-2024.4.3/arts/thoughts/2022/现代工人的螺丝钉处境/art.json
+-rw-r--r--   0        0        0     1374 2024-01-16 22:36:30.326371 arts-2024.4.3/arts/thoughts/2022/现代工人的螺丝钉处境/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.542208 arts-2024.4.3/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/art.json
+-rw-r--r--   0        0        0     1346 2024-01-30 04:04:01.359662 arts-2024.4.3/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.562268 arts-2024.4.3/arts/thoughts/2023/专利是个公平的赛道/art.json
+-rw-r--r--   0        0        0     1340 2024-03-27 02:41:37.370555 arts-2024.4.3/arts/thoughts/2023/专利是个公平的赛道/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.547209 arts-2024.4.3/arts/thoughts/2023/事情的真实性是由度的/art.json
+-rw-r--r--   0        0        0     1001 2024-01-16 22:36:30.329386 arts-2024.4.3/arts/thoughts/2023/事情的真实性是由度的/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.556244 arts-2024.4.3/arts/thoughts/2023/人无法摆脱兽性/art.json
+-rw-r--r--   0        0        0     1659 2024-01-16 22:36:30.330406 arts-2024.4.3/arts/thoughts/2023/人无法摆脱兽性/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.551211 arts-2024.4.3/arts/thoughts/2023/什么是极端？/art.json
+-rw-r--r--   0        0        0      884 2024-01-16 22:36:30.330406 arts-2024.4.3/arts/thoughts/2023/什么是极端？/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.541243 arts-2024.4.3/arts/thoughts/2023/保护好人/art.json
+-rw-r--r--   0        0        0      802 2024-01-16 22:36:30.331373 arts-2024.4.3/arts/thoughts/2023/保护好人/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.554209 arts-2024.4.3/arts/thoughts/2023/只筛选，不教化/art.json
+-rw-r--r--   0        0        0      853 2024-01-16 22:36:30.331373 arts-2024.4.3/arts/thoughts/2023/只筛选，不教化/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.549209 arts-2024.4.3/arts/thoughts/2023/喊高考加油是刷存在感/art.json
+-rw-r--r--   0        0        0     1047 2024-01-16 22:36:30.332406 arts-2024.4.3/arts/thoughts/2023/喊高考加油是刷存在感/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.552210 arts-2024.4.3/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/art.json
+-rw-r--r--   0        0        0     1630 2024-01-16 22:36:30.333372 arts-2024.4.3/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.553243 arts-2024.4.3/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/art.json
+-rw-r--r--   0        0        0     2475 2024-01-30 04:03:34.796607 arts-2024.4.3/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.561243 arts-2024.4.3/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/art.json
+-rw-r--r--   0        0        0      833 2024-01-18 01:51:26.994040 arts-2024.4.3/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.545246 arts-2024.4.3/arts/thoughts/2023/想去国外了解自己/art.json
+-rw-r--r--   0        0        0      966 2024-01-16 22:36:30.335371 arts-2024.4.3/arts/thoughts/2023/想去国外了解自己/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.548245 arts-2024.4.3/arts/thoughts/2023/现代化的分工合作机制/art.json
+-rw-r--r--   0        0        0     1668 2024-01-16 22:36:30.335371 arts-2024.4.3/arts/thoughts/2023/现代化的分工合作机制/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.544210 arts-2024.4.3/arts/thoughts/2023/用理性处理简单的事情/art.json
+-rw-r--r--   0        0        0     1587 2024-01-16 22:36:30.336371 arts-2024.4.3/arts/thoughts/2023/用理性处理简单的事情/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.557226 arts-2024.4.3/arts/thoughts/2023/真正的问题无法通过花招解决/art.json
+-rw-r--r--   0        0        0      977 2024-01-16 22:36:30.336371 arts-2024.4.3/arts/thoughts/2023/真正的问题无法通过花招解决/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.560208 arts-2024.4.3/arts/thoughts/2023/艺术本天成，媒介偶显之/art.json
+-rw-r--r--   0        0        0      629 2024-01-16 22:36:30.337410 arts-2024.4.3/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.558244 arts-2024.4.3/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/art.json
+-rw-r--r--   0        0        0     1168 2024-01-16 22:36:30.338372 arts-2024.4.3/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html
+-rw-r--r--   0        0        0       44 2024-01-13 21:13:40.122707 arts-2024.4.3/arts/thoughts/2024/不要害怕犯错/art.json
+-rw-r--r--   0        0        0      698 2024-01-16 22:36:30.339373 arts-2024.4.3/arts/thoughts/2024/不要害怕犯错/index.html
+-rw-r--r--   0        0        0       44 2024-04-03 04:23:50.480393 arts-2024.4.3/arts/thoughts/2024/做有趣的事情/art.json
+-rw-r--r--   0        0        0     2071 2024-04-03 05:42:46.206515 arts-2024.4.3/arts/thoughts/2024/做有趣的事情/index.html
+-rw-r--r--   0        0        0       44 2024-01-01 14:23:12.130009 arts-2024.4.3/arts/thoughts/2024/新年题诗/art.json
+-rw-r--r--   0        0        0     1152 2024-01-18 06:19:08.705581 arts-2024.4.3/arts/thoughts/2024/新年题诗/index.html
+-rw-r--r--   0        0        0       44 2024-01-03 04:10:15.709103 arts-2024.4.3/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/art.json
+-rw-r--r--   0        0        0     1270 2024-01-16 22:36:30.341372 arts-2024.4.3/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html
+-rw-r--r--   0        0        0       44 2024-03-24 15:35:39.622105 arts-2024.4.3/arts/thoughts/2024/编程语言的进化/art.json
+-rw-r--r--   0        0        0     1022 2024-03-24 16:22:12.389078 arts-2024.4.3/arts/thoughts/2024/编程语言的进化/example.html
+-rw-r--r--   0        0        0     1520 2024-03-25 03:53:51.266590 arts-2024.4.3/arts/thoughts/2024/编程语言的进化/index.html
+-rw-r--r--   0        0        0       44 2024-01-30 04:08:51.850343 arts-2024.4.3/arts/thoughts/2024/萝莉岛事件引发的信任危机/art.json
+-rw-r--r--   0        0        0     1077 2024-01-30 04:15:45.681734 arts-2024.4.3/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html
+-rw-r--r--   0        0        0       44 2024-01-18 06:20:18.873404 arts-2024.4.3/arts/thoughts/2024/霍金去萝莉岛干嘛了/art.json
+-rw-r--r--   0        0        0     1174 2024-01-18 06:24:05.339876 arts-2024.4.3/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html
+-rw-r--r--   0        0        0      103 2024-03-03 07:12:46.987154 arts-2024.4.3/arts/tutorials/150-操作MySQL/art.json
+-rw-r--r--   0        0        0      103 2024-03-06 00:50:30.486267 arts-2024.4.3/arts/tutorials/225-操作MongoDB/art.json
+-rw-r--r--   0        0        0      146 2024-02-25 14:11:14.480558 arts-2024.4.3/arts/tutorials/300-开发桌面GUI应用/art.json
+-rw-r--r--   0        0        0      103 2024-02-18 14:43:25.042841 arts-2024.4.3/arts/tutorials/450-对接ChatGPT/art.json
+-rw-r--r--   0        0        0      122 2024-03-22 15:10:08.573597 arts-2024.4.3/arts/tutorials/525-时间模块/art.json
+-rw-r--r--   0        0        0      100 2024-03-06 01:01:25.689741 arts-2024.4.3/arts/tutorials/562-面向对象数据库/art.json
+-rw-r--r--   0        0        0     3415 2023-12-20 10:09:07.822297 arts-2024.4.3/arts/tutorials/600-用37行代码实现AI五子棋/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:14:03.255370 arts-2024.4.3/arts/tutorials/600-用37行代码实现AI五子棋/art.json
+-rw-r--r--   0        0        0     8070 2024-02-25 05:45:21.624081 arts-2024.4.3/arts/tutorials/750-正则表达式/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:13:55.412792 arts-2024.4.3/arts/tutorials/750-正则表达式/art.json
+-rw-r--r--   0        0        0       44 2024-01-30 03:46:52.790397 arts-2024.4.3/arts/videos/200-秦时明月[项羽]·谪居/art.json
+-rw-r--r--   0        0        0       44 2023-12-19 10:07:05.944886 arts-2024.4.3/arts/videos/400-李连杰[霍元甲]·兰亭序/art.json
+-rw-r--r--   0        0        0       44 2023-12-19 10:07:05.933448 arts-2024.4.3/arts/videos/600-楚门的世界·五月雨/art.json
+-rw-r--r--   0        0        0       44 2024-01-05 13:31:13.729378 arts-2024.4.3/arts/videos/800-AI是这样画包拯的/art.json
+-rw-r--r--   0        0        0      524 2024-04-03 06:13:45.949704 arts-2024.4.3/pyproject.toml
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 arts-2024.4.3/PKG-INFO
```

### Comparing `arts-2024.4.1/.gitignore` & `arts-2024.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/CoolMemory-English/README.md` & `arts-2024.4.3/arts/CoolMemory-English/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/Python/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Python/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/WeChat-Art-Museum/index.html` & `arts-2024.4.3/arts/WeChat-Art-Museum/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,126 +1,128 @@
 <!DOCTYPE html>
-<html class='ch_149 ch_150' style="background-color:black;"><head>
+<html class='ch_150 ch_151' style="background-color:black;"><head>
 <title>微信艺术馆</title><meta charset='utf-8'><meta name='viewport' content='width=device-width, initial-scale=1.0'>
 <style>
     * {vertical-align:middle; text-decoration:none; position:relative; padding:0; overflow:auto; outline:none; margin:0; font-family:'Chinese Quote', 'Segoe UI', Roboto, RobotoNum, 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'Helvetica Neue', Helvetica, Arial, sans-serif; box-sizing:border-box; border-width:0; border-style:solid;}
-    .ch_149 {width:100vw; height:100vh; display:block; background-color:white;}
-    .ch_151 {width:100%; height:100%; display:block; border-radius:2rem; background-color:rgb(235, 235, 235);}
-    .ch_164 {display:inline-block;}
-    .ch_176 {top:0.4rem; text-align:center; font-size:1.2rem; display:inline-block;}
-    .ch_167 {width:100%; height:4rem; grid-template-columns:3rem 1fr; display:inline-grid; column-gap:0.1rem; align-items:center;}
-    .ch_173 {display:inline-grid;}
-    .ch_181 {width:100%; padding:0 0 0 1rem; height:10rem; grid-template-columns:auto 1fr; display:inline-grid; column-gap:1rem; align-content:center;}
+    .ch_151 {width:100vw; height:100vh; display:block; background-color:white;}
+    .ch_153 {width:100%; height:100%; display:block; border-radius:2rem; background-color:rgb(235, 235, 235);}
+    .ch_165 {display:inline-block;}
+    .ch_178 {top:0.4rem; text-align:center; font-size:1.2rem; display:inline-block;}
+    .ch_168 {width:100%; height:4rem; grid-template-columns:3rem 1fr; display:inline-grid; column-gap:0.1rem; align-items:center;}
+    .ch_175 {display:inline-grid;}
+    .ch_182 {width:100%; padding:0 0 0 1rem; height:10rem; grid-template-columns:auto 1fr; display:inline-grid; column-gap:1rem; align-content:center;}
     .ch_187 {width:100%; height:4rem; grid-template-columns:3rem 1fr; display:inline-grid; column-gap:0.1rem; align-items:center;}
-    .ch_192 {width:100%; grid-template-columns:1fr 1fr 1fr; display:inline-grid;}
-    .ch_165 {width:100%; scrollbar-width:none; padding:0 0.7rem 0 0.7rem; height:100%; grid-auto-flow:row; display:inline-grid; background-color:white; align-content:start; -ms-overflow-style:none  /* 对 IE 和 Edge 隐藏滚动条 */;}
-    .ch_177 {width:100%; scrollbar-width:none; padding:0 0.7rem 0 0.7rem; height:100%; grid-auto-flow:row; display:inline-grid; background-color:white; align-content:start; -ms-overflow-style:none  /* 对 IE 和 Edge 隐藏滚动条 */;}
-    .ch_207 {scrollbar-width:none; height:100%; grid-auto-flow:row; display:inline-grid; align-content:start; -ms-overflow-style:none  /* 对 IE 和 Edge 隐藏滚动条 */;}
-    .ch_293 {scrollbar-width:none; height:100%; grid-auto-flow:row; display:inline-grid; align-content:start; -ms-overflow-style:none  /* 对 IE 和 Edge 隐藏滚动条 */;}
+    .ch_195 {width:100%; grid-template-columns:1fr 1fr 1fr; display:inline-grid;}
+    .ch_167 {width:100%; scrollbar-width:none; padding:0 0.7rem 0 0.7rem; height:100%; grid-auto-flow:row; display:inline-grid; background-color:white; align-content:start; -ms-overflow-style:none  /* 对 IE 和 Edge 隐藏滚动条 */;}
+    .ch_179 {width:100%; scrollbar-width:none; padding:0 0.7rem 0 0.7rem; height:100%; grid-auto-flow:row; display:inline-grid; background-color:white; align-content:start; -ms-overflow-style:none  /* 对 IE 和 Edge 隐藏滚动条 */;}
+    .ch_212 {scrollbar-width:none; height:100%; grid-auto-flow:row; display:inline-grid; align-content:start; -ms-overflow-style:none  /* 对 IE 和 Edge 隐藏滚动条 */;}
+    .ch_302 {scrollbar-width:none; height:100%; grid-auto-flow:row; display:inline-grid; align-content:start; -ms-overflow-style:none  /* 对 IE 和 Edge 隐藏滚动条 */;}
     .ch_166::-webkit-scrollbar {display:none;}
-    .ch_216 {padding:0.618em 1em 0.618em 1em; border-radius:3em; background-color:rgb(0, 179, 98);}
-    .ch_284 {padding:0.618em 1em 0.618em 1em; border-radius:3em; background-color:rgb(239, 239, 239);}
-    .ch_215:hover {background-color:rgb(0, 196, 108);}
-    .ch_283:hover {background-color:rgb(249, 249, 249);}
-    .ch_214:active {background-color:rgb(0, 143, 81);}
-    .ch_282:active {background-color:transparent;}
-    .ch_193 {padding:0.618em 1em 0.618em 1em; color:black; background-color:transparent;}
-    body[is_x_screen='True'] .ch_194:not([is_current_nav="True"]):hover {color:rgb(52, 187, 52);}
-    .ch_195[is_current_nav="True"] {color:rgb(0, 197, 0);}
-    .ch_159 {white-space:nowrap; scrollbar-width:none; overflow-x:auto; display:inline-block; -ms-overflow-style:none;}
-    .ch_158:not(.ch_exec_smooth_to_scrollLeft) {scroll-snap-type:x mandatory;}
+    .ch_217 {padding:0.618em 1em 0.618em 1em; border-radius:3em; background-color:rgb(0, 179, 98);}
+    .ch_286 {padding:0.618em 1em 0.618em 1em; border-radius:3em; background-color:rgb(239, 239, 239);}
+    .ch_216:hover {background-color:rgb(0, 196, 108);}
+    .ch_287:hover {background-color:rgb(249, 249, 249);}
+    .ch_215:active {background-color:rgb(0, 143, 81);}
+    .ch_285:active {background-color:transparent;}
+    .ch_197 {padding:0.618em 1em 0.618em 1em; color:black; background-color:transparent;}
+    body[is_x_screen='True'] .ch_196:not([is_current_nav="True"]):hover {color:rgb(52, 187, 52);}
+    .ch_198[is_current_nav="True"] {color:rgb(0, 197, 0);}
+    .ch_160 {white-space:nowrap; scrollbar-width:none; overflow-x:auto; display:inline-block; -ms-overflow-style:none;}
+    .ch_162:not(.ch_exec_smooth_to_scrollLeft) {scroll-snap-type:x mandatory;}
     .ch_161::-webkit-scrollbar {display:none;}
-    .ch_160 > * {white-space:normal;}
-    .ch_155 {white-space:nowrap; scrollbar-width:none; overflow-x:auto; display:inline-block; -ms-overflow-style:none;}
-    .ch_154:not(.ch_exec_smooth_to_scrollLeft) {scroll-snap-type:x mandatory;}
-    .ch_153::-webkit-scrollbar {display:none;}
-    .ch_156 > * {white-space:normal;}
-    .ch_157 {width:100%; scroll-snap-align:start; overflow:auto; margin:0; height:100%; flex-wrap:wrap; display:inline-flex;}
-    .ch_162 {width:100%; scroll-snap-align:start; overflow:auto; margin:0; height:100%; grid-template-rows:auto 1fr; flex-wrap:wrap; display:inline-grid;}
-    .ch_199 {width:100%; scroll-snap-align:start; overflow:auto; margin:0; height:100%; grid-template-rows:auto 1fr auto; flex-wrap:wrap; display:inline-grid;}
-    .ch_273 {width:100%; scroll-snap-align:start; overflow:auto; margin:0; height:100%; grid-template-rows:auto auto 1fr; flex-wrap:wrap; display:inline-grid; background-color:white;}
-    .ch_172 {vertical-align:middle;}
-    .ch_210 {vertical-align:baseline; display:inline-block;}
+    .ch_159 > * {white-space:normal;}
+    .ch_156 {white-space:nowrap; scrollbar-width:none; overflow-x:auto; display:inline-block; -ms-overflow-style:none;}
+    .ch_155:not(.ch_exec_smooth_to_scrollLeft) {scroll-snap-type:x mandatory;}
+    .ch_154::-webkit-scrollbar {display:none;}
+    .ch_157 > * {white-space:normal;}
+    .ch_158 {width:100%; scroll-snap-align:start; overflow:auto; margin:0; height:100%; flex-wrap:wrap; display:inline-flex;}
+    .ch_163 {width:100%; scroll-snap-align:start; overflow:auto; margin:0; height:100%; grid-template-rows:auto 1fr; flex-wrap:wrap; display:inline-grid;}
+    .ch_201 {width:100%; scroll-snap-align:start; overflow:auto; margin:0; height:100%; grid-template-rows:auto 1fr auto; flex-wrap:wrap; display:inline-grid;}
+    .ch_274 {width:100%; scroll-snap-align:start; overflow:auto; margin:0; height:100%; grid-template-rows:auto auto 1fr; flex-wrap:wrap; display:inline-grid; background-color:white;}
+    .ch_174 {vertical-align:middle;}
+    .ch_231 {vertical-align:baseline; display:inline-block;}
     .ch_213 {white-space:pre-wrap; vertical-align:baseline; padding:0.75em; line-height:1.5; font-size:1rem; border-radius:0.75em;}
-    .ch_211 {white-space:pre-wrap; vertical-align:baseline; padding:0.75em 1.5em 0.75em 1.5em; overflow-wrap:break-word; line-height:1.75; font-size:1rem; border-radius:0.75em;}
-    .ch_278 {width:100%; white-space:pre-wrap; vertical-align:baseline; padding:1rem; overflow-wrap:break-word; line-height:1.75; height:100%; font-size:1rem; border-radius:0.75em;}
-    .ch_184 {vertical-align:baseline; display:inline-block; color:rgba(0, 89, 255, 0.758);}
-    .ch_183:hover {color:rgb(0, 55, 255);}
-    .ch_182:visited {color:rgba(0, 89, 255, 0.758);}
+    .ch_230 {white-space:pre-wrap; vertical-align:baseline; padding:0.75em 1.5em 0.75em 1.5em; overflow-wrap:break-word; line-height:1.75; font-size:1rem; border-radius:0.75em;}
+    .ch_279 {width:100%; white-space:pre-wrap; vertical-align:baseline; padding:1rem; overflow-wrap:break-word; line-height:1.75; height:100%; font-size:1rem; border-radius:0.75em;}
+    .ch_186 {vertical-align:baseline; display:inline-block; color:rgba(0, 89, 255, 0.758);}
+    .ch_185:hover {color:rgb(0, 55, 255);}
+    .ch_184:visited {color:rgba(0, 89, 255, 0.758);}
     .ch_152[is_x_screen='True'] {width:30%;}
-    .ch_163 > :nth-child(1) {text-align:center; padding:0.8rem 0 0.8rem 0;}
-    .ch_179 > :nth-child(1) {height:5rem;}
+    .ch_164 > :nth-child(1) {text-align:center; padding:0.8rem 0 0.8rem 0;}
+    .ch_183 > :nth-child(1) {height:5rem;}
     .ch_180 > :nth-child(2) {height:5rem; grid-template-rows:auto auto; align-content:space-around;}
-    .ch_178 > :nth-child(2) > :nth-child(1) {font-size:1.5rem;}
-    .ch_186 > :nth-child(1) {width:2.5rem; height:2.5rem;}
-    .ch_185 > :nth-child(2) {padding:0.5rem 5rem 0.5rem 0; height:100%; border-width:0 0 0.1rem 0; border-color:rgb(235, 235, 235); align-content:center;}
-    .ch_171 > :nth-child(1) {width:2.5rem; height:2.5rem;}
-    .ch_168 > :nth-child(2) {padding:0.5rem 5rem 0.5rem 0; height:100%; grid-template-rows:auto auto; border-width:0 0 0.1rem 0; border-color:rgb(235, 235, 235); align-content:center;}
-    .ch_169 > :nth-child(3) {right:0.8rem; position:absolute; font-size:0.8rem; color:rgb(152, 152, 152);}
-    .ch_170 > :nth-child(2) > :nth-child(2) {white-space:nowrap; overflow:hidden; font-size:0.8rem; color:rgb(152, 152, 152);}
-    .ch_208 > * {width:100%; margin:0.5rem 0 0.5rem 0; justify-items:center; height:max-content; grid-template-columns:3.5rem 1fr 3.5rem; align-items:start;}
-    .ch_209 > * > :nth-child(2) {padding:0.5em; min-height:2.5rem; max-width:100%; line-height:1.25; border-radius:0.3em;}
-    .ch_204 > * > img + pre {justify-self:left; background-color:white;}
-    .ch_205 > * > span + pre {justify-self:right; background-color:rgb(124, 218, 62);}
-    .ch_206 > * > img {width:2.5rem; height:2.5rem;}
-    .ch_212::-webkit-scrollbar {display:none;}
-    .ch_201 > :nth-child(1) {text-align:center; padding:0.8rem 0 0.8rem 0; background-color:rgb(244, 244, 244);}
-    .ch_200 > :nth-child(3) {width:100%; padding:0.3rem 1.5rem 0.3rem 1.5rem; grid-template-columns:1fr auto; column-gap:0.5rem; background-color:rgb(244, 244, 244); align-items:center;}
-    .ch_198 > :nth-child(1) > :nth-child(1) {transform:rotate(45deg); top:0.5rem; position:absolute; left:1rem; font-size:1.2rem;}
-    .ch_272 > :nth-child(1) {text-align:center; padding:0.8rem 0 0.8rem 0; background-color:rgb(244, 244, 244);}
-    .ch_271 > :nth-child(1) > :nth-child(1) {transform:rotate(45deg); top:0.5rem; position:absolute; left:1rem; font-size:1.2rem;}
-    .ch_295 > * {width:100%; padding:0 0.5rem 0 0; margin:2rem 0 0.5rem 0; height:max-content; grid-template-columns:3.5rem 1fr; align-items:start;}
-    .ch_297 > :nth-child(1) {width:100%; padding:0 0 0 0; margin:0;}
-    .ch_299 > * > img {width:2.5rem; justify-self:center; height:2.5rem;}
-    .ch_291 > * > :nth-child(2) > :nth-child(1) {padding:0 0.5em 0.5em 0; line-height:1; color:rgb(47, 74, 144); border-radius:0;}
-    .ch_292 > * > :nth-child(2) > :nth-child(2) {padding:0 0.5em 0.5em 0; min-height:2.5rem; max-width:100%; line-height:1.75; border-radius:0.3em;}
-    .ch_294 > * > :nth-child(2) > :nth-child(3) {width:100%; position:relative; margin:0 0 1rem 0; justify-content:start;}
-    .ch_296 > * > :nth-child(2) > :nth-child(3) > * {width:100%; margin:0 0 0.25rem 0;}
-    .ch_298 > * > :nth-child(2) > :nth-child(3) > * > * {object-fit:cover;}
-    .ch_276 a {vertical-align:baseline; color:rgba(0, 89, 255, 0.758);}
-    .ch_279 a:hover {color:rgb(0, 55, 255);}
-    .ch_277 a:visited {color:rgba(0, 89, 255, 0.758);}
-    .ch_197 {display:none;}
-    .ch_196 ~ * {display:none;}
+    .ch_181 > :nth-child(2) > :nth-child(1) {font-size:1.5rem;}
+    .ch_188:active {background-color:rgb(244, 244, 244);}
+    .ch_190 > :nth-child(1) {width:2.5rem; height:2.5rem;}
+    .ch_189 > :nth-child(2) {padding:0.5rem 5rem 0.5rem 0; height:100%; border-width:0 0 0.1rem 0; border-color:rgb(235, 235, 235); align-content:center;}
+    .ch_169:active {background-color:rgb(244, 244, 244);}
+    .ch_170 > :nth-child(1) {width:2.5rem; height:2.5rem;}
+    .ch_171 > :nth-child(2) {padding:0.5rem 5rem 0.5rem 0; height:100%; grid-template-rows:auto auto; border-width:0 0 0.1rem 0; border-color:rgb(235, 235, 235); align-content:center;}
+    .ch_172 > :nth-child(3) {right:0.8rem; position:absolute; font-size:0.8rem; color:rgb(152, 152, 152);}
+    .ch_173 > :nth-child(2) > :nth-child(2) {white-space:nowrap; overflow:hidden; font-size:0.8rem; color:rgb(152, 152, 152);}
+    .ch_207 > * {width:100%; margin:0.5rem 0 0.5rem 0; justify-items:center; height:max-content; grid-template-columns:3.5rem 1fr 3.5rem; align-items:start;}
+    .ch_208 > * > :nth-child(2) {padding:0.5em; min-height:2.5rem; max-width:100%; line-height:1.25; border-radius:0.3em;}
+    .ch_209 > * > img + pre {justify-self:left; background-color:white;}
+    .ch_210 > * > span + pre {justify-self:right; background-color:rgb(124, 218, 62);}
+    .ch_211 > * > img {width:2.5rem; height:2.5rem;}
+    .ch_214::-webkit-scrollbar {display:none;}
+    .ch_203 > :nth-child(1) {text-align:center; padding:0.8rem 0 0.8rem 0; background-color:rgb(244, 244, 244);}
+    .ch_202 > :nth-child(3) {width:100%; padding:0.3rem 1.5rem 0.3rem 1.5rem; grid-template-columns:1fr auto; column-gap:0.5rem; background-color:rgb(244, 244, 244); align-items:center;}
+    .ch_204 > :nth-child(1) > :nth-child(1) {transform:rotate(45deg); top:0.5rem; position:absolute; left:1rem; font-size:1.2rem;}
+    .ch_276 > :nth-child(1) {text-align:center; padding:0.8rem 0 0.8rem 0; background-color:rgb(244, 244, 244);}
+    .ch_275 > :nth-child(1) > :nth-child(1) {transform:rotate(45deg); top:0.5rem; position:absolute; left:1rem; font-size:1.2rem;}
+    .ch_294 > * {width:100%; padding:0 0.5rem 0 0; margin:2rem 0 0.5rem 0; height:max-content; grid-template-columns:3.5rem 1fr; align-items:start;}
+    .ch_296 > :nth-child(1) {width:100%; padding:0 0 0 0; margin:0;}
+    .ch_298 > * > img {width:2.5rem; justify-self:center; height:2.5rem;}
+    .ch_299 > * > :nth-child(2) > :nth-child(1) {padding:0 0.5em 0.5em 0; line-height:1; color:rgb(47, 74, 144); border-radius:0;}
+    .ch_300 > * > :nth-child(2) > :nth-child(2) {padding:0 0.5em 0.5em 0; min-height:2.5rem; max-width:100%; line-height:1.75; border-radius:0.3em;}
+    .ch_301 > * > :nth-child(2) > :nth-child(3) {width:100%; position:relative; margin:0 0 1rem 0; justify-content:start;}
+    .ch_295 > * > :nth-child(2) > :nth-child(3) > * {width:100%; margin:0 0 0.25rem 0;}
+    .ch_297 > * > :nth-child(2) > :nth-child(3) > * > * {object-fit:cover;}
+    .ch_282 a {vertical-align:baseline; color:rgba(0, 89, 255, 0.758);}
+    .ch_281 a:hover {color:rgb(0, 55, 255);}
+    .ch_280 a:visited {color:rgba(0, 89, 255, 0.758);}
+    .ch_200 {display:none;}
+    .ch_199 ~ * {display:none;}
 </style></head>
-<body class='ch_151 ch_152'>
+<body class='ch_152 ch_153'>
 <script>const ch = {}
-</script><div class='ch_153 ch_154 ch_155 ch_156' id='ch_14' style="height:100%; width:100%;"><div class='ch_157' style="display:inline-grid; grid-template-rows:1fr auto;"><div class='ch_158 ch_159 ch_160 ch_161' id='ch_129' style="height:100%;"><div class='ch_162 ch_163'><div class='ch_164'>微信</div><div class='ch_165 ch_166' id='ch_7'><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_28'><img class='ch_172' src='ip_static/头像/JS小黄老师.jpg'><div class='ch_173'><div class='ch_164'>JS小黄老师</div><div class='ch_164'>0,1,2,3,4,5,6,7,8,9</div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_36'><img class='ch_172' src='ip_static/头像/会说话的汤姆猫.jpg'><div class='ch_173'><div class='ch_164'>会说话的汤姆猫</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_42'><img class='ch_172' src='ip_static/头像/鲁迅.jpg'><div class='ch_173'><div class='ch_164'>鲁迅</div><div class='ch_164'>什么是滑坡论证？</div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_48'><img class='ch_172' src='ip_static/头像/刘德华.jpg'><div class='ch_173'><div class='ch_164'>刘德华</div><div class='ch_164'>唉··· 今天你就见到了</div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_54'><img class='ch_172' src='ip_static/头像/项羽.jpg'><div class='ch_173'><div class='ch_164'>项羽</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_60'><img class='ch_172' src='ip_static/头像/李连杰.jpg'><div class='ch_173'><div class='ch_164'>李连杰</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_66'><img class='ch_172' src='ip_static/头像/楚门.jpg'><div class='ch_173'><div class='ch_164'>楚门</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_72'><img class='ch_172' src='ip_static/头像/亚里士多德.jpg'><div class='ch_173'><div class='ch_164'>亚里士多德</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_78'><img class='ch_172' src='ip_static/头像/霍金.jpg'><div class='ch_173'><div class='ch_164'>霍金</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_84'><img class='ch_172' src='ip_static/头像/牛顿.jpg'><div class='ch_173'><div class='ch_164'>牛顿</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_90'><img class='ch_172' src='ip_static/头像/爱因斯坦.jpg'><div class='ch_173'><div class='ch_164'>爱因斯坦</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_96'><img class='ch_172' src='ip_static/头像/玻尔.jpg'><div class='ch_173'><div class='ch_164'>玻尔</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_102'><img class='ch_172' src='ip_static/头像/岸本齐史.jpg'><div class='ch_173'><div class='ch_164'>岸本齐史</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_108'><img class='ch_172' src='ip_static/头像/叔本华.jpg'><div class='ch_173'><div class='ch_164'>叔本华</div><div class='ch_164'></div></div><div class='ch_164'>刚刚</div></div></div></div><div class='ch_162 ch_163'><div class='ch_164'>发现</div><div class='ch_165 ch_166' id='ch_10'><div class='ch_167 ch_168 ch_169 ch_170 ch_171' id='ch_174'><div class='ch_176'>🌐</div><div class='ch_173'>朋友圈</div></div><div class='ch_167 ch_168 ch_169 ch_170 ch_171' style="color:rgb(167, 165, 165);"><div class='ch_176'>🎲</div><div class='ch_173'>小程序</div></div></div></div><div class='ch_157'><div class='ch_177 ch_166' id='ch_12'><div class='ch_178 ch_179 ch_180 ch_181'><img class='ch_172' src='ip_static/头像/我.jpg'><div class='ch_173'><div class='ch_164'><a class='ch_182 ch_183 ch_184' href='https://lcctoor.github.io/arts/' target='_blank'>江南雨上</a></div><div class='ch_164'>艺术本天成，媒介偶显之。</div></div></div><div class='ch_185 ch_186 ch_187'><div class='ch_176'>💰</div><div class='ch_173' id='ch_188'>钱包</div></div><div class='ch_185 ch_186 ch_187' style="color:rgb(167, 165, 165);"><div class='ch_176'>⚙️</div><div class='ch_173'>设置</div></div><div class='ch_185 ch_186 ch_187' id='ch_190'><div class='ch_176'>📃</div><div class='ch_173'>关于此项目</div></div></div></div></div><div class='ch_192' id='ch_122'><button class='is_nav ch_193 ch_194 ch_195' is_current_nav='True'>💬<br/>聊天</button><button class='is_nav ch_193 ch_194 ch_195'>🌍<br/>发现</button><button class='is_nav ch_193 ch_194 ch_195'>👨‍💻<br/>我</button></div></div><span class='ch_196 ch_197' id='ch_16'></span><div class='ch_198 ch_199 ch_200 ch_201' id='ch_30'><div class='ch_164'>JS小黄老师<div class='ch_164' id='ch_202'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_26'><div class='ch_173'><span class='ch_210'></span><pre class='ch_211'>'你好呀'</pre><img class='ch_172' src='ip_static/头像/我.jpg'></div><div class='ch_173'><img class='ch_172' src='ip_static/头像/JS小黄老师.jpg'><pre class='ch_211'>你好呀</pre><span class='ch_210'></span></div><div class='ch_173'><span class='ch_210'></span><pre class='ch_211'>1 + 1</pre><img class='ch_172' src='ip_static/头像/我.jpg'></div><div class='ch_173'><img class='ch_172' src='ip_static/头像/JS小黄老师.jpg'><pre class='ch_211'>2</pre><span class='ch_210'></span></div><div class='ch_173'><span class='ch_210'></span><pre class='ch_211'>[...Array(10).keys()]</pre><img class='ch_172' src='ip_static/头像/我.jpg'></div><div class='ch_173'><img class='ch_172' src='ip_static/头像/JS小黄老师.jpg'><pre class='ch_211'>0,1,2,3,4,5,6,7,8,9</pre><span class='ch_210'></span></div></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_217'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_38'><div class='ch_164'>会说话的汤姆猫<div class='ch_164' id='ch_219'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_34'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2' id='ch_134'></textarea><button class='ch_214 ch_215 ch_216' id='ch_221'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_44'><div class='ch_164'>鲁迅<div class='ch_164' id='ch_223'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_40'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2' id='ch_136'></textarea><button class='ch_214 ch_215 ch_216' id='ch_225'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_50'><div class='ch_164'>刘德华<div class='ch_164' id='ch_227'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_46'><div class='ch_173'><img class='ch_172' src='ip_static/头像/刘德华.jpg'><pre class='ch_211'>我长这么大，没见过这么嚣张的人</pre><span class='ch_210'></span></div><div class='ch_173'><span class='ch_210'></span><pre class='ch_211'>唉··· 今天你就见到了</pre><img class='ch_172' src='ip_static/头像/我.jpg'></div></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_229'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_56'><div class='ch_164'>项羽<div class='ch_164' id='ch_231'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_52'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_233'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_62'><div class='ch_164'>李连杰<div class='ch_164' id='ch_235'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_58'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_237'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_68'><div class='ch_164'>楚门<div class='ch_164' id='ch_239'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_64'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_241'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_74'><div class='ch_164'>亚里士多德<div class='ch_164' id='ch_243'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_70'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_245'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_80'><div class='ch_164'>霍金<div class='ch_164' id='ch_247'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_76'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_249'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_86'><div class='ch_164'>牛顿<div class='ch_164' id='ch_251'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_82'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_253'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_92'><div class='ch_164'>爱因斯坦<div class='ch_164' id='ch_255'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_88'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_257'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_98'><div class='ch_164'>玻尔<div class='ch_164' id='ch_259'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_94'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_261'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_104'><div class='ch_164'>岸本齐史<div class='ch_164' id='ch_263'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_100'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_265'>发送</button></div></div><div class='ch_198 ch_199 ch_200 ch_201' id='ch_110'><div class='ch_164'>叔本华<div class='ch_164' id='ch_267'>∟</div></div><div class='ch_204 ch_205 ch_206 ch_207 ch_208 ch_166 ch_209' id='ch_106'></div><div class='ch_173'><textarea class='ch_212 ch_213' rows='2'></textarea><button class='ch_214 ch_215 ch_216' id='ch_269'>发送</button></div></div><div class='ch_271 ch_272 ch_273' id='ch_138' style="grid-template-rows:auto 1fr;"><div class='ch_164'>关于此项目<div class='ch_164' id='ch_274'>∟</div></div><pre class='ch_276 ch_277 ch_278 ch_279'>
+</script><div class='ch_154 ch_155 ch_156 ch_157' id='ch_13' style="height:100%; width:100%;"><div class='ch_158' style="display:inline-grid; grid-template-rows:1fr auto;"><div class='ch_159 ch_160 ch_161 ch_162' id='ch_129' style="height:100%;"><div class='ch_163 ch_164'><div class='ch_165'>聊天</div><div class='ch_166 ch_167' id='ch_6'><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_27'><img class='ch_174' src='ip_static/头像/JS小黄老师.jpg'><div class='ch_175'><div class='ch_165'>JS小黄老师</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_36'><img class='ch_174' src='ip_static/头像/会说话的汤姆猫.jpg'><div class='ch_175'><div class='ch_165'>会说话的汤姆猫</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_42'><img class='ch_174' src='ip_static/头像/鲁迅.jpg'><div class='ch_175'><div class='ch_165'>鲁迅</div><div class='ch_165'>什么是滑坡论证？</div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_48'><img class='ch_174' src='ip_static/头像/刘德华.jpg'><div class='ch_175'><div class='ch_165'>刘德华</div><div class='ch_165'>唉··· 今天你就见到了</div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_54'><img class='ch_174' src='ip_static/头像/项羽.jpg'><div class='ch_175'><div class='ch_165'>项羽</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_60'><img class='ch_174' src='ip_static/头像/李连杰.jpg'><div class='ch_175'><div class='ch_165'>李连杰</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_66'><img class='ch_174' src='ip_static/头像/楚门.jpg'><div class='ch_175'><div class='ch_165'>楚门</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_72'><img class='ch_174' src='ip_static/头像/亚里士多德.jpg'><div class='ch_175'><div class='ch_165'>亚里士多德</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_78'><img class='ch_174' src='ip_static/头像/霍金.jpg'><div class='ch_175'><div class='ch_165'>霍金</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_84'><img class='ch_174' src='ip_static/头像/牛顿.jpg'><div class='ch_175'><div class='ch_165'>牛顿</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_90'><img class='ch_174' src='ip_static/头像/爱因斯坦.jpg'><div class='ch_175'><div class='ch_165'>爱因斯坦</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_96'><img class='ch_174' src='ip_static/头像/玻尔.jpg'><div class='ch_175'><div class='ch_165'>玻尔</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_102'><img class='ch_174' src='ip_static/头像/岸本齐史.jpg'><div class='ch_175'><div class='ch_165'>岸本齐史</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_108'><img class='ch_174' src='ip_static/头像/叔本华.jpg'><div class='ch_175'><div class='ch_165'>叔本华</div><div class='ch_165'></div></div><div class='ch_165'>刚刚</div></div></div></div><div class='ch_163 ch_164'><div class='ch_165'>发现</div><div class='ch_166 ch_167' id='ch_9'><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' id='ch_176'><div class='ch_178'>🌐</div><div class='ch_175'>朋友圈</div></div><div class='ch_168 ch_169 ch_170 ch_171 ch_172 ch_173' style="color:rgb(167, 165, 165);"><div class='ch_178'>🎲</div><div class='ch_175'>小程序</div></div></div></div><div class='ch_158'><div class='ch_179 ch_166' id='ch_11'><div class='ch_180 ch_181 ch_182 ch_183'><img class='ch_174' src='ip_static/头像/我.jpg'><div class='ch_175'><div class='ch_165'><a class='ch_184 ch_185 ch_186' href='https://lcctoor.github.io/arts/' target='_blank'>江南雨上</a></div><div class='ch_165'>艺术本天成，媒介偶显之。</div></div></div><div class='ch_187 ch_188 ch_189 ch_190'><div class='ch_178'>💰</div><div class='ch_175' id='ch_191'>钱包</div></div><div class='ch_187 ch_188 ch_189 ch_190' style="color:rgb(167, 165, 165);"><div class='ch_178'>⚙️</div><div class='ch_175'>设置</div></div><div class='ch_187 ch_188 ch_189 ch_190' id='ch_193'><div class='ch_178'>📃</div><div class='ch_175'>关于此项目</div></div></div></div></div><div class='ch_195' id='ch_122'><button class='is_nav ch_196 ch_197 ch_198' is_current_nav='True'>💬<br/>聊天</button><button class='is_nav ch_196 ch_197 ch_198'>🌍<br/>发现</button><button class='is_nav ch_196 ch_197 ch_198'>👨‍💻<br/>我</button></div></div><span class='ch_199 ch_200' id='ch_15'></span><div class='ch_201 ch_202 ch_203 ch_204' id='ch_29'><div class='ch_165'>JS小黄老师<div class='ch_165' id='ch_205'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_25'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_218'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_38'><div class='ch_165'>会说话的汤姆猫<div class='ch_165' id='ch_220'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_34'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2' id='ch_135'></textarea><button class='ch_215 ch_216 ch_217' id='ch_222'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_44'><div class='ch_165'>鲁迅<div class='ch_165' id='ch_224'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_40'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2' id='ch_137'></textarea><button class='ch_215 ch_216 ch_217' id='ch_226'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_50'><div class='ch_165'>刘德华<div class='ch_165' id='ch_228'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_46'><div class='ch_175'><img class='ch_174' src='ip_static/头像/刘德华.jpg'><pre class='ch_230'>我长这么大，没见过这么嚣张的人</pre><span class='ch_231'></span></div><div class='ch_175'><span class='ch_231'></span><pre class='ch_230'>唉··· 今天你就见到了</pre><img class='ch_174' src='ip_static/头像/我.jpg'></div></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_232'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_56'><div class='ch_165'>项羽<div class='ch_165' id='ch_234'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_52'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_236'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_62'><div class='ch_165'>李连杰<div class='ch_165' id='ch_238'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_58'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_240'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_68'><div class='ch_165'>楚门<div class='ch_165' id='ch_242'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_64'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_244'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_74'><div class='ch_165'>亚里士多德<div class='ch_165' id='ch_246'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_70'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_248'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_80'><div class='ch_165'>霍金<div class='ch_165' id='ch_250'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_76'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_252'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_86'><div class='ch_165'>牛顿<div class='ch_165' id='ch_254'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_82'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_256'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_92'><div class='ch_165'>爱因斯坦<div class='ch_165' id='ch_258'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_88'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_260'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_98'><div class='ch_165'>玻尔<div class='ch_165' id='ch_262'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_94'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_264'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_104'><div class='ch_165'>岸本齐史<div class='ch_165' id='ch_266'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_100'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_268'>发送</button></div></div><div class='ch_201 ch_202 ch_203 ch_204' id='ch_110'><div class='ch_165'>叔本华<div class='ch_165' id='ch_270'>∟</div></div><div class='ch_207 ch_208 ch_209 ch_210 ch_166 ch_211 ch_212' id='ch_106'></div><div class='ch_175'><textarea class='ch_213 ch_214' rows='2'></textarea><button class='ch_215 ch_216 ch_217' id='ch_272'>发送</button></div></div><div class='ch_274 ch_275 ch_276' id='ch_139' style="grid-template-rows:auto 1fr;"><div class='ch_165'>关于此项目<div class='ch_165' id='ch_277'>∟</div></div><pre class='ch_279 ch_280 ch_281 ch_282'>
 <h1>版权声明</h1>
 Copyright 2024 lcctoor@outlook.com
 
 <h1>作者</h1>
 <a href='mailto:lcctoor@outlook.com' target='_blank'>江南雨上</a>
 <a href='https://lcctoor.github.io/arts' target='_blank'>主页</a> | <a href='https://github.com/lcctoor' target='_blank'>Github</a> | <a href='https://pypi.org/user/lcctoor' target='_blank'>PyPi</a> | <a href='https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg' target='_blank'>微信</a> | <a href='mailto:lcctoor@outlook.com' target='_blank'>邮箱</a> | <a href='https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg' target='_blank'>捐赠</a>
 
 <h1>Bug提交、功能提议</h1>
 你可以通过 <a href='https://github.com/lcctoor/arts/issues' target='_blank'>Github-Issues</a>、<a href='https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg' target='_blank'>微信</a> 与我联系。
 
 <h1><a href='https://github.com/lcctoor/arts/tree/main/arts/WeChat-Art-Museum' target='_blank'>项目地址 👈</a></h1>
-</pre></div><div class='ch_271 ch_272 ch_273' id='ch_140'><div class='ch_164'>钱包<div class='ch_164' id='ch_280'>∟</div></div><div class='ch_173' style="background-color:rgb(38, 170, 82); justify-content:space-around; grid-template-columns:auto auto; border-radius:1rem; height:9rem; margin:0.5rem; align-content:center; align-items:center;"><div class='ch_173' style="grid-template-rows:1fr 1fr; color:white; height:5rem; width:7rem; justify-content:center; justify-items:center; text-align:center; align-content:center; align-items:center; border-radius:1rem;"><span class='ch_210' style="align-self:end;">余额</span><span class='ch_210' style="align-self:start;">¥499.00</span></div><button class='ch_282 ch_283 ch_284' id='ch_285'>提现</button></div></div><div class='ch_271 ch_272 ch_273' id='ch_142' style="grid-template-rows:auto 1fr;"><div class='ch_164'>捐赠<div class='ch_164' id='ch_287'>∟</div></div><div class='ch_173' style="grid-template-rows:auto auto; justify-content:center; align-content:space-evenly; justify-items:center; padding:1rem; text-align:center;"><img class='ch_172' src='https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg' style="height:15rem;"><div class='ch_164' style="font-size:1.5rem;">感谢你进入到这里，这说明你对这个软件还是有一些兴趣的！如果你喜欢这个作品，就请支持一下吧！(^_^)</div></div></div><div class='ch_271 ch_272 ch_273' id='ch_146'><div class='ch_164'>朋友圈<div class='ch_164' id='ch_289'>∟</div></div><div class='ch_291 ch_292 ch_293 ch_294 ch_295 ch_166 ch_296 ch_297 ch_298 ch_299' id='ch_144'><img class='ch_172' src='ip_static/封面.jpg'><div class='ch_173'><img class='ch_172' src='ip_static/头像/李连杰.jpg'><div class='ch_164'><pre class='ch_211'>李连杰</pre><pre class='ch_211'>我发布了短视频</pre><div class='ch_164'><video loading='lazy' controls><source src='https://lcctoor.github.io/arts/arts/videos/400-李连杰[霍元甲]·兰亭序/README.mp4' type='video/mp4'></video></div></div></div><div class='ch_173'><img class='ch_172' src='ip_static/头像/项羽.jpg'><div class='ch_164'><pre class='ch_211'>项羽</pre><pre class='ch_211'>我发布了短视频</pre><div class='ch_164'><video loading='lazy' controls><source src='https://lcctoor.github.io/arts/arts/videos/200-秦时明月[项羽]·谪居/README.mp4' type='video/mp4'></video></div></div></div><div class='ch_173'><img class='ch_172' src='ip_static/头像/项羽.jpg'><div class='ch_164'><pre class='ch_211'>项羽</pre><pre class='ch_211'>明天的鸿门宴不知道刘邦会不会来……</pre></div></div><div class='ch_173'><img class='ch_172' src='ip_static/头像/楚门.jpg'><div class='ch_164'><pre class='ch_211'>楚门</pre><pre class='ch_211'>我发布了短视频</pre><div class='ch_164'><video loading='lazy' controls><source src='https://lcctoor.github.io/arts/arts/videos/600-楚门的世界·五月雨/README.mp4' type='video/mp4'></video></div></div></div><div class='ch_173'><img class='ch_172' src='ip_static/头像/爱因斯坦.jpg'><div class='ch_164'><pre class='ch_211'>爱因斯坦</pre><pre class='ch_211'>在这个充满未知的宇宙中，“上帝不会掷骰子”是我对那些随机性信徒的幽默回应。玻尔可能认为宇宙像个巨大的赌场，但我可不买账。宇宙中的每个角落都遵循着严格而精妙的规则，将宇宙的深奥之处简化为一场赌博，这不是天真就是单纯。</pre></div></div><div class='ch_173'><img class='ch_172' src='ip_static/头像/玻尔.jpg'><div class='ch_164'><pre class='ch_211'>玻尔</pre><pre class='ch_211'>在这个由无数概率编织而成的奇妙宇宙中，“上帝是个赌徒”是我对那些过分执着于确定性的朋友们的幽默抚慰。爱因斯坦先生似乎更喜欢他的宇宙像个精确无误的瑞士钟表，但我要说，亲爱的阿尔伯特，如果宇宙真的像你想象的那样毫无意外，那该有多无趣啊！所以，下次当你感叹“上帝不会掷骰子”时，也许上帝和我正在一起笑着掷下一枚骰子，而你所坚信的那个巨大的钟表，却在不知不觉中成了我们游戏的一部分。</pre></div></div></div></div></div><div class='ch_164' style="display:none;"><div class='ch_164' id='ch_21'><div class='ch_173'><img class='ch_172' src='ip_static/头像/{speaker}.jpg'><pre class='ch_211'>{content}</pre><span class='ch_210'></span></div></div><div class='ch_164' id='ch_23'><div class='ch_173'><span class='ch_210'></span><pre class='ch_211'>{content}</pre><img class='ch_172' src='ip_static/头像/{speaker}.jpg'></div></div></div>
+</pre></div><div class='ch_274 ch_275 ch_276' id='ch_141'><div class='ch_165'>钱包<div class='ch_165' id='ch_283'>∟</div></div><div class='ch_175' style="background-color:rgb(38, 170, 82); justify-content:space-around; grid-template-columns:auto auto; border-radius:1rem; height:9rem; margin:0.5rem; align-content:center; align-items:center;"><div class='ch_175' style="grid-template-rows:1fr 1fr; color:white; height:5rem; width:7rem; justify-content:center; justify-items:center; text-align:center; align-content:center; align-items:center; border-radius:1rem;"><span class='ch_231' style="align-self:end;">余额</span><span class='ch_231' style="align-self:start;">¥499.00</span></div><button class='ch_285 ch_286 ch_287' id='ch_288'>提现</button></div></div><div class='ch_274 ch_275 ch_276' id='ch_143' style="grid-template-rows:auto 1fr;"><div class='ch_165'>捐赠<div class='ch_165' id='ch_290'>∟</div></div><div class='ch_175' style="grid-template-rows:auto auto; justify-content:center; align-content:space-evenly; justify-items:center; padding:1rem; text-align:center;"><img class='ch_174' src='https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg' style="height:15rem;"><div class='ch_165' style="font-size:1.5rem;">感谢你进入到这里，这说明你对这个软件还是有一些兴趣的！如果你喜欢这个作品，就请支持一下吧！(^_^)</div></div></div><div class='ch_274 ch_275 ch_276' id='ch_147'><div class='ch_165'>朋友圈<div class='ch_165' id='ch_292'>∟</div></div><div class='ch_294 ch_295 ch_296 ch_297 ch_298 ch_299 ch_166 ch_300 ch_301 ch_302' id='ch_145'><img class='ch_174' src='ip_static/封面.jpg'><div class='ch_175'><img class='ch_174' src='ip_static/头像/林宥嘉.jpg'><div class='ch_165'><pre class='ch_230'>林宥嘉</pre><pre class='ch_230'>我发布了音乐</pre><div class='ch_165'><audio loading='lazy' controls><source src="ip_static/天将明 -林宥嘉.flac" type="audio/flac">天将明 -林宥嘉.flac</audio></div></div></div><div class='ch_175'><img class='ch_174' src='ip_static/头像/李连杰.jpg'><div class='ch_165'><pre class='ch_230'>李连杰</pre><pre class='ch_230'>我发布了短视频</pre><div class='ch_165'><video loading='lazy' controls><source src='https://lcctoor.github.io/arts/arts/videos/400-李连杰[霍元甲]·兰亭序/README.mp4' type='video/mp4'></video></div></div></div><div class='ch_175'><img class='ch_174' src='ip_static/头像/项羽.jpg'><div class='ch_165'><pre class='ch_230'>项羽</pre><pre class='ch_230'>我发布了短视频</pre><div class='ch_165'><video loading='lazy' controls><source src='https://lcctoor.github.io/arts/arts/videos/200-秦时明月[项羽]·谪居/README.mp4' type='video/mp4'></video></div></div></div><div class='ch_175'><img class='ch_174' src='ip_static/头像/项羽.jpg'><div class='ch_165'><pre class='ch_230'>项羽</pre><pre class='ch_230'>明天的鸿门宴不知道刘邦会不会来……</pre></div></div><div class='ch_175'><img class='ch_174' src='ip_static/头像/楚门.jpg'><div class='ch_165'><pre class='ch_230'>楚门</pre><pre class='ch_230'>我发布了短视频</pre><div class='ch_165'><video loading='lazy' controls><source src='https://lcctoor.github.io/arts/arts/videos/600-楚门的世界·五月雨/README.mp4' type='video/mp4'></video></div></div></div><div class='ch_175'><img class='ch_174' src='ip_static/头像/爱因斯坦.jpg'><div class='ch_165'><pre class='ch_230'>爱因斯坦</pre><pre class='ch_230'>在这个充满未知的宇宙中，“上帝不会掷骰子”是我对那些随机性信徒的幽默回应。玻尔可能认为宇宙像个巨大的赌场，但我可不买账。宇宙中的每个角落都遵循着严格而精妙的规则，将宇宙的深奥之处简化为一场赌博，这不是天真就是单纯。</pre></div></div><div class='ch_175'><img class='ch_174' src='ip_static/头像/玻尔.jpg'><div class='ch_165'><pre class='ch_230'>玻尔</pre><pre class='ch_230'>在这个由无数概率编织而成的奇妙宇宙中，“上帝是个赌徒”是我对那些过分执着于确定性的朋友们的幽默抚慰。爱因斯坦先生似乎更喜欢他的宇宙像个精确无误的瑞士钟表，但我要说，亲爱的阿尔伯特，如果宇宙真的像你想象的那样毫无意外，那该有多无趣啊！所以，下次当你感叹“上帝不会掷骰子”时，也许上帝和我正在一起笑着掷下一枚骰子，而你所坚信的那个巨大的钟表，却在不知不觉中成了我们游戏的一部分。</pre></div></div></div></div></div><div class='ch_165' style="display:none;"><div class='ch_165' id='ch_20'><div class='ch_175'><img class='ch_174' src='ip_static/头像/{speaker}.jpg'><pre class='ch_230'>{content}</pre><span class='ch_231'></span></div></div><div class='ch_165' id='ch_22'><div class='ch_175'><span class='ch_231'></span><pre class='ch_230'>{content}</pre><img class='ch_174' src='ip_static/头像/{speaker}.jpg'></div></div></div>
 <script>
 ch.ch_1 = () => window.innerWidth > window.innerHeight
 ch.ch_2 = (ele, name, value) => {
             ele.setAttribute(name, value)
             ele[name] = value
         }
 ch.ch_3 = document.body
-ch.ch_20 = () => {
+ch.ch_19 = () => {
             let value = ch.ch_1()
             if (value)
                 { ch.ch_2(ch.ch_3, 'is_x_screen', 'True') }
             else
                 { ch.ch_2(ch.ch_3, 'is_x_screen', 'False') }
             return value
         }
-ch.ch_20()
-ch.ch_22 = document.getElementById("ch_21")
-ch.ch_24 = document.getElementById("ch_23")
-ch.ch_29 = document.getElementById("ch_28")
-ch.ch_31 = document.getElementById("ch_30")
+ch.ch_19()
+ch.ch_21 = document.getElementById("ch_20")
+ch.ch_23 = document.getElementById("ch_22")
+ch.ch_28 = document.getElementById("ch_27")
+ch.ch_30 = document.getElementById("ch_29")
 ch.ch_37 = document.getElementById("ch_36")
 ch.ch_39 = document.getElementById("ch_38")
 ch.ch_43 = document.getElementById("ch_42")
 ch.ch_45 = document.getElementById("ch_44")
 ch.ch_49 = document.getElementById("ch_48")
 ch.ch_51 = document.getElementById("ch_50")
 ch.ch_55 = document.getElementById("ch_54")
@@ -139,96 +141,109 @@
 ch.ch_93 = document.getElementById("ch_92")
 ch.ch_97 = document.getElementById("ch_96")
 ch.ch_99 = document.getElementById("ch_98")
 ch.ch_103 = document.getElementById("ch_102")
 ch.ch_105 = document.getElementById("ch_104")
 ch.ch_109 = document.getElementById("ch_108")
 ch.ch_111 = document.getElementById("ch_110")
-ch.ch_25 = new Map([[ch.ch_29, ch.ch_31], [ch.ch_31, ch.ch_29], [ch.ch_37, ch.ch_39], [ch.ch_39, ch.ch_37], [ch.ch_43, ch.ch_45], [ch.ch_45, ch.ch_43], [ch.ch_49, ch.ch_51], [ch.ch_51, ch.ch_49], [ch.ch_55, ch.ch_57], [ch.ch_57, ch.ch_55], [ch.ch_61, ch.ch_63], [ch.ch_63, ch.ch_61], [ch.ch_67, ch.ch_69], [ch.ch_69, ch.ch_67], [ch.ch_73, ch.ch_75], [ch.ch_75, ch.ch_73], [ch.ch_79, ch.ch_81], [ch.ch_81, ch.ch_79], [ch.ch_85, ch.ch_87], [ch.ch_87, ch.ch_85], [ch.ch_91, ch.ch_93], [ch.ch_93, ch.ch_91], [ch.ch_97, ch.ch_99], [ch.ch_99, ch.ch_97], [ch.ch_103, ch.ch_105], [ch.ch_105, ch.ch_103], [ch.ch_109, ch.ch_111], [ch.ch_111, ch.ch_109]])
-ch.ch_8 = document.getElementById("ch_7")
+ch.ch_24 = new Map([[ch.ch_28, ch.ch_30], [ch.ch_30, ch.ch_28], [ch.ch_37, ch.ch_39], [ch.ch_39, ch.ch_37], [ch.ch_43, ch.ch_45], [ch.ch_45, ch.ch_43], [ch.ch_49, ch.ch_51], [ch.ch_51, ch.ch_49], [ch.ch_55, ch.ch_57], [ch.ch_57, ch.ch_55], [ch.ch_61, ch.ch_63], [ch.ch_63, ch.ch_61], [ch.ch_67, ch.ch_69], [ch.ch_69, ch.ch_67], [ch.ch_73, ch.ch_75], [ch.ch_75, ch.ch_73], [ch.ch_79, ch.ch_81], [ch.ch_81, ch.ch_79], [ch.ch_85, ch.ch_87], [ch.ch_87, ch.ch_85], [ch.ch_91, ch.ch_93], [ch.ch_93, ch.ch_91], [ch.ch_97, ch.ch_99], [ch.ch_99, ch.ch_97], [ch.ch_103, ch.ch_105], [ch.ch_105, ch.ch_103], [ch.ch_109, ch.ch_111], [ch.ch_111, ch.ch_109]])
+ch.ch_7 = document.getElementById("ch_6")
 ch.ch_133 = (chat_page, site, speaker, msg_text, clear_input=false) => {
             chat_page.children[2].children[0].focus()
             if (site === 'left') {
-                let row = ch.ch_22.firstElementChild.outerHTML.replace('{speaker}', speaker).replace('{content}', msg_text)
+                let row = ch.ch_21.firstElementChild.outerHTML.replace('{speaker}', speaker).replace('{content}', msg_text)
                 row = new DOMParser().parseFromString(row, 'text/html').body.firstChild
                 chat_page.children[1].appendChild(row)
             }
             else {
-                let row = ch.ch_24.firstElementChild.outerHTML.replace('{speaker}', speaker).replace('{content}', msg_text)
+                let row = ch.ch_23.firstElementChild.outerHTML.replace('{speaker}', speaker).replace('{content}', msg_text)
                 row = new DOMParser().parseFromString(row, 'text/html').body.firstChild
                 chat_page.children[1].appendChild(row)
             }
             chat_page.children[1].scrollTop += 99999
             if (clear_input)
                 chat_page.children[2].children[0].value = ''
-            let nav = ch.ch_25.get(chat_page)
+            let nav = ch.ch_24.get(chat_page)
             nav.children[1].children[1].innerHTML = msg_text
-            ch.ch_8.insertBefore(nav, ch.ch_8.firstChild)
+            ch.ch_7.insertBefore(nav, ch.ch_7.firstChild)
         }
-ch.ch_133(ch.ch_31, 'right', '我', 'new Date()')
-        ch.ch_133(ch.ch_31, 'left', 'JS小黄老师', new Date())
-ch.ch_135 = document.getElementById("ch_134")
-ch.ch_135.value =  "Hello, Tom Cat!"
-ch.ch_137 = document.getElementById("ch_136")
-ch.ch_137.value =  "什么是滑坡论证？"
-ch.ch_15 = document.getElementById("ch_14")
+ch.ch_134 = (key) => {
+            let chat_page = ch.ch_30
+            ch.ch_133(chat_page, 'right', '我', key, true)
+            let value = ''
+            try {value = String(eval(key))} catch (e) {value = e.toString()}
+            ch.ch_133(chat_page, 'left', 'JS小黄老师', value)
+        }
+ch.ch_134("'你好呀！'")
+        ch.ch_134('1 + 1')
+        ch.ch_134('new Date()')
+        ch.ch_134("user = '小明'")
+        ch.ch_134("action = '喝水'")
+        ch.ch_134("user + action")
+ch.ch_136 = document.getElementById("ch_135")
+ch.ch_136.value =  "Hello, Tom Cat!"
+ch.ch_138 = document.getElementById("ch_137")
+ch.ch_138.value =  "什么是滑坡论证？"
+ch.ch_14 = document.getElementById("ch_13")
 ch.ch_116 = new Map([["current_index", null]])
 ch.ch_112 = (last_value, items) =>
             value => {
                 if (last_value.get('last_value') !== value) {
                     last_value.set('last_value', value)
                     for (let set_value of items)
                         {set_value(value)}
                 }
             }
 ch.ch_113 = new Map([["last_value", null]])
-ch.ch_4 = (ele, scrollLeft, seconds=0, callback=null) => {
+ch.ch_4 = async (ele, scrollLeft, seconds=0) => {
             if (seconds) {
                 let start_time = performance.now()  // 立即获取当前时间，以尽可能让时间准确
+                ele.classList.add('ch_exec_smooth_to_scrollLeft')  // 立即设为 ch_exec_smooth_to_scrollLeft
                 let milliseconds = seconds * 1000
                 let end_time = start_time + milliseconds
                 let start_scrollLeft = ele.scrollLeft
                 let distance = scrollLeft - start_scrollLeft
                 let gradient = distance / milliseconds  // 斜率
-                ele.classList.add('ch_exec_smooth_to_scrollLeft')
+                let state = {'finished': false}
                 let scroll = () => {
                     let current_time = performance.now()
-                    if (current_time < end_time) {
+                    if (current_time < end_time)
                         ele.scrollLeft = gradient * (current_time - start_time) + start_scrollLeft  // y = k*x + b
-                        requestAnimationFrame(scroll)  // requestAnimationFrame 和 setTimeout 都可用于延迟运行，但前者是专为动画设计的
-                    }
-                    else {
-                        ele.classList.remove('ch_exec_smooth_to_scrollLeft')
-                        ele.scrollLeft = scrollLeft  // 两个功能：确保最终位置正确、激活同步
-                        if (callback) callback()
-                    }
+                    else
+                        state['finished'] = true
                 }
-                scroll()
+                while (true) {
+                    await new Promise(resolve => requestAnimationFrame(() => {scroll(); resolve()}))  // 在这一步会释放事件循环的loop
+                    // requestAnimationFrame 和 setTimeout 都可用于延迟运行。但前者是专为动画设计的，会在浏览器下一次重绘前被执行
+                    if (state['finished']) break
+                }
+                ele.classList.remove('ch_exec_smooth_to_scrollLeft')
+                ele.scrollLeft = scrollLeft  // 两个功能：确保最终位置正确、激活同步
             }
             else
                 ele.scrollLeft = scrollLeft
         }
 ch.ch_115 = (pages_box, current_index, scroll_seconds) =>
-            value => {
+            async value => {
                 let index = Number(value)
                 if (Number.isInteger(index))  {  // 3.0、4.0 这种格式也会表现为 True
                     index = parseInt(index)  // 转化为 3、4 这种真正的整数
                     if ( index !== current_index.get('current_index') ) {
                         let page = pages_box.children[index - 1]
                         if (page) {
                             current_index.set('current_index', index)
                             if (scroll_seconds)
-                                ch.ch_4(pages_box, page.offsetLeft, scroll_seconds)
+                                await ch.ch_4(pages_box, page.offsetLeft, scroll_seconds)
                             else
                                 pages_box.scrollLeft = page.offsetLeft
                         }
                     }
                 }
             }
-ch.ch_119 = ch.ch_115(ch.ch_15, ch.ch_116, 0.2)
+ch.ch_119 = ch.ch_115(ch.ch_14, ch.ch_116, 0.2)
 ch.ch_114 = [ch.ch_119]
 ch.ch_117 = ch.ch_112(ch.ch_113, ch.ch_114)
 ch.ch_130 = document.getElementById("ch_129")
 ch.ch_131 = new Map([["current_index", null]])
 ch.ch_120 = new Map([["last_value", null]])
 ch.ch_124 = (navigation, navs, value) => {
             let index = Number(value)
@@ -264,302 +279,324 @@
                             current_index.set('current_index', index)
                             sync_value( String(index) )
                         }
                     }
                 }
             )
         }
-ch.ch_118(ch.ch_15, ch.ch_116, ch.ch_117)
+ch.ch_118(ch.ch_14, ch.ch_116, ch.ch_117)
 ch.ch_127 = (navigation, navs, sync_value) => {
             navigation.addEventListener('click',
                 () => {
                     let nav = event.target
                     if (nav.classList.contains('is_nav'))
                         {sync_value(String( navs.indexOf(nav)+1 ))}
                 }
             )
         }
 ch.ch_127(ch.ch_123, ch.ch_125, ch.ch_126)
 ch.ch_118(ch.ch_130, ch.ch_131, ch.ch_126)
-ch.ch_17 = document.getElementById("ch_16")
-ch.ch_18 = new Map([["is_scrolling", false]])
-ch.ch_19 = (pages_box, door, scroll_records) => {
+ch.ch_16 = document.getElementById("ch_15")
+ch.ch_17 = new Map([["is_scrolling", false]])
+ch.ch_18 = (pages_box, door, scroll_records) => {
                 let current_index = 0
                 let round_index = 0
+                let restore_scroll_records = () => scroll_records.set('is_scrolling', false)
+                let restore_scroll_records_task = null
                 let move_door = () => {
+                    // move_door
                     let current_page = pages_box.children[round_index]
                     pages_box.insertBefore(door, current_page.nextElementSibling)
+                    // restore_scroll_records
+                    restore_scroll_records()  // 最好放在 move_door 后面, 以保持流程有序
                 }
                 let move_door_task = null
-                let restore_scroll_records = () => scroll_records.set('is_scrolling', false)
-                let restore_scroll_records_task = null
                 pages_box.addEventListener('scroll',
                     () => {
                         clearTimeout(restore_scroll_records_task)  // clearTimeout(null) 不会报错
                         clearTimeout(move_door_task)
                         scroll_records.set('is_scrolling', true)  // 防跳屏措施
                         let index = pages_box.scrollLeft / pages_box.clientWidth
                         let trunc_index = Math.trunc(index)
                         round_index = Math.round(index)
                         if (round_index !== current_index) current_index = round_index
-                        if (index - trunc_index < 0.02) {  // 右滑到右边缘处, 把屏幕分成50份
-                            move_door_task = setTimeout(move_door, 50)  // 0.05秒, 对应屏幕刷新率为20HZ
+                        if (index - trunc_index < 0.02) {  // 右滑到右边缘处, 把屏幕分成50份。越小越允许用户手指停留
+                            move_door_task = setTimeout(move_door, 50)  // 0.05秒, 对应屏幕刷新率为20HZ。越小越早走完流程, 但不能小于 async_smooth_to_scrollLeft 的刷新频率
+                        }
+                        else {
+                            restore_scroll_records_task = setTimeout(restore_scroll_records, 50)
                         }
-                        restore_scroll_records_task = setTimeout(restore_scroll_records, 100)  // 最好比 move_door_task 的延时高, 以让 move_door_task 先执行完成, 以保持流程有序
                     }
                 )
             }
-ch.ch_19(ch.ch_15, ch.ch_17, ch.ch_18)
-ch.ch_11 = document.getElementById("ch_10")
-ch.ch_13 = document.getElementById("ch_12")
-ch.ch_27 = document.getElementById("ch_26")
+ch.ch_18(ch.ch_14, ch.ch_16, ch.ch_17)
+ch.ch_10 = document.getElementById("ch_9")
+ch.ch_12 = document.getElementById("ch_11")
+ch.ch_26 = document.getElementById("ch_25")
 ch.ch_35 = document.getElementById("ch_34")
 ch.ch_41 = document.getElementById("ch_40")
 ch.ch_47 = document.getElementById("ch_46")
 ch.ch_53 = document.getElementById("ch_52")
 ch.ch_59 = document.getElementById("ch_58")
 ch.ch_65 = document.getElementById("ch_64")
 ch.ch_71 = document.getElementById("ch_70")
 ch.ch_77 = document.getElementById("ch_76")
 ch.ch_83 = document.getElementById("ch_82")
 ch.ch_89 = document.getElementById("ch_88")
 ch.ch_95 = document.getElementById("ch_94")
 ch.ch_101 = document.getElementById("ch_100")
 ch.ch_107 = document.getElementById("ch_106")
-ch.ch_145 = document.getElementById("ch_144")
-ch.ch_9 = (ele, px) => {
+ch.ch_146 = document.getElementById("ch_145")
+ch.ch_8 = (ele, px) => {
                     ele.scrollTop += px
                     event.preventDefault()  // 阻止其它默认行为
                 }
-ch.ch_8.addEventListener('wheel', () => {ch.ch_9(ch.ch_8, event.deltaY)})
-ch.ch_139 = document.getElementById("ch_138")
-ch.ch_141 = document.getElementById("ch_140")
-ch.ch_143 = document.getElementById("ch_142")
-ch.ch_147 = document.getElementById("ch_146")
-ch.ch_32 = (pages_box, page, scroll_seconds, scroll_records) => {
+ch.ch_7.addEventListener('wheel', () => {ch.ch_8(ch.ch_7, event.deltaY)})
+ch.ch_140 = document.getElementById("ch_139")
+ch.ch_142 = document.getElementById("ch_141")
+ch.ch_144 = document.getElementById("ch_143")
+ch.ch_148 = document.getElementById("ch_147")
+ch.ch_31 = async (pages_box, page, scroll_records) => {
                 if (! scroll_records.get('is_scrolling')) {
-                    let current_page = pages_box.children[Math.round(pages_box.scrollLeft / pages_box.clientWidth)]
+                    let index = Math.round(pages_box.scrollLeft / pages_box.clientWidth)
+                    await ch.ch_4(pages_box, pages_box.clientWidth * index, 0)  // 防跳屏措施。如果 pages_box 没有滚动到位就执行insertBefore, 会直接从第一屏跳到第三屏
+                    let current_page = pages_box.children[index]
                     pages_box.insertBefore(page, current_page.nextElementSibling)
-                    ch.ch_4(pages_box, pages_box.scrollLeft + pages_box.clientWidth * 1, scroll_seconds)
                 }
             }
-ch.ch_29.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_31, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_27, 99999)})
-ch.ch_37.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_39, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_35, 99999)})
-ch.ch_43.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_45, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_41, 99999)})
-ch.ch_49.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_51, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_47, 99999)})
-ch.ch_55.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_57, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_53, 99999)})
-ch.ch_61.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_63, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_59, 99999)})
-ch.ch_67.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_69, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_65, 99999)})
-ch.ch_73.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_75, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_71, 99999)})
-ch.ch_79.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_81, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_77, 99999)})
-ch.ch_85.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_87, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_83, 99999)})
-ch.ch_91.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_93, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_89, 99999)})
-ch.ch_97.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_99, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_95, 99999)})
-ch.ch_103.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_105, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_101, 99999)})
-ch.ch_109.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_111, 0.2, ch.ch_18)
-ch.ch_9(ch.ch_107, 99999)})
-ch.ch_11.addEventListener('wheel', () => {ch.ch_9(ch.ch_11, event.deltaY)})
-ch.ch_175 = document.getElementById("ch_174")
-ch.ch_175.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_147, 0.2, ch.ch_18)})
-ch.ch_13.addEventListener('wheel', () => {ch.ch_9(ch.ch_13, event.deltaY)})
-ch.ch_189 = document.getElementById("ch_188")
-ch.ch_189.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_141, 0.2, ch.ch_18)})
-ch.ch_191 = document.getElementById("ch_190")
-ch.ch_191.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_139, 0.2, ch.ch_18)})
-ch.ch_148 = () => {
-            for (let video of ch.ch_147.querySelectorAll('video')) {
+ch.ch_32 = async (pages_box, relative_index, scroll_seconds, callback) =>
+                    await ch.ch_4(pages_box, pages_box.scrollLeft + pages_box.clientWidth * relative_index, scroll_seconds, callback)
+ch.ch_28.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_30, ch.ch_17)
+ch.ch_8(ch.ch_26, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_37.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_39, ch.ch_17)
+ch.ch_8(ch.ch_35, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_43.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_45, ch.ch_17)
+ch.ch_8(ch.ch_41, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_49.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_51, ch.ch_17)
+ch.ch_8(ch.ch_47, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_55.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_57, ch.ch_17)
+ch.ch_8(ch.ch_53, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_61.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_63, ch.ch_17)
+ch.ch_8(ch.ch_59, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_67.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_69, ch.ch_17)
+ch.ch_8(ch.ch_65, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_73.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_75, ch.ch_17)
+ch.ch_8(ch.ch_71, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_79.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_81, ch.ch_17)
+ch.ch_8(ch.ch_77, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_85.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_87, ch.ch_17)
+ch.ch_8(ch.ch_83, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_91.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_93, ch.ch_17)
+ch.ch_8(ch.ch_89, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_97.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_99, ch.ch_17)
+ch.ch_8(ch.ch_95, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_103.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_105, ch.ch_17)
+ch.ch_8(ch.ch_101, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_109.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_111, ch.ch_17)
+ch.ch_8(ch.ch_107, 99999)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_10.addEventListener('wheel', () => {ch.ch_8(ch.ch_10, event.deltaY)})
+ch.ch_177 = document.getElementById("ch_176")
+ch.ch_177.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_148, ch.ch_17)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_12.addEventListener('wheel', () => {ch.ch_8(ch.ch_12, event.deltaY)})
+ch.ch_192 = document.getElementById("ch_191")
+ch.ch_192.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_142, ch.ch_17)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_194 = document.getElementById("ch_193")
+ch.ch_194.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_140, ch.ch_17)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_149 = () => {
+            for (let video of ch.ch_148.querySelectorAll('video')) {
                 video.pause()
             }
         }
-ch.ch_33 = (pages_box, door, scroll_seconds, callback) => {
-                ch.ch_4(pages_box, pages_box.scrollLeft + pages_box.clientWidth * -1, scroll_seconds, callback)
+ch.ch_33 = async (pages_box, door, scroll_seconds, callback) => {
+                await ch.ch_4(pages_box, pages_box.scrollLeft + pages_box.clientWidth * -1, scroll_seconds, callback)
             }
-ch.ch_203 = document.getElementById("ch_202")
-ch.ch_203.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_27.addEventListener('wheel', () => {ch.ch_9(ch.ch_27, event.deltaY)})
-ch.ch_218 = document.getElementById("ch_217")
-ch.ch_218.addEventListener('click', () => {{
-                let chat_page = ch.ch_31
-                let key = chat_page.children[2].children[0].value
-                ch.ch_133(chat_page, 'right', '我', key, true)
-                let value = ''
-                try {value = String(eval(key))} catch (e) {value = e.toString()}
-                ch.ch_133(chat_page, 'left', 'JS小黄老师', value)
-            }})
-ch.ch_220 = document.getElementById("ch_219")
-ch.ch_220.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_35.addEventListener('wheel', () => {ch.ch_9(ch.ch_35, event.deltaY)})
-ch.ch_222 = document.getElementById("ch_221")
-ch.ch_222.addEventListener('click', () => {{
+ch.ch_206 = document.getElementById("ch_205")
+ch.ch_206.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_26.addEventListener('wheel', () => {ch.ch_8(ch.ch_26, event.deltaY)})
+ch.ch_219 = document.getElementById("ch_218")
+ch.ch_219.addEventListener('click', () => {{
+                let chat_page = ch.ch_30
+                ch.ch_134(chat_page.children[2].children[0].value)
+            }})
+ch.ch_221 = document.getElementById("ch_220")
+ch.ch_221.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_35.addEventListener('wheel', () => {ch.ch_8(ch.ch_35, event.deltaY)})
+ch.ch_223 = document.getElementById("ch_222")
+ch.ch_223.addEventListener('click', () => {{
                 let chat_page = ch.ch_39
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
                 
                 let say = () => {window.speechSynthesis.speak(new SpeechSynthesisUtterance(key))}
-                let row = ch.ch_22.firstElementChild.outerHTML.replace('{speaker}', '会说话的汤姆猫').replace('{content}', '🔊' + key.length + ' ')
+                let row = ch.ch_21.firstElementChild.outerHTML.replace('{speaker}', '会说话的汤姆猫').replace('{content}', '🔊' + key.length + ' ')
                 row = new DOMParser().parseFromString(row, 'text/html').body.firstChild
                 row.children[1].addEventListener('click', say)
                 chat_page.children[1].appendChild(row)
                 say()
 
                 chat_page.children[1].scrollTop += 99999
-                let nav = ch.ch_25.get(chat_page)
+                let nav = ch.ch_24.get(chat_page)
                 nav.children[1].children[1].innerHTML = key
-                ch.ch_8.insertBefore(nav, ch.ch_8.firstChild)
+                ch.ch_7.insertBefore(nav, ch.ch_7.firstChild)
             }})
-ch.ch_224 = document.getElementById("ch_223")
-ch.ch_224.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_41.addEventListener('wheel', () => {ch.ch_9(ch.ch_41, event.deltaY)})
-ch.ch_226 = document.getElementById("ch_225")
-ch.ch_226.addEventListener('click', () => {{
+ch.ch_225 = document.getElementById("ch_224")
+ch.ch_225.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_41.addEventListener('wheel', () => {ch.ch_8(ch.ch_41, event.deltaY)})
+ch.ch_227 = document.getElementById("ch_226")
+ch.ch_227.addEventListener('click', () => {{
                 let chat_page = ch.ch_45
                 let key = chat_page.children[2].children[0].value
                 let value = '一见短袖子，立刻想到白臂膊，立刻想到全裸体，立刻想到生殖器，立刻想到性交，立刻想到杂交，立刻想到私生子。'
                 ch.ch_133(chat_page, 'right', '我', key, true)
-                let nav = ch.ch_25.get(chat_page)
+                let nav = ch.ch_24.get(chat_page)
                 if (key.includes('什么是滑坡论证')) {
-                    let row = ch.ch_22.firstElementChild.outerHTML.replace('{speaker}', '鲁迅').replace('{content}', '')
+                    let row = ch.ch_21.firstElementChild.outerHTML.replace('{speaker}', '鲁迅').replace('{content}', '')
                     row = new DOMParser().parseFromString(row, 'text/html').body.firstChild
                     let pre = row.children[1]
                     chat_page.children[1].appendChild(row)
                     async function input_() {
                         await new Promise(resolve => setTimeout(resolve, 1000))
                         for (let t of value) {
                             pre.innerHTML += t
-                            chat_page.children[1].scrollTop += 999
+                            chat_page.children[1].scrollTop += 99999
                             await new Promise(resolve => setTimeout(resolve, 200))
                         }
                         nav.children[1].children[1].innerHTML = value
                     }
                     input_()
                 }
                 else
                     nav.children[1].children[1].innerHTML = key
-                ch.ch_8.insertBefore(nav, ch.ch_8.firstChild)
+                ch.ch_7.insertBefore(nav, ch.ch_7.firstChild)
             }})
-ch.ch_228 = document.getElementById("ch_227")
-ch.ch_228.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_47.addEventListener('wheel', () => {ch.ch_9(ch.ch_47, event.deltaY)})
-ch.ch_230 = document.getElementById("ch_229")
-ch.ch_230.addEventListener('click', () => {{
+ch.ch_229 = document.getElementById("ch_228")
+ch.ch_229.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_47.addEventListener('wheel', () => {ch.ch_8(ch.ch_47, event.deltaY)})
+ch.ch_233 = document.getElementById("ch_232")
+ch.ch_233.addEventListener('click', () => {{
                 let chat_page = ch.ch_51
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_232 = document.getElementById("ch_231")
-ch.ch_232.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_53.addEventListener('wheel', () => {ch.ch_9(ch.ch_53, event.deltaY)})
-ch.ch_234 = document.getElementById("ch_233")
-ch.ch_234.addEventListener('click', () => {{
+ch.ch_235 = document.getElementById("ch_234")
+ch.ch_235.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_53.addEventListener('wheel', () => {ch.ch_8(ch.ch_53, event.deltaY)})
+ch.ch_237 = document.getElementById("ch_236")
+ch.ch_237.addEventListener('click', () => {{
                 let chat_page = ch.ch_57
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_236 = document.getElementById("ch_235")
-ch.ch_236.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_59.addEventListener('wheel', () => {ch.ch_9(ch.ch_59, event.deltaY)})
-ch.ch_238 = document.getElementById("ch_237")
-ch.ch_238.addEventListener('click', () => {{
+ch.ch_239 = document.getElementById("ch_238")
+ch.ch_239.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_59.addEventListener('wheel', () => {ch.ch_8(ch.ch_59, event.deltaY)})
+ch.ch_241 = document.getElementById("ch_240")
+ch.ch_241.addEventListener('click', () => {{
                 let chat_page = ch.ch_63
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_240 = document.getElementById("ch_239")
-ch.ch_240.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_65.addEventListener('wheel', () => {ch.ch_9(ch.ch_65, event.deltaY)})
-ch.ch_242 = document.getElementById("ch_241")
-ch.ch_242.addEventListener('click', () => {{
+ch.ch_243 = document.getElementById("ch_242")
+ch.ch_243.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_65.addEventListener('wheel', () => {ch.ch_8(ch.ch_65, event.deltaY)})
+ch.ch_245 = document.getElementById("ch_244")
+ch.ch_245.addEventListener('click', () => {{
                 let chat_page = ch.ch_69
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_244 = document.getElementById("ch_243")
-ch.ch_244.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_71.addEventListener('wheel', () => {ch.ch_9(ch.ch_71, event.deltaY)})
-ch.ch_246 = document.getElementById("ch_245")
-ch.ch_246.addEventListener('click', () => {{
+ch.ch_247 = document.getElementById("ch_246")
+ch.ch_247.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_71.addEventListener('wheel', () => {ch.ch_8(ch.ch_71, event.deltaY)})
+ch.ch_249 = document.getElementById("ch_248")
+ch.ch_249.addEventListener('click', () => {{
                 let chat_page = ch.ch_75
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_248 = document.getElementById("ch_247")
-ch.ch_248.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_77.addEventListener('wheel', () => {ch.ch_9(ch.ch_77, event.deltaY)})
-ch.ch_250 = document.getElementById("ch_249")
-ch.ch_250.addEventListener('click', () => {{
+ch.ch_251 = document.getElementById("ch_250")
+ch.ch_251.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_77.addEventListener('wheel', () => {ch.ch_8(ch.ch_77, event.deltaY)})
+ch.ch_253 = document.getElementById("ch_252")
+ch.ch_253.addEventListener('click', () => {{
                 let chat_page = ch.ch_81
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_252 = document.getElementById("ch_251")
-ch.ch_252.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_83.addEventListener('wheel', () => {ch.ch_9(ch.ch_83, event.deltaY)})
-ch.ch_254 = document.getElementById("ch_253")
-ch.ch_254.addEventListener('click', () => {{
+ch.ch_255 = document.getElementById("ch_254")
+ch.ch_255.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_83.addEventListener('wheel', () => {ch.ch_8(ch.ch_83, event.deltaY)})
+ch.ch_257 = document.getElementById("ch_256")
+ch.ch_257.addEventListener('click', () => {{
                 let chat_page = ch.ch_87
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_256 = document.getElementById("ch_255")
-ch.ch_256.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_89.addEventListener('wheel', () => {ch.ch_9(ch.ch_89, event.deltaY)})
-ch.ch_258 = document.getElementById("ch_257")
-ch.ch_258.addEventListener('click', () => {{
+ch.ch_259 = document.getElementById("ch_258")
+ch.ch_259.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_89.addEventListener('wheel', () => {ch.ch_8(ch.ch_89, event.deltaY)})
+ch.ch_261 = document.getElementById("ch_260")
+ch.ch_261.addEventListener('click', () => {{
                 let chat_page = ch.ch_93
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_260 = document.getElementById("ch_259")
-ch.ch_260.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_95.addEventListener('wheel', () => {ch.ch_9(ch.ch_95, event.deltaY)})
-ch.ch_262 = document.getElementById("ch_261")
-ch.ch_262.addEventListener('click', () => {{
+ch.ch_263 = document.getElementById("ch_262")
+ch.ch_263.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_95.addEventListener('wheel', () => {ch.ch_8(ch.ch_95, event.deltaY)})
+ch.ch_265 = document.getElementById("ch_264")
+ch.ch_265.addEventListener('click', () => {{
                 let chat_page = ch.ch_99
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_264 = document.getElementById("ch_263")
-ch.ch_264.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_101.addEventListener('wheel', () => {ch.ch_9(ch.ch_101, event.deltaY)})
-ch.ch_266 = document.getElementById("ch_265")
-ch.ch_266.addEventListener('click', () => {{
+ch.ch_267 = document.getElementById("ch_266")
+ch.ch_267.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_101.addEventListener('wheel', () => {ch.ch_8(ch.ch_101, event.deltaY)})
+ch.ch_269 = document.getElementById("ch_268")
+ch.ch_269.addEventListener('click', () => {{
                 let chat_page = ch.ch_105
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_268 = document.getElementById("ch_267")
-ch.ch_268.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_107.addEventListener('wheel', () => {ch.ch_9(ch.ch_107, event.deltaY)})
-ch.ch_270 = document.getElementById("ch_269")
-ch.ch_270.addEventListener('click', () => {{
+ch.ch_271 = document.getElementById("ch_270")
+ch.ch_271.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_107.addEventListener('wheel', () => {ch.ch_8(ch.ch_107, event.deltaY)})
+ch.ch_273 = document.getElementById("ch_272")
+ch.ch_273.addEventListener('click', () => {{
                 let chat_page = ch.ch_111
                 let key = chat_page.children[2].children[0].value
                 ch.ch_133(chat_page, 'right', '我', key, true)
             }})
-ch.ch_275 = document.getElementById("ch_274")
-ch.ch_275.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_281 = document.getElementById("ch_280")
-ch.ch_281.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_286 = document.getElementById("ch_285")
-ch.ch_286.addEventListener('click', () => {ch.ch_32(ch.ch_15, ch.ch_143, 0.2, ch.ch_18)})
-ch.ch_288 = document.getElementById("ch_287")
-ch.ch_288.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, null)})
-ch.ch_290 = document.getElementById("ch_289")
-ch.ch_290.addEventListener('click', () => {ch.ch_33(ch.ch_15, ch.ch_17, 0.2, ch.ch_148)})
-ch.ch_145.addEventListener('wheel', () => {ch.ch_9(ch.ch_145, event.deltaY)})
+ch.ch_278 = document.getElementById("ch_277")
+ch.ch_278.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_284 = document.getElementById("ch_283")
+ch.ch_284.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_289 = document.getElementById("ch_288")
+ch.ch_289.addEventListener('click', async () => {await ch.ch_31(ch.ch_14, ch.ch_144, ch.ch_17)
+await ch.ch_32(ch.ch_14, 1, 0.2, null)})
+ch.ch_291 = document.getElementById("ch_290")
+ch.ch_291.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, null)})
+ch.ch_293 = document.getElementById("ch_292")
+ch.ch_293.addEventListener('click', () => {ch.ch_33(ch.ch_14, ch.ch_16, 0.2, ch.ch_149)})
+ch.ch_146.addEventListener('wheel', () => {ch.ch_8(ch.ch_146, event.deltaY)})
 
 </script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-微信
+聊天
 [ip_static/头像/JS小黄老师.jpg]
 JS小黄老师
-0,1,2,3,4,5,6,7,8,9
 刚刚
 [ip_static/头像/会说话的汤姆猫.jpg]
 会说话的汤姆猫
 刚刚
 [ip_static/头像/鲁迅.jpg]
 鲁迅
 什么是滑坡论证？
@@ -60,26 +59,14 @@
 关于此项目
 💬
 聊天🌍
 发现👨‍💻
 我
 JS小黄老师
 ∟
-'你好呀'
-[ip_static/头像/我.jpg]
-[ip_static/头像/JS小黄老师.jpg]
-你好呀
-1 + 1
-[ip_static/头像/我.jpg]
-[ip_static/头像/JS小黄老师.jpg]
-2
-[...Array(10).keys()]
-[ip_static/头像/我.jpg]
-[ip_static/头像/JS小黄老师.jpg]
-0,1,2,3,4,5,6,7,8,9
 发送
 会说话的汤姆猫
 ∟
 发送
 鲁迅
 ∟
 发送
@@ -143,14 +130,18 @@
 捐赠
 ∟
 [https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg]
 感谢你进入到这里，这说明你对这个软件还是有一些兴趣的！如果你喜欢这个作品，就请支持一下吧！(^_^)
 朋友圈
 ∟
 [ip_static/封面.jpg]
+[ip_static/头像/林宥嘉.jpg]
+林宥嘉
+我发布了音乐
+天将明 -林宥嘉.flac
 [ip_static/头像/李连杰.jpg]
 李连杰
 我发布了短视频
 [ip_static/头像/项羽.jpg]
 项羽
 我发布了短视频
 [ip_static/头像/项羽.jpg]
```

### Comparing `arts-2024.4.1/arts/articles/010-赚钱宝典/010-财富的本质/README.md` & `arts-2024.4.3/arts/articles/010-赚钱宝典/010-财富的本质/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/010-赚钱宝典/020-商业价值/README.md` & `arts-2024.4.3/arts/articles/010-赚钱宝典/020-商业价值/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md` & `arts-2024.4.3/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md` & `arts-2024.4.3/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md` & `arts-2024.4.3/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/150-小民参政/300-广义的民主/README.md` & `arts-2024.4.3/arts/articles/150-小民参政/300-广义的民主/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md` & `arts-2024.4.3/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md` & `arts-2024.4.3/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md` & `arts-2024.4.3/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md` & `arts-2024.4.3/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md` & `arts-2024.4.3/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/700-堕胎自由权/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/700-堕胎自由权/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md` & `arts-2024.4.3/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md` & `arts-2024.4.3/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md` & `arts-2024.4.3/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md` & `arts-2024.4.3/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md` & `arts-2024.4.3/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md` & `arts-2024.4.3/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md` & `arts-2024.4.3/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md` & `arts-2024.4.3/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/cooltypes/LICENSE` & `arts-2024.4.3/arts/cooltypes/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/cooltypes/envname/README.md` & `arts-2024.4.3/arts/cooltypes/envname/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/cooltypes/moduledb/README.md` & `arts-2024.4.3/arts/cooltypes/moduledb/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/cooltypes/moduledb/_core.py` & `arts-2024.4.3/arts/cooltypes/moduledb/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/cooltypes/modules/coolstr/_core.py` & `arts-2024.4.3/arts/cooltypes/modules/coolstr/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/cooltypes/modules/cooltime/README.md` & `arts-2024.4.3/arts/cooltypes/modules/cooltime/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/cooltypes/modules/cooltime/_core.py` & `arts-2024.4.3/arts/cooltypes/modules/cooltime/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/cooltypes/modules/rslice/README.md` & `arts-2024.4.3/arts/cooltypes/modules/rslice/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/cooltypes/modules/rslice/_core.py` & `arts-2024.4.3/arts/cooltypes/modules/rslice/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/cooltypes/modules/vtype/_core.py` & `arts-2024.4.3/arts/cooltypes/modules/vtype/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/index.html` & `arts-2024.4.3/arts/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 <!DOCTYPE html>
-<html class='ch_148 ch_149'><head>
-<title id='ch_143'>江南雨上</title><meta name='msvalidate.01' content='FFA2094263C9178678410FC784304549'><meta name='google-site-verification' content='UNx53G5kjiaAzNZavgTE604GQpveJ6pEtTPi3IMDfPg'><meta charset='utf-8'><meta name='viewport' content='width=device-width, initial-scale=1.0'>
+<html class='ch_151 ch_152'><head>
+<title id='ch_146'>江南雨上</title><meta name='msvalidate.01' content='FFA2094263C9178678410FC784304549'><meta name='google-site-verification' content='UNx53G5kjiaAzNZavgTE604GQpveJ6pEtTPi3IMDfPg'><meta charset='utf-8'><meta name='viewport' content='width=device-width, initial-scale=1.0'>
 <style>
     * {vertical-align:middle; text-decoration:none; position:relative; padding:0; overflow:auto; outline:none; margin:0; font-family:'Chinese Quote', 'Segoe UI', Roboto, RobotoNum, 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'Helvetica Neue', Helvetica, Arial, sans-serif; box-sizing:border-box; border-width:0; border-style:solid;}
-    .ch_149 {width:100vw; height:100vh; display:block; background-color:white;}
-    .ch_176 {display:inline-block; align-self:end;}
-    .ch_177 {display:inline-block; align-self:start;}
-    .ch_150 {width:100%; padding:0.5rem 0 0 0; height:100%; grid-auto-rows:3rem 1fr; display:inline-grid; background-color:white;}
-    .ch_161 {z-index:100; width:100%; min-height:calc(100vh - 3rem - 3.1rem); display:inline-grid; align-content:start;}
-    .ch_162 {padding:0 1.25rem; margin:0.5rem 0; justify-content:flex-start; font-weight:500; font-size:1.5rem; display:inline-grid; color:rgb(225, 172, 12);}
-    .ch_165 {width:15rem; text-decoration:none; height:9.27rem; grid-template-rows:1fr auto; display:inline-grid; color:black; background-size:cover; background-color:rgb(255, 237, 195);}
-    .ch_167 {width:100%; text-align:center; line-height:1.5; letter-spacing:0.075em; height:100%; font-size:1.1rem; display:inline-grid; align-items:center;}
-    .ch_168 {padding:0 0.25rem 0.25rem 0.25rem; justify-items:end; display:inline-grid; color:green; align-items:end;}
-    .ch_169 {width:100%; display:inline-grid;}
-    .ch_170 {width:100%; text-shadow:black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em; text-align:center; line-height:1.5; letter-spacing:0.075em; height:100%; font-weight:600; font-size:1.2rem; display:inline-grid; color:white; align-items:center; -webkit-font-smoothing:antialiased;}
-    .ch_171 {display:inline-grid;}
-    .ch_174 {row-gap:0.5rem; justify-items:center; justify-content:center; grid-template-rows:auto auto; grid-auto-flow:column; font-weight:500; font-size:1.1rem; display:inline-grid; column-gap:4rem; align-content:center;}
-    body[is_x_screen='False'] .ch_173 {grid-auto-flow:row; display:inline-grid;}
-    body[is_x_screen='False'] .ch_175 {padding:1.5em 0 0 0; display:inline-grid; color:rgb(225, 172, 12);}
-    .ch_152 {z-index:200; white-space:nowrap; scrollbar-width:none; overflow:auto; max-width:100%; margin:0 1.25rem; justify-content:space-between; display:inline-block; background-color:white; -ms-overflow-style:none;}
-    .ch_151::-webkit-scrollbar {display:none;}
-    .ch_163 {row-gap:1.5rem; justify-content:center; grid-template-columns:repeat(auto-fill, 15rem); display:inline-grid; column-gap:1.5rem;}
-    .ch_154 {padding:0.618em 1em 0.618em 1em; font-size:1rem; border-radius:3em; background-color:transparent;}
-    body[is_x_screen='True'] .ch_153:not([is_current_nav="True"]):hover {background-color:rgba(247, 215, 114, 0.45);}
-    .ch_155[is_current_nav="True"] {background-color:rgba(247, 215, 114, 1);}
-    .ch_157 {white-space:nowrap; scrollbar-width:none; overflow-x:auto; display:inline-block; -ms-overflow-style:none;}
-    .ch_159:not(.ch_exec_smooth_to_scrollLeft) {scroll-snap-type:x mandatory;}
-    .ch_158::-webkit-scrollbar {display:none;}
-    .ch_156 > * {white-space:normal;}
-    .ch_160 {width:100%; scroll-snap-align:start; padding:0; overflow:auto; margin:0; height:100%; flex-wrap:wrap; display:inline-flex;}
-    .ch_181 {vertical-align:middle;}
-    .ch_178 {vertical-align:baseline; display:inline-block; color:rgba(0, 89, 255, 0.758);}
-    .ch_180:hover {color:rgb(0, 55, 255);}
-    .ch_179:visited {color:rgba(0, 89, 255, 0.758);}
-    .ch_172 {margin:1em 0; justify-self:center; font-weight:500; font-size:1.5rem; color:rgb(225, 172, 12);}
-    .ch_166:hover::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.3);}
-    .ch_164:active::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.5);}
+    .ch_152 {width:100vw; height:100vh; display:block; background-color:white;}
+    .ch_180 {display:inline-block; align-self:end;}
+    .ch_181 {display:inline-block; align-self:start;}
+    .ch_153 {width:100%; padding:0.5rem 0 0 0; height:100%; grid-auto-rows:3rem 1fr; display:inline-grid; background-color:white;}
+    .ch_164 {z-index:100; width:100%; min-height:calc(100vh - 3rem - 3.1rem); display:inline-grid; align-content:start;}
+    .ch_165 {padding:0 1.25rem; margin:0.5rem 0; justify-content:flex-start; font-weight:500; font-size:1.5rem; display:inline-grid; color:rgb(225, 172, 12);}
+    .ch_166 {width:100%; display:inline-grid;}
+    .ch_170 {width:15rem; text-decoration:none; height:9.27rem; grid-template-rows:1fr auto; display:inline-grid; color:black; background-size:cover; background-color:rgb(255, 237, 195);}
+    .ch_172 {width:100%; text-align:center; line-height:1.5; letter-spacing:0.075em; height:100%; font-size:1.1rem; display:inline-grid; align-items:center;}
+    .ch_173 {padding:0 0.25rem 0.25rem 0.25rem; justify-items:end; display:inline-grid; color:green; align-items:end;}
+    .ch_174 {width:100%; text-shadow:black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em; text-align:center; line-height:1.5; letter-spacing:0.075em; height:100%; font-weight:600; font-size:1.2rem; display:inline-grid; color:white; align-items:center; -webkit-font-smoothing:antialiased;}
+    .ch_175 {display:inline-grid;}
+    .ch_177 {row-gap:0.5rem; justify-items:center; justify-content:center; grid-template-rows:auto auto; grid-auto-flow:column; font-weight:500; font-size:1.1rem; display:inline-grid; column-gap:4rem; align-content:center;}
+    body[is_x_screen='False'] .ch_178 {grid-auto-flow:row; display:inline-grid;}
+    body[is_x_screen='False'] .ch_179 {padding:1.5em 0 0 0; display:inline-grid; color:rgb(225, 172, 12);}
+    .ch_155 {z-index:200; white-space:nowrap; scrollbar-width:none; overflow:auto; max-width:100%; margin:0 1.25rem; justify-content:space-between; display:inline-block; background-color:white; -ms-overflow-style:none;}
+    .ch_154::-webkit-scrollbar {display:none;}
+    .ch_168 {row-gap:1.5rem; justify-content:center; grid-template-columns:repeat(auto-fill, 15rem); display:inline-grid; column-gap:1.5rem;}
+    .ch_158 {padding:0.618em 1em 0.618em 1em; font-size:1rem; border-radius:3em; background-color:transparent;}
+    body[is_x_screen='True'] .ch_157:not([is_current_nav="True"]):hover {background-color:rgba(247, 215, 114, 0.45);}
+    .ch_156[is_current_nav="True"] {background-color:rgba(247, 215, 114, 1);}
+    .ch_159 {white-space:nowrap; scrollbar-width:none; overflow-x:auto; display:inline-block; -ms-overflow-style:none;}
+    .ch_162:not(.ch_exec_smooth_to_scrollLeft) {scroll-snap-type:x mandatory;}
+    .ch_161::-webkit-scrollbar {display:none;}
+    .ch_160 > * {white-space:normal;}
+    .ch_163 {width:100%; scroll-snap-align:start; padding:0; overflow:auto; margin:0; height:100%; flex-wrap:wrap; display:inline-flex;}
+    .ch_185 {vertical-align:middle;}
+    .ch_182 {vertical-align:baseline; display:inline-block; color:rgba(0, 89, 255, 0.758);}
+    .ch_184:hover {color:rgb(0, 55, 255);}
+    .ch_183:visited {color:rgba(0, 89, 255, 0.758);}
+    .ch_167 {border-width:0.02rem; border-color:rgb(205, 205, 205);}
+    .ch_176 {margin:1em 0; justify-self:center; font-weight:500; font-size:1.5rem; color:rgb(225, 172, 12);}
+    .ch_169:hover::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.3);}
+    .ch_171:active::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.5);}
 </style></head>
-<body class='ch_150'>
+<body class='ch_153'>
 <script>const ch = {}
-</script><div class='ch_151 ch_152' id='ch_124'><button class='ch_153 ch_154 is_nav ch_155' is_current_nav='True'>动态</button><button class='ch_153 ch_154 is_nav ch_155'>视频</button><button class='ch_153 ch_154 is_nav ch_155'>文章</button><button class='ch_153 ch_154 is_nav ch_155'>想法</button><button class='ch_153 ch_154 is_nav ch_155'>软件</button><button class='ch_153 ch_154 is_nav ch_155'>Python教程</button><button class='ch_153 ch_154 is_nav ch_155'>生活</button><button class='ch_153 ch_154 is_nav ch_155'>自述</button></div><div class='ch_156 ch_157 ch_158 ch_159' id='ch_137'><div class='ch_160'><div class='ch_161'><div class='ch_162'>2024-03-31</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_167'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_168'>2024-03-31</div></a></div><div class='ch_162'>2024-03-18</div><iframe class='ch_169' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id='ch_106'></iframe><hr style="width:100%;"><iframe class='ch_169' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id='ch_10'></iframe><hr style="width:100%;"><div class='ch_162'>2024-03-06</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='oodb/README.md' target='_blank'><div class='ch_167'>oodb<br/>（面向对象数据库）</div><div class='ch_168'>2024-03-06</div></a><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_167'>面向对象数据库</div><div class='ch_168'>2024-03-06</div></a></div><div class='ch_162'>2024-02-13</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='miumapp/README.md' target='_blank'><div class='ch_167'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_168'>2024-02-13</div></a><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_167'>开发跨平台GUI应用</div><div class='ch_168'>2024-02-13</div></a></div><div class='ch_162'>2024-01-30</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_170'>秦时明月[项羽]·谪居</div><div class='ch_168'>2024-01-30</div></a></div><div class='ch_162'>2024-01-25</div><iframe class='ch_169' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id='ch_14'></iframe><hr style="width:100%;"><div class='ch_162'>2024-01-13</div><iframe class='ch_169' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id='ch_18'></iframe><hr style="width:100%;"><div class='ch_162'>2024-01-09</div><iframe class='ch_169' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id='ch_22'></iframe><hr style="width:100%;"><div class='ch_162'>2024-01-03</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_170'>产业升级与失业潮</div><div class='ch_168'>2024-01-03</div></a><a class='ch_164 ch_165 ch_166' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_167'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_168'>2024-01-03</div></a></div><iframe class='ch_169' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id='ch_26'></iframe><hr style="width:100%;"><div class='ch_162'>2024-01-01</div><iframe class='ch_169' src='thoughts/2024/新年题诗/index.html' loading='lazy' id='ch_30'></iframe><hr style="width:100%;"><div class='ch_162'>2023-12-28</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_167'>那些年，我们经历过的历史</div><div class='ch_168'>2023-12-28</div></a></div><div class='ch_162'>2023-12-22</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_167'>财富稳定型社会</div><div class='ch_168'>2023-12-22</div></a></div><div class='ch_162'>2023-12-11</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='CoolMemory-English/README.md' target='_blank'><div class='ch_167'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_168'>2023-12-11</div></a></div><div class='ch_162'>2023-11-12</div><iframe class='ch_169' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id='ch_34'></iframe><hr style="width:100%;"><div class='ch_162'>2023-11-02</div><iframe class='ch_169' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id='ch_38'></iframe><hr style="width:100%;"><div class='ch_162'>2023-10-24</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_167'>年轻人不结婚是文明的进步</div><div class='ch_168'>2023-10-24</div></a></div><div class='ch_162'>2023-10-09</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_167'>未经他人苦，莫劝他人善？</div><div class='ch_168'>2023-10-09</div></a></div><div class='ch_162'>2023-10-06</div><iframe class='ch_169' src='life/2023/更换微信账号了/index.html' loading='lazy' id='ch_110'></iframe><hr style="width:100%;"><div class='ch_162'>2023-09-22</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_167'>商业价值</div><div class='ch_168'>2023-09-22</div></a></div><div class='ch_162'>2023-09-20</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_167'>财富的本质</div><div class='ch_168'>2023-09-20</div></a></div><div class='ch_162'>2023-09-15</div><iframe class='ch_169' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id='ch_42'></iframe><hr style="width:100%;"><iframe class='ch_169' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id='ch_46'></iframe><hr style="width:100%;"><div class='ch_162'>2023-09-08</div><iframe class='ch_169' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id='ch_50'></iframe><hr style="width:100%;"><div class='ch_162'>2023-08-18</div><iframe class='ch_169' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id='ch_54'></iframe><hr style="width:100%;"><div class='ch_162'>2023-08-17</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_167'>人们为什么希望拥有后代</div><div class='ch_168'>2023-08-17</div></a></div><div class='ch_162'>2023-08-06</div><iframe class='ch_169' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id='ch_58'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-30</div><iframe class='ch_169' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id='ch_62'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-20</div><iframe class='ch_169' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id='ch_66'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-19</div><iframe class='ch_169' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id='ch_70'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-11</div><iframe class='ch_169' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id='ch_74'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-10</div><iframe class='ch_169' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id='ch_78'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-09</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_167'>一元官司有意义吗？</div><div class='ch_168'>2023-07-09</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_167'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_168'>2023-07-09</div></a></div><div class='ch_162'>2023-07-06</div><iframe class='ch_169' src='thoughts/2023/保护好人/index.html' loading='lazy' id='ch_82'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-04</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_167'>心理学中个案研究有意义吗？</div><div class='ch_168'>2023-07-04</div></a></div><div class='ch_162'>2023-07-01</div><iframe class='ch_169' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id='ch_86'></iframe><hr style="width:100%;"><div class='ch_162'>2023-06-25</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_167'>时间模块</div><div class='ch_168'>2023-06-25</div></a></div><div class='ch_162'>2023-06-19</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_167'>正则表达式</div><div class='ch_168'>2023-06-19</div></a></div><div class='ch_162'>2023-06-18</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_170'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_168'>2023-06-18</div></a></div><div class='ch_162'>2023-06-09</div><iframe class='ch_169' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id='ch_90'></iframe><hr style="width:100%;"><div class='ch_162'>2023-06-07</div><iframe class='ch_169' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id='ch_94'></iframe><hr style="width:100%;"><div class='ch_162'>2023-05-26</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_167'>万物为什么会遵循着物理定律？</div><div class='ch_168'>2023-05-26</div></a></div><div class='ch_162'>2023-05-13</div><iframe class='ch_169' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id='ch_98'></iframe><hr style="width:100%;"><div class='ch_162'>2023-03-07</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='openai2/README.md' target='_blank'><div class='ch_167'>openai2<br/>（openai接口封装）</div><div class='ch_168'>2023-03-07</div></a><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_167'>对接ChatGPT</div><div class='ch_168'>2023-03-07</div></a></div><div class='ch_162'>2023-03-06</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_167'>ChatGPT已经有自我意识了</div><div class='ch_168'>2023-03-06</div></a></div><div class='ch_162'>2022-12-31</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_167'>务实与务虚</div><div class='ch_168'>2022-12-31</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_167'>人人平等是个伪概念</div><div class='ch_168'>2022-12-31</div></a></div><div class='ch_162'>2022-12-25</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_170'>人工智能会不会统治人类？</div><div class='ch_168'>2022-12-25</div></a></div><div class='ch_162'>2022-12-16</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_170'>广义的民主</div><div class='ch_168'>2022-12-16</div></a></div><div class='ch_162'>2022-11-25</div><iframe class='ch_169' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id='ch_114'></iframe><hr style="width:100%;"><div class='ch_162'>2022-09-27</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_170'>李连杰[霍元甲]·兰亭序</div><div class='ch_168'>2022-09-27</div></a></div><div class='ch_162'>2022-09-21</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_167'>堕胎自由权</div><div class='ch_168'>2022-09-21</div></a></div><div class='ch_162'>2022-09-08</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_170'>楚门的世界·五月雨</div><div class='ch_168'>2022-09-08</div></a></div><div class='ch_162'>2022-08-12</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_167'>被绑架</div><div class='ch_168'>2022-08-12</div></a></div><div class='ch_162'>2022-08-01</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_167'>怎么理解「迷信科学」？</div><div class='ch_168'>2022-08-01</div></a></div><div class='ch_162'>2022-06-15</div><iframe class='ch_169' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id='ch_102'></iframe><hr style="width:100%;"><div class='ch_162'>2021-07-28</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_170'>AI是这样画包拯的</div><div class='ch_168'>2021-07-28</div></a></div><div class='ch_162'>2021-06-11</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_167'>“自由意志”其实是“随机意志”</div><div class='ch_168'>2021-06-11</div></a></div><div class='ch_162'>2021-06-10</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_167'>有无相生，难易相成的启发</div><div class='ch_168'>2021-06-10</div></a></div><div class='ch_162'>2021-06-09</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_170'>占卜真的存在吗？</div><div class='ch_168'>2021-06-09</div></a></div><div class='ch_162'>2021-06-07</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_167'>我们可能处在人造世界</div><div class='ch_168'>2021-06-07</div></a></div><div class='ch_162'>2021-06-06</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='oomongo/README.md' target='_blank'><div class='ch_167'>oomongo<br/>（MongoDB ODM）</div><div class='ch_168'>2021-06-06</div></a><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_167'>操作MongoDB</div><div class='ch_168'>2021-06-06</div></a><a class='ch_164 ch_165 ch_166' href='oomysql/README.md' target='_blank'><div class='ch_167'>oomysql<br/>（MySQL ORM）</div><div class='ch_168'>2021-06-06</div></a><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_167'>操作MySQL</div><div class='ch_168'>2021-06-06</div></a></div><div class='ch_162'>2021-06-05</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_170'>轮回转世真的存在吗？</div><div class='ch_168'>2021-06-05</div></a></div><div class='ch_162'>2021-06-03</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_170'>唯有变化是不变的？</div><div class='ch_168'>2021-06-03</div></a></div><div class='ch_162'>2021-06-01</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_167'>忒修斯之船悖论</div><div class='ch_168'>2021-06-01</div></a></div><div class='ch_162'>2020-12-31</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_167'>燕山宝藏 第1章</div><div class='ch_168'>2020-12-31</div></a></div><div class='ch_162'>2019-08-05</div><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_167'>用37行代码实现AI五子棋</div><div class='ch_168'>2019-08-05</div></a></div><div class='ch_162'>2019-05-01</div><iframe class='ch_169' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id='ch_118'></iframe><hr style="width:100%;"><div class='ch_162'>2018-05-28</div><iframe class='ch_169' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id='ch_122'></iframe><hr style="width:100%;"></div><div class='ch_171' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_160'><div class='ch_161'><h3 class='ch_172'>videos</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_170'>秦时明月[项羽]·谪居</div><div class='ch_168'>2024-01-30</div></a><a class='ch_164 ch_165 ch_166' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_170'>李连杰[霍元甲]·兰亭序</div><div class='ch_168'>2022-09-27</div></a><a class='ch_164 ch_165 ch_166' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_170'>楚门的世界·五月雨</div><div class='ch_168'>2022-09-08</div></a><a class='ch_164 ch_165 ch_166' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_170'>AI是这样画包拯的</div><div class='ch_168'>2021-07-28</div></a></div></div><div class='ch_171' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_160'><div class='ch_161'><h3 class='ch_172'>赚钱宝典</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_167'>财富的本质</div><div class='ch_168'>2023-09-20</div></a><a class='ch_164 ch_165 ch_166' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_167'>商业价值</div><div class='ch_168'>2023-09-22</div></a><a class='ch_164 ch_165 ch_166' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_167'>财富稳定型社会</div><div class='ch_168'>2023-12-22</div></a></div><h3 class='ch_172'>追英赶美</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_170'>产业升级与失业潮</div><div class='ch_168'>2024-01-03</div></a><a class='ch_164 ch_165 ch_166' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_167'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_168'>2024-01-03</div></a></div><h3 class='ch_172'>小民参政</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_170'>广义的民主</div><div class='ch_168'>2022-12-16</div></a><a class='ch_164 ch_165 ch_166' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_167'>年轻人不结婚是文明的进步</div><div class='ch_168'>2023-10-24</div></a></div><h3 class='ch_172'>批判那些伪文艺</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_167'>一元官司有意义吗？</div><div class='ch_168'>2023-07-09</div></a><a class='ch_164 ch_165 ch_166' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_170'>唯有变化是不变的？</div><div class='ch_168'>2021-06-03</div></a><a class='ch_164 ch_165 ch_166' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_167'>未经他人苦，莫劝他人善？</div><div class='ch_168'>2023-10-09</div></a><a class='ch_164 ch_165 ch_166' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_167'>务实与务虚</div><div class='ch_168'>2022-12-31</div></a></div><h3 class='ch_172'>万象思考</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_167'>ChatGPT已经有自我意识了</div><div class='ch_168'>2023-03-06</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_167'>怎么理解「迷信科学」？</div><div class='ch_168'>2022-08-01</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_167'>心理学中个案研究有意义吗？</div><div class='ch_168'>2023-07-04</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_170'>人工智能会不会统治人类？</div><div class='ch_168'>2022-12-25</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_167'>忒修斯之船悖论</div><div class='ch_168'>2021-06-01</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_167'>有无相生，难易相成的启发</div><div class='ch_168'>2021-06-10</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_167'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_168'>2023-07-09</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_167'>人们为什么希望拥有后代</div><div class='ch_168'>2023-08-17</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_167'>万物为什么会遵循着物理定律？</div><div class='ch_168'>2023-05-26</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_167'>堕胎自由权</div><div class='ch_168'>2022-09-21</div></a><a class='ch_164 ch_165 ch_166' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_167'>人人平等是个伪概念</div><div class='ch_168'>2022-12-31</div></a></div><h3 class='ch_172'>时空猜想</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_170'>轮回转世真的存在吗？</div><div class='ch_168'>2021-06-05</div></a><a class='ch_164 ch_165 ch_166' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_167'>我们可能处在人造世界</div><div class='ch_168'>2021-06-07</div></a><a class='ch_164 ch_165 ch_166' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_170'>占卜真的存在吗？</div><div class='ch_168'>2021-06-09</div></a><a class='ch_164 ch_165 ch_166' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_167'>“自由意志”其实是“随机意志”</div><div class='ch_168'>2021-06-11</div></a></div><h3 class='ch_172'>论时事</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_167'>那些年，我们经历过的历史</div><div class='ch_168'>2023-12-28</div></a><a class='ch_164 ch_165 ch_166' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_170'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_168'>2023-06-18</div></a></div><h3 class='ch_172'>小说 / 陆小凤新传</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_167'>燕山宝藏 第1章</div><div class='ch_168'>2020-12-31</div></a></div><h3 class='ch_172'>小说 / 一念天堂</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_167'>被绑架</div><div class='ch_168'>2022-08-12</div></a></div></div><div class='ch_171' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_160'><div class='ch_161'><div class='ch_162'>2024-03-18</div><iframe class='ch_169' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id='ch_7'></iframe><hr style="width:100%;"><div class='ch_162'>2024-01-25</div><iframe class='ch_169' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id='ch_12'></iframe><hr style="width:100%;"><div class='ch_162'>2024-01-13</div><iframe class='ch_169' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id='ch_16'></iframe><hr style="width:100%;"><div class='ch_162'>2024-01-09</div><iframe class='ch_169' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id='ch_20'></iframe><hr style="width:100%;"><div class='ch_162'>2024-01-03</div><iframe class='ch_169' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id='ch_24'></iframe><hr style="width:100%;"><div class='ch_162'>2024-01-01</div><iframe class='ch_169' src='thoughts/2024/新年题诗/index.html' loading='lazy' id='ch_28'></iframe><hr style="width:100%;"><div class='ch_162'>2023-11-12</div><iframe class='ch_169' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id='ch_32'></iframe><hr style="width:100%;"><div class='ch_162'>2023-11-02</div><iframe class='ch_169' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id='ch_36'></iframe><hr style="width:100%;"><div class='ch_162'>2023-09-15</div><iframe class='ch_169' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id='ch_40'></iframe><hr style="width:100%;"><iframe class='ch_169' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id='ch_44'></iframe><hr style="width:100%;"><div class='ch_162'>2023-09-08</div><iframe class='ch_169' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id='ch_48'></iframe><hr style="width:100%;"><div class='ch_162'>2023-08-18</div><iframe class='ch_169' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id='ch_52'></iframe><hr style="width:100%;"><div class='ch_162'>2023-08-06</div><iframe class='ch_169' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id='ch_56'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-30</div><iframe class='ch_169' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id='ch_60'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-20</div><iframe class='ch_169' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id='ch_64'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-19</div><iframe class='ch_169' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id='ch_68'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-11</div><iframe class='ch_169' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id='ch_72'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-10</div><iframe class='ch_169' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id='ch_76'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-06</div><iframe class='ch_169' src='thoughts/2023/保护好人/index.html' loading='lazy' id='ch_80'></iframe><hr style="width:100%;"><div class='ch_162'>2023-07-01</div><iframe class='ch_169' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id='ch_84'></iframe><hr style="width:100%;"><div class='ch_162'>2023-06-09</div><iframe class='ch_169' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id='ch_88'></iframe><hr style="width:100%;"><div class='ch_162'>2023-06-07</div><iframe class='ch_169' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id='ch_92'></iframe><hr style="width:100%;"><div class='ch_162'>2023-05-13</div><iframe class='ch_169' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id='ch_96'></iframe><hr style="width:100%;"><div class='ch_162'>2022-06-15</div><iframe class='ch_169' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id='ch_100'></iframe><hr style="width:100%;"></div><div class='ch_171' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_160'><div class='ch_161'><h3 class='ch_172'>software</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='CoolMemory-English/README.md' target='_blank'><div class='ch_167'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_168'>2023-12-11</div></a><a class='ch_164 ch_165 ch_166' href='miumapp/README.md' target='_blank'><div class='ch_167'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_168'>2024-02-13</div></a><a class='ch_164 ch_165 ch_166' href='oodb/README.md' target='_blank'><div class='ch_167'>oodb<br/>（面向对象数据库）</div><div class='ch_168'>2024-03-06</div></a><a class='ch_164 ch_165 ch_166' href='oomongo/README.md' target='_blank'><div class='ch_167'>oomongo<br/>（MongoDB ODM）</div><div class='ch_168'>2021-06-06</div></a><a class='ch_164 ch_165 ch_166' href='oomysql/README.md' target='_blank'><div class='ch_167'>oomysql<br/>（MySQL ORM）</div><div class='ch_168'>2021-06-06</div></a><a class='ch_164 ch_165 ch_166' href='openai2/README.md' target='_blank'><div class='ch_167'>openai2<br/>（openai接口封装）</div><div class='ch_168'>2023-03-07</div></a><a class='ch_164 ch_165 ch_166' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_167'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_168'>2024-03-31</div></a></div></div><div class='ch_171' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_160'><div class='ch_161'><h3 class='ch_172'>tutorials</h3><div class='ch_163'><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_167'>操作MySQL</div><div class='ch_168'>2021-06-06</div></a><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_167'>操作MongoDB</div><div class='ch_168'>2021-06-06</div></a><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_167'>开发跨平台GUI应用</div><div class='ch_168'>2024-02-13</div></a><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_167'>对接ChatGPT</div><div class='ch_168'>2023-03-07</div></a><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_167'>时间模块</div><div class='ch_168'>2023-06-25</div></a><a class='ch_164 ch_165 ch_166' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_167'>面向对象数据库</div><div class='ch_168'>2024-03-06</div></a><a class='ch_164 ch_165 ch_166' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_167'>用37行代码实现AI五子棋</div><div class='ch_168'>2019-08-05</div></a><a class='ch_164 ch_165 ch_166' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_167'>正则表达式</div><div class='ch_168'>2023-06-19</div></a></div></div><div class='ch_171' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_160'><div class='ch_161'><div class='ch_162'>2024-03-18</div><iframe class='ch_169' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id='ch_104'></iframe><hr style="width:100%;"><div class='ch_162'>2023-10-06</div><iframe class='ch_169' src='life/2023/更换微信账号了/index.html' loading='lazy' id='ch_108'></iframe><hr style="width:100%;"><div class='ch_162'>2022-11-25</div><iframe class='ch_169' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id='ch_112'></iframe><hr style="width:100%;"><div class='ch_162'>2019-05-01</div><iframe class='ch_169' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id='ch_116'></iframe><hr style="width:100%;"><div class='ch_162'>2018-05-28</div><iframe class='ch_169' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id='ch_120'></iframe><hr style="width:100%;"></div><div class='ch_171' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_160'><div class='ch_161' style="align-content:stretch;"><div class='ch_173 ch_174'><div class='ch_175 ch_176'>邮箱</div><div class='ch_177'><a class='ch_178 ch_179 ch_180' href='mailto:lcctoor@outlook.com'>lcctoor@outlook.com</a></div><div class='ch_175 ch_176'>微信</div><div class='ch_177'><img class='ch_181' src='./ip_static/WeChatQRC.jpg' style="max-width:15rem; height:auto;"></div><div class='ch_175 ch_176'>捐赠</div><div class='ch_177'><img class='ch_181' src='./ip_static/DonationQRC-0rmb.jpg' style="max-width:15rem; height:auto;"></div></div></div><div class='ch_171' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div></div>
+</script><div class='ch_154 ch_155' id='ch_127'><button class='ch_156 ch_157 is_nav ch_158' is_current_nav='True'>动态</button><button class='ch_156 ch_157 is_nav ch_158'>视频</button><button class='ch_156 ch_157 is_nav ch_158'>文章</button><button class='ch_156 ch_157 is_nav ch_158'>想法</button><button class='ch_156 ch_157 is_nav ch_158'>软件</button><button class='ch_156 ch_157 is_nav ch_158'>Python教程</button><button class='ch_156 ch_157 is_nav ch_158'>生活</button><button class='ch_156 ch_157 is_nav ch_158'>自述</button></div><div class='ch_159 ch_160 ch_161 ch_162' id='ch_140'><div class='ch_163'><div class='ch_164'><div class='ch_165'>2024-04-03</div><iframe class='ch_166' src='thoughts/2024/做有趣的事情/index.html' loading='lazy' id='ch_9'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-03-31</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_172'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_173'>2024-03-31</div></a></div><div class='ch_165'>2024-03-18</div><iframe class='ch_166' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id='ch_109'></iframe><hr class='ch_167' style="width:100%;"><iframe class='ch_166' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id='ch_13'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-03-06</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='oodb/README.md' target='_blank'><div class='ch_172'>oodb<br/>（面向对象数据库）</div><div class='ch_173'>2024-03-06</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_172'>面向对象数据库</div><div class='ch_173'>2024-03-06</div></a></div><div class='ch_165'>2024-02-13</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='miumapp/README.md' target='_blank'><div class='ch_172'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_173'>2024-02-13</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_172'>开发跨平台GUI应用</div><div class='ch_173'>2024-02-13</div></a></div><div class='ch_165'>2024-01-30</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_174'>秦时明月[项羽]·谪居</div><div class='ch_173'>2024-01-30</div></a></div><div class='ch_165'>2024-01-25</div><iframe class='ch_166' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id='ch_17'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-13</div><iframe class='ch_166' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id='ch_21'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-09</div><iframe class='ch_166' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id='ch_25'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-03</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_174'>产业升级与失业潮</div><div class='ch_173'>2024-01-03</div></a><a class='ch_169 ch_170 ch_171' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_172'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_173'>2024-01-03</div></a></div><iframe class='ch_166' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id='ch_29'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-01</div><iframe class='ch_166' src='thoughts/2024/新年题诗/index.html' loading='lazy' id='ch_33'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-12-28</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_172'>那些年，我们经历过的历史</div><div class='ch_173'>2023-12-28</div></a></div><div class='ch_165'>2023-12-22</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_172'>财富稳定型社会</div><div class='ch_173'>2023-12-22</div></a></div><div class='ch_165'>2023-12-11</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='CoolMemory-English/README.md' target='_blank'><div class='ch_172'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_173'>2023-12-11</div></a></div><div class='ch_165'>2023-11-12</div><iframe class='ch_166' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id='ch_37'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-11-02</div><iframe class='ch_166' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id='ch_41'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-10-24</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_172'>年轻人不结婚是文明的进步</div><div class='ch_173'>2023-10-24</div></a></div><div class='ch_165'>2023-10-09</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_172'>未经他人苦，莫劝他人善？</div><div class='ch_173'>2023-10-09</div></a></div><div class='ch_165'>2023-10-06</div><iframe class='ch_166' src='life/2023/更换微信账号了/index.html' loading='lazy' id='ch_113'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-09-22</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_172'>商业价值</div><div class='ch_173'>2023-09-22</div></a></div><div class='ch_165'>2023-09-20</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_172'>财富的本质</div><div class='ch_173'>2023-09-20</div></a></div><div class='ch_165'>2023-09-15</div><iframe class='ch_166' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id='ch_45'></iframe><hr class='ch_167' style="width:100%;"><iframe class='ch_166' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id='ch_49'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-09-08</div><iframe class='ch_166' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id='ch_53'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-08-18</div><iframe class='ch_166' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id='ch_57'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-08-17</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_172'>人们为什么希望拥有后代</div><div class='ch_173'>2023-08-17</div></a></div><div class='ch_165'>2023-08-06</div><iframe class='ch_166' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id='ch_61'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-30</div><iframe class='ch_166' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id='ch_65'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-20</div><iframe class='ch_166' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id='ch_69'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-19</div><iframe class='ch_166' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id='ch_73'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-11</div><iframe class='ch_166' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id='ch_77'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-10</div><iframe class='ch_166' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id='ch_81'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-09</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_172'>一元官司有意义吗？</div><div class='ch_173'>2023-07-09</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_172'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_173'>2023-07-09</div></a></div><div class='ch_165'>2023-07-06</div><iframe class='ch_166' src='thoughts/2023/保护好人/index.html' loading='lazy' id='ch_85'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-04</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_172'>心理学中个案研究有意义吗？</div><div class='ch_173'>2023-07-04</div></a></div><div class='ch_165'>2023-07-01</div><iframe class='ch_166' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id='ch_89'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-06-25</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_172'>时间模块</div><div class='ch_173'>2023-06-25</div></a></div><div class='ch_165'>2023-06-19</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_172'>正则表达式</div><div class='ch_173'>2023-06-19</div></a></div><div class='ch_165'>2023-06-18</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_174'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_173'>2023-06-18</div></a></div><div class='ch_165'>2023-06-09</div><iframe class='ch_166' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id='ch_93'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-06-07</div><iframe class='ch_166' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id='ch_97'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-05-26</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_172'>万物为什么会遵循着物理定律？</div><div class='ch_173'>2023-05-26</div></a></div><div class='ch_165'>2023-05-13</div><iframe class='ch_166' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id='ch_101'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-03-07</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='openai2/README.md' target='_blank'><div class='ch_172'>openai2<br/>（openai接口封装）</div><div class='ch_173'>2023-03-07</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_172'>对接ChatGPT</div><div class='ch_173'>2023-03-07</div></a></div><div class='ch_165'>2023-03-06</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_172'>ChatGPT已经有自我意识了</div><div class='ch_173'>2023-03-06</div></a></div><div class='ch_165'>2022-12-31</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_172'>务实与务虚</div><div class='ch_173'>2022-12-31</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_172'>人人平等是个伪概念</div><div class='ch_173'>2022-12-31</div></a></div><div class='ch_165'>2022-12-25</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_174'>人工智能会不会统治人类？</div><div class='ch_173'>2022-12-25</div></a></div><div class='ch_165'>2022-12-16</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_174'>广义的民主</div><div class='ch_173'>2022-12-16</div></a></div><div class='ch_165'>2022-11-25</div><iframe class='ch_166' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id='ch_117'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2022-09-27</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_174'>李连杰[霍元甲]·兰亭序</div><div class='ch_173'>2022-09-27</div></a></div><div class='ch_165'>2022-09-21</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_172'>堕胎自由权</div><div class='ch_173'>2022-09-21</div></a></div><div class='ch_165'>2022-09-08</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_174'>楚门的世界·五月雨</div><div class='ch_173'>2022-09-08</div></a></div><div class='ch_165'>2022-08-12</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_172'>被绑架</div><div class='ch_173'>2022-08-12</div></a></div><div class='ch_165'>2022-08-01</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_172'>怎么理解「迷信科学」？</div><div class='ch_173'>2022-08-01</div></a></div><div class='ch_165'>2022-06-15</div><iframe class='ch_166' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id='ch_105'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2021-07-28</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_174'>AI是这样画包拯的</div><div class='ch_173'>2021-07-28</div></a></div><div class='ch_165'>2021-06-11</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_172'>“自由意志”其实是“随机意志”</div><div class='ch_173'>2021-06-11</div></a></div><div class='ch_165'>2021-06-10</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_172'>有无相生，难易相成的启发</div><div class='ch_173'>2021-06-10</div></a></div><div class='ch_165'>2021-06-09</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_174'>占卜真的存在吗？</div><div class='ch_173'>2021-06-09</div></a></div><div class='ch_165'>2021-06-07</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_172'>我们可能处在人造世界</div><div class='ch_173'>2021-06-07</div></a></div><div class='ch_165'>2021-06-06</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='oomongo/README.md' target='_blank'><div class='ch_172'>oomongo<br/>（MongoDB ODM）</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_172'>操作MongoDB</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='oomysql/README.md' target='_blank'><div class='ch_172'>oomysql<br/>（MySQL ORM）</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_172'>操作MySQL</div><div class='ch_173'>2021-06-06</div></a></div><div class='ch_165'>2021-06-05</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_174'>轮回转世真的存在吗？</div><div class='ch_173'>2021-06-05</div></a></div><div class='ch_165'>2021-06-03</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_174'>唯有变化是不变的？</div><div class='ch_173'>2021-06-03</div></a></div><div class='ch_165'>2021-06-01</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_172'>忒修斯之船悖论</div><div class='ch_173'>2021-06-01</div></a></div><div class='ch_165'>2020-12-31</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_172'>燕山宝藏 第1章</div><div class='ch_173'>2020-12-31</div></a></div><div class='ch_165'>2019-08-05</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_172'>用37行代码实现AI五子棋</div><div class='ch_173'>2019-08-05</div></a></div><div class='ch_165'>2019-05-01</div><iframe class='ch_166' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id='ch_121'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2018-05-28</div><iframe class='ch_166' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id='ch_125'></iframe><hr class='ch_167' style="width:100%;"></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><h3 class='ch_176'>videos</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_174'>秦时明月[项羽]·谪居</div><div class='ch_173'>2024-01-30</div></a><a class='ch_169 ch_170 ch_171' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_174'>李连杰[霍元甲]·兰亭序</div><div class='ch_173'>2022-09-27</div></a><a class='ch_169 ch_170 ch_171' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_174'>楚门的世界·五月雨</div><div class='ch_173'>2022-09-08</div></a><a class='ch_169 ch_170 ch_171' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_174'>AI是这样画包拯的</div><div class='ch_173'>2021-07-28</div></a></div></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><h3 class='ch_176'>赚钱宝典</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_172'>财富的本质</div><div class='ch_173'>2023-09-20</div></a><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_172'>商业价值</div><div class='ch_173'>2023-09-22</div></a><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_172'>财富稳定型社会</div><div class='ch_173'>2023-12-22</div></a></div><h3 class='ch_176'>追英赶美</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_174'>产业升级与失业潮</div><div class='ch_173'>2024-01-03</div></a><a class='ch_169 ch_170 ch_171' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_172'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_173'>2024-01-03</div></a></div><h3 class='ch_176'>小民参政</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_174'>广义的民主</div><div class='ch_173'>2022-12-16</div></a><a class='ch_169 ch_170 ch_171' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_172'>年轻人不结婚是文明的进步</div><div class='ch_173'>2023-10-24</div></a></div><h3 class='ch_176'>批判那些伪文艺</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_172'>一元官司有意义吗？</div><div class='ch_173'>2023-07-09</div></a><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_174'>唯有变化是不变的？</div><div class='ch_173'>2021-06-03</div></a><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_172'>未经他人苦，莫劝他人善？</div><div class='ch_173'>2023-10-09</div></a><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_172'>务实与务虚</div><div class='ch_173'>2022-12-31</div></a></div><h3 class='ch_176'>万象思考</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_172'>ChatGPT已经有自我意识了</div><div class='ch_173'>2023-03-06</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_172'>怎么理解「迷信科学」？</div><div class='ch_173'>2022-08-01</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_172'>心理学中个案研究有意义吗？</div><div class='ch_173'>2023-07-04</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_174'>人工智能会不会统治人类？</div><div class='ch_173'>2022-12-25</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_172'>忒修斯之船悖论</div><div class='ch_173'>2021-06-01</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_172'>有无相生，难易相成的启发</div><div class='ch_173'>2021-06-10</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_172'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_173'>2023-07-09</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_172'>人们为什么希望拥有后代</div><div class='ch_173'>2023-08-17</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_172'>万物为什么会遵循着物理定律？</div><div class='ch_173'>2023-05-26</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_172'>堕胎自由权</div><div class='ch_173'>2022-09-21</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_172'>人人平等是个伪概念</div><div class='ch_173'>2022-12-31</div></a></div><h3 class='ch_176'>时空猜想</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_174'>轮回转世真的存在吗？</div><div class='ch_173'>2021-06-05</div></a><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_172'>我们可能处在人造世界</div><div class='ch_173'>2021-06-07</div></a><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_174'>占卜真的存在吗？</div><div class='ch_173'>2021-06-09</div></a><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_172'>“自由意志”其实是“随机意志”</div><div class='ch_173'>2021-06-11</div></a></div><h3 class='ch_176'>论时事</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_172'>那些年，我们经历过的历史</div><div class='ch_173'>2023-12-28</div></a><a class='ch_169 ch_170 ch_171' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_174'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_173'>2023-06-18</div></a></div><h3 class='ch_176'>小说 / 陆小凤新传</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_172'>燕山宝藏 第1章</div><div class='ch_173'>2020-12-31</div></a></div><h3 class='ch_176'>小说 / 一念天堂</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_172'>被绑架</div><div class='ch_173'>2022-08-12</div></a></div></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><div class='ch_165'>2024-04-03</div><iframe class='ch_166' src='thoughts/2024/做有趣的事情/index.html' loading='lazy' id='ch_6'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-03-18</div><iframe class='ch_166' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id='ch_11'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-25</div><iframe class='ch_166' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id='ch_15'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-13</div><iframe class='ch_166' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id='ch_19'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-09</div><iframe class='ch_166' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id='ch_23'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-03</div><iframe class='ch_166' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id='ch_27'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-01</div><iframe class='ch_166' src='thoughts/2024/新年题诗/index.html' loading='lazy' id='ch_31'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-11-12</div><iframe class='ch_166' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id='ch_35'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-11-02</div><iframe class='ch_166' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id='ch_39'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-09-15</div><iframe class='ch_166' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id='ch_43'></iframe><hr class='ch_167' style="width:100%;"><iframe class='ch_166' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id='ch_47'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-09-08</div><iframe class='ch_166' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id='ch_51'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-08-18</div><iframe class='ch_166' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id='ch_55'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-08-06</div><iframe class='ch_166' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id='ch_59'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-30</div><iframe class='ch_166' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id='ch_63'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-20</div><iframe class='ch_166' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id='ch_67'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-19</div><iframe class='ch_166' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id='ch_71'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-11</div><iframe class='ch_166' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id='ch_75'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-10</div><iframe class='ch_166' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id='ch_79'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-06</div><iframe class='ch_166' src='thoughts/2023/保护好人/index.html' loading='lazy' id='ch_83'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-01</div><iframe class='ch_166' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id='ch_87'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-06-09</div><iframe class='ch_166' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id='ch_91'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-06-07</div><iframe class='ch_166' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id='ch_95'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-05-13</div><iframe class='ch_166' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id='ch_99'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2022-06-15</div><iframe class='ch_166' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id='ch_103'></iframe><hr class='ch_167' style="width:100%;"></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><h3 class='ch_176'>software</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='CoolMemory-English/README.md' target='_blank'><div class='ch_172'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_173'>2023-12-11</div></a><a class='ch_169 ch_170 ch_171' href='miumapp/README.md' target='_blank'><div class='ch_172'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_173'>2024-02-13</div></a><a class='ch_169 ch_170 ch_171' href='oodb/README.md' target='_blank'><div class='ch_172'>oodb<br/>（面向对象数据库）</div><div class='ch_173'>2024-03-06</div></a><a class='ch_169 ch_170 ch_171' href='oomongo/README.md' target='_blank'><div class='ch_172'>oomongo<br/>（MongoDB ODM）</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='oomysql/README.md' target='_blank'><div class='ch_172'>oomysql<br/>（MySQL ORM）</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='openai2/README.md' target='_blank'><div class='ch_172'>openai2<br/>（openai接口封装）</div><div class='ch_173'>2023-03-07</div></a><a class='ch_169 ch_170 ch_171' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_172'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_173'>2024-03-31</div></a></div></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><h3 class='ch_176'>tutorials</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_172'>操作MySQL</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_172'>操作MongoDB</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_172'>开发跨平台GUI应用</div><div class='ch_173'>2024-02-13</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_172'>对接ChatGPT</div><div class='ch_173'>2023-03-07</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_172'>时间模块</div><div class='ch_173'>2023-06-25</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_172'>面向对象数据库</div><div class='ch_173'>2024-03-06</div></a><a class='ch_169 ch_170 ch_171' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_172'>用37行代码实现AI五子棋</div><div class='ch_173'>2019-08-05</div></a><a class='ch_169 ch_170 ch_171' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_172'>正则表达式</div><div class='ch_173'>2023-06-19</div></a></div></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><div class='ch_165'>2024-03-18</div><iframe class='ch_166' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id='ch_107'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-10-06</div><iframe class='ch_166' src='life/2023/更换微信账号了/index.html' loading='lazy' id='ch_111'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2022-11-25</div><iframe class='ch_166' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id='ch_115'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2019-05-01</div><iframe class='ch_166' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id='ch_119'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2018-05-28</div><iframe class='ch_166' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id='ch_123'></iframe><hr class='ch_167' style="width:100%;"></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164' style="align-content:stretch;"><div class='ch_177 ch_178'><div class='ch_179 ch_180'>邮箱</div><div class='ch_181'><a class='ch_182 ch_183 ch_184' href='mailto:lcctoor@outlook.com'>lcctoor@outlook.com</a></div><div class='ch_179 ch_180'>微信</div><div class='ch_181'><img class='ch_185' src='./ip_static/WeChatQRC.jpg' style="max-width:15rem; height:auto;"></div><div class='ch_179 ch_180'>捐赠</div><div class='ch_181'><img class='ch_185' src='./ip_static/DonationQRC-0rmb.jpg' style="max-width:15rem; height:auto;"></div></div></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div></div>
 <script>
 ch.ch_1 = () => window.innerWidth > window.innerHeight
 ch.ch_2 = (ele, name, value) => {
             ele.setAttribute(name, value)
             ele[name] = value
         }
 ch.ch_3 = document.body
-ch.ch_127 = () => {
+ch.ch_130 = () => {
             let value = ch.ch_1()
             if (value)
                 { ch.ch_2(ch.ch_3, 'is_x_screen', 'True') }
             else
                 { ch.ch_2(ch.ch_3, 'is_x_screen', 'False') }
             return value
         }
-ch.ch_127()
-ch.ch_125 = document.getElementById("ch_124")
-ch.ch_132 = Array.from(ch.ch_125.querySelectorAll('.is_nav'))
-ch.ch_128 = (last_value, items) =>
+ch.ch_130()
+ch.ch_128 = document.getElementById("ch_127")
+ch.ch_135 = Array.from(ch.ch_128.querySelectorAll('.is_nav'))
+ch.ch_131 = (last_value, items) =>
             value => {
                 if (last_value.get('last_value') !== value) {
                     last_value.set('last_value', value)
                     for (let set_value of items)
                         {set_value(value)}
                 }
             }
-ch.ch_129 = new Map([["last_value", null]])
-ch.ch_131 = (navigation, navs, value) => {
+ch.ch_132 = new Map([["last_value", null]])
+ch.ch_134 = (navigation, navs, value) => {
             let index = Number(value)
             if (Number.isInteger(index))  {  // 3.0、4.0 这种格式也会表现为 True
                 let nav = navs[parseInt(index) - 1]
                 if (nav) {
                     for (let x of navs)
                         { x.setAttribute('is_current_nav', 'False') }
                     nav.setAttribute('is_current_nav', 'True')
@@ -82,176 +83,180 @@
                     if (right > 0)
                         { navigation.scrollLeft += right }
                     else if (left < 0)
                         { navigation.scrollLeft += left }
                 }
             }
         }
-ch.ch_135 = value => ch.ch_131(ch.ch_125, ch.ch_132, value)
-ch.ch_4 = (ele, scrollLeft, seconds=0, callback=null) => {
+ch.ch_138 = value => ch.ch_134(ch.ch_128, ch.ch_135, value)
+ch.ch_4 = async (ele, scrollLeft, seconds=0) => {
             if (seconds) {
                 let start_time = performance.now()  // 立即获取当前时间，以尽可能让时间准确
+                ele.classList.add('ch_exec_smooth_to_scrollLeft')  // 立即设为 ch_exec_smooth_to_scrollLeft
                 let milliseconds = seconds * 1000
                 let end_time = start_time + milliseconds
                 let start_scrollLeft = ele.scrollLeft
                 let distance = scrollLeft - start_scrollLeft
                 let gradient = distance / milliseconds  // 斜率
-                ele.classList.add('ch_exec_smooth_to_scrollLeft')
+                let state = {'finished': false}
                 let scroll = () => {
                     let current_time = performance.now()
-                    if (current_time < end_time) {
+                    if (current_time < end_time)
                         ele.scrollLeft = gradient * (current_time - start_time) + start_scrollLeft  // y = k*x + b
-                        requestAnimationFrame(scroll)  // requestAnimationFrame 和 setTimeout 都可用于延迟运行，但前者是专为动画设计的
-                    }
-                    else {
-                        ele.classList.remove('ch_exec_smooth_to_scrollLeft')
-                        ele.scrollLeft = scrollLeft  // 两个功能：确保最终位置正确、激活同步
-                        if (callback) callback()
-                    }
+                    else
+                        state['finished'] = true
                 }
-                scroll()
+                while (true) {
+                    await new Promise(resolve => requestAnimationFrame(() => {scroll(); resolve()}))  // 在这一步会释放事件循环的loop
+                    // requestAnimationFrame 和 setTimeout 都可用于延迟运行。但前者是专为动画设计的，会在浏览器下一次重绘前被执行
+                    if (state['finished']) break
+                }
+                ele.classList.remove('ch_exec_smooth_to_scrollLeft')
+                ele.scrollLeft = scrollLeft  // 两个功能：确保最终位置正确、激活同步
             }
             else
                 ele.scrollLeft = scrollLeft
         }
-ch.ch_136 = (pages_box, current_index, scroll_seconds) =>
-            value => {
+ch.ch_139 = (pages_box, current_index, scroll_seconds) =>
+            async value => {
                 let index = Number(value)
                 if (Number.isInteger(index))  {  // 3.0、4.0 这种格式也会表现为 True
                     index = parseInt(index)  // 转化为 3、4 这种真正的整数
                     if ( index !== current_index.get('current_index') ) {
                         let page = pages_box.children[index - 1]
                         if (page) {
                             current_index.set('current_index', index)
                             if (scroll_seconds)
-                                ch.ch_4(pages_box, page.offsetLeft, scroll_seconds)
+                                await ch.ch_4(pages_box, page.offsetLeft, scroll_seconds)
                             else
                                 pages_box.scrollLeft = page.offsetLeft
                         }
                     }
                 }
             }
-ch.ch_138 = document.getElementById("ch_137")
-ch.ch_139 = new Map([["current_index", null]])
-ch.ch_141 = ch.ch_136(ch.ch_138, ch.ch_139, 0.2)
-ch.ch_142 = (ele, set_dict, value) => {
+ch.ch_141 = document.getElementById("ch_140")
+ch.ch_142 = new Map([["current_index", null]])
+ch.ch_144 = ch.ch_139(ch.ch_141, ch.ch_142, 0.2)
+ch.ch_145 = (ele, set_dict, value) => {
             value = set_dict.has(value) ? set_dict.get(value) : value
             ele.firstChild.textContent = value
         }
-ch.ch_144 = document.getElementById("ch_143")
-ch.ch_145 = new Map([["1", "动态"], ["2", "视频"], ["3", "文章"], ["4", "想法"], ["5", "软件"], ["6", "Python教程"], ["7", "生活"], ["8", "自述"]])
-ch.ch_147 = value => ch.ch_142(ch.ch_144, ch.ch_145, value)
-ch.ch_130 = [ch.ch_135, ch.ch_141, ch.ch_147]
-ch.ch_133 = ch.ch_128(ch.ch_129, ch.ch_130)
-ch.ch_134 = (navigation, navs, sync_value) => {
+ch.ch_147 = document.getElementById("ch_146")
+ch.ch_148 = new Map([["1", "动态"], ["2", "视频"], ["3", "文章"], ["4", "想法"], ["5", "软件"], ["6", "Python教程"], ["7", "生活"], ["8", "自述"]])
+ch.ch_150 = value => ch.ch_145(ch.ch_147, ch.ch_148, value)
+ch.ch_133 = [ch.ch_138, ch.ch_144, ch.ch_150]
+ch.ch_136 = ch.ch_131(ch.ch_132, ch.ch_133)
+ch.ch_137 = (navigation, navs, sync_value) => {
             navigation.addEventListener('click',
                 () => {
                     let nav = event.target
                     if (nav.classList.contains('is_nav'))
                         {sync_value(String( navs.indexOf(nav)+1 ))}
                 }
             )
         }
-ch.ch_134(ch.ch_125, ch.ch_132, ch.ch_133)
-ch.ch_140 = (pages_box, current_index, sync_value) => {
+ch.ch_137(ch.ch_128, ch.ch_135, ch.ch_136)
+ch.ch_143 = (pages_box, current_index, sync_value) => {
             pages_box.addEventListener('scroll',
                 () => {
                     if (! pages_box.classList.contains('ch_exec_smooth_to_scrollLeft')) {
                         let index = Math.round(pages_box.scrollLeft / pages_box.clientWidth) + 1
                         if (index !== current_index.get('current_index')) {
                             current_index.set('current_index', index)
                             sync_value( String(index) )
                         }
                     }
                 }
             )
         }
-ch.ch_140(ch.ch_138, ch.ch_139, ch.ch_133)
-ch.ch_6 = window.MutationObserver || window.WebKitMutationObserver || window.MozMutationObserver
-ch.ch_146 = (sync_value, ele, last_value, set_dict) => {
+ch.ch_143(ch.ch_141, ch.ch_142, ch.ch_136)
+ch.ch_5 = window.MutationObserver || window.WebKitMutationObserver || window.MozMutationObserver
+ch.ch_149 = (sync_value, ele, last_value, set_dict) => {
             let textNode = null
             let firstSon = ele.firstChild
             if (firstSon && firstSon.nodeName === '#text')
                 { textNode = firstSon }
             else {
                 textNode = document.createTextNode('')
                 if (firstSon)
                     { ele.insertBefore(textNode, firstSon) }
                 else
                     { ele.appendChild(textNode) }
             }
-            new ch.ch_6(
+            new ch.ch_5(
                 (records, _) => { sync_value(textNode.textContent) }
             ).observe(textNode, {characterData: true})
         }
-ch.ch_146(ch.ch_133, ch.ch_144, ch.ch_129, ch.ch_145)
-ch.ch_126 = (ele, px) => {
+ch.ch_149(ch.ch_136, ch.ch_147, ch.ch_132, ch.ch_148)
+ch.ch_129 = (ele, px) => {
                     ele.scrollLeft += px
                     event.preventDefault()  // 阻止其它默认行为
                 }
-ch.ch_125.addEventListener('wheel', () => {ch.ch_126(ch.ch_125, event.deltaY)})
-ch.ch_8 = document.getElementById("ch_7")
-ch.ch_11 = document.getElementById("ch_10")
-ch.ch_13 = document.getElementById("ch_12")
-ch.ch_15 = document.getElementById("ch_14")
-ch.ch_17 = document.getElementById("ch_16")
-ch.ch_19 = document.getElementById("ch_18")
-ch.ch_21 = document.getElementById("ch_20")
-ch.ch_23 = document.getElementById("ch_22")
-ch.ch_25 = document.getElementById("ch_24")
-ch.ch_27 = document.getElementById("ch_26")
-ch.ch_29 = document.getElementById("ch_28")
-ch.ch_31 = document.getElementById("ch_30")
-ch.ch_33 = document.getElementById("ch_32")
-ch.ch_35 = document.getElementById("ch_34")
-ch.ch_37 = document.getElementById("ch_36")
-ch.ch_39 = document.getElementById("ch_38")
-ch.ch_41 = document.getElementById("ch_40")
-ch.ch_43 = document.getElementById("ch_42")
-ch.ch_45 = document.getElementById("ch_44")
-ch.ch_47 = document.getElementById("ch_46")
-ch.ch_49 = document.getElementById("ch_48")
-ch.ch_51 = document.getElementById("ch_50")
-ch.ch_53 = document.getElementById("ch_52")
-ch.ch_55 = document.getElementById("ch_54")
-ch.ch_57 = document.getElementById("ch_56")
-ch.ch_59 = document.getElementById("ch_58")
-ch.ch_61 = document.getElementById("ch_60")
-ch.ch_63 = document.getElementById("ch_62")
-ch.ch_65 = document.getElementById("ch_64")
-ch.ch_67 = document.getElementById("ch_66")
-ch.ch_69 = document.getElementById("ch_68")
-ch.ch_71 = document.getElementById("ch_70")
-ch.ch_73 = document.getElementById("ch_72")
-ch.ch_75 = document.getElementById("ch_74")
-ch.ch_77 = document.getElementById("ch_76")
-ch.ch_79 = document.getElementById("ch_78")
-ch.ch_81 = document.getElementById("ch_80")
-ch.ch_83 = document.getElementById("ch_82")
-ch.ch_85 = document.getElementById("ch_84")
-ch.ch_87 = document.getElementById("ch_86")
-ch.ch_89 = document.getElementById("ch_88")
-ch.ch_91 = document.getElementById("ch_90")
-ch.ch_93 = document.getElementById("ch_92")
-ch.ch_95 = document.getElementById("ch_94")
-ch.ch_97 = document.getElementById("ch_96")
-ch.ch_99 = document.getElementById("ch_98")
-ch.ch_101 = document.getElementById("ch_100")
-ch.ch_103 = document.getElementById("ch_102")
-ch.ch_105 = document.getElementById("ch_104")
-ch.ch_107 = document.getElementById("ch_106")
-ch.ch_109 = document.getElementById("ch_108")
-ch.ch_111 = document.getElementById("ch_110")
-ch.ch_113 = document.getElementById("ch_112")
-ch.ch_115 = document.getElementById("ch_114")
-ch.ch_117 = document.getElementById("ch_116")
-ch.ch_119 = document.getElementById("ch_118")
-ch.ch_121 = document.getElementById("ch_120")
-ch.ch_123 = document.getElementById("ch_122")
-ch.ch_9 = iframe => {
+ch.ch_128.addEventListener('wheel', () => {ch.ch_129(ch.ch_128, event.deltaY)})
+ch.ch_7 = document.getElementById("ch_6")
+ch.ch_10 = document.getElementById("ch_9")
+ch.ch_12 = document.getElementById("ch_11")
+ch.ch_14 = document.getElementById("ch_13")
+ch.ch_16 = document.getElementById("ch_15")
+ch.ch_18 = document.getElementById("ch_17")
+ch.ch_20 = document.getElementById("ch_19")
+ch.ch_22 = document.getElementById("ch_21")
+ch.ch_24 = document.getElementById("ch_23")
+ch.ch_26 = document.getElementById("ch_25")
+ch.ch_28 = document.getElementById("ch_27")
+ch.ch_30 = document.getElementById("ch_29")
+ch.ch_32 = document.getElementById("ch_31")
+ch.ch_34 = document.getElementById("ch_33")
+ch.ch_36 = document.getElementById("ch_35")
+ch.ch_38 = document.getElementById("ch_37")
+ch.ch_40 = document.getElementById("ch_39")
+ch.ch_42 = document.getElementById("ch_41")
+ch.ch_44 = document.getElementById("ch_43")
+ch.ch_46 = document.getElementById("ch_45")
+ch.ch_48 = document.getElementById("ch_47")
+ch.ch_50 = document.getElementById("ch_49")
+ch.ch_52 = document.getElementById("ch_51")
+ch.ch_54 = document.getElementById("ch_53")
+ch.ch_56 = document.getElementById("ch_55")
+ch.ch_58 = document.getElementById("ch_57")
+ch.ch_60 = document.getElementById("ch_59")
+ch.ch_62 = document.getElementById("ch_61")
+ch.ch_64 = document.getElementById("ch_63")
+ch.ch_66 = document.getElementById("ch_65")
+ch.ch_68 = document.getElementById("ch_67")
+ch.ch_70 = document.getElementById("ch_69")
+ch.ch_72 = document.getElementById("ch_71")
+ch.ch_74 = document.getElementById("ch_73")
+ch.ch_76 = document.getElementById("ch_75")
+ch.ch_78 = document.getElementById("ch_77")
+ch.ch_80 = document.getElementById("ch_79")
+ch.ch_82 = document.getElementById("ch_81")
+ch.ch_84 = document.getElementById("ch_83")
+ch.ch_86 = document.getElementById("ch_85")
+ch.ch_88 = document.getElementById("ch_87")
+ch.ch_90 = document.getElementById("ch_89")
+ch.ch_92 = document.getElementById("ch_91")
+ch.ch_94 = document.getElementById("ch_93")
+ch.ch_96 = document.getElementById("ch_95")
+ch.ch_98 = document.getElementById("ch_97")
+ch.ch_100 = document.getElementById("ch_99")
+ch.ch_102 = document.getElementById("ch_101")
+ch.ch_104 = document.getElementById("ch_103")
+ch.ch_106 = document.getElementById("ch_105")
+ch.ch_108 = document.getElementById("ch_107")
+ch.ch_110 = document.getElementById("ch_109")
+ch.ch_112 = document.getElementById("ch_111")
+ch.ch_114 = document.getElementById("ch_113")
+ch.ch_116 = document.getElementById("ch_115")
+ch.ch_118 = document.getElementById("ch_117")
+ch.ch_120 = document.getElementById("ch_119")
+ch.ch_122 = document.getElementById("ch_121")
+ch.ch_124 = document.getElementById("ch_123")
+ch.ch_126 = document.getElementById("ch_125")
+ch.ch_8 = iframe => {
             let i_document = iframe.contentDocument || iframe.contentWindow.document
             try {
                 let anchor = i_document.querySelector('a[href^="https://lcctoor.github.io"]')
                 if (anchor) {anchor.parentElement.remove()}
                 for (let a of i_document.querySelectorAll('a'))
                     { a.setAttribute('target', '_blank') }
             }
@@ -271,69 +276,71 @@
                     iframe.contentWindow.removeEventListener('click', set_height)
                 }
             }
             iframe.contentWindow.addEventListener('mouseover', set_height)
             iframe.contentWindow.addEventListener('wheel', set_height)
             iframe.contentWindow.addEventListener('click', set_height)
         }
-ch.ch_107.addEventListener('load', () => {ch.ch_9(ch.ch_107)})
-ch.ch_11.addEventListener('load', () => {ch.ch_9(ch.ch_11)})
-ch.ch_15.addEventListener('load', () => {ch.ch_9(ch.ch_15)})
-ch.ch_19.addEventListener('load', () => {ch.ch_9(ch.ch_19)})
-ch.ch_23.addEventListener('load', () => {ch.ch_9(ch.ch_23)})
-ch.ch_27.addEventListener('load', () => {ch.ch_9(ch.ch_27)})
-ch.ch_31.addEventListener('load', () => {ch.ch_9(ch.ch_31)})
-ch.ch_35.addEventListener('load', () => {ch.ch_9(ch.ch_35)})
-ch.ch_39.addEventListener('load', () => {ch.ch_9(ch.ch_39)})
-ch.ch_111.addEventListener('load', () => {ch.ch_9(ch.ch_111)})
-ch.ch_43.addEventListener('load', () => {ch.ch_9(ch.ch_43)})
-ch.ch_47.addEventListener('load', () => {ch.ch_9(ch.ch_47)})
-ch.ch_51.addEventListener('load', () => {ch.ch_9(ch.ch_51)})
-ch.ch_55.addEventListener('load', () => {ch.ch_9(ch.ch_55)})
-ch.ch_59.addEventListener('load', () => {ch.ch_9(ch.ch_59)})
-ch.ch_63.addEventListener('load', () => {ch.ch_9(ch.ch_63)})
-ch.ch_67.addEventListener('load', () => {ch.ch_9(ch.ch_67)})
-ch.ch_71.addEventListener('load', () => {ch.ch_9(ch.ch_71)})
-ch.ch_75.addEventListener('load', () => {ch.ch_9(ch.ch_75)})
-ch.ch_79.addEventListener('load', () => {ch.ch_9(ch.ch_79)})
-ch.ch_83.addEventListener('load', () => {ch.ch_9(ch.ch_83)})
-ch.ch_87.addEventListener('load', () => {ch.ch_9(ch.ch_87)})
-ch.ch_91.addEventListener('load', () => {ch.ch_9(ch.ch_91)})
-ch.ch_95.addEventListener('load', () => {ch.ch_9(ch.ch_95)})
-ch.ch_99.addEventListener('load', () => {ch.ch_9(ch.ch_99)})
-ch.ch_115.addEventListener('load', () => {ch.ch_9(ch.ch_115)})
-ch.ch_103.addEventListener('load', () => {ch.ch_9(ch.ch_103)})
-ch.ch_119.addEventListener('load', () => {ch.ch_9(ch.ch_119)})
-ch.ch_123.addEventListener('load', () => {ch.ch_9(ch.ch_123)})
-ch.ch_8.addEventListener('load', () => {ch.ch_9(ch.ch_8)})
-ch.ch_13.addEventListener('load', () => {ch.ch_9(ch.ch_13)})
-ch.ch_17.addEventListener('load', () => {ch.ch_9(ch.ch_17)})
-ch.ch_21.addEventListener('load', () => {ch.ch_9(ch.ch_21)})
-ch.ch_25.addEventListener('load', () => {ch.ch_9(ch.ch_25)})
-ch.ch_29.addEventListener('load', () => {ch.ch_9(ch.ch_29)})
-ch.ch_33.addEventListener('load', () => {ch.ch_9(ch.ch_33)})
-ch.ch_37.addEventListener('load', () => {ch.ch_9(ch.ch_37)})
-ch.ch_41.addEventListener('load', () => {ch.ch_9(ch.ch_41)})
-ch.ch_45.addEventListener('load', () => {ch.ch_9(ch.ch_45)})
-ch.ch_49.addEventListener('load', () => {ch.ch_9(ch.ch_49)})
-ch.ch_53.addEventListener('load', () => {ch.ch_9(ch.ch_53)})
-ch.ch_57.addEventListener('load', () => {ch.ch_9(ch.ch_57)})
-ch.ch_61.addEventListener('load', () => {ch.ch_9(ch.ch_61)})
-ch.ch_65.addEventListener('load', () => {ch.ch_9(ch.ch_65)})
-ch.ch_69.addEventListener('load', () => {ch.ch_9(ch.ch_69)})
-ch.ch_73.addEventListener('load', () => {ch.ch_9(ch.ch_73)})
-ch.ch_77.addEventListener('load', () => {ch.ch_9(ch.ch_77)})
-ch.ch_81.addEventListener('load', () => {ch.ch_9(ch.ch_81)})
-ch.ch_85.addEventListener('load', () => {ch.ch_9(ch.ch_85)})
-ch.ch_89.addEventListener('load', () => {ch.ch_9(ch.ch_89)})
-ch.ch_93.addEventListener('load', () => {ch.ch_9(ch.ch_93)})
-ch.ch_97.addEventListener('load', () => {ch.ch_9(ch.ch_97)})
-ch.ch_101.addEventListener('load', () => {ch.ch_9(ch.ch_101)})
-ch.ch_105.addEventListener('load', () => {ch.ch_9(ch.ch_105)})
-ch.ch_109.addEventListener('load', () => {ch.ch_9(ch.ch_109)})
-ch.ch_113.addEventListener('load', () => {ch.ch_9(ch.ch_113)})
-ch.ch_117.addEventListener('load', () => {ch.ch_9(ch.ch_117)})
-ch.ch_121.addEventListener('load', () => {ch.ch_9(ch.ch_121)})
+ch.ch_10.addEventListener('load', () => {ch.ch_8(ch.ch_10)})
+ch.ch_110.addEventListener('load', () => {ch.ch_8(ch.ch_110)})
+ch.ch_14.addEventListener('load', () => {ch.ch_8(ch.ch_14)})
+ch.ch_18.addEventListener('load', () => {ch.ch_8(ch.ch_18)})
+ch.ch_22.addEventListener('load', () => {ch.ch_8(ch.ch_22)})
+ch.ch_26.addEventListener('load', () => {ch.ch_8(ch.ch_26)})
+ch.ch_30.addEventListener('load', () => {ch.ch_8(ch.ch_30)})
+ch.ch_34.addEventListener('load', () => {ch.ch_8(ch.ch_34)})
+ch.ch_38.addEventListener('load', () => {ch.ch_8(ch.ch_38)})
+ch.ch_42.addEventListener('load', () => {ch.ch_8(ch.ch_42)})
+ch.ch_114.addEventListener('load', () => {ch.ch_8(ch.ch_114)})
+ch.ch_46.addEventListener('load', () => {ch.ch_8(ch.ch_46)})
+ch.ch_50.addEventListener('load', () => {ch.ch_8(ch.ch_50)})
+ch.ch_54.addEventListener('load', () => {ch.ch_8(ch.ch_54)})
+ch.ch_58.addEventListener('load', () => {ch.ch_8(ch.ch_58)})
+ch.ch_62.addEventListener('load', () => {ch.ch_8(ch.ch_62)})
+ch.ch_66.addEventListener('load', () => {ch.ch_8(ch.ch_66)})
+ch.ch_70.addEventListener('load', () => {ch.ch_8(ch.ch_70)})
+ch.ch_74.addEventListener('load', () => {ch.ch_8(ch.ch_74)})
+ch.ch_78.addEventListener('load', () => {ch.ch_8(ch.ch_78)})
+ch.ch_82.addEventListener('load', () => {ch.ch_8(ch.ch_82)})
+ch.ch_86.addEventListener('load', () => {ch.ch_8(ch.ch_86)})
+ch.ch_90.addEventListener('load', () => {ch.ch_8(ch.ch_90)})
+ch.ch_94.addEventListener('load', () => {ch.ch_8(ch.ch_94)})
+ch.ch_98.addEventListener('load', () => {ch.ch_8(ch.ch_98)})
+ch.ch_102.addEventListener('load', () => {ch.ch_8(ch.ch_102)})
+ch.ch_118.addEventListener('load', () => {ch.ch_8(ch.ch_118)})
+ch.ch_106.addEventListener('load', () => {ch.ch_8(ch.ch_106)})
+ch.ch_122.addEventListener('load', () => {ch.ch_8(ch.ch_122)})
+ch.ch_126.addEventListener('load', () => {ch.ch_8(ch.ch_126)})
+ch.ch_7.addEventListener('load', () => {ch.ch_8(ch.ch_7)})
+ch.ch_12.addEventListener('load', () => {ch.ch_8(ch.ch_12)})
+ch.ch_16.addEventListener('load', () => {ch.ch_8(ch.ch_16)})
+ch.ch_20.addEventListener('load', () => {ch.ch_8(ch.ch_20)})
+ch.ch_24.addEventListener('load', () => {ch.ch_8(ch.ch_24)})
+ch.ch_28.addEventListener('load', () => {ch.ch_8(ch.ch_28)})
+ch.ch_32.addEventListener('load', () => {ch.ch_8(ch.ch_32)})
+ch.ch_36.addEventListener('load', () => {ch.ch_8(ch.ch_36)})
+ch.ch_40.addEventListener('load', () => {ch.ch_8(ch.ch_40)})
+ch.ch_44.addEventListener('load', () => {ch.ch_8(ch.ch_44)})
+ch.ch_48.addEventListener('load', () => {ch.ch_8(ch.ch_48)})
+ch.ch_52.addEventListener('load', () => {ch.ch_8(ch.ch_52)})
+ch.ch_56.addEventListener('load', () => {ch.ch_8(ch.ch_56)})
+ch.ch_60.addEventListener('load', () => {ch.ch_8(ch.ch_60)})
+ch.ch_64.addEventListener('load', () => {ch.ch_8(ch.ch_64)})
+ch.ch_68.addEventListener('load', () => {ch.ch_8(ch.ch_68)})
+ch.ch_72.addEventListener('load', () => {ch.ch_8(ch.ch_72)})
+ch.ch_76.addEventListener('load', () => {ch.ch_8(ch.ch_76)})
+ch.ch_80.addEventListener('load', () => {ch.ch_8(ch.ch_80)})
+ch.ch_84.addEventListener('load', () => {ch.ch_8(ch.ch_84)})
+ch.ch_88.addEventListener('load', () => {ch.ch_8(ch.ch_88)})
+ch.ch_92.addEventListener('load', () => {ch.ch_8(ch.ch_92)})
+ch.ch_96.addEventListener('load', () => {ch.ch_8(ch.ch_96)})
+ch.ch_100.addEventListener('load', () => {ch.ch_8(ch.ch_100)})
+ch.ch_104.addEventListener('load', () => {ch.ch_8(ch.ch_104)})
+ch.ch_108.addEventListener('load', () => {ch.ch_8(ch.ch_108)})
+ch.ch_112.addEventListener('load', () => {ch.ch_8(ch.ch_112)})
+ch.ch_116.addEventListener('load', () => {ch.ch_8(ch.ch_116)})
+ch.ch_120.addEventListener('load', () => {ch.ch_8(ch.ch_120)})
+ch.ch_124.addEventListener('load', () => {ch.ch_8(ch.ch_124)})
 
 </script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
 动态视频文章想法软件Python教程生活自述
+2024-04-03
+===============================================================================
 2024-03-31
 _W_e_C_h_a_t_ _A_r_t_ _M_u_s_e_u_m
 _（_微_信_艺_术_馆_）
 _2_0_2_4_-_0_3_-_3_1
 2024-03-18
 ===============================================================================
 ===============================================================================
@@ -276,14 +278,16 @@
 ******** ?小?说 // ?陆?小?凤?新?传 ********
 _燕_山_宝_藏_ _第_1_章
 _2_0_2_0_-_1_2_-_3_1
 ******** ?小?说 // ?一?念?天?堂 ********
 _被_绑_架
 _2_0_2_2_-_0_8_-_1_2
 Copyright 2018-2024 lcctoor@outlook.com
+2024-04-03
+===============================================================================
 2024-03-18
 ===============================================================================
 2024-01-25
 ===============================================================================
 2024-01-13
 ===============================================================================
 2024-01-09
```

### Comparing `arts-2024.4.1/arts/life/2018/莆田学院·毕业生留影/index.html` & `arts-2024.4.3/arts/life/2018/莆田学院·毕业生留影/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/life/2019/苏州市虎丘山/index.html` & `arts-2024.4.3/arts/life/2019/苏州市虎丘山/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/life/2022/泉州市丰泽区·雨后街道/index.html` & `arts-2024.4.3/arts/life/2022/泉州市丰泽区·雨后街道/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/life/2023/更换微信账号了/index.html` & `arts-2024.4.3/arts/life/2023/更换微信账号了/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     <meta charset='utf-8'>
     <meta content='width=device-width, initial-scale=1.0' name='viewport'>
     <link rel="stylesheet" href="https://lcctoor.github.io/arts/arts/ip_static/01/article_css.css">
     <link rel="stylesheet" href="C:/bpath/offline_files/lcctoor.github.io/arts/ip_static/01/article_css.css">
 </head>
 <body>
 <pre>
-由于一些原因，我的原微信账号已无法登录，也无法查看好友，请朋友们看到后添加我的新账号。
+由于一些原因，我的原微信账号已无法登录，也无法查看好友，请朋友们看到后添加我的新账号。有些朋友，我无法告知他们这件事情，有点遗憾。
 </pre>
     <script>
         media = ['https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg']
     </script>
     <script src="https://lcctoor.github.io/arts/arts/ip_static/01/article_js.js"></script>
     <script src="C:/bpath/offline_files/lcctoor.github.io/arts/ip_static/01/article_js.js"></script>
 </body>
```

#### html2text {}

```diff
@@ -1 +1 @@
-由于一些原因，我的原微信账号已无法登录，也无法查看好友，请朋友们看到后添加我的新账号。
+由于一些原因，我的原微信账号已无法登录，也无法查看好友，请朋友们看到后添加我的新账号。有些朋友，我无法告知他们这件事情，有点遗憾。
```

### Comparing `arts-2024.4.1/arts/life/2024/泉州市承天禅寺/index.html` & `arts-2024.4.3/arts/life/2024/泉州市承天禅寺/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/miumapp/LICENSE` & `arts-2024.4.3/arts/miumapp/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/miumapp/README.md` & `arts-2024.4.3/arts/miumapp/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/miumapp/_core.py` & `arts-2024.4.3/arts/miumapp/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/miumapp/licenses/pyppeteer/LICENSE` & `arts-2024.4.3/arts/miumapp/licenses/pyppeteer/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/miumapp/licenses/tornado/LICENSE` & `arts-2024.4.3/arts/miumapp/licenses/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/miumapp/miumapp/demo.html` & `arts-2024.4.3/arts/miumapp/miumapp/demo.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/miumapp/miumapp/demo.py` & `arts-2024.4.3/arts/miumapp/miumapp/demo.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/miumapp/pyproject.toml` & `arts-2024.4.3/arts/miumapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oodb/LICENSE` & `arts-2024.4.3/arts/oodb/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oodb/README.md` & `arts-2024.4.3/arts/oodb/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oodb/_core.py` & `arts-2024.4.3/arts/oodb/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oodb/licenses/pymongo/LICENSE` & `arts-2024.4.3/arts/oodb/licenses/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oodb/pyproject.toml` & `arts-2024.4.3/arts/oodb/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomongo/LICENSE` & `arts-2024.4.3/arts/oomongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomongo/README.md` & `arts-2024.4.3/arts/oomongo/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomongo/_core.py` & `arts-2024.4.3/arts/oomongo/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomongo/licenses/motor/LICENSE` & `arts-2024.4.3/arts/oomongo/licenses/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomongo/licenses/pymongo/LICENSE` & `arts-2024.4.3/arts/oomongo/licenses/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomongo/pyproject.toml` & `arts-2024.4.3/arts/oomongo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomysql/LICENSE` & `arts-2024.4.3/arts/oomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomysql/README.md` & `arts-2024.4.3/arts/oomysql/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomysql/_core.py` & `arts-2024.4.3/arts/oomysql/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomysql/licenses/aiomysql/LICENSE` & `arts-2024.4.3/arts/oomysql/licenses/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomysql/licenses/pymysql/LICENSE` & `arts-2024.4.3/arts/oomysql/licenses/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/oomysql/pyproject.toml` & `arts-2024.4.3/arts/oomysql/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/openai2/LICENSE` & `arts-2024.4.3/arts/openai2/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/openai2/README.md` & `arts-2024.4.3/arts/openai2/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/openai2/_core/GroupChat.py` & `arts-2024.4.3/arts/openai2/_core/GroupChat.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/openai2/_core/chat.py` & `arts-2024.4.3/arts/openai2/_core/chat.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/openai2/_core/chat_in_cmd.py` & `arts-2024.4.3/arts/openai2/_core/chat_in_cmd.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/openai2/licenses/openai/LICENSE` & `arts-2024.4.3/arts/openai2/licenses/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/openai2/pyproject.toml` & `arts-2024.4.3/arts/openai2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/skybox/README.md` & `arts-2024.4.3/arts/skybox/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/skybox/skybox/files_hashes` & `arts-2024.4.3/arts/skybox/skybox/files_hashes`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2022/现代工人的螺丝钉处境/index.html` & `arts-2024.4.3/arts/thoughts/2022/现代工人的螺丝钉处境/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html` & `arts-2024.4.3/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/专利是个公平的赛道/index.html` & `arts-2024.4.3/arts/thoughts/2023/专利是个公平的赛道/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/事情的真实性是由度的/index.html` & `arts-2024.4.3/arts/thoughts/2023/事情的真实性是由度的/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/人无法摆脱兽性/index.html` & `arts-2024.4.3/arts/thoughts/2023/人无法摆脱兽性/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/什么是极端？/index.html` & `arts-2024.4.3/arts/thoughts/2023/什么是极端？/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/保护好人/index.html` & `arts-2024.4.3/arts/thoughts/2023/保护好人/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/只筛选，不教化/index.html` & `arts-2024.4.3/arts/thoughts/2023/只筛选，不教化/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/喊高考加油是刷存在感/index.html` & `arts-2024.4.3/arts/thoughts/2023/喊高考加油是刷存在感/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html` & `arts-2024.4.3/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html` & `arts-2024.4.3/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html` & `arts-2024.4.3/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/想去国外了解自己/index.html` & `arts-2024.4.3/arts/thoughts/2023/想去国外了解自己/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/现代化的分工合作机制/index.html` & `arts-2024.4.3/arts/thoughts/2023/现代化的分工合作机制/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/用理性处理简单的事情/index.html` & `arts-2024.4.3/arts/thoughts/2023/用理性处理简单的事情/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/真正的问题无法通过花招解决/index.html` & `arts-2024.4.3/arts/thoughts/2023/真正的问题无法通过花招解决/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html` & `arts-2024.4.3/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html` & `arts-2024.4.3/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2024/不要害怕犯错/index.html` & `arts-2024.4.3/arts/thoughts/2024/不要害怕犯错/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2024/新年题诗/index.html` & `arts-2024.4.3/arts/thoughts/2024/新年题诗/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html` & `arts-2024.4.3/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2024/编程语言的进化/example.html` & `arts-2024.4.3/arts/thoughts/2024/编程语言的进化/example.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2024/编程语言的进化/index.html` & `arts-2024.4.3/arts/thoughts/2024/编程语言的进化/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html` & `arts-2024.4.3/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html` & `arts-2024.4.3/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/tutorials/600-用37行代码实现AI五子棋/README.md` & `arts-2024.4.3/arts/tutorials/600-用37行代码实现AI五子棋/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/arts/tutorials/750-正则表达式/README.md` & `arts-2024.4.3/arts/tutorials/750-正则表达式/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.1/pyproject.toml` & `arts-2024.4.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "arts"
-version = "2024.4.1"
+version = "2024.4.3"
 description = "对 Python 开发中常用功能的封装"
 dependencies = ["openai>=1.2.4", "numpy", "pymysql", "aiomysql", "pymongo", "motor", "pyppeteer>=2.0.0", "tornado"]
 
 
 requires-python = ">=3.10"
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
```

### Comparing `arts-2024.4.1/PKG-INFO` & `arts-2024.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arts
-Version: 2024.4.1
+Version: 2024.4.3
 Summary: 对 Python 开发中常用功能的封装
 Author-email: 江南雨上 <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.2.4
 Requires-Dist: numpy
 Requires-Dist: pymysql
```

