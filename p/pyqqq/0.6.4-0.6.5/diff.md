# Comparing `tmp/pyqqq-0.6.4.tar.gz` & `tmp/pyqqq-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.6.4.tar", max compression
+gzip compressed data, was "pyqqq-0.6.5.tar", max compression
```

## Comparing `pyqqq-0.6.4.tar` & `pyqqq-0.6.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      588 2024-03-27 01:29:00.427186 pyqqq-0.6.4/README.md
--rw-r--r--   0        0        0      770 2024-04-03 05:32:08.773410 pyqqq-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-27 01:29:00.428734 pyqqq-0.6.4/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681470 pyqqq-0.6.4/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-06 00:30:01.958621 pyqqq-0.6.4/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    38283 2024-04-03 05:31:36.560592 pyqqq-0.6.4/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-27 01:29:00.428888 pyqqq-0.6.4/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    23893 2024-03-21 21:27:23.752968 pyqqq-0.6.4/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-27 03:32:53.313827 pyqqq-0.6.4/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681703 pyqqq-0.6.4/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   185553 2024-03-27 01:29:00.429675 pyqqq-0.6.4/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-27 01:29:00.429820 pyqqq-0.6.4/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-06 00:30:01.960145 pyqqq-0.6.4/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    23713 2024-04-03 03:29:49.352039 pyqqq-0.6.4/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-13 01:10:46.718207 pyqqq-0.6.4/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      437 2024-03-27 01:29:00.429926 pyqqq-0.6.4/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-06 03:23:32.374681 pyqqq-0.6.4/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     4156 2024-04-02 21:29:24.457028 pyqqq-0.6.4/pyqqq/data/daily.py
--rw-r--r--   0        0        0     4732 2024-04-03 05:31:57.184605 pyqqq-0.6.4/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     7295 2024-04-03 04:32:36.601513 pyqqq-0.6.4/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     1254 2024-03-12 13:30:35.556769 pyqqq-0.6.4/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-06 03:23:38.166158 pyqqq-0.6.4/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-02 21:29:24.457837 pyqqq-0.6.4/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 13:30:35.556892 pyqqq-0.6.4/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-28 02:16:13.684707 pyqqq-0.6.4/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-27 01:29:00.430437 pyqqq-0.6.4/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-02 21:29:24.458374 pyqqq-0.6.4/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-28 02:16:13.684870 pyqqq-0.6.4/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-27 01:29:00.427186 pyqqq-0.6.5/README.md
+-rw-r--r--   0        0        0      770 2024-04-03 06:12:52.118412 pyqqq-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-27 01:29:00.428734 pyqqq-0.6.5/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681470 pyqqq-0.6.5/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-06 00:30:01.958621 pyqqq-0.6.5/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39030 2024-04-03 05:52:28.780328 pyqqq-0.6.5/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-27 01:29:00.428888 pyqqq-0.6.5/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    23893 2024-03-21 21:27:23.752968 pyqqq-0.6.5/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-27 03:32:53.313827 pyqqq-0.6.5/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681703 pyqqq-0.6.5/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187666 2024-04-03 06:12:11.736185 pyqqq-0.6.5/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-27 01:29:00.429820 pyqqq-0.6.5/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-06 00:30:01.960145 pyqqq-0.6.5/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    23713 2024-04-03 03:29:49.352039 pyqqq-0.6.5/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-13 01:10:46.718207 pyqqq-0.6.5/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      437 2024-03-27 01:29:00.429926 pyqqq-0.6.5/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:23:32.374681 pyqqq-0.6.5/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-02 21:29:24.457028 pyqqq-0.6.5/pyqqq/data/daily.py
+-rw-r--r--   0        0        0     4732 2024-04-03 05:31:57.184605 pyqqq-0.6.5/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     7295 2024-04-03 04:32:36.601513 pyqqq-0.6.5/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     1254 2024-03-12 13:30:35.556769 pyqqq-0.6.5/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:23:38.166158 pyqqq-0.6.5/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-02 21:29:24.457837 pyqqq-0.6.5/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 13:30:35.556892 pyqqq-0.6.5/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-28 02:16:13.684707 pyqqq-0.6.5/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-27 01:29:00.430437 pyqqq-0.6.5/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-02 21:29:24.458374 pyqqq-0.6.5/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-02-28 02:16:13.684870 pyqqq-0.6.5/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.5/PKG-INFO
```

### Comparing `pyqqq-0.6.4/README.md` & `pyqqq-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyproject.toml` & `pyqqq-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.6.4"
+version = "0.6.5"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.6.4/pyqqq/__init__.py` & `pyqqq-0.6.5/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.6.5/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -915,15 +915,15 @@
         self, gubun: str, jongchk: str, cts_shcode: str = "", tr_cont_key: str = ""
     ):
         """
         ([주식]시세) 관리/불성실/투자유의조회 (t1404)
 
         Args:
             gubun (str): 구분 (0:전체 1:코스피 2:코스닥)
-            jongchk (str): 종목체크 (1:투자경고 2:매매정지 3:정리매매 4:투자주의 5:투자위험 6:위험예고 7:단기과열지정 8:이상급등종목 9:상장주식수부족)
+            jongchk (str): 종목체크 (1:관리 2:불성실공시 3:투자유의 4.투자환기)
             cts_shcode (str): 연속종목코드 - 연속조회시 OutBlock의 동일필드 입력
 
         Returns:
             dict: 관리/불성실/투자유의 정보
 
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
@@ -957,14 +957,33 @@
         }
 
         return result
 
     def get_alert_stocks(
         self, gubun: str, jongchk: str, cts_shcode: str = "", tr_cont_key=""
     ):
+        """
+        ([주식]시세) 투자경고/매매정지/정리매매조회 (t1405)
+
+         Args:
+            gubun (str): 구분 (0:전체 1:코스피 2:코스닥)
+            jongchk (str): 종목체크 (1:투자경고 2:매매정지 3:정리매매 4:투자주의 5:투자위험 6:위험예고 7:단기과열지정 8:이상급등종목 9:상장주식수부족)
+            cts_shcode (str): 연속종목코드 - 연속조회시 OutBlock의 동일필드 입력
+
+        Returns:
+            dict: 투자경고/매매정지/정리매매 정보
+
+            - rsp_cd (str): 응답코드
+            - rsp_msg (str): 응답메시지
+            - tr_cont (str): 연속조회여부
+            - tr_cont_key (str): 연속조회키
+            - output1 (dict): 연속조회정보
+            - output2 (list): 종목 별 정보
+
+        """
         tr_cd = "t1405"
         req_body = {
             f"{tr_cd}InBlock": {
                 "gubun": gubun,
                 "jongchk": jongchk,
                 "cts_shcode": cts_shcode,
             }
```

### Comparing `pyqqq-0.6.4/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.6.5/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.6.5/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.6.5/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.6.5/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -2584,14 +2584,72 @@
             'msg_cd': res_body['msg_cd'],
             'msg1': res_body['msg1'],
             'output': output
         }
 
         return result
 
+    def get_income_statement(self, fid_div_cls_code: str, fid_input_iscd: str):
+        """
+        (국내주식시세) 국내주식 손익계산서[v1_국내주식-079]
+
+        Args:
+            fid_div_cls_code (str): 분류 구분 코드 (0:년 1:분기)
+            fid_input_iscd (str): 종목코드
+
+        Returns:
+            dict:
+
+            - rt_cd (str): 응답코드
+            - msg_cd (str): 메시지코드
+            - msg1 (str): 메시지
+            - output (list): 응답상세
+                - stac_yymm: 결산 년월
+                - sale_account: 매출액
+                - sale_cost: 매출 원가
+                - sale_totl_prfi: 매출 총
+                - depr_cost: 감가상각비 - 출력되지 않는 데이터(99.99 로 표시)
+                - sell_mang: 판매 및 관리비 - 출력되지 않는 데이터(99.99 로 표시)
+                - bsop_prti: 영업 이익
+                - bsop_non_ernn: 영업 외 수익 - 출력되지 않는 데이터(99.99 로 표시)
+                - bsop_non_expn: 영업 외 비용 - 출력되지 않는 데이터(99.99 로 표시)
+                - op_prfi: 경상 이익
+                - spec_prfi: 특별 이익
+                - spec_loss: 특별 손실
+                - thtr_ntin: 당기순이익
+        """
+
+        assert fid_div_cls_code in ["0", "1"]
+        assert len(fid_input_iscd) >= 6
+
+        path = "/uapi/domestic-stock/v1/finance/income-statement"
+        tr_id = "FHKST66430200"
+        params = {
+            "fid_div_cls_code": fid_div_cls_code,
+            "fid_cond_mrkt_div_code": "J",
+            "fid_input_iscd": fid_input_iscd,
+        }
+
+        res_body, _ = self._tr_request(path, tr_id, params=params)
+        output = res_body["output"]
+
+        for item in output:
+            for key in item:
+                if key != 'stac_yymm':
+                    item[key] = Decimal(item[key])
+
+        result = {
+            "rt_cd": res_body["rt_cd"],
+            "msg_cd": res_body["msg_cd"],
+            "msg1": res_body["msg1"],
+            "output": output,
+        }
+
+        return result
+
     def order_cash(self,
                     cano: str,
                     acnt_prdt_cd: str,
                     side: str,
                     pdno: str,
                     ord_dvsn: str,
                     ord_qty: int,
```

### Comparing `pyqqq-0.6.4/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.6.5/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.6.5/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.6.5/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.6.5/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/data/daily.py` & `pyqqq-0.6.5/pyqqq/data/daily.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/data/domestic.py` & `pyqqq-0.6.5/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/data/realtime.py` & `pyqqq-0.6.5/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/datatypes.py` & `pyqqq-0.6.5/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/utils/display.py` & `pyqqq-0.6.5/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/utils/kvstore.py` & `pyqqq-0.6.5/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/utils/limiter.py` & `pyqqq-0.6.5/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/utils/logger.py` & `pyqqq-0.6.5/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/utils/market_schedule.py` & `pyqqq-0.6.5/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/pyqqq/utils/retry.py` & `pyqqq-0.6.5/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.4/PKG-INFO` & `pyqqq-0.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.6.4
+Version: 0.6.5
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

