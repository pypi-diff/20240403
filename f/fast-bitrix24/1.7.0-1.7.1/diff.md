# Comparing `tmp/fast_bitrix24-1.7.0.tar.gz` & `tmp/fast_bitrix24-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_bitrix24-1.7.0.tar", last modified: Fri Mar 29 20:58:01 2024, max compression
+gzip compressed data, was "fast_bitrix24-1.7.1.tar", last modified: Wed Apr  3 19:42:18 2024, max compression
```

## Comparing `fast_bitrix24-1.7.0.tar` & `fast_bitrix24-1.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:58:01.332428 fast_bitrix24-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21730 2024-03-29 20:58:01.332428 fast_bitrix24-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:58:01.328428 fast_bitrix24-1.7.0/fast_bitrix24/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/bitrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/correct_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/mult_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/server_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/srh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)    13514 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/fast_bitrix24/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:58:01.332428 fast_bitrix24-1.7.0/fast_bitrix24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21730 2024-03-29 20:58:01.000000 fast_bitrix24-1.7.0/fast_bitrix24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-29 20:58:01.000000 fast_bitrix24-1.7.0/fast_bitrix24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 20:58:01.000000 fast_bitrix24-1.7.0/fast_bitrix24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-29 20:58:01.000000 fast_bitrix24-1.7.0/fast_bitrix24.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 20:58:01.000000 fast_bitrix24-1.7.0/fast_bitrix24.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 20:58:01.332428 fast_bitrix24-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:58:01.332428 fast_bitrix24-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/tests/test_server_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/tests/test_srh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/tests/test_throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-29 20:57:45.000000 fast_bitrix24-1.7.0/tests/test_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:42:18.739182 fast_bitrix24-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-04-03 19:42:18.739182 fast_bitrix24-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:42:18.735182 fast_bitrix24-1.7.1/fast_bitrix24/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/bitrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/correct_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/mult_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/server_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/srh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15253 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:42:18.739182 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-04-03 19:42:18.000000 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-03 19:42:18.000000 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:42:18.000000 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 19:42:18.000000 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 19:42:18.000000 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:42:18.739182 fast_bitrix24-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:42:18.739182 fast_bitrix24-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_server_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_srh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_warnings.py
```

### Comparing `fast_bitrix24-1.7.0/LICENSE` & `fast_bitrix24-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/PKG-INFO` & `fast_bitrix24-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_bitrix24
-Version: 1.7.0
+Version: 1.7.1
 Summary: API wrapper для быстрого получения данных от Битрикс24 через REST API. Параллельные запросы к серверу, упаковка запросов в батчи, контроль скорости запросов, есть синхронный и асинхронный клиенты.
 Home-page: https://github.com/leshchenko1979/fast_bitrix24
 Author: Alexey Leshchenko
 Author-email: leshchenko@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -71,37 +71,37 @@
 Далее в python:
 
 ```python
 from fast_bitrix24 import Bitrix
 
 # замените на ваш вебхук для доступа к Bitrix24
 webhook = "https://your_domain.bitrix24.ru/rest/1/your_code/"
-b = Bitrix(webhook)
+bx = Bitrix(webhook)
 ```
 
-Методы полученного объекта `b` в дальнейшем используются для взаимодействия с сервером Битрикс24.
+Методы полученного объекта `bx` в дальнейшем используются для взаимодействия с сервером Битрикс24.
 
 ## Примеры использования
 
 ### `get_all()`
 
 Чтобы получить полностью список сущностей, используйте метод [`get_all()`](API.md#метод-getallself-method-str-params-dict--none---list--dict):
 
 ```python
 # список лидов
-leads = b.get_all('crm.lead.list')
+leads = bx.get_all('crm.lead.list')
 ```
 
 Метод [`get_all()`](API.md#метод-getallself-method-str-params-dict--none---list--dict) возвращает список, где каждый элемент списка является словарем, описывающим одну сущность из запрошенного списка.
 
 Вы также можете использовать параметр `params`, чтобы кастомизировать запрос:
 
 ```python
 # список сделок в работе, включая пользовательские поля
-deals = b.get_all(
+deals = bx.get_all(
     'crm.deal.list',
     params={
         'select': ['*', 'UF_*'],
         'filter': {'CLOSED': 'N'}
 })
 ```
 
@@ -115,15 +115,15 @@
 {
     ID_сделки_1: [контакт_1, контакт_2, ...],
     ID_сделки_2: [контакт_1, контакт_2, ...],
     ...
 }
 '''
 
-contacts = b.get_by_ID(
+contacts = bx.get_by_ID(
     'crm.deal.contact.items.get',
     [d['ID'] for d in deals])
 ```
 Метод [`get_by_ID()`](API.md#метод-getbyidself-method-str-idlist-iterable-idfieldname-str--id-params-dict--none---dict) возвращает словарь с элементами вида `ID: result`, где `result` - ответ сервера относительно этого `ID`.
 
 ### `call()`
 Чтобы создавать, изменять или удалять список сущностей, используйте метод [`call()`](API.md#метод-callself-method-str-items-dict--iterabledict--any--none--raw-bool--false---dict--listdict--any):
@@ -136,62 +136,62 @@
         'fields': {
             'TITLE': f'{d["ID"]} - {d["TITLE"]}'
         }
     }
     for d in deals
 ]
 
-b.call('crm.deal.update', tasks)
+bx.call('crm.deal.update', tasks)
 ```
 Метод [`call()`](API.md#метод-callself-method-str-items-dict--iterabledict--any--none--raw-bool--false---dict--listdict--any) возвращает список ответов сервера по каждому элементу переданного списка.
 
 ### call(raw=True)
 Вызов `call` с парамтером `raw=True` отправляет на сервер переданные ему параметры в оригинальном, необработанном виде (пропуская упаковку в батчи), и возвращает ответ сервера без какой-либо обработки.
 
 Подобный вызов можно использовать в отладочных целях, но кроме того, придется его использовать для отправки запросов, которые:
 - в параметрах имеют `None` (None применяется для стирания значения полей, а упаковка в батчи мешает передавать `None`),
-- используют устревшие методы Битрикс24, которые принимают на вход список (см. [#157](https://github.com/leshchenko1979/fast_bitrix24/issues/157)).
+- используют устревшие методы Битрикс24, которые принимают на вход список (см. [#157](https://githubx.com/leshchenko1979/fast_bitrix24/issues/157)).
 
 
 ```python
 # стереть DESCRIPTION в лиде 123
 params = {"ID": 123, "fields": {"DESCRIPTION": None}}
-b.call('crm.lead.update', params, raw=True)
+bx.call('crm.lead.update', params, raw=True)
 
 # добавить комментарий к задаче
-b.call(
+bx.call(
     'task.commentitem.add',
     [123, {"POST_MESSAGE": "Комментарий к задаче"}],
     raw=True
 )
 ```
 
 ### `call_batch()`
 Если вы хотите вызвать пакетный метод, используйте [`call_batch()`](API.md#метод-callbatchself-params-dict---dict):
 
 ```python
-results = b.call_batch ({
+results = bx.call_batch ({
     'halt': 0,
     'cmd': {
         'deals': 'crm.deal.list', # берем список сделок
         # и берем список дел по первой из них
         'activities': 'crm.activity.list?filter[ENTITY_TYPE]=3&filter[ENTITY_ID]=$result[deals][0][ID]'
     }
 })
 
 ```
 ### Асинхронные вызовы
 Если требуется использование бибилиотеки в асинхронном коде, то вместо клиента `Bitrix()` создавайте клиент класса `BitrixAsync()`:
 ```python
 from fast_bitrix24 import BitrixAsync
-b = BitrixAsync(webhook)
+bx = BitrixAsync(webhook)
 ```
 Все методы у него - синхронные аналоги методов из `Bitrix()`, описанных выше:
 ```python
-leads = await b.get_all('crm.lead.list')
+leads = await bx.get_all('crm.lead.list')
 ```
 ## Как это работает
 1. Перед обращением к серверу во всех методах класса `Bitrix` происходит проверка корректности самых популярных параметров, передаваемых к серверу, и поднимаются исключения `TypeError` и `ValueError` при наличии ошибок.
 2. Cоздаются запросы на получение всех элементов из запрошенного списка.
 3. Созданные запросы упаковываются в батчи по 50 запросов в каждом.
 4. Полученные батчи параллельно отправляются на сервер с регулировкой скорости запросов (см. ниже "Как fast_bitrix24 регулирует скорость запросов").
 5. Ответы (содержимое поля `result`) собираются в единый плоский список и возвращаются пользователю.
@@ -235,78 +235,78 @@
 logging.getLogger('fast_bitrix24').addHandler(logging.StreamHandler())
 ```
 
 ### Я хочу добавить несколько лидов списком, но получаю ошибку сервера.
 Оберните вызов `call()` в `slow`:
 
 ```python
-with b.slow():
-    results = b.call('crm.lead.add', tasks)
+with bx.slow():
+    results = bx.call('crm.lead.add', tasks)
 ```
 
 [См. подробнее](API.md#контекстный-менеджер-slowmaxconcurrentrequests-int--1) о `slow`.
 
 ### Я хочу вызвать `call()` только один раз, а не по списку.
 Передавайте параметры запроса методу `call()`, он может делать как запросы по списку, так и единичный запрос:
 
 ```python
 method = 'crm.lead.add'
 params = {'fields': {'TITLE': 'Чпок'}}
-b.call(method, params)
+bx.call(method, params)
 ```
 Результатом будет ответ сервера по этому одному элементу.
 
 Однако, если такие вызовы делаются несколько раз, то более эффективно формировать из них список и вызывать `call()` единожды по всему списку.
 
 ### Как сортируются результаты при вызове `get_all()`?
 Пока что никак.
 
 Все обращения к серверу происходят асинхронно и список результатов отсортирован в том порядке, в котором сервер возвращал ответы. Если вам требуется сортировка, то вам нужно делать ее самостоятельно, например:
 
 ```python
-deals = b.get_all('crm.deal.list')
+deals = bx.get_all('crm.deal.list')
 deals.sort(key = lambda d: int(d['ID']))
 ```
 
 ### Я использую `get_all()` для получения всех полей всех элементов списка, но это происходит слишком долго. Как ускорить этот процесс?
 Сейчас, кода Битрикс ограничивает скорость запросов к серверу, ключевым методом ускорения остается сокращение количества информации, которую вы загружаете с сервера, и сохранение скорости скачивания в пределах, установленных Битриксом. Это может быть достигнуто за счет кэширования и сокращения количества скачиваемых полей.
 
 Нарушение политики Битриска по скорости запросов влечет за собой штрафы, поэтому мы рекомендуем соблюдать её (параметр `respect_velocity_policy=True`).
 
 ### Я получаю ошибку сертификата SSL. Что делать?
 Если вы получаете `SSLCertVerificationError` / `CERTIFICATE_VERIFY_FAILED`, попробуйте отключить верификацию сертификата SSL:
 ```python
-b = BitrixAsync(webhook, ssl=False)
+bx = BitrixAsync(webhook, ssl=False)
 ```
 
 ## Я использую вашу библиотеку из ноутбуков или из Spyder и получаю ошибки. Что делать?
 
 Ваша cреда выполнения самостоятельно управляет примитивами asyncio ([см. больше](https://stackoverflow.com/questions/56154176/runtimeerror-asyncio-run-cannot-be-called-from-a-running-event-loop-in-spyd)).
 
 Используйте асинхронный клиент. То есть, вместо кода:
 
 ```python
 from fast_bitrix24 import Bitrix
-b = Bitrix(webhook)
-leads = b.get_all('crm.lead.list')
+bx = Bitrix(webhook)
+leads = bx.get_all('crm.lead.list')
 ```
 
 используйте код:
 
 ```python
 from fast_bitrix24 import BitrixAsync
-b = BitrixAsync(webhook)
-leads = await b.get_all('crm.lead.list')
+bx = BitrixAsync(webhook)
+leads = await bx.get_all('crm.lead.list')
 ```
 
 ## У меня Энтерпрайз. Как мне настроить более высокую скорость запросов?
 
 В конструкторе указывайте параметры `request_pool_size=250` и `requests_per_second=5`:
 
 ```python
 from fast_bitrix24 import Bitrix
-b = Bitrix(webhook, request_pool_size=250, requests_per_second=5)
+bx = Bitrix(webhook, request_pool_size=250, requests_per_second=5)
 ```
 
 ## Как связаться с автором
 - telegram: https://t.me/+U7hfrV7h53bRvKAS
 - создать новый github issue: https://github.com/leshchenko1979/fast_bitrix24/issues/new
```

### Comparing `fast_bitrix24-1.7.0/README.md` & `fast_bitrix24-1.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,37 +51,37 @@
 Далее в python:
 
 ```python
 from fast_bitrix24 import Bitrix
 
 # замените на ваш вебхук для доступа к Bitrix24
 webhook = "https://your_domain.bitrix24.ru/rest/1/your_code/"
-b = Bitrix(webhook)
+bx = Bitrix(webhook)
 ```
 
-Методы полученного объекта `b` в дальнейшем используются для взаимодействия с сервером Битрикс24.
+Методы полученного объекта `bx` в дальнейшем используются для взаимодействия с сервером Битрикс24.
 
 ## Примеры использования
 
 ### `get_all()`
 
 Чтобы получить полностью список сущностей, используйте метод [`get_all()`](API.md#метод-getallself-method-str-params-dict--none---list--dict):
 
 ```python
 # список лидов
-leads = b.get_all('crm.lead.list')
+leads = bx.get_all('crm.lead.list')
 ```
 
 Метод [`get_all()`](API.md#метод-getallself-method-str-params-dict--none---list--dict) возвращает список, где каждый элемент списка является словарем, описывающим одну сущность из запрошенного списка.
 
 Вы также можете использовать параметр `params`, чтобы кастомизировать запрос:
 
 ```python
 # список сделок в работе, включая пользовательские поля
-deals = b.get_all(
+deals = bx.get_all(
     'crm.deal.list',
     params={
         'select': ['*', 'UF_*'],
         'filter': {'CLOSED': 'N'}
 })
 ```
 
@@ -95,15 +95,15 @@
 {
     ID_сделки_1: [контакт_1, контакт_2, ...],
     ID_сделки_2: [контакт_1, контакт_2, ...],
     ...
 }
 '''
 
-contacts = b.get_by_ID(
+contacts = bx.get_by_ID(
     'crm.deal.contact.items.get',
     [d['ID'] for d in deals])
 ```
 Метод [`get_by_ID()`](API.md#метод-getbyidself-method-str-idlist-iterable-idfieldname-str--id-params-dict--none---dict) возвращает словарь с элементами вида `ID: result`, где `result` - ответ сервера относительно этого `ID`.
 
 ### `call()`
 Чтобы создавать, изменять или удалять список сущностей, используйте метод [`call()`](API.md#метод-callself-method-str-items-dict--iterabledict--any--none--raw-bool--false---dict--listdict--any):
@@ -116,62 +116,62 @@
         'fields': {
             'TITLE': f'{d["ID"]} - {d["TITLE"]}'
         }
     }
     for d in deals
 ]
 
-b.call('crm.deal.update', tasks)
+bx.call('crm.deal.update', tasks)
 ```
 Метод [`call()`](API.md#метод-callself-method-str-items-dict--iterabledict--any--none--raw-bool--false---dict--listdict--any) возвращает список ответов сервера по каждому элементу переданного списка.
 
 ### call(raw=True)
 Вызов `call` с парамтером `raw=True` отправляет на сервер переданные ему параметры в оригинальном, необработанном виде (пропуская упаковку в батчи), и возвращает ответ сервера без какой-либо обработки.
 
 Подобный вызов можно использовать в отладочных целях, но кроме того, придется его использовать для отправки запросов, которые:
 - в параметрах имеют `None` (None применяется для стирания значения полей, а упаковка в батчи мешает передавать `None`),
-- используют устревшие методы Битрикс24, которые принимают на вход список (см. [#157](https://github.com/leshchenko1979/fast_bitrix24/issues/157)).
+- используют устревшие методы Битрикс24, которые принимают на вход список (см. [#157](https://githubx.com/leshchenko1979/fast_bitrix24/issues/157)).
 
 
 ```python
 # стереть DESCRIPTION в лиде 123
 params = {"ID": 123, "fields": {"DESCRIPTION": None}}
-b.call('crm.lead.update', params, raw=True)
+bx.call('crm.lead.update', params, raw=True)
 
 # добавить комментарий к задаче
-b.call(
+bx.call(
     'task.commentitem.add',
     [123, {"POST_MESSAGE": "Комментарий к задаче"}],
     raw=True
 )
 ```
 
 ### `call_batch()`
 Если вы хотите вызвать пакетный метод, используйте [`call_batch()`](API.md#метод-callbatchself-params-dict---dict):
 
 ```python
-results = b.call_batch ({
+results = bx.call_batch ({
     'halt': 0,
     'cmd': {
         'deals': 'crm.deal.list', # берем список сделок
         # и берем список дел по первой из них
         'activities': 'crm.activity.list?filter[ENTITY_TYPE]=3&filter[ENTITY_ID]=$result[deals][0][ID]'
     }
 })
 
 ```
 ### Асинхронные вызовы
 Если требуется использование бибилиотеки в асинхронном коде, то вместо клиента `Bitrix()` создавайте клиент класса `BitrixAsync()`:
 ```python
 from fast_bitrix24 import BitrixAsync
-b = BitrixAsync(webhook)
+bx = BitrixAsync(webhook)
 ```
 Все методы у него - синхронные аналоги методов из `Bitrix()`, описанных выше:
 ```python
-leads = await b.get_all('crm.lead.list')
+leads = await bx.get_all('crm.lead.list')
 ```
 ## Как это работает
 1. Перед обращением к серверу во всех методах класса `Bitrix` происходит проверка корректности самых популярных параметров, передаваемых к серверу, и поднимаются исключения `TypeError` и `ValueError` при наличии ошибок.
 2. Cоздаются запросы на получение всех элементов из запрошенного списка.
 3. Созданные запросы упаковываются в батчи по 50 запросов в каждом.
 4. Полученные батчи параллельно отправляются на сервер с регулировкой скорости запросов (см. ниже "Как fast_bitrix24 регулирует скорость запросов").
 5. Ответы (содержимое поля `result`) собираются в единый плоский список и возвращаются пользователю.
@@ -215,78 +215,78 @@
 logging.getLogger('fast_bitrix24').addHandler(logging.StreamHandler())
 ```
 
 ### Я хочу добавить несколько лидов списком, но получаю ошибку сервера.
 Оберните вызов `call()` в `slow`:
 
 ```python
-with b.slow():
-    results = b.call('crm.lead.add', tasks)
+with bx.slow():
+    results = bx.call('crm.lead.add', tasks)
 ```
 
 [См. подробнее](API.md#контекстный-менеджер-slowmaxconcurrentrequests-int--1) о `slow`.
 
 ### Я хочу вызвать `call()` только один раз, а не по списку.
 Передавайте параметры запроса методу `call()`, он может делать как запросы по списку, так и единичный запрос:
 
 ```python
 method = 'crm.lead.add'
 params = {'fields': {'TITLE': 'Чпок'}}
-b.call(method, params)
+bx.call(method, params)
 ```
 Результатом будет ответ сервера по этому одному элементу.
 
 Однако, если такие вызовы делаются несколько раз, то более эффективно формировать из них список и вызывать `call()` единожды по всему списку.
 
 ### Как сортируются результаты при вызове `get_all()`?
 Пока что никак.
 
 Все обращения к серверу происходят асинхронно и список результатов отсортирован в том порядке, в котором сервер возвращал ответы. Если вам требуется сортировка, то вам нужно делать ее самостоятельно, например:
 
 ```python
-deals = b.get_all('crm.deal.list')
+deals = bx.get_all('crm.deal.list')
 deals.sort(key = lambda d: int(d['ID']))
 ```
 
 ### Я использую `get_all()` для получения всех полей всех элементов списка, но это происходит слишком долго. Как ускорить этот процесс?
 Сейчас, кода Битрикс ограничивает скорость запросов к серверу, ключевым методом ускорения остается сокращение количества информации, которую вы загружаете с сервера, и сохранение скорости скачивания в пределах, установленных Битриксом. Это может быть достигнуто за счет кэширования и сокращения количества скачиваемых полей.
 
 Нарушение политики Битриска по скорости запросов влечет за собой штрафы, поэтому мы рекомендуем соблюдать её (параметр `respect_velocity_policy=True`).
 
 ### Я получаю ошибку сертификата SSL. Что делать?
 Если вы получаете `SSLCertVerificationError` / `CERTIFICATE_VERIFY_FAILED`, попробуйте отключить верификацию сертификата SSL:
 ```python
-b = BitrixAsync(webhook, ssl=False)
+bx = BitrixAsync(webhook, ssl=False)
 ```
 
 ## Я использую вашу библиотеку из ноутбуков или из Spyder и получаю ошибки. Что делать?
 
 Ваша cреда выполнения самостоятельно управляет примитивами asyncio ([см. больше](https://stackoverflow.com/questions/56154176/runtimeerror-asyncio-run-cannot-be-called-from-a-running-event-loop-in-spyd)).
 
 Используйте асинхронный клиент. То есть, вместо кода:
 
 ```python
 from fast_bitrix24 import Bitrix
-b = Bitrix(webhook)
-leads = b.get_all('crm.lead.list')
+bx = Bitrix(webhook)
+leads = bx.get_all('crm.lead.list')
 ```
 
 используйте код:
 
 ```python
 from fast_bitrix24 import BitrixAsync
-b = BitrixAsync(webhook)
-leads = await b.get_all('crm.lead.list')
+bx = BitrixAsync(webhook)
+leads = await bx.get_all('crm.lead.list')
 ```
 
 ## У меня Энтерпрайз. Как мне настроить более высокую скорость запросов?
 
 В конструкторе указывайте параметры `request_pool_size=250` и `requests_per_second=5`:
 
 ```python
 from fast_bitrix24 import Bitrix
-b = Bitrix(webhook, request_pool_size=250, requests_per_second=5)
+bx = Bitrix(webhook, request_pool_size=250, requests_per_second=5)
 ```
 
 ## Как связаться с автором
 - telegram: https://t.me/+U7hfrV7h53bRvKAS
 - создать новый github issue: https://github.com/leshchenko1979/fast_bitrix24/issues/new
```

### Comparing `fast_bitrix24-1.7.0/fast_bitrix24/bitrix.py` & `fast_bitrix24-1.7.1/fast_bitrix24/bitrix.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/fast_bitrix24/logger.py` & `fast_bitrix24-1.7.1/fast_bitrix24/logger.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/fast_bitrix24/mult_request.py` & `fast_bitrix24-1.7.1/fast_bitrix24/mult_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,19 +44,24 @@
         for batch in batches:
             yield ensure_future(self.srh.single_request("batch", batch))
 
     def package_batch(self, chunk):
         return {
             "halt": 0,
             "cmd": {
-                f"cmd{i:010}": f"{self.method}?{http_build_query(item)}"
+                self.batch_command_label(
+                    i, item
+                ): f"{self.method}?{http_build_query(item)}"
                 for i, item in enumerate(chunk)
             },
         }
 
+    def batch_command_label(self, i, item):
+        return f"cmd{i:010}"
+
     async def run(self) -> Union[Dict, List]:
         self.top_up_tasks()
 
         with self.get_pbar() as pbar:
             while self.tasks:
                 done, self.tasks = await wait(self.tasks, return_when=FIRST_COMPLETED)
                 extracted_len = self.process_done_tasks(done)
```

### Comparing `fast_bitrix24-1.7.0/fast_bitrix24/server_response.py` & `fast_bitrix24-1.7.1/fast_bitrix24/server_response.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/fast_bitrix24/srh.py` & `fast_bitrix24-1.7.1/fast_bitrix24/srh.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/fast_bitrix24/throttle.py` & `fast_bitrix24-1.7.1/fast_bitrix24/throttle.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/fast_bitrix24/user_request.py` & `fast_bitrix24-1.7.1/fast_bitrix24/user_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 TOP_MOST_LIBRARY_MODULES = [
     "fast_bitrix24\\bitrix",
     "fast_bitrix24\\logger",
     "fast_bitrix24/bitrix",
     "fast_bitrix24/logger",
 ]
 
+# методы, возвращающие только списки
+GET_ALL_ENDINGS = (".list", ".getlist", ".fields", ".getavaliableforpayment", ".types")
+
+# методы, возвращающие как списки, так и отдельные сущности
+AMBIGUOUS_ENDINGS = (".get", )
+
+ALL_ENDINGS = (*GET_ALL_ENDINGS, *AMBIGUOUS_ENDINGS)
 
 class UserRequestAbstract:
     @beartype
     @icontract.require(lambda method: method, "Method cannot be empty")
     def __init__(
         self,
         bitrix,
@@ -119,18 +126,19 @@
     @icontract.require(
         lambda self: not self.st_method.startswith("tasks.elapseditem."),
         "get_all() shouldn't be used with 'tasks.elapseditem.*' method group. "
         "Use call(raw=True) instead. Read more: "
         "https://github.com/leshchenko1979/fast_bitrix24/issues/199",
     )
     def check_special_limitations(self):
-        if not self.st_method.endswith((".list", ".getlist")):
+        if not self.st_method.endswith(ALL_ENDINGS):
             warnings.warn(
-                "get_all() should be used only with methods that end with '.list' or '.getlist'. "
-                "You are using '{self.st_method}'. Use get_by_ID() or call() instead.",
+                "get_all() should be used only with methods that end with "
+                f"the following: {ALL_ENDINGS}. You are using '{self.st_method}'. "
+                "Use get_by_ID() or call() instead.",
                 UserWarning,
                 stacklevel=get_warning_stack_level(TOP_MOST_LIBRARY_MODULES),
             )
 
         if self.st_params and "LIMIT" in self.st_params:
             warnings.warn(
                 "Bitrix servers don't seem to support the 'LIMIT' parameter.",
@@ -285,15 +293,21 @@
         lambda self: not self.bitrix.verbose
         or not self.ID_list
         or "__len__" in dir(self.ID_list),
         "call(): 'ID_list' should be a Sequence "
         "if a progress bar is to be displayed",
     )
     def check_special_limitations(self):
-        return True
+        if self.st_method.endswith(GET_ALL_ENDINGS):
+            warnings.warn(
+                "It's better to use get_all() with methods that end with "
+                f"the following: {GET_ALL_ENDINGS}. You are using '{self.st_method}'.",
+                UserWarning,
+                stacklevel=get_warning_stack_level(TOP_MOST_LIBRARY_MODULES),
+            )
 
     async def run(self):
 
         is_single_item = isinstance(self.item_list, dict)
         if is_single_item:
             self.item_list = [self.item_list]
 
@@ -312,21 +326,30 @@
         else:
             # бывают случаи, что возвращается список
             results = raw_results
 
         return results[0] if results and is_single_item else results
 
     def prepare_item_list(self):
-        # добавим порядковый номер
+        # При отправке батчей на сервер результаты приходят не в том порядке,
+        # в котором они отправлялись. Для того, чтобы пользователь мог понять,
+        # какой результат пришел по каждому конкретному элементу списка,
+        # переданному в call(), нужно возвращать не результаты запроса общим списком,
+        # где может быть нарушен порядок, а словарь, содержащий на результаты запроса
+        # по каждому элементу списка.
+
+        # Для этого добавляем к каждому элементу списка ключ "__order",
+        # который при извелечении результатов запросов будет возвращен пользователю
+        # как ключ словаря с результатами.
+
         self.item_list = [
             ChainMap(item, {self.ID_field_name: f"order{i:010}"})
             for i, item in enumerate(self.item_list)
         ]
 
-
 class RawCallUserRequest:
     """Отправляем на сервер один элемент, не обрабатывая его и не заворачивая в батчи.
 
     Нужно для устревших методов, которые принимают на вход список
     (https://github.com/leshchenko1979/fast_bitrix24/issues/157),
     а также для отправки на сервер значений None, которые преобразуются
     в строку при заворачивании в батч
```

### Comparing `fast_bitrix24-1.7.0/fast_bitrix24/utils.py` & `fast_bitrix24-1.7.1/fast_bitrix24/utils.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/fast_bitrix24.egg-info/PKG-INFO` & `fast_bitrix24-1.7.1/fast_bitrix24.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_bitrix24
-Version: 1.7.0
+Version: 1.7.1
 Summary: API wrapper для быстрого получения данных от Битрикс24 через REST API. Параллельные запросы к серверу, упаковка запросов в батчи, контроль скорости запросов, есть синхронный и асинхронный клиенты.
 Home-page: https://github.com/leshchenko1979/fast_bitrix24
 Author: Alexey Leshchenko
 Author-email: leshchenko@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -71,37 +71,37 @@
 Далее в python:
 
 ```python
 from fast_bitrix24 import Bitrix
 
 # замените на ваш вебхук для доступа к Bitrix24
 webhook = "https://your_domain.bitrix24.ru/rest/1/your_code/"
-b = Bitrix(webhook)
+bx = Bitrix(webhook)
 ```
 
-Методы полученного объекта `b` в дальнейшем используются для взаимодействия с сервером Битрикс24.
+Методы полученного объекта `bx` в дальнейшем используются для взаимодействия с сервером Битрикс24.
 
 ## Примеры использования
 
 ### `get_all()`
 
 Чтобы получить полностью список сущностей, используйте метод [`get_all()`](API.md#метод-getallself-method-str-params-dict--none---list--dict):
 
 ```python
 # список лидов
-leads = b.get_all('crm.lead.list')
+leads = bx.get_all('crm.lead.list')
 ```
 
 Метод [`get_all()`](API.md#метод-getallself-method-str-params-dict--none---list--dict) возвращает список, где каждый элемент списка является словарем, описывающим одну сущность из запрошенного списка.
 
 Вы также можете использовать параметр `params`, чтобы кастомизировать запрос:
 
 ```python
 # список сделок в работе, включая пользовательские поля
-deals = b.get_all(
+deals = bx.get_all(
     'crm.deal.list',
     params={
         'select': ['*', 'UF_*'],
         'filter': {'CLOSED': 'N'}
 })
 ```
 
@@ -115,15 +115,15 @@
 {
     ID_сделки_1: [контакт_1, контакт_2, ...],
     ID_сделки_2: [контакт_1, контакт_2, ...],
     ...
 }
 '''
 
-contacts = b.get_by_ID(
+contacts = bx.get_by_ID(
     'crm.deal.contact.items.get',
     [d['ID'] for d in deals])
 ```
 Метод [`get_by_ID()`](API.md#метод-getbyidself-method-str-idlist-iterable-idfieldname-str--id-params-dict--none---dict) возвращает словарь с элементами вида `ID: result`, где `result` - ответ сервера относительно этого `ID`.
 
 ### `call()`
 Чтобы создавать, изменять или удалять список сущностей, используйте метод [`call()`](API.md#метод-callself-method-str-items-dict--iterabledict--any--none--raw-bool--false---dict--listdict--any):
@@ -136,62 +136,62 @@
         'fields': {
             'TITLE': f'{d["ID"]} - {d["TITLE"]}'
         }
     }
     for d in deals
 ]
 
-b.call('crm.deal.update', tasks)
+bx.call('crm.deal.update', tasks)
 ```
 Метод [`call()`](API.md#метод-callself-method-str-items-dict--iterabledict--any--none--raw-bool--false---dict--listdict--any) возвращает список ответов сервера по каждому элементу переданного списка.
 
 ### call(raw=True)
 Вызов `call` с парамтером `raw=True` отправляет на сервер переданные ему параметры в оригинальном, необработанном виде (пропуская упаковку в батчи), и возвращает ответ сервера без какой-либо обработки.
 
 Подобный вызов можно использовать в отладочных целях, но кроме того, придется его использовать для отправки запросов, которые:
 - в параметрах имеют `None` (None применяется для стирания значения полей, а упаковка в батчи мешает передавать `None`),
-- используют устревшие методы Битрикс24, которые принимают на вход список (см. [#157](https://github.com/leshchenko1979/fast_bitrix24/issues/157)).
+- используют устревшие методы Битрикс24, которые принимают на вход список (см. [#157](https://githubx.com/leshchenko1979/fast_bitrix24/issues/157)).
 
 
 ```python
 # стереть DESCRIPTION в лиде 123
 params = {"ID": 123, "fields": {"DESCRIPTION": None}}
-b.call('crm.lead.update', params, raw=True)
+bx.call('crm.lead.update', params, raw=True)
 
 # добавить комментарий к задаче
-b.call(
+bx.call(
     'task.commentitem.add',
     [123, {"POST_MESSAGE": "Комментарий к задаче"}],
     raw=True
 )
 ```
 
 ### `call_batch()`
 Если вы хотите вызвать пакетный метод, используйте [`call_batch()`](API.md#метод-callbatchself-params-dict---dict):
 
 ```python
-results = b.call_batch ({
+results = bx.call_batch ({
     'halt': 0,
     'cmd': {
         'deals': 'crm.deal.list', # берем список сделок
         # и берем список дел по первой из них
         'activities': 'crm.activity.list?filter[ENTITY_TYPE]=3&filter[ENTITY_ID]=$result[deals][0][ID]'
     }
 })
 
 ```
 ### Асинхронные вызовы
 Если требуется использование бибилиотеки в асинхронном коде, то вместо клиента `Bitrix()` создавайте клиент класса `BitrixAsync()`:
 ```python
 from fast_bitrix24 import BitrixAsync
-b = BitrixAsync(webhook)
+bx = BitrixAsync(webhook)
 ```
 Все методы у него - синхронные аналоги методов из `Bitrix()`, описанных выше:
 ```python
-leads = await b.get_all('crm.lead.list')
+leads = await bx.get_all('crm.lead.list')
 ```
 ## Как это работает
 1. Перед обращением к серверу во всех методах класса `Bitrix` происходит проверка корректности самых популярных параметров, передаваемых к серверу, и поднимаются исключения `TypeError` и `ValueError` при наличии ошибок.
 2. Cоздаются запросы на получение всех элементов из запрошенного списка.
 3. Созданные запросы упаковываются в батчи по 50 запросов в каждом.
 4. Полученные батчи параллельно отправляются на сервер с регулировкой скорости запросов (см. ниже "Как fast_bitrix24 регулирует скорость запросов").
 5. Ответы (содержимое поля `result`) собираются в единый плоский список и возвращаются пользователю.
@@ -235,78 +235,78 @@
 logging.getLogger('fast_bitrix24').addHandler(logging.StreamHandler())
 ```
 
 ### Я хочу добавить несколько лидов списком, но получаю ошибку сервера.
 Оберните вызов `call()` в `slow`:
 
 ```python
-with b.slow():
-    results = b.call('crm.lead.add', tasks)
+with bx.slow():
+    results = bx.call('crm.lead.add', tasks)
 ```
 
 [См. подробнее](API.md#контекстный-менеджер-slowmaxconcurrentrequests-int--1) о `slow`.
 
 ### Я хочу вызвать `call()` только один раз, а не по списку.
 Передавайте параметры запроса методу `call()`, он может делать как запросы по списку, так и единичный запрос:
 
 ```python
 method = 'crm.lead.add'
 params = {'fields': {'TITLE': 'Чпок'}}
-b.call(method, params)
+bx.call(method, params)
 ```
 Результатом будет ответ сервера по этому одному элементу.
 
 Однако, если такие вызовы делаются несколько раз, то более эффективно формировать из них список и вызывать `call()` единожды по всему списку.
 
 ### Как сортируются результаты при вызове `get_all()`?
 Пока что никак.
 
 Все обращения к серверу происходят асинхронно и список результатов отсортирован в том порядке, в котором сервер возвращал ответы. Если вам требуется сортировка, то вам нужно делать ее самостоятельно, например:
 
 ```python
-deals = b.get_all('crm.deal.list')
+deals = bx.get_all('crm.deal.list')
 deals.sort(key = lambda d: int(d['ID']))
 ```
 
 ### Я использую `get_all()` для получения всех полей всех элементов списка, но это происходит слишком долго. Как ускорить этот процесс?
 Сейчас, кода Битрикс ограничивает скорость запросов к серверу, ключевым методом ускорения остается сокращение количества информации, которую вы загружаете с сервера, и сохранение скорости скачивания в пределах, установленных Битриксом. Это может быть достигнуто за счет кэширования и сокращения количества скачиваемых полей.
 
 Нарушение политики Битриска по скорости запросов влечет за собой штрафы, поэтому мы рекомендуем соблюдать её (параметр `respect_velocity_policy=True`).
 
 ### Я получаю ошибку сертификата SSL. Что делать?
 Если вы получаете `SSLCertVerificationError` / `CERTIFICATE_VERIFY_FAILED`, попробуйте отключить верификацию сертификата SSL:
 ```python
-b = BitrixAsync(webhook, ssl=False)
+bx = BitrixAsync(webhook, ssl=False)
 ```
 
 ## Я использую вашу библиотеку из ноутбуков или из Spyder и получаю ошибки. Что делать?
 
 Ваша cреда выполнения самостоятельно управляет примитивами asyncio ([см. больше](https://stackoverflow.com/questions/56154176/runtimeerror-asyncio-run-cannot-be-called-from-a-running-event-loop-in-spyd)).
 
 Используйте асинхронный клиент. То есть, вместо кода:
 
 ```python
 from fast_bitrix24 import Bitrix
-b = Bitrix(webhook)
-leads = b.get_all('crm.lead.list')
+bx = Bitrix(webhook)
+leads = bx.get_all('crm.lead.list')
 ```
 
 используйте код:
 
 ```python
 from fast_bitrix24 import BitrixAsync
-b = BitrixAsync(webhook)
-leads = await b.get_all('crm.lead.list')
+bx = BitrixAsync(webhook)
+leads = await bx.get_all('crm.lead.list')
 ```
 
 ## У меня Энтерпрайз. Как мне настроить более высокую скорость запросов?
 
 В конструкторе указывайте параметры `request_pool_size=250` и `requests_per_second=5`:
 
 ```python
 from fast_bitrix24 import Bitrix
-b = Bitrix(webhook, request_pool_size=250, requests_per_second=5)
+bx = Bitrix(webhook, request_pool_size=250, requests_per_second=5)
 ```
 
 ## Как связаться с автором
 - telegram: https://t.me/+U7hfrV7h53bRvKAS
 - создать новый github issue: https://github.com/leshchenko1979/fast_bitrix24/issues/new
```

### Comparing `fast_bitrix24-1.7.0/fast_bitrix24.egg-info/SOURCES.txt` & `fast_bitrix24-1.7.1/fast_bitrix24.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/setup.py` & `fast_bitrix24-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/tests/test_async.py` & `fast_bitrix24-1.7.1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/tests/test_exceptions.py` & `fast_bitrix24-1.7.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/tests/test_helpers.py` & `fast_bitrix24-1.7.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/tests/test_server_responses.py` & `fast_bitrix24-1.7.1/tests/test_server_responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,33 +63,40 @@
     assert isinstance(results, dict)
 
 
 def test_call_several_success(bx_dummy):
     from tests.real_responses.call_several_success import response
 
     bx_dummy.srh = MockSRH(response)
-    results = bx_dummy.call("crm.lead.get", [{"ID": 35943}, {"ID": 161}, {"ID": 171}])
+
+    ID_list = [161, 35943, 171]
+    results = bx_dummy.call("crm.lead.get", [{"ID": ID} for ID in ID_list])
+
     assert isinstance(results, tuple)
     assert len(results) == 3
     assert isinstance(results[0], dict)
 
+    # нужен какой-то другой тест для контроля порядока результатов
+    # assert [result["ID"] for result in results] == ID_list, "Incorrect order of IDs"
+
 
 def test_call_list_empty(bx_dummy):
     from tests.real_responses.batch_list_empty import response
 
     bx_dummy.srh = MockSRH(response)
     results = bx_dummy.call(
         "crm.lead.list", ({"filter": {"PHONE": "+0000877578564"}, "select": ["ID"]},)
     )
     assert isinstance(results, list)
     assert len(results) == 0
 
     bx_dummy.srh = MockSRH(response)
     results = bx_dummy.call(
-        "crm.lead.list", {"filter": {"PHONE": "+0000877578564"}, "select": ["ID"]})
+        "crm.lead.list", {"filter": {"PHONE": "+0000877578564"}, "select": ["ID"]}
+    )
     assert isinstance(results, list)
     assert len(results) == 0
 
 
 def test_get_all_non_list_method(bx_dummy, recwarn):
     from tests.real_responses.user_fields import response
 
@@ -205,14 +212,23 @@
 
     bx_dummy.srh = MockSRH(response)
     results = bx_dummy.get_all("catalog.document.element.list")
 
     assert len(results) == 95
 
 
+def test_crm_item_productrow_list(bx_dummy):
+    from tests.real_responses.crm_item_productrow_list import response
+
+    bx_dummy.srh = MockSRH(response)
+    results = bx_dummy.get_all("crm.item.productrow.list")
+
+    assert len(results) == 2
+
+
 def test_crm_stagehistory_list(bx_dummy):
     from tests.real_responses.crm_stagehistory_list import response
 
     bx_dummy.srh = MockSRH(response)
     results = bx_dummy.get_all("crm.stagehistory.list")
 
     assert len(results) == 9
```

### Comparing `fast_bitrix24-1.7.0/tests/test_srh.py` & `fast_bitrix24-1.7.1/tests/test_srh.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/tests/test_sync.py` & `fast_bitrix24-1.7.1/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/tests/test_throttle.py` & `fast_bitrix24-1.7.1/tests/test_throttle.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.0/tests/test_warnings.py` & `fast_bitrix24-1.7.1/tests/test_warnings.py`

 * *Files identical despite different names*

