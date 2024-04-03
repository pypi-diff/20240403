# Comparing `tmp/pyqqq-0.6.3.tar.gz` & `tmp/pyqqq-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.6.3.tar", max compression
+gzip compressed data, was "pyqqq-0.6.4.tar", max compression
```

## Comparing `pyqqq-0.6.3.tar` & `pyqqq-0.6.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      588 2024-03-27 01:29:00.427186 pyqqq-0.6.3/README.md
--rw-r--r--   0        0        0      770 2024-04-03 04:05:18.294961 pyqqq-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-27 01:29:00.428734 pyqqq-0.6.3/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681470 pyqqq-0.6.3/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-06 00:30:01.958621 pyqqq-0.6.3/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    35704 2024-03-27 03:32:53.313494 pyqqq-0.6.3/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-27 01:29:00.428888 pyqqq-0.6.3/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    23893 2024-03-21 21:27:23.752968 pyqqq-0.6.3/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-27 03:32:53.313827 pyqqq-0.6.3/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681703 pyqqq-0.6.3/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   185553 2024-03-27 01:29:00.429675 pyqqq-0.6.3/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-27 01:29:00.429820 pyqqq-0.6.3/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-06 00:30:01.960145 pyqqq-0.6.3/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    23713 2024-04-03 03:29:49.352039 pyqqq-0.6.3/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-13 01:10:46.718207 pyqqq-0.6.3/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      437 2024-03-27 01:29:00.429926 pyqqq-0.6.3/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-06 03:23:32.374681 pyqqq-0.6.3/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     4156 2024-04-02 21:29:24.457028 pyqqq-0.6.3/pyqqq/data/daily.py
--rw-r--r--   0        0        0     4674 2024-03-27 01:29:00.430134 pyqqq-0.6.3/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     7226 2024-04-03 04:04:23.380482 pyqqq-0.6.3/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     1254 2024-03-12 13:30:35.556769 pyqqq-0.6.3/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-06 03:23:38.166158 pyqqq-0.6.3/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-02 21:29:24.457837 pyqqq-0.6.3/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 13:30:35.556892 pyqqq-0.6.3/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-28 02:16:13.684707 pyqqq-0.6.3/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-27 01:29:00.430437 pyqqq-0.6.3/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-02 21:29:24.458374 pyqqq-0.6.3/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-28 02:16:13.684870 pyqqq-0.6.3/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-27 01:29:00.427186 pyqqq-0.6.4/README.md
+-rw-r--r--   0        0        0      770 2024-04-03 05:32:08.773410 pyqqq-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-27 01:29:00.428734 pyqqq-0.6.4/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681470 pyqqq-0.6.4/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-06 00:30:01.958621 pyqqq-0.6.4/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    38283 2024-04-03 05:31:36.560592 pyqqq-0.6.4/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-27 01:29:00.428888 pyqqq-0.6.4/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    23893 2024-03-21 21:27:23.752968 pyqqq-0.6.4/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-27 03:32:53.313827 pyqqq-0.6.4/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681703 pyqqq-0.6.4/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   185553 2024-03-27 01:29:00.429675 pyqqq-0.6.4/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-27 01:29:00.429820 pyqqq-0.6.4/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-06 00:30:01.960145 pyqqq-0.6.4/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    23713 2024-04-03 03:29:49.352039 pyqqq-0.6.4/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-13 01:10:46.718207 pyqqq-0.6.4/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      437 2024-03-27 01:29:00.429926 pyqqq-0.6.4/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:23:32.374681 pyqqq-0.6.4/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-02 21:29:24.457028 pyqqq-0.6.4/pyqqq/data/daily.py
+-rw-r--r--   0        0        0     4732 2024-04-03 05:31:57.184605 pyqqq-0.6.4/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     7295 2024-04-03 04:32:36.601513 pyqqq-0.6.4/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     1254 2024-03-12 13:30:35.556769 pyqqq-0.6.4/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:23:38.166158 pyqqq-0.6.4/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-02 21:29:24.457837 pyqqq-0.6.4/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 13:30:35.556892 pyqqq-0.6.4/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-28 02:16:13.684707 pyqqq-0.6.4/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-27 01:29:00.430437 pyqqq-0.6.4/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-02 21:29:24.458374 pyqqq-0.6.4/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-02-28 02:16:13.684870 pyqqq-0.6.4/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.4/PKG-INFO
```

### Comparing `pyqqq-0.6.3/README.md` & `pyqqq-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyproject.toml` & `pyqqq-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.6.3"
+version = "0.6.4"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.6.3/pyqqq/__init__.py` & `pyqqq-0.6.4/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.6.4/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files 3% similar despite different names*

```diff
@@ -907,14 +907,88 @@
             "rsp_msg": res_body["rsp_msg"],
             "output1": res_body.get(f"{tr_cd}OutBlock1", []),
             "output2": res_body.get(f"{tr_cd}OutBlock2", []),
         }
 
         return result
 
+    def get_management_stocks(
+        self, gubun: str, jongchk: str, cts_shcode: str = "", tr_cont_key: str = ""
+    ):
+        """
+        ([주식]시세) 관리/불성실/투자유의조회 (t1404)
+
+        Args:
+            gubun (str): 구분 (0:전체 1:코스피 2:코스닥)
+            jongchk (str): 종목체크 (1:투자경고 2:매매정지 3:정리매매 4:투자주의 5:투자위험 6:위험예고 7:단기과열지정 8:이상급등종목 9:상장주식수부족)
+            cts_shcode (str): 연속종목코드 - 연속조회시 OutBlock의 동일필드 입력
+
+        Returns:
+            dict: 관리/불성실/투자유의 정보
+
+            - rsp_cd (str): 응답코드
+            - rsp_msg (str): 응답메시지
+            - tr_cont (str): 연속조회여부
+            - tr_cont_key (str): 연속조회키
+            - output1 (dict): 연속조회정보
+            - output2 (list): 종목 별 정보
+        """
+        tr_cd = "t1404"
+        req_body = {
+            f"{tr_cd}InBlock": {
+                "gubun": gubun,
+                "jongchk": jongchk,
+                "cts_shcode": cts_shcode,
+            }
+        }
+
+        tr_cont = "Y" if cts_shcode else "N"
+
+        res_body, _ = self._tr_request(
+            "/stock/market-data", tr_cd, tr_cont, tr_cont_key, body=req_body
+        )
+
+        result = {
+            "rsp_cd": res_body["rsp_cd"],
+            "rsp_msg": res_body["rsp_msg"],
+            "tr_cont": res_body.get("tr_cont", ""),
+            "tr_cont_key": res_body.get("tr_cont_key", ""),
+            "output1": res_body.get("t1404OutBlock", {}),
+            "output2": res_body.get("t1404OutBlock1", []),
+        }
+
+        return result
+
+    def get_alert_stocks(
+        self, gubun: str, jongchk: str, cts_shcode: str = "", tr_cont_key=""
+    ):
+        tr_cd = "t1405"
+        req_body = {
+            f"{tr_cd}InBlock": {
+                "gubun": gubun,
+                "jongchk": jongchk,
+                "cts_shcode": cts_shcode,
+            }
+        }
+        tr_cont = "Y" if cts_shcode else "N"
+        res_body, res_header = self._tr_request(
+            "/stock/market-data", tr_cd, tr_cont, tr_cont_key, body=req_body
+        )
+
+        result = {
+            "rsp_cd": res_body["rsp_cd"],
+            "rsp_msg": res_body["rsp_msg"],
+            "tr_cont": res_header.get("tr_cont", ""),
+            "tr_cont_key": res_header.get("tr_cont_key", ""),
+            "output1": res_body.get("t1405OutBlock", {}),
+            "output2": res_body.get("t1405OutBlock1", []),
+        }
+
+        return result
+
     async def listen_trade_event(
         self,
         market: str,
         asset_codes: list[str],
         stop_event: asyncio.Event = None,
     ) -> AsyncGenerator:
         """
```

### Comparing `pyqqq-0.6.3/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.6.4/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.6.4/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.6.4/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.6.4/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.6.4/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.6.4/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.6.4/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.6.4/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/data/daily.py` & `pyqqq-0.6.4/pyqqq/data/daily.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/data/domestic.py` & `pyqqq-0.6.4/pyqqq/data/domestic.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     r = _send_request("GET", url, params=params)
     if r.status_code == 404:
         return None
     else:
         _raise_for_status(r)
 
         df = pd.DataFrame(r.json())
-        df.set_index("code", inplace=True)
+        if not df.empty:
+            df.set_index("code", inplace=True)
         return df
 
 
 def get_management_stocks(date: dtm.date = None) -> pd.DataFrame | None:
     """
     관리종목을 조회합니다.
 
@@ -92,15 +93,16 @@
     r = _send_request("GET", url, params=params)
     if r.status_code == 404:
         return None
     else:
         _raise_for_status(r)
 
         df = pd.DataFrame(r.json())
-        df.set_index("code", inplace=True)
+        if not df.empty:
+            df.set_index("code", inplace=True)
         return df
 
 
 @retry(requests.HTTPError)
 def _send_request(method: str, url: str, **kwargs):
     api_key = get_api_key()
     if not api_key:
```

### Comparing `pyqqq-0.6.3/pyqqq/data/realtime.py` & `pyqqq-0.6.4/pyqqq/data/realtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         028300 2024-04-02 13:00:00  100400  100500  100300  100500    4701
         ...                    ...     ...     ...     ...     ...     ...
         002600 2024-04-02 13:00:00  171900  171900  171900  171900       1
         001725 2024-04-02 13:00:00   63400   63400   63400   63400      83
         005745 2024-04-02 13:00:00    9770    9770    9770    9770     400
         032685 2024-04-02 13:00:00   10090   10090   10090   10090      12
         003075 2024-04-02 13:00:00   13790   13790   13790   13790       1
-
         [1981 rows x 6 columns]
 
     """
     tz = pytz.timezone("Asia/Seoul")
 
     url = f"{c.PYQQQ_API_URL}/domestic-stock/ohlcv/minutes/all/{time.date()}/{time.strftime('%H%M')}"
     if include_empty:
@@ -131,35 +130,32 @@
         dict[str, pd.DataFrame]: 주식 코드를 키로 하고, 해당 주식의 일일 OHLCV 데이터가 포함된 pandas DataFrame을 값으로 하는 딕셔너리.
         각 DataFrame에는 변환된 'time' 열이 포함되어 있으며, 이는 조회된 데이터의 시간을 나타냅니다. 'code' 열은 DataFrame의 인덱스로 설정됩니다.
 
     Raises:
         requests.exceptions.RequestException: PYQQQ API로부터 데이터를 검색하는 과정에서 오류가 발생한 경우.
 
     Examples:
-
-    >> result = get_all_day_data(dtm.date(2024, 4, 2))
-    >> len(result.keys())
-    3703
-    >> print(result["069500"])
-                          time   open   high    low  close  volume
-    code
-    069500 2024-04-02 08:31:00  37975  37975  37975  37975       1
-    069500 2024-04-02 08:34:00  37975  37975  37975  37975     139
-    069500 2024-04-02 08:35:00  37975  37975  37975  37975      31
-    069500 2024-04-02 09:00:00  37950  37950  37905  37915   41852
-    069500 2024-04-02 09:01:00  37970  37990  37950  37975   34895
-    ...                    ...    ...    ...    ...    ...     ...
-    069500 2024-04-02 17:10:00  38095  38095  38095  38095    1000
-    069500 2024-04-02 17:20:00  38100  38100  38100  38100    3937
-    069500 2024-04-02 17:40:00  38100  38100  38100  38100    1015
-    069500 2024-04-02 17:50:00  38090  38090  38090  38090     145
-    069500 2024-04-02 18:00:00  38100  38100  38100  38100     510
-
-    [398 rows x 6 columns]
-
+        >>> result = get_all_day_data(dtm.date(2024, 4, 2))
+        >>> len(result.keys())
+        3703
+        >>> print(result["069500"])
+                            time   open   high    low  close  volume
+        code
+        069500 2024-04-02 08:31:00  37975  37975  37975  37975       1
+        069500 2024-04-02 08:34:00  37975  37975  37975  37975     139
+        069500 2024-04-02 08:35:00  37975  37975  37975  37975      31
+        069500 2024-04-02 09:00:00  37950  37950  37905  37915   41852
+        069500 2024-04-02 09:01:00  37970  37990  37950  37975   34895
+        ...                    ...    ...    ...    ...    ...     ...
+        069500 2024-04-02 17:10:00  38095  38095  38095  38095    1000
+        069500 2024-04-02 17:20:00  38100  38100  38100  38100    3937
+        069500 2024-04-02 17:40:00  38100  38100  38100  38100    1015
+        069500 2024-04-02 17:50:00  38090  38090  38090  38090     145
+        069500 2024-04-02 18:00:00  38100  38100  38100  38100     510
+        [398 rows x 6 columns]
     """
     assert isinstance(date, dtm.date), "date must be a datetime.date object"
     if codes:
         assert isinstance(codes, list), "codes must be a list of strings"
         assert all(
             isinstance(code, str) for code in codes
         ), "codes must be a list of strings"
```

### Comparing `pyqqq-0.6.3/pyqqq/datatypes.py` & `pyqqq-0.6.4/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/utils/display.py` & `pyqqq-0.6.4/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/utils/kvstore.py` & `pyqqq-0.6.4/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/utils/limiter.py` & `pyqqq-0.6.4/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/utils/logger.py` & `pyqqq-0.6.4/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/utils/market_schedule.py` & `pyqqq-0.6.4/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/pyqqq/utils/retry.py` & `pyqqq-0.6.4/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.3/PKG-INFO` & `pyqqq-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.6.3
+Version: 0.6.4
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

