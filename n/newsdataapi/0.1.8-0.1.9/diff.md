# Comparing `tmp/newsdataapi-0.1.8.tar.gz` & `tmp/newsdataapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newsdataapi-0.1.8.tar", last modified: Fri Aug 25 10:37:46 2023, max compression
+gzip compressed data, was "newsdataapi-0.1.9.tar", last modified: Wed Dec  6 08:08:56 2023, max compression
```

## Comparing `newsdataapi-0.1.8.tar` & `newsdataapi-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 10:37:46.107046 newsdataapi-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-08-25 10:37:46.107046 newsdataapi-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 10:37:46.103047 newsdataapi-0.1.8/newsdataapi/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/newsdataapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/newsdataapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/newsdataapi/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/newsdataapi/newsdataapi_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/newsdataapi/newsdataapi_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/newsdataapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 10:37:46.103047 newsdataapi-0.1.8/newsdataapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-08-25 10:37:45.000000 newsdataapi-0.1.8/newsdataapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-25 10:37:46.000000 newsdataapi-0.1.8/newsdataapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-25 10:37:45.000000 newsdataapi-0.1.8/newsdataapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-25 10:37:45.000000 newsdataapi-0.1.8/newsdataapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-25 10:37:45.000000 newsdataapi-0.1.8/newsdataapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-25 10:37:46.107046 newsdataapi-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-25 10:37:46.103047 newsdataapi-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-25 10:37:31.000000 newsdataapi-0.1.8/tests/test_newsdataapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:08:56.400593 newsdataapi-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2023-12-06 08:08:56.400593 newsdataapi-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:08:56.396593 newsdataapi-0.1.9/newsdataapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/newsdataapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/newsdataapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/newsdataapi/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/newsdataapi/newsdataapi_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/newsdataapi/newsdataapi_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/newsdataapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:08:56.396593 newsdataapi-0.1.9/newsdataapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2023-12-06 08:08:56.000000 newsdataapi-0.1.9/newsdataapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-06 08:08:56.000000 newsdataapi-0.1.9/newsdataapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 08:08:56.000000 newsdataapi-0.1.9/newsdataapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-06 08:08:56.000000 newsdataapi-0.1.9/newsdataapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-06 08:08:56.000000 newsdataapi-0.1.9/newsdataapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 08:08:56.400593 newsdataapi-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:08:56.400593 newsdataapi-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2023-12-06 08:08:39.000000 newsdataapi-0.1.9/tests/test_newsdataapi.py
```

### Comparing `newsdataapi-0.1.8/LICENSE` & `newsdataapi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `newsdataapi-0.1.8/PKG-INFO` & `newsdataapi-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newsdataapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python library for newsdata client-API Call
 Home-page: https://github.com/newsdataapi/python-client
 Author: NewsData.io
 Author-email: contact@newsdata.io
 License: MIT
 Description: 
         ![Alt text](https://raw.githubusercontent.com/newsdataapi/python-client/main/newsdata-logo.png)
```

### Comparing `newsdataapi-0.1.8/README.md` & `newsdataapi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `newsdataapi-0.1.8/newsdataapi/helpers.py` & `newsdataapi-0.1.9/newsdataapi/helpers.py`

 * *Files identical despite different names*

### Comparing `newsdataapi-0.1.8/newsdataapi/newsdataapi_client.py` & `newsdataapi-0.1.9/newsdataapi/newsdataapi_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.request_timeout = request_timeout
 
     def api_proxies( self, proxies:dict)->None:
         """ Configure Proxie dictionary """
         self.proxies = proxies
     
     def __validate_parms(self,param:str,value:Union[list,int,str,bool])->dict:
-        bool_params = {'full_content','image','video'}
+        bool_params = {'full_content','image','video','cryptofeeds'}
         int_params = {'size','timeframe'}
         string_params = {'q','qInTitle','country','category','language','domain','domainurl','excludedomain','timezone','page','from_date','to_date','apikey','qInMeta','prioritydomain'}
 
         if param in string_params:
             if isinstance(value,list):
                 value = ','.join(value)
             if not isinstance(value,str):
@@ -146,45 +146,45 @@
             return self.__get_feeds(url=f'{constants.NEWS_URL}?{URL_parameters_encoded}') 
 
     def archive_api(
             self, q:Optional[str]=None, qInTitle:Optional[str]=None, country:Optional[Union[str, list]]=None, category:Optional[Union[str, list]]=None,
             language:Optional[Union[str, list]]=None, domain:Optional[Union[str, list]]=None, size:Optional[int]=None,domainurl:Optional[Union[str, list]]=None,
             excludedomain:Optional[Union[str, list]]=None, timezone:Optional[str]=None, full_content:Optional[bool]=None,image:Optional[bool]=None,
             video:Optional[bool]=None,prioritydomain:Optional[str]=None, page:Optional[str]=None, scroll:Optional[bool]=False, max_result:Optional[int]=None,
-            from_date:Optional[str]=None, to_date:Optional[str]=None, qInMeta:Optional[str]=None
+            from_date:Optional[str]=None, to_date:Optional[str]=None, qInMeta:Optional[str]=None, cryptofeeds:Optional[bool]=None
     ) -> dict:
         """
         Sending GET request to the archive api
         For more information about parameters and input, Please visit our documentation page: https://newsdata.io/documentation
         """
         params = {
             'q':q,'qInTitle':qInTitle,'country':country,'category':category,'language':language,'domain':domain,'size':size,'domainurl':domainurl,'excludedomain':excludedomain,
             'timezone':timezone,'full_content':full_content,'image':image,'video':video,'prioritydomain':prioritydomain,'page':page,'from_date':from_date,'to_date':to_date,
-            'apikey':self.apikey,'qInMeta':qInMeta
+            'apikey':self.apikey,'qInMeta':qInMeta,'cryptofeeds':cryptofeeds
         }
         URL_parameters = {}
         for key,value in params.items():
             if value is not None:
                 URL_parameters.update(self.__validate_parms(param=key,value=value))
 
         URL_parameters_encoded = urlencode(URL_parameters, quote_via=quote)
         if scroll == True:
             if max_result:
                 self.max_result = max_result 
             return self.__get_feeds_all(url=f'{constants.ARCHIVE_URL}?{URL_parameters_encoded}')
         else:
             return self.__get_feeds(url=f'{constants.ARCHIVE_URL}?{URL_parameters_encoded}') 
     
-    def sources_api( self, country:Optional[str]= None, category:Optional[str]= None, language:Optional[str]= None):
+    def sources_api( self, country:Optional[str]= None, category:Optional[str]= None, language:Optional[str]= None, prioritydomain:Optional[str]= None):
         """ 
         Sending GET request to the sources api
         For more information about parameters and input, Please visit our documentation page: https://newsdata.io/documentation
         """
         URL_parameters = {}
-        params = {"apikey":self.apikey, "country":country, "category":category, "language":language}
+        params = {"apikey":self.apikey, "country":country, "category":category, "language":language, "prioritydomain":prioritydomain}
 
         URL_parameters = {}
         for key,value in params.items():
             if value is not None:
                 URL_parameters.update(self.__validate_parms(param=key,value=value))
 
         URL_parameters_encoded = urlencode(URL_parameters, quote_via=quote)
```

### Comparing `newsdataapi-0.1.8/newsdataapi.egg-info/PKG-INFO` & `newsdataapi-0.1.9/newsdataapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newsdataapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python library for newsdata client-API Call
 Home-page: https://github.com/newsdataapi/python-client
 Author: NewsData.io
 Author-email: contact@newsdata.io
 License: MIT
 Description: 
         ![Alt text](https://raw.githubusercontent.com/newsdataapi/python-client/main/newsdata-logo.png)
```

### Comparing `newsdataapi-0.1.8/setup.py` & `newsdataapi-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='newsdataapi',
-    version='0.1.8',
+    version='0.1.9',
     packages=['newsdataapi'],
     description='Python library for newsdata client-API Call',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/newsdataapi/python-client',
     author='NewsData.io',
     author_email='contact@newsdata.io',
```

### Comparing `newsdataapi-0.1.8/tests/test_newsdataapi.py` & `newsdataapi-0.1.9/tests/test_newsdataapi.py`

 * *Files identical despite different names*

