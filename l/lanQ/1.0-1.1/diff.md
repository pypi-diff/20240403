# Comparing `tmp/lanQ-1.0.tar.gz` & `tmp/lanQ-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanQ-1.0.tar", last modified: Mon Mar 25 07:00:26 2024, max compression
+gzip compressed data, was "lanQ-1.1.tar", last modified: Wed Apr  3 05:59:27 2024, max compression
```

## Comparing `lanQ-1.0.tar` & `lanQ-1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 07:00:26.359308 lanQ-1.0/
--rw-rw-rw-   0        0        0      192 2024-03-25 07:00:26.357313 lanQ-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6314 2024-03-18 02:40:45.000000 lanQ-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-25 07:00:26.355317 lanQ-1.0/lanQ.egg-info/
--rw-rw-rw-   0        0        0      192 2024-03-25 07:00:26.000000 lanQ-1.0/lanQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-03-25 07:00:26.000000 lanQ-1.0/lanQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 07:00:26.000000 lanQ-1.0/lanQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-25 07:00:26.000000 lanQ-1.0/lanQ.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-25 07:00:26.352327 lanQ-1.0/lanQ_rule/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:32:28.000000 lanQ-1.0/lanQ_rule/__init__.py
--rw-rw-rw-   0        0        0    11105 2024-03-25 07:00:01.000000 lanQ-1.0/lanQ_rule/common_rule.py
--rw-rw-rw-   0        0        0      868 2024-03-25 03:11:10.000000 lanQ-1.0/lanQ_rule/const.py
--rw-rw-rw-   0        0        0      982 2024-03-25 03:11:10.000000 lanQ-1.0/lanQ_rule/model_rule.py
--rw-rw-rw-   0        0        0     1106 2024-03-25 03:11:10.000000 lanQ-1.0/lanQ_rule/prompt_rule.py
--rw-rw-rw-   0        0        0       42 2024-03-25 07:00:26.359308 lanQ-1.0/setup.cfg
--rw-rw-rw-   0        0        0      405 2024-03-19 08:32:28.000000 lanQ-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:59:27.862362 lanQ-1.1/
+-rw-rw-rw-   0        0        0      192 2024-04-03 05:59:27.860368 lanQ-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7924 2024-04-03 05:56:27.000000 lanQ-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 05:59:27.859397 lanQ-1.1/lanQ.egg-info/
+-rw-rw-rw-   0        0        0      192 2024-04-03 05:59:27.000000 lanQ-1.1/lanQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-03 05:59:27.000000 lanQ-1.1/lanQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 05:59:27.000000 lanQ-1.1/lanQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 05:59:27.000000 lanQ-1.1/lanQ.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 05:59:27.857376 lanQ-1.1/lanQ_rule/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:32:28.000000 lanQ-1.1/lanQ_rule/__init__.py
+-rw-rw-rw-   0        0        0     3465 2024-04-03 05:46:02.000000 lanQ-1.1/lanQ_rule/base.py
+-rw-rw-rw-   0        0        0     7941 2024-04-03 05:50:12.000000 lanQ-1.1/lanQ_rule/common_rule.py
+-rw-rw-rw-   0        0        0      868 2024-03-25 03:11:10.000000 lanQ-1.1/lanQ_rule/const.py
+-rw-rw-rw-   0        0        0      975 2024-04-03 05:52:18.000000 lanQ-1.1/lanQ_rule/model_rule.py
+-rw-rw-rw-   0        0        0     1126 2024-04-03 05:46:02.000000 lanQ-1.1/lanQ_rule/prompt_rule.py
+-rw-rw-rw-   0        0        0       42 2024-04-03 05:59:27.863363 lanQ-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      405 2024-04-03 05:58:48.000000 lanQ-1.1/setup.py
```

### Comparing `lanQ-1.0/README.md` & `lanQ-1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,69 @@
 # lanQ
 
 Language quality evaluation tool.
 
 ## Getting started
 
-To make it easy for you to get started with GitLab, here's a list of recommended next steps.
+```
+pip install lanQ==1.0
+```
+
+## Upload 
 
-Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
+Make a .tar file for using in other project. 
+You will get a .tar file in `lanQ/dist/`
 
-## Add your files
+```
+python .\setup.py sdist
+```
 
-- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
-- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+Upload the .tar file to Internet.
 
 ```
-cd existing_repo
-git remote add origin https://gitlab.pjlab.org.cn/qa/lanq.git
-git branch -M main
-git push -uf origin main
+twine upload .\dist\lanQ-1.0.tar.gz
 ```
 
-## Integrate with your tools
+## Summary of Quality Functions
+
+Arrange in alphabetical order.
 
-- [ ] [Set up project integrations](http://gitlab.pjlab.org.cn/qa/lanq/-/settings/integrations)
+Function Name | Description                                             | Category | Version
+-|---------------------------------------------------------|----------|-
+common_bracket_unmatch | check whether bracket is matches                        | common   | 1.0
+common_chaos_en | check whether content has English messy code            | common   | 1.0
+common_chaos_symbol | check whether content has a lot of meaningless words    | common   | 1.0
+common_chaos_zh | check whether content has Chinese messy code            | common   | 1.0
+common_colon_end | check whether the last char is ':'                      | common   | 1.0
+common_content_null | check whether content is null | common   | 1.0
+common_doc_repeat | check whether content repeats                           | common   | 1.0
+common_enter_continuous | check whether content has more than 8 continious enter | common   | 1.0
+common_enter_more | check whether enter / content is more than 25% | common   | 1.0
+common_language_mixed | check whether content is mixed in Chinese and English   | common   | 1.0
+common_no_punc | check whether content has paragraph without punctuations | common   | 1.0
+common_space_more | check whether content has more than 500 space | common   | 1.0
+common_special_character | check whether special char in content, such as '�'      | common   | 1.0
+common_url_only | check whether content is all urls | common   | 1.0
+common_word_stuck | check whether words are stuck | common   | 1.0
+model_advertisement | check whether content has model advertisement | model    | 1.0
+model_watermark | check whether content has watermark | model    | 1.0
+prompt_chinese_produce_english | check whether chinese prompt produce english prediction | prompt   | 1.0
+prompt_english_produce_chinese | check whether english prompt produce chinese prediction | prompt   | 1.0
+
+## Release Notes
+ - 1.1:
+   - 新增 base.py 抽取基础功能;
+   - functions 按字母顺序排列
+ - 1.0:   
+   - 新增 1.0 functions;  
+   - 新增 common_rule 模块;  
+   - 新增 model_rule 模块;  
+   - 新增 prompt_rule 模块;  
+   - 新增 convert 功能;
+   - 新增 main.py 支持本质运行。
 
 ## Collaborate with your team
 
 - [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
 - [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
 - [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
 - [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lanQ-1.0/lanQ_rule/const.py` & `lanQ-1.1/lanQ_rule/const.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.0/lanQ_rule/model_rule.py` & `lanQ-1.1/lanQ_rule/model_rule.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import re
 import os
 import sys
 
 sys.path.append(os.path.dirname(__file__))
 
+from base import *
 from const import *
-from common_rule import *
-
-def model_watermark(content: str) -> dict:
-    """检查content内是否有水印."""
-    res = {'error_status': False}
-    watermark_list = ['仩嗨亾笁潪能', '上s海h人r工g智z能n实s验y室s']
-    matches = re.findall('|'.join(watermark_list), content)
-    if matches:
-        res["error_status"] = True
-        res["error_type"] = ERROR_WATERMARK
-        res['error_reason'] = '存在水印'
-    return res
 
 def model_advertisement(content: str) -> dict:
     """检查content内是否有广告."""
     res = {'error_status': False}
     ad_list_en = ['deadlinesOrder', 'Kindly click on ORDER NOW to receive an']
     matches = re.findall('|'.join(ad_list_en), content)
     if matches:
         res["error_status"] = True
         res["error_type"] = ERROR_ADVERTISEMENT
         res['error_reason'] = matches
+    return res
+
+def model_watermark(content: str) -> dict:
+    """检查content内是否有水印."""
+    res = {'error_status': False}
+    watermark_list = ['仩嗨亾笁潪能', '上s海h人r工g智z能n实s验y室s']
+    matches = re.findall('|'.join(watermark_list), content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_WATERMARK
+        res['error_reason'] = '存在水印'
     return res
```

### Comparing `lanQ-1.0/lanQ_rule/prompt_rule.py` & `lanQ-1.1/lanQ_rule/prompt_rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import os
 import sys
 import langid
 
 sys.path.append(os.path.dirname(__file__))
 
+from base import *
 from const import *
 
 def prompt_chinese_produce_english(prompt: str, prediction: str) -> dict:
     """检查中文promt生成英文prediction."""
     res = {'error_status': False}
     lan_prompt = langid.classify(prompt)[0]
     lan_prediction = langid.classify(prediction)[0]
```

