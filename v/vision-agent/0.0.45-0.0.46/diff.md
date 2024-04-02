# Comparing `tmp/vision_agent-0.0.45.tar.gz` & `tmp/vision_agent-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.0.45.tar", max compression
+gzip compressed data, was "vision_agent-0.0.46.tar", max compression
```

## Comparing `vision_agent-0.0.45.tar` & `vision_agent-0.0.46.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-04-01 23:22:01.202070 vision_agent-0.0.45/LICENSE
--rw-r--r--   0        0        0     4191 2024-04-01 23:22:01.202070 vision_agent-0.0.45/README.md
--rw-r--r--   0        0        0     2166 2024-04-01 23:22:01.746071 vision_agent-0.0.45/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      306 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4493 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10101 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    17449 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     6151 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0       46 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/data/__init__.py
--rw-r--r--   0        0        0     5122 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/data/data.py
--rw-r--r--   0        0        0       75 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/emb/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/emb/emb.py
--rw-r--r--   0        0        0     4420 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/image_utils.py
--rw-r--r--   0        0        0       32 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     3904 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       51 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0     8438 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      235 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1416 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    23447 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7476 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/tools/video.py
--rw-r--r--   0        0        0     5340 1970-01-01 00:00:00.000000 vision_agent-0.0.45/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-02 17:30:28.214672 vision_agent-0.0.46/LICENSE
+-rw-r--r--   0        0        0     4415 2024-04-02 17:30:28.214672 vision_agent-0.0.46/README.md
+-rw-r--r--   0        0        0     2166 2024-04-02 17:30:28.750675 vision_agent-0.0.46/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4493 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10101 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    17449 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     6151 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0       46 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/data/__init__.py
+-rw-r--r--   0        0        0     5122 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/data/data.py
+-rw-r--r--   0        0        0       75 2024-04-02 17:30:28.226673 vision_agent-0.0.46/vision_agent/emb/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-02 17:30:28.230672 vision_agent-0.0.46/vision_agent/emb/emb.py
+-rw-r--r--   0        0        0     4420 2024-04-02 17:30:28.230672 vision_agent-0.0.46/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       32 2024-04-02 17:30:28.230672 vision_agent-0.0.46/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     3904 2024-04-02 17:30:28.230672 vision_agent-0.0.46/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       51 2024-04-02 17:30:28.230672 vision_agent-0.0.46/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0     8438 2024-04-02 17:30:28.230672 vision_agent-0.0.46/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      235 2024-04-02 17:30:28.230672 vision_agent-0.0.46/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1416 2024-04-02 17:30:28.230672 vision_agent-0.0.46/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    23447 2024-04-02 17:30:28.230672 vision_agent-0.0.46/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7476 2024-04-02 17:30:28.230672 vision_agent-0.0.46/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 vision_agent-0.0.46/PKG-INFO
```

### Comparing `vision_agent-0.0.45/LICENSE` & `vision_agent-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/README.md` & `vision_agent-0.0.46/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -99,11 +99,13 @@
 | CLIP | CLIP is a tool that can classify or tag any image given a set of input classes or tags. |
 | GroundingDINO | GroundingDINO is a tool that can detect arbitrary objects with inputs such as category names or referring expressions. |
 | GroundingSAM | GroundingSAM is a tool that can detect and segment arbitrary objects with inputs such as category names or referring expressions. |
 | Counter | Counter detects and counts the number of objects in an image given an input such as a category name or referring expression. |
 | Crop | Crop crops an image given a bounding box and returns a file name of the cropped image. |
 | BboxArea | BboxArea returns the area of the bounding box in pixels normalized to 2 decimal places. |
 | SegArea | SegArea returns the area of the segmentation mask in pixels normalized to 2 decimal places. |
-| ExtractFrames | ExtractFrames extracts image frames from the input video. |
+| BboxIoU | BboxIoU returns the intersection over union of two bounding boxes normalized to 2 decimal places. |
+| SegIoU | SegIoU returns the intersection over union of two segmentation masks normalized to 2 decimal places. |
+| ExtractFrames | ExtractFrames extracts frames with motion from a video. |
 
 
 It also has a basic set of calculate tools such as add, subtract, multiply and divide.
```

### Comparing `vision_agent-0.0.45/pyproject.toml` & `vision_agent-0.0.46/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.0.45"
+version = "0.0.46"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.0.45/vision_agent/agent/easytool.py` & `vision_agent-0.0.46/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.0.46/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/agent/reflexion.py` & `vision_agent-0.0.46/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.0.46/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/agent/vision_agent.py` & `vision_agent-0.0.46/vision_agent/agent/vision_agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.0.46/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/data/data.py` & `vision_agent-0.0.46/vision_agent/data/data.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/emb/emb.py` & `vision_agent-0.0.46/vision_agent/emb/emb.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/image_utils.py` & `vision_agent-0.0.46/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/llm/llm.py` & `vision_agent-0.0.46/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/lmm/lmm.py` & `vision_agent-0.0.46/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/tools/prompts.py` & `vision_agent-0.0.46/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/tools/tools.py` & `vision_agent-0.0.46/vision_agent/tools/tools.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/vision_agent/tools/video.py` & `vision_agent-0.0.46/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.45/PKG-INFO` & `vision_agent-0.0.46/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.0.45
+Version: 0.0.46
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -128,12 +128,14 @@
 | CLIP | CLIP is a tool that can classify or tag any image given a set of input classes or tags. |
 | GroundingDINO | GroundingDINO is a tool that can detect arbitrary objects with inputs such as category names or referring expressions. |
 | GroundingSAM | GroundingSAM is a tool that can detect and segment arbitrary objects with inputs such as category names or referring expressions. |
 | Counter | Counter detects and counts the number of objects in an image given an input such as a category name or referring expression. |
 | Crop | Crop crops an image given a bounding box and returns a file name of the cropped image. |
 | BboxArea | BboxArea returns the area of the bounding box in pixels normalized to 2 decimal places. |
 | SegArea | SegArea returns the area of the segmentation mask in pixels normalized to 2 decimal places. |
-| ExtractFrames | ExtractFrames extracts image frames from the input video. |
+| BboxIoU | BboxIoU returns the intersection over union of two bounding boxes normalized to 2 decimal places. |
+| SegIoU | SegIoU returns the intersection over union of two segmentation masks normalized to 2 decimal places. |
+| ExtractFrames | ExtractFrames extracts frames with motion from a video. |
 
 
 It also has a basic set of calculate tools such as add, subtract, multiply and divide.
```

