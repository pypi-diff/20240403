# Comparing `tmp/surfkit-0.1.3.tar.gz` & `tmp/surfkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfkit-0.1.3.tar", max compression
+gzip compressed data, was "surfkit-0.1.4.tar", max compression
```

## Comparing `surfkit-0.1.3.tar` & `surfkit-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-04-02 20:08:38.101639 surfkit-0.1.3/LICENSE
--rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.3/README.md
--rw-r--r--   0        0        0      442 2024-04-03 04:16:18.189257 surfkit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      610 2024-04-02 20:50:51.383715 surfkit-0.1.3/surfkit/agent.py
--rw-r--r--   0        0        0        0 2024-04-02 20:19:29.385009 surfkit-0.1.3/surfkit/cli.py
--rw-r--r--   0        0        0     2013 2024-04-03 02:11:06.207281 surfkit-0.1.3/surfkit/db/conn.py
--rw-r--r--   0        0        0     1499 2024-04-03 04:02:27.111787 surfkit-0.1.3/surfkit/db/models.py
--rw-r--r--   0        0        0      195 2024-04-02 20:23:26.016439 surfkit-0.1.3/surfkit/env.py
--rw-r--r--   0        0        0     5444 2024-04-02 20:43:49.583063 surfkit-0.1.3/surfkit/llm.py
--rw-r--r--   0        0        0     1656 2024-04-03 02:10:36.829145 surfkit-0.1.3/surfkit/models.py
--rw-r--r--   0        0        0     9000 2024-04-03 02:10:58.047265 surfkit-0.1.3/surfkit/types.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 surfkit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-02 20:08:38.101639 surfkit-0.1.4/LICENSE
+-rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.4/README.md
+-rw-r--r--   0        0        0      442 2024-04-03 16:42:13.558020 surfkit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      610 2024-04-03 16:41:37.648579 surfkit-0.1.4/surfkit/agent.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:41:36.393225 surfkit-0.1.4/surfkit/cli.py
+-rw-r--r--   0        0        0     2013 2024-04-03 02:11:06.207281 surfkit-0.1.4/surfkit/db/conn.py
+-rw-r--r--   0        0        0     1473 2024-04-03 16:41:49.842770 surfkit-0.1.4/surfkit/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-03 16:41:34.576256 surfkit-0.1.4/surfkit/env.py
+-rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.4/surfkit/hub.py
+-rw-r--r--   0        0        0     5413 2024-04-03 16:40:41.438440 surfkit-0.1.4/surfkit/llm.py
+-rw-r--r--   0        0        0     1619 2024-04-03 16:42:08.726348 surfkit-0.1.4/surfkit/models.py
+-rw-r--r--   0        0        0     9000 2024-04-03 02:10:58.047265 surfkit-0.1.4/surfkit/types.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 surfkit-0.1.4/PKG-INFO
```

### Comparing `surfkit-0.1.3/LICENSE` & `surfkit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.3/surfkit/agent.py` & `surfkit-0.1.4/surfkit/agent.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.3/surfkit/db/conn.py` & `surfkit-0.1.4/surfkit/db/conn.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.3/surfkit/db/models.py` & `surfkit-0.1.4/surfkit/db/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import uuid
 import time
 
-from sqlalchemy import Column, String, ForeignKey, Boolean, Float, Integer
-from sqlalchemy.orm import relationship, declarative_base
+from sqlalchemy import Column, String, Boolean, Float, Integer
+from sqlalchemy.orm import declarative_base
 
 from ..models import V1UserProfile
 
 Base = declarative_base()
 
 
 class UserRecord(Base):
```

### Comparing `surfkit-0.1.3/surfkit/llm.py` & `surfkit-0.1.4/surfkit/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import logging
 from typing import Optional, List, Dict
 import json
 
 from litellm import Router
-from pydantic import BaseModel
-
 from taskara import Task
+
 from .models import EnvVarOptModel, LLMProviderOption
 
 
 class LLMProvider:
     """
     A chat provider based on LiteLLM
     """
```

### Comparing `surfkit-0.1.3/surfkit/models.py` & `surfkit-0.1.4/surfkit/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import List, Optional, Dict
 
 from pydantic import BaseModel
-from taskara.models import TaskModel
 
 
 class EnvVarOptModel(BaseModel):
     name: str
     description: Optional[str] = None
     required: bool = False
     default: Optional[str] = None
```

### Comparing `surfkit-0.1.3/surfkit/types.py` & `surfkit-0.1.4/surfkit/types.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.3/PKG-INFO` & `surfkit-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surfkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: A toolkit to build GUI surfing AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

