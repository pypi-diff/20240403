# Comparing `tmp/cdsclient-1.1.7-py3-none-any.whl.zip` & `tmp/cdsclient-1.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 386629 bytes, number of entries: 140
+Zip file size: 386628 bytes, number of entries: 140
 -rw-r--r--  2.0 unx     1523 b- defN 20-Feb-02 00:00 cdsclient/LICENSE.txt
 -rw-r--r--  2.0 unx       62 b- defN 20-Feb-02 00:00 cdsclient/__init__.py
 -rwxr-xr-x  2.0 unx     9946 b- defN 20-Feb-02 00:00 cdsclient/find_2020aj_159_84b.py
 -rwxr-xr-x  2.0 unx     7100 b- defN 20-Feb-02 00:00 cdsclient/find_2mass.py
 -rwxr-xr-x  2.0 unx     9986 b- defN 20-Feb-02 00:00 cdsclient/find_2mass6x.py
 -rwxr-xr-x  2.0 unx     7074 b- defN 20-Feb-02 00:00 cdsclient/find_2psc3.py
 -rwxr-xr-x  2.0 unx    10090 b- defN 20-Feb-02 00:00 cdsclient/find_allwise.py
@@ -132,11 +132,11 @@
 -rwxr-xr-x  2.0 unx    10026 b- defN 20-Feb-02 00:00 cdsclient/find_vvv_cat_dr2.py
 -rwxr-xr-x  2.0 unx     9948 b- defN 20-Feb-02 00:00 cdsclient/find_vvv_cat_dr4.py
 -rwxr-xr-x  2.0 unx    10014 b- defN 20-Feb-02 00:00 cdsclient/find_vvv_dr1.py
 -rwxr-xr-x  2.0 unx    10086 b- defN 20-Feb-02 00:00 cdsclient/find_vvv_virac_pm_dr41.py
 -rwxr-xr-x  2.0 unx     9989 b- defN 20-Feb-02 00:00 cdsclient/find_wise_allsky.py
 -rwxr-xr-x  2.0 unx    10086 b- defN 20-Feb-02 00:00 cdsclient/find_xpm.py
 -rwxr-xr-x  2.0 unx    12716 b- defN 20-Feb-02 00:00 cdsclient/vizquery.py
-?rw-r--r--  2.0 unx     2024 b- defN 20-Feb-02 00:00 cdsclient-1.1.7.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 cdsclient-1.1.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11835 b- defN 20-Feb-02 00:00 cdsclient-1.1.7.dist-info/RECORD
-140 files, 1293417 bytes uncompressed, 368233 bytes compressed:  71.5%
+?rw-r--r--  2.0 unx     2024 b- defN 20-Feb-02 00:00 cdsclient-1.1.8.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 cdsclient-1.1.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11835 b- defN 20-Feb-02 00:00 cdsclient-1.1.8.dist-info/RECORD
+140 files, 1293417 bytes uncompressed, 368232 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -405,17 +405,17 @@
 
 Filename: cdsclient/find_xpm.py
 Comment: 
 
 Filename: cdsclient/vizquery.py
 Comment: 
 
-Filename: cdsclient-1.1.7.dist-info/METADATA
+Filename: cdsclient-1.1.8.dist-info/METADATA
 Comment: 
 
-Filename: cdsclient-1.1.7.dist-info/WHEEL
+Filename: cdsclient-1.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: cdsclient-1.1.7.dist-info/RECORD
+Filename: cdsclient-1.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cdsclient-1.1.7.dist-info/METADATA` & `cdsclient-1.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cdsclient
-Version: 1.1.7
+Version: 1.1.8
 Summary: CDS VizieR client (query large table)
 Project-URL: repository, https://github.com/cds-astro/cds.cdsclient
 Author: Gilles Landais (CDS)
 Keywords: astronomy
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

## Comparing `cdsclient-1.1.7.dist-info/RECORD` & `cdsclient-1.1.8.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -131,10 +131,10 @@
 cdsclient/find_vvv_cat_dr2.py,sha256=wZEIbDmLQLOZQM6OEEpFiKkoiOJJOINQUV3WvLYbGQk,10026
 cdsclient/find_vvv_cat_dr4.py,sha256=bIwd3kN9g0SzXNJ1-hD8-tVkTaEkhbwi1WIinaUjfNM,9948
 cdsclient/find_vvv_dr1.py,sha256=8sf6ojjHzz0_BCK0jnP7P_YUgPF5obhwML-0QbQHAfo,10014
 cdsclient/find_vvv_virac_pm_dr41.py,sha256=nH22QOvOOKnK16raBKTcvO-GgiX038mLRyyLwHfFjKU,10086
 cdsclient/find_wise_allsky.py,sha256=igTjmnafEFphsyq-LbztdLlJfLK5__m9ofxZCrWDKeI,9989
 cdsclient/find_xpm.py,sha256=izKEtQ756VXpTeCatax3DYlCO1Ed338i4xyPHnszROk,10086
 cdsclient/vizquery.py,sha256=3YZ564Dxqf2sJ0OWjYRLXObvumQMjdqOzcFVjipjf_g,12716
-cdsclient-1.1.7.dist-info/METADATA,sha256=RPg-UU0twsufsQSACcYAZb9V_fwq9AW_SutCOru60AE,2024
-cdsclient-1.1.7.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
-cdsclient-1.1.7.dist-info/RECORD,,
+cdsclient-1.1.8.dist-info/METADATA,sha256=n6QXHSVJduU0VpGKJ9wW1fgxYIhHHi8kShOHLbWLne8,2024
+cdsclient-1.1.8.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
+cdsclient-1.1.8.dist-info/RECORD,,
```

