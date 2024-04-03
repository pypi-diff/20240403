# Comparing `tmp/fei_crypto-0.1.4.tar.gz` & `tmp/fei_crypto-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fei_crypto-0.1.4.tar", max compression
+gzip compressed data, was "fei_crypto-0.1.5.tar", max compression
```

## Comparing `fei_crypto-0.1.4.tar` & `fei_crypto-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,51 @@
--rw-r--r--   0        0        0      140 2023-12-20 05:11:49.661668 fei_crypto-0.1.4/fei_crypto/__init__.py
--rw-r--r--   0        0        0      887 2024-03-21 05:14:18.936639 fei_crypto-0.1.4/fei_crypto/captcha.py
--rw-r--r--   0        0        0      488 2023-11-29 13:54:30.172545 fei_crypto-0.1.4/fei_crypto/crypto.py
--rw-r--r--   0        0        0     1218 2024-03-29 08:54:22.246792 fei_crypto-0.1.4/fei_crypto/discordwebhook.py
--rw-r--r--   0        0        0       79 2024-03-21 04:40:21.216364 fei_crypto-0.1.4/fei_crypto/env.py
--rw-r--r--   0        0        0      137 2023-09-26 15:21:11.446999 fei_crypto-0.1.4/fei_crypto/md5.py
--rw-r--r--   0        0        0      319 2023-09-26 14:30:44.514337 fei_crypto-0.1.4/fei_crypto/os.py
--rw-r--r--   0        0        0     1338 2023-11-29 17:18:37.219370 fei_crypto-0.1.4/fei_crypto/rmw.py
--rw-r--r--   0        0        0     1138 2023-09-28 06:14:48.561059 fei_crypto-0.1.4/fei_crypto/rnd_emoj.py
--rw-r--r--   0        0        0     2166 2024-03-29 02:58:44.194898 fei_crypto-0.1.4/fei_crypto/t2m.py
--rw-r--r--   0        0        0      369 2023-09-26 14:38:05.472651 fei_crypto-0.1.4/fei_crypto/time.py
--rw-r--r--   0        0        0     1067 2023-09-18 06:59:02.002584 fei_crypto-0.1.4/LICENSE
--rw-r--r--   0        0        0       58 2023-09-26 14:44:19.909970 fei_crypto-0.1.4/main/__init__.py
--rw-r--r--   0        0        0      120 2023-12-20 05:11:23.650909 fei_crypto-0.1.4/main/btc_eth.py
--rw-r--r--   0        0        0      137 2024-03-29 08:38:57.954290 fei_crypto-0.1.4/main/captcha.py
--rw-r--r--   0        0        0      138 2024-03-29 08:38:24.168499 fei_crypto-0.1.4/main/dc_send.py
--rw-r--r--   0        0        0      124 2023-12-20 05:11:23.620986 fei_crypto-0.1.4/main/emoj.py
--rw-r--r--   0        0        0      266 2023-12-20 05:11:23.679147 fei_crypto-0.1.4/main/env.py
--rw-r--r--   0        0        0      159 2023-12-20 05:11:54.326071 fei_crypto-0.1.4/main/main.py
--rw-r--r--   0        0        0       98 2023-12-20 05:11:23.591706 fei_crypto-0.1.4/main/os.py
--rw-r--r--   0        0        0      125 2023-12-20 05:11:23.709307 fei_crypto-0.1.4/main/rmw.py
--rw-r--r--   0        0        0       60 2023-09-26 16:09:10.583645 fei_crypto-0.1.4/main/say.py
--rw-r--r--   0        0        0      125 2024-03-28 19:31:13.343469 fei_crypto-0.1.4/main/t2m.py
--rw-r--r--   0        0        0       47 2023-11-29 14:13:02.125511 fei_crypto-0.1.4/main/tg_login.py
--rw-r--r--   0        0        0      348 2023-12-20 05:11:23.737349 fei_crypto-0.1.4/main/ts.py
--rw-r--r--   0        0        0       97 2023-09-26 16:09:52.597612 fei_crypto-0.1.4/main/uu_id.py
--rw-r--r--   0        0        0     1322 2024-04-01 02:25:55.670836 fei_crypto-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2386 2024-03-29 14:08:52.660646 fei_crypto-0.1.4/README.md
--rw-r--r--   0        0        0       80 2023-11-29 14:13:56.426212 fei_crypto-0.1.4/tg/__init__.py
--rw-r--r--   0        0        0     1694 2023-12-20 05:11:44.225236 fei_crypto-0.1.4/tg/cli.py
--rw-r--r--   0        0        0     3011 2023-09-19 10:57:34.533302 fei_crypto-0.1.4/tg/login.py
--rw-r--r--   0        0        0     3189 1970-01-01 00:00:00.000000 fei_crypto-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      140 2023-12-20 05:11:49.661668 fei_crypto-0.1.5/fei_crypto/__init__.py
+-rw-r--r--   0        0        0      887 2024-03-21 05:14:18.936639 fei_crypto-0.1.5/fei_crypto/captcha.py
+-rw-r--r--   0        0        0      488 2023-11-29 13:54:30.172545 fei_crypto-0.1.5/fei_crypto/crypto.py
+-rw-r--r--   0        0        0     1218 2024-03-29 08:54:22.246792 fei_crypto-0.1.5/fei_crypto/discordwebhook.py
+-rw-r--r--   0        0        0       79 2024-03-21 04:40:21.216364 fei_crypto-0.1.5/fei_crypto/env.py
+-rw-r--r--   0        0        0      137 2023-09-26 15:21:11.446999 fei_crypto-0.1.5/fei_crypto/md5.py
+-rw-r--r--   0        0        0      319 2023-09-26 14:30:44.514337 fei_crypto-0.1.5/fei_crypto/os.py
+-rw-r--r--   0        0        0     1338 2023-11-29 17:18:37.219370 fei_crypto-0.1.5/fei_crypto/rmw.py
+-rw-r--r--   0        0        0     1138 2023-09-28 06:14:48.561059 fei_crypto-0.1.5/fei_crypto/rnd_emoj.py
+-rw-r--r--   0        0        0     2166 2024-03-29 02:58:44.194898 fei_crypto-0.1.5/fei_crypto/t2m.py
+-rw-r--r--   0        0        0      369 2023-09-26 14:38:05.472651 fei_crypto-0.1.5/fei_crypto/time.py
+-rw-r--r--   0        0        0     1067 2023-09-18 06:59:02.002584 fei_crypto-0.1.5/LICENSE
+-rw-r--r--   0        0        0       58 2023-09-26 14:44:19.909970 fei_crypto-0.1.5/main/__init__.py
+-rw-r--r--   0        0        0      120 2023-12-20 05:11:23.650909 fei_crypto-0.1.5/main/btc_eth.py
+-rw-r--r--   0        0        0      137 2024-03-29 08:38:57.954290 fei_crypto-0.1.5/main/captcha.py
+-rw-r--r--   0        0        0      138 2024-03-29 08:38:24.168499 fei_crypto-0.1.5/main/dc_webhook_send.py
+-rw-r--r--   0        0        0      124 2023-12-20 05:11:23.620986 fei_crypto-0.1.5/main/emoj.py
+-rw-r--r--   0        0        0      266 2023-12-20 05:11:23.679147 fei_crypto-0.1.5/main/env.py
+-rw-r--r--   0        0        0      159 2023-12-20 05:11:54.326071 fei_crypto-0.1.5/main/main.py
+-rw-r--r--   0        0        0       98 2023-12-20 05:11:23.591706 fei_crypto-0.1.5/main/os.py
+-rw-r--r--   0        0        0      125 2023-12-20 05:11:23.709307 fei_crypto-0.1.5/main/rmw.py
+-rw-r--r--   0        0        0       60 2023-09-26 16:09:10.583645 fei_crypto-0.1.5/main/say.py
+-rw-r--r--   0        0        0      125 2024-03-28 19:31:13.343469 fei_crypto-0.1.5/main/t2m.py
+-rw-r--r--   0        0        0       81 2024-04-02 12:09:40.362527 fei_crypto-0.1.5/main/tg_forward.py
+-rw-r--r--   0        0        0       75 2024-04-02 12:07:53.673901 fei_crypto-0.1.5/main/tg_login.py
+-rw-r--r--   0        0        0      348 2023-12-20 05:11:23.737349 fei_crypto-0.1.5/main/ts.py
+-rw-r--r--   0        0        0       97 2023-09-26 16:09:52.597612 fei_crypto-0.1.5/main/uu_id.py
+-rw-r--r--   0        0        0     1453 2024-04-03 08:51:31.022597 fei_crypto-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3309 2024-04-03 08:49:10.430965 fei_crypto-0.1.5/README.md
+-rw-r--r--   0        0        0       56 2024-04-02 12:07:46.806912 fei_crypto-0.1.5/tg/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-02 20:14:26.971417 fei_crypto-0.1.5/tg/bot/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-03 08:01:55.185079 fei_crypto-0.1.5/tg/bot/live_bot.py
+-rw-r--r--   0        0        0     1908 2024-04-02 17:24:42.314843 fei_crypto-0.1.5/tg/bot/utils.py
+-rw-r--r--   0        0        0     3966 2024-04-03 08:28:04.109210 fei_crypto-0.1.5/tg/cli_forward.py
+-rw-r--r--   0        0        0     1665 2024-04-03 03:07:19.467042 fei_crypto-0.1.5/tg/cli_login.py
+-rw-r--r--   0        0        0     6472 2024-04-03 08:27:32.982473 fei_crypto-0.1.5/tg/config.py
+-rw-r--r--   0        0        0      338 2024-04-03 08:04:18.836132 fei_crypto-0.1.5/tg/const.py
+-rw-r--r--   0        0        0     3903 2024-04-03 08:01:55.176079 fei_crypto-0.1.5/tg/live.py
+-rw-r--r--   0        0        0     2974 2024-04-03 03:07:42.633426 fei_crypto-0.1.5/tg/login.py
+-rw-r--r--   0        0        0     2274 2024-04-03 08:01:56.268330 fei_crypto-0.1.5/tg/message.py
+-rw-r--r--   0        0        0      356 2024-04-02 17:19:01.228599 fei_crypto-0.1.5/tg/parse.py
+-rw-r--r--   0        0        0     3031 2024-04-03 08:31:15.484901 fei_crypto-0.1.5/tg/past.py
+-rw-r--r--   0        0        0     1504 2024-04-03 03:07:53.634670 fei_crypto-0.1.5/tg/plugin_models.py
+-rw-r--r--   0        0        0     2533 2024-04-03 08:01:56.261327 fei_crypto-0.1.5/tg/plugins/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-03 03:06:07.826906 fei_crypto-0.1.5/tg/plugins/caption.py
+-rw-r--r--   0        0        0     2401 2024-04-03 07:12:39.950474 fei_crypto-0.1.5/tg/plugins/filter.py
+-rw-r--r--   0        0        0      608 2024-04-03 03:06:20.136916 fei_crypto-0.1.5/tg/plugins/fmt.py
+-rw-r--r--   0        0        0      573 2024-04-03 03:05:11.028077 fei_crypto-0.1.5/tg/plugins/replace.py
+-rw-r--r--   0        0        0      905 2024-04-02 12:49:19.540873 fei_crypto-0.1.5/tg/storage.py
+-rw-r--r--   0        0        0     1779 2024-04-02 18:16:11.762778 fei_crypto-0.1.5/tg/utils.py
+-rw-r--r--   0        0        0     4301 1970-01-01 00:00:00.000000 fei_crypto-0.1.5/PKG-INFO
```

### Comparing `fei_crypto-0.1.4/fei_crypto/captcha.py` & `fei_crypto-0.1.5/fei_crypto/captcha.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.4/fei_crypto/discordwebhook.py` & `fei_crypto-0.1.5/fei_crypto/discordwebhook.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.4/fei_crypto/rmw.py` & `fei_crypto-0.1.5/fei_crypto/rmw.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.4/fei_crypto/rnd_emoj.py` & `fei_crypto-0.1.5/fei_crypto/rnd_emoj.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.4/fei_crypto/t2m.py` & `fei_crypto-0.1.5/fei_crypto/t2m.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.4/LICENSE` & `fei_crypto-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.4/pyproject.toml` & `fei_crypto-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,45 +5,51 @@
 name = "fei-crypto"
 packages = [
     { include = "fei_crypto" },
     { include = "tg" },
     { include = "main" },
 ]
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 cowsay = "^6.1"
 filestools = "^0.2.1"
 pillow = "^9.5.0"
 python = "<3.12,>=3.10"
 #python = "~3.11"
 python-dotenv = "^1.0.0"
 python-socks = { extras = ["asyncio"], version = "^2.4.3" }
 requests = { extras = ["socks"], version = "^2.31.0" }
-telethon = "^1.32.1"
+telethon = "^1.34.0"
 typer = { extras = ["all"], version = "^0.9.0" }
 manim = "^0.18.0"
 discord-webhook = "^1.3.1"
+verlat = "^0.1.0.post1"
+rich = "^13.7.1"
+ipython = "^8.23.0"
+pymongo = "^4.6.3"
+pyyaml = "^6.0.1"
 
 [tool.poetry.scripts]
 btc-eth = 'main.btc_eth:run'
 dt = 'main.ts:run'
 e = 'main.env:run'
 ms = 'main.ts:ms'
 nano = 'main.ts:nano'
 os = 'main.os:run'
 rmw = 'main.rmw:run'
 say = 'main.say:run'
-tg-login = 'main.tg_login:run'
+tgl = 'main.tg_login:run'
+tgf = 'main.tg_forward:run'
 ts = 'main.ts:sec'
 uuid = 'main.uu_id:run'
 captcha = 'main.captcha:run'
 t2m = 'main.t2m:run'
-dc-send = 'main.dc_send:run'
+dcw = 'main.dc_webhook_send:run'
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [[tool.poetry.source]]
 name = "aliyun"
```

### Comparing `fei_crypto-0.1.4/README.md` & `fei_crypto-0.1.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,71 @@
 # 项目
 
 - https://www.feicrypto.top
 - [联系方式-telegram](https://t.me/feicrypto)
+- 开发python版本:"<3.12,>=3.10"
 
 # 安装
 
 1. pipx install fei-crypto
 2. pipx upgrade fei-crypto
 
 # 命令行
 
 1. say -t 'hello world' # 打印内容
 2. os # operating system # 打印操作系统
 3. dt # 打印datetime
 4. ts # 打印timestamp
 5. ms # 打印milliseconds
 6. nano # 打印nanoseconds
-7. e # 打印环境变量 示例:`e 'PATH'`
+7. e # 打印环境变量
+    - 示例:`e 'PATH'`
     - env_name:环境变量名
     - --help:帮助
 8. uuid # 打印uuid
 9. btc-eth # 从币安获取比特币和以太坊的价格 支持socks5代理设置,设置环境变量->HTTP_PROXY=socks5h://127.0.0.1:7890
-10. rmw # 简单的去水印 示例:`rmw './1.png'`
+10. rmw # 简单的去水印
+    - 示例:`rmw './1.png'`
     - file_path:例如`./1.png`
     - --colors:取色对比次数,默认值`5`
     - --help:帮助文档
-11. tg-login # telegram bot或user获取sessionString
-12. captcha # 阿里云验证码识别 示例:`captcha 'file_abs_path' 'aliyun_ocr_appcode'`
+11. tgl # telegram login bot或user获取sessionString
+12. captcha # 阿里云验证码识别
+    - 示例:`captcha 'file_abs_path' 'aliyun_ocr_appcode'`
     - file_abs_path:图片绝对路径
     - aliyun_ocr_appcode:
       阿里云appcode [购买地址](https://market.aliyun.com/products/57124001/cmapi030368.html?spm=5176.2020520132.101.3.596972189IxPGX)
     - --pri_id:文字类型（dn：纯数字，ne：英文数字，de：纯英文）
-13. t2m # 需安装依赖`scoop install ffmpeg` 简单的文字转视频,示例:`t2m 'BTC-USDT' --out-filename btc --style 1 --preview` 
+13. t2m # 简单的文字转视频
+    - 依赖安装Ubuntu: `apt install -y gcc libpango1.0-dev pkg-config python3-dev ffmpeg`
+    - 依赖安装windows: `scoop install gcc msys2 ffmpeg`
+    - 示例:`t2m 'BTC-USDT' --out-filename btc --style 1 --preview`
     - text:文本内容,文字长度最好不要超过15个字符
     - --out_filename:输出文件名,输出目录为当前目录下的media文件夹,默认值`t2m`
     - --quality:生成媒体质量,默认`low_quality`,还可设置为`medium_quality`|`high_quality`
     - --out_format:输出格式`png`,`gif`,`mp4`,`webm`,`mov`. 默认`gif`
     - --style:动画样式,默认值`0`
     - --preview:是否生成后立即预览
     - --help:帮助文档
-14. dc-send # 使用discord webhook发送消息
-    示例:`dc-send 'https://discord.com/api/webhooks/{}' --text 'hello' --file-paths 'e:/btc.mp4,e:/pepe.mp4'`
+14. dcw # 使用discord webhook send发送消息
+    - 示例:`dc-send 'https://discord.com/api/webhooks/{}' --text 'hello' --file-paths 'e:/btc.mp4,e:/pepe.mp4'`
     - webhook_url:webhook url
     - --text:发送的文本
     - --file-paths:发送的文件路径,多个路径用逗号分隔
     - --proxy:使用代理,例如`http://127.0.0.1:7890`
     - --help:帮助文档
-
+15. tgf # 转发telegram group或channel,支持用户转发和机器人转发
+    - 用户转发需申请对应的api_id,api_hash,并使用以上`tgl`命令获取`sesssionString`,网址:`https://my.telegram.org/auth`
+    - 机器人转发直接到telegram`@BotFather` 里按流程申请Token
+    - 示例:`run tgf live -c "d:/tg.config.json"` 默认值:当前目录下的`tg.config.json`
+    - mode:`live`或者`past` live:实时转发 past:每分钟读取历史记录转发,第一次默认读取一个小时内的记录
+    - --config-path,-c: 配置文件路径,不传会在当前目录下创建`tg.config.json`,在json文件中填写配置重新运行即可
+    - --version,-v: 查看版本信息
+    - --help:帮助文档
+    
 # dev
 
 ```shell
 poetry shell
 poetry run python --version
 poetry run os
 poetry run dt
```

### Comparing `fei_crypto-0.1.4/tg/cli.py` & `fei_crypto-0.1.5/tg/cli_login.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from typing import Optional
 import typer
-from dotenv import load_dotenv
 from .login import login
 from rich import console
 
 from fei_crypto import __version__
 
-load_dotenv()
 
-app = typer.Typer(add_completion=False)
+tg_login_app = typer.Typer(add_completion=False)
 
 con = console.Console()
 
 
 def version_callback(value: bool):
     """Show current version and exit."""
 
     if value:
         con.print(__version__)
         raise typer.Exit()
 
 
-@app.command()
+@tg_login_app.command()
 def main(
         api_id: int = typer.Option(
             ...,
             "--API_ID",
             help="API ID obtained from my.telegram.org",
             # envvar="TG_LOGIN_API_ID",
             prompt="Paste your API ID (input hidden)",
```

### Comparing `fei_crypto-0.1.4/tg/login.py` & `fei_crypto-0.1.5/tg/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import os
 import sys
-from logging import warn
 
 from dotenv import load_dotenv
 from telethon.sessions import StringSession
 from telethon.sync import TelegramClient
 
 load_dotenv()
```

### Comparing `fei_crypto-0.1.4/PKG-INFO` & `fei_crypto-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,100 @@
 Metadata-Version: 2.1
 Name: fei-crypto
-Version: 0.1.4
+Version: 0.1.5
 Summary: fei crypto command utils
 License: MIT
 Author: feicrypto
 Author-email: feicrypto@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cowsay (>=6.1,<7.0)
 Requires-Dist: discord-webhook (>=1.3.1,<2.0.0)
 Requires-Dist: filestools (>=0.2.1,<0.3.0)
+Requires-Dist: ipython (>=8.23.0,<9.0.0)
 Requires-Dist: manim (>=0.18.0,<0.19.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-socks[asyncio] (>=2.4.3,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests[socks] (>=2.31.0,<3.0.0)
-Requires-Dist: telethon (>=1.32.1,<2.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: telethon (>=1.34.0,<2.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: verlat (>=0.1.0.post1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # 项目
 
 - https://www.feicrypto.top
 - [联系方式-telegram](https://t.me/feicrypto)
+- 开发python版本:"<3.12,>=3.10"
 
 # 安装
 
 1. pipx install fei-crypto
 2. pipx upgrade fei-crypto
 
 # 命令行
 
 1. say -t 'hello world' # 打印内容
 2. os # operating system # 打印操作系统
 3. dt # 打印datetime
 4. ts # 打印timestamp
 5. ms # 打印milliseconds
 6. nano # 打印nanoseconds
-7. e # 打印环境变量 示例:`e 'PATH'`
+7. e # 打印环境变量
+    - 示例:`e 'PATH'`
     - env_name:环境变量名
     - --help:帮助
 8. uuid # 打印uuid
 9. btc-eth # 从币安获取比特币和以太坊的价格 支持socks5代理设置,设置环境变量->HTTP_PROXY=socks5h://127.0.0.1:7890
-10. rmw # 简单的去水印 示例:`rmw './1.png'`
+10. rmw # 简单的去水印
+    - 示例:`rmw './1.png'`
     - file_path:例如`./1.png`
     - --colors:取色对比次数,默认值`5`
     - --help:帮助文档
-11. tg-login # telegram bot或user获取sessionString
-12. captcha # 阿里云验证码识别 示例:`captcha 'file_abs_path' 'aliyun_ocr_appcode'`
+11. tgl # telegram login bot或user获取sessionString
+12. captcha # 阿里云验证码识别
+    - 示例:`captcha 'file_abs_path' 'aliyun_ocr_appcode'`
     - file_abs_path:图片绝对路径
     - aliyun_ocr_appcode:
       阿里云appcode [购买地址](https://market.aliyun.com/products/57124001/cmapi030368.html?spm=5176.2020520132.101.3.596972189IxPGX)
     - --pri_id:文字类型（dn：纯数字，ne：英文数字，de：纯英文）
-13. t2m # 需安装依赖`scoop install ffmpeg` 简单的文字转视频,示例:`t2m 'BTC-USDT' --out-filename btc --style 1 --preview` 
+13. t2m # 简单的文字转视频
+    - 依赖安装Ubuntu: `apt install -y gcc libpango1.0-dev pkg-config python3-dev ffmpeg`
+    - 依赖安装windows: `scoop install gcc msys2 ffmpeg`
+    - 示例:`t2m 'BTC-USDT' --out-filename btc --style 1 --preview`
     - text:文本内容,文字长度最好不要超过15个字符
     - --out_filename:输出文件名,输出目录为当前目录下的media文件夹,默认值`t2m`
     - --quality:生成媒体质量,默认`low_quality`,还可设置为`medium_quality`|`high_quality`
     - --out_format:输出格式`png`,`gif`,`mp4`,`webm`,`mov`. 默认`gif`
     - --style:动画样式,默认值`0`
     - --preview:是否生成后立即预览
     - --help:帮助文档
-14. dc-send # 使用discord webhook发送消息
-    示例:`dc-send 'https://discord.com/api/webhooks/{}' --text 'hello' --file-paths 'e:/btc.mp4,e:/pepe.mp4'`
+14. dcw # 使用discord webhook send发送消息
+    - 示例:`dc-send 'https://discord.com/api/webhooks/{}' --text 'hello' --file-paths 'e:/btc.mp4,e:/pepe.mp4'`
     - webhook_url:webhook url
     - --text:发送的文本
     - --file-paths:发送的文件路径,多个路径用逗号分隔
     - --proxy:使用代理,例如`http://127.0.0.1:7890`
     - --help:帮助文档
-
+15. tgf # 转发telegram group或channel,支持用户转发和机器人转发
+    - 用户转发需申请对应的api_id,api_hash,并使用以上`tgl`命令获取`sesssionString`,网址:`https://my.telegram.org/auth`
+    - 机器人转发直接到telegram`@BotFather` 里按流程申请Token
+    - 示例:`run tgf live -c "d:/tg.config.json"` 默认值:当前目录下的`tg.config.json`
+    - mode:`live`或者`past` live:实时转发 past:每分钟读取历史记录转发,第一次默认读取一个小时内的记录
+    - --config-path,-c: 配置文件路径,不传会在当前目录下创建`tg.config.json`,在json文件中填写配置重新运行即可
+    - --version,-v: 查看版本信息
+    - --help:帮助文档
+    
 # dev
 
 ```shell
 poetry shell
 poetry run python --version
 poetry run os
 poetry run dt
```

