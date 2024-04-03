# Comparing `tmp/substrate-120240315.0.1.tar.gz` & `tmp/substrate-120240403.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240315.0.1.tar", max compression
+gzip compressed data, was "substrate-120240403.0.1.tar", max compression
```

## Comparing `substrate-120240315.0.1.tar` & `substrate-120240403.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240315.0.1/LICENSE
--rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240315.0.1/README.md
--rw-r--r--   0        0        0     2016 2024-03-22 03:06:06.247009 substrate-120240315.0.1/pyproject.toml
--rw-r--r--   0        0        0       17 2024-03-21 21:46:59.000000 substrate-120240315.0.1/substrate/GEN_VERSION
--rw-r--r--   0        0        0     1174 2024-03-21 21:46:59.000000 substrate-120240315.0.1/substrate/__init__.py
--rw-r--r--   0        0        0     5582 2024-03-21 22:51:25.550938 substrate-120240315.0.1/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240315.0.1/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-03-22 02:40:53.485082 substrate-120240315.0.1/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-03-22 02:40:53.484982 substrate-120240315.0.1/substrate/core/_version.py
--rw-r--r--   0        0        0     2200 2024-03-22 02:40:53.485388 substrate-120240315.0.1/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-03-22 02:40:53.485633 substrate-120240315.0.1/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-03-22 02:40:53.485740 substrate-120240315.0.1/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2620 2024-03-22 02:40:53.485929 substrate-120240315.0.1/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-03-22 02:40:53.485558 substrate-120240315.0.1/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-03-22 02:40:53.485247 substrate-120240315.0.1/substrate/core/coregraph.py
--rw-r--r--   0        0        0     1973 2024-03-22 02:40:53.481594 substrate-120240315.0.1/substrate/core/corenode.py
--rw-r--r--   0        0        0      894 2024-03-22 02:40:53.481402 substrate-120240315.0.1/substrate/core/id_generator.py
--rw-r--r--   0        0        0    27982 2024-03-22 02:40:53.484396 substrate-120240315.0.1/substrate/core/models.py
--rw-r--r--   0        0        0     1405 2024-03-22 02:40:53.481238 substrate-120240315.0.1/substrate/core/sb.py
--rw-r--r--   0        0        0    24491 2024-03-21 21:46:59.000000 substrate-120240315.0.1/substrate/dataclass_models.py
--rw-r--r--   0        0        0    32037 2024-03-21 21:46:59.000000 substrate-120240315.0.1/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    29520 2024-03-21 21:46:59.000000 substrate-120240315.0.1/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240315.0.1/substrate/py.typed
--rw-r--r--   0        0        0     1583 2024-03-18 04:02:11.878694 substrate-120240315.0.1/substrate/substrate.py
--rw-r--r--   0        0        0    26407 2024-03-21 21:46:59.000000 substrate-120240315.0.1/substrate/typeddict_models.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240315.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240403.0.1/LICENSE
+-rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240403.0.1/README.md
+-rw-r--r--   0        0        0     2023 2024-04-03 05:09:40.191891 substrate-120240403.0.1/pyproject.toml
+-rw-r--r--   0        0        0       17 2024-04-03 04:58:23.000000 substrate-120240403.0.1/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     1508 2024-04-03 04:58:24.000000 substrate-120240403.0.1/substrate/__init__.py
+-rw-r--r--   0        0        0     5582 2024-03-21 22:51:25.550938 substrate-120240403.0.1/substrate/_client.py
+-rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240403.0.1/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-04-03 05:00:31.508855 substrate-120240403.0.1/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-03 05:00:31.508762 substrate-120240403.0.1/substrate/core/_version.py
+-rw-r--r--   0        0        0     2200 2024-04-03 05:00:31.509086 substrate-120240403.0.1/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-04-03 05:00:31.509323 substrate-120240403.0.1/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-03 05:00:31.509454 substrate-120240403.0.1/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2620 2024-04-03 05:00:31.509658 substrate-120240403.0.1/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-04-03 05:00:31.509261 substrate-120240403.0.1/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-04-03 05:00:31.508969 substrate-120240403.0.1/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     1960 2024-04-03 05:00:31.508332 substrate-120240403.0.1/substrate/core/corenode.py
+-rw-r--r--   0        0        0      894 2024-04-03 05:00:31.508168 substrate-120240403.0.1/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    31860 2024-04-03 05:00:31.508519 substrate-120240403.0.1/substrate/core/models.py
+-rw-r--r--   0        0        0     1405 2024-04-03 05:00:31.507983 substrate-120240403.0.1/substrate/core/sb.py
+-rw-r--r--   0        0        0    27585 2024-04-03 04:58:22.000000 substrate-120240403.0.1/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    36470 2024-04-03 04:58:23.000000 substrate-120240403.0.1/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    40093 2024-04-03 04:58:24.000000 substrate-120240403.0.1/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240403.0.1/substrate/py.typed
+-rw-r--r--   0        0        0     1583 2024-03-18 04:02:11.878694 substrate-120240403.0.1/substrate/substrate.py
+-rw-r--r--   0        0        0    29794 2024-04-03 04:58:21.000000 substrate-120240403.0.1/substrate/typeddict_models.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240403.0.1/PKG-INFO
```

### Comparing `substrate-120240315.0.1/LICENSE` & `substrate-120240403.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240315.0.1/pyproject.toml` & `substrate-120240403.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
-requires = ["poetry-core"]
+requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240315.0.1"
+version = "120240403.0.1"
 description = "Substrate Python SDK"
 readme = "README.md"
-authors = ["vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>"]
+authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
 typeCheckingMode = "basic"
 pythonVersion = "3.7"
-exclude = [".venv"]
+exclude = [ ".venv",]
 
 [tool.ruff]
 line-length = 120
 output-format = "grouped"
 target-version = "py310"
 
 [tool.mypy]
@@ -46,33 +46,30 @@
 networkx = ">=3.2.1"
 httpx = ">=0.26.0"
 distro = ">=1.8.0"
 typing-extensions = "^4.10.0"
 
 [tool.ruff.lint]
 ignore-init-module-imports = true
-ignore = ["B006", "T201", "T203", "ARG002", "ARG001"]
-unfixable = ["T201", "T203"]
-select = ["I", "B", "F401", "E722", "ARG", "TCH004"]
+ignore = [ "B006", "T201", "T203", "ARG002", "ARG001",]
+unfixable = [ "T201", "T203",]
+select = [ "I", "B", "F401", "E722", "ARG", "TCH004",]
 
 [tool.ruff.format]
 docstring-code-format = true
 
 [tool.pytest.ini_options]
-markers = [
-    "unit: tests intended to be run against only local code - no external integrations",
-    "e2e: tests intended to encapsulate the entire lifecycle of an interaction with the substrate system",
-]
+markers = [ "unit: tests intended to be run against only local code - no external integrations", "e2e: tests intended to encapsulate the entire lifecycle of an interaction with the substrate system",]
 
 [tool.ruff.lint.isort]
 length-sort = true
 length-sort-straight = true
 combine-as-imports = true
-extra-standard-library = ["typing_extensions"]
-known-first-party = ["substrate", "tests"]
+extra-standard-library = [ "typing_extensions",]
+known-first-party = [ "substrate", "tests",]
 
 [tool.poetry.group.dev.dependencies]
 pyright = ">=1.1.342"
 ruff = "^0.2.1"
 pytest = "^8.0.0"
 types-networkx = "^3.2.1.20240205"
 types-toml = "^0.10.8.7"
```

### Comparing `substrate-120240315.0.1/substrate/_client.py` & `substrate-120240403.0.1/substrate/_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240315.0.1/substrate/core/base_future.py` & `substrate-120240403.0.1/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240315.0.1/substrate/core/client/find_futures_client.py` & `substrate-120240403.0.1/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240315.0.1/substrate/core/client/future.py` & `substrate-120240403.0.1/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240315.0.1/substrate/core/client/graph.py` & `substrate-120240403.0.1/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240315.0.1/substrate/core/coregraph.py` & `substrate-120240403.0.1/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240315.0.1/substrate/core/corenode.py` & `substrate-120240403.0.1/substrate/core/corenode.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 from .id_generator import IDGenerator
 from .client.future import TracedFuture
 from .client.find_futures_client import find_futures_client
 
 
 class CoreNode:
     def __init__(self, **attr):
-        self.node = None
+        self.node = self.__class__.__name__
         self.args = attr
-        class_name = self.__class__.__name__
-        generator_instance = IDGenerator.get_instance(class_name)
+        generator_instance = IDGenerator.get_instance(self.__class__.__name__)
         self.id = generator_instance.get_next_id()
         self._global_output_keys = None
         self._should_output_globally: bool = False
         self.SG = nx.DiGraph()
         if attr:
             self.args = BaseFuture.replace_futures_with_placeholder(attr)
         else:
```

### Comparing `substrate-120240315.0.1/substrate/core/id_generator.py` & `substrate-120240403.0.1/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240315.0.1/substrate/core/models.py` & `substrate-120240403.0.1/substrate/dataclass_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,329 +4,406 @@
 (using datamodel-codegen)
 """
 
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
-from typing_extensions import Literal, Annotated
+from dataclasses import dataclass
+from typing_extensions import Literal
 
-from pydantic import Extra, Field, BaseModel
-
-
-class ErrorOut(BaseModel):
-    class Config:
-        extra = Extra.allow
 
+@dataclass
+class ErrorOut:
     type: Literal["api_error", "invalid_request_error"]
     """
     The type of error returned.
     """
     message: str
     """
     A message providing more details about the error.
     """
 
 
-class ResponseFormat(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    type: Literal["json_object", "text"]
+@dataclass
+class GenerateTextIn:
+    prompt: str
     """
-    Type of response.
+    Input prompt.
     """
-    json_schema: Optional[Dict[str, Any]] = None
+    temperature: Optional[int] = 4
     """
-    JSON schema to guide `json_object` response.
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    Maximum number of tokens to generate.
+    """
+    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
     """
+    Selected node.
+    """
+
 
+@dataclass
+class GenerateTextOut:
+    text: Optional[str] = None
+    """
+    Text response.
+    """
 
-class GenerateTextIn(BaseModel):
-    class Config:
-        extra = Extra.allow
 
+@dataclass
+class GenerateJSONIn:
     prompt: str
     """
     Input prompt.
     """
-    model: Optional[Literal["mistral-7b-instruct"]] = "mistral-7b-instruct"
+    json_schema: Dict[str, Any]
     """
-    Selected model.
+    JSON schema to guide `json_object` response.
     """
-    response_format: Optional[ResponseFormat] = None
+    temperature: Optional[int] = 4
     """
-    Format of the response.
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
-    temperature: Annotated[Optional[int], Field(ge=1, le=10)] = 4
+    max_tokens: Optional[int] = None
+    """
+    Maximum number of tokens to generate.
+    """
+    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    """
+    Selected node.
+    """
+
+
+@dataclass
+class GenerateJSONOut:
+    json_object: Optional[Dict[str, Any]] = None
+    """
+    JSON response.
+    """
+
+
+@dataclass
+class MultiGenerateTextIn:
+    prompt: str
+    """
+    Input prompt.
+    """
+    num_choices: int
+    """
+    Number of choices to generate.
+    """
+    temperature: Optional[int] = 4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
-    max_tokens: Optional[int] = 800
+    max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
+    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    """
+    Selected node.
+    """
 
 
-class MultiGenerateTextIn(BaseModel):
-    class Config:
-        extra = Extra.allow
+@dataclass
+class MultiGenerateTextOut:
+    choices: List[GenerateTextOut]
+
 
+@dataclass
+class MultiGenerateJSONIn:
     prompt: str
     """
     Input prompt.
     """
+    json_schema: Dict[str, Any]
+    """
+    JSON schema to guide `json_object` response.
+    """
     num_choices: int
     """
     Number of choices to generate.
     """
-    model: Optional[Literal["mistral-7b-instruct"]] = "mistral-7b-instruct"
+    temperature: Optional[int] = 4
     """
-    Selected model.
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    Maximum number of tokens to generate.
+    """
+    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    """
+    Selected node.
+    """
+
+
+@dataclass
+class MultiGenerateJSONOut:
+    choices: List[GenerateJSONOut]
+
+
+@dataclass
+class Mistral7BInstructIn:
+    prompt: str
+    """
+    Input prompt.
+    """
+    num_choices: int
     """
-    response_format: Optional[ResponseFormat] = None
+    Number of choices to generate.
+    """
+    json_schema: Optional[Dict[str, Any]] = None
     """
-    Format of the response.
+    JSON schema to guide response.
     """
-    temperature: Annotated[Optional[int], Field(ge=1, le=10)] = 4
+    temperature: Optional[float] = None
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
-    max_tokens: Optional[int] = 800
+    max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
 
 
-class GenerateTextOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class Mistral7BInstructChoice:
     text: Optional[str] = None
     """
-    Text response.
+    Text response, if `json_schema` was not provided.
     """
     json_object: Optional[Dict[str, Any]] = None
     """
-    JSON response.
+    JSON response, if `json_schema` was provided.
     """
 
 
-class MultiGenerateTextOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    choices: List[GenerateTextOut]
+@dataclass
+class Mistral7BInstructOut:
+    choices: List[Mistral7BInstructChoice]
 
 
-class GenerateTextVisionIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class GenerateTextVisionIn:
     prompt: str
     """
     Text prompt.
     """
-    image_uris: Optional[List[str]] = None
+    image_uris: List[str]
     """
     Image prompts.
     """
-    model: Optional[Literal["firellava-13b"]] = "firellava-13b"
-    """
-    Selected model.
-    """
-    temperature: Annotated[Optional[int], Field(ge=1, le=10)] = 4
+    temperature: Optional[int] = 4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = 800
     """
     Maximum number of tokens to generate.
     """
+    node: Optional[Literal["Firellava13B"]] = "Firellava13B"
+    """
+    Selected node.
+    """
 
 
-class GenerateTextVisionOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class GenerateTextVisionOut:
     text: str
     """
     Text response.
     """
 
 
-class GenerateImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class Firellava13BIn:
     prompt: str
     """
     Text prompt.
     """
-    image_prompt_uri: Optional[str] = None
-    """
-    Image prompt.
+    image_uris: List[str]
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
-    """
-    Selected model.
+    Image prompts.
     """
-    image_influence: Annotated[Optional[float], Field(ge=0.0, le=10.0)] = 5
+    temperature: Optional[float] = None
     """
-    Controls the influence of the image prompt on the generated output.
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
-    negative_prompt: Optional[str] = None
+    max_tokens: Optional[int] = 800
     """
-    Negative input prompt.
+    Maximum number of tokens to generate.
     """
-    store: Optional[str] = None
+
+
+@dataclass
+class Firellava13BOut:
+    text: str
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Text response.
     """
-    width: Optional[int] = None
+
+
+@dataclass
+class GenerateImageIn:
+    prompt: str
     """
-    Width of output image, in pixels.
+    Text prompt.
     """
-    height: Optional[int] = None
+    store: Optional[str] = None
     """
-    Height of output image, in pixels.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    seed: Optional[int] = None
+    node: Optional[Literal["StableDiffusionXL"]] = "StableDiffusionXL"
     """
-    Seed for deterministic generation. Default is a random seed.
+    Selected node.
     """
 
 
-class GenerateImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class GenerateImageOut:
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
-    seed: int
-    """
-    The random noise seed used for generation.
-    """
 
 
-class MultiGenerateImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class MultiGenerateImageIn:
     prompt: str
     """
     Text prompt.
     """
-    image_prompt_uri: Optional[str] = None
-    """
-    Image prompt.
-    """
     num_images: int
     """
     Number of images to generate.
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
+    store: Optional[str] = None
     """
-    Selected model.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    image_influence: Annotated[Optional[float], Field(ge=0.0, le=10.0)] = 5
+    node: Optional[Literal["StableDiffusionXL"]] = "StableDiffusionXL"
     """
-    Controls the influence of the image prompt on the generated output.
+    Selected node.
+    """
+
+
+@dataclass
+class MultiGenerateImageOut:
+    outputs: List[GenerateImageOut]
+
+
+@dataclass
+class StableDiffusionXLIn:
+    prompt: str
+    """
+    Text prompt.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
+    steps: Optional[int] = None
+    """
+    Number of diffusion steps.
+    """
+    num_images: Optional[int] = None
+    """
+    Number of images to generate.
+    """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
+    height: Optional[int] = None
+    """
+    Height of output image, in pixels.
+    """
     width: Optional[int] = None
     """
     Width of output image, in pixels.
     """
-    height: Optional[int] = None
+    seeds: Optional[int] = None
     """
-    Height of output image, in pixels.
+    Seeds for deterministic generation. Default is a random seed.
     """
-    seeds: Optional[List[int]] = None
+    guidance_scale: Optional[float] = 5
     """
-    Random noise seeds. Default is random seeds for each generation.
+    Higher values adhere to the text prompt more strongly, typically at the expense of image quality.
     """
 
 
-class MultiGenerateImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    outputs: List[GenerateImageOut]
-
-
-class ControlledGenerateImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class StableDiffusionImage:
     image_uri: str
     """
-    Input image.
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
-    control_method: Literal["edge", "depth", "illusion"]
+    seed: int
     """
-    Strategy to control generation using the input image.
+    The random noise seed used for generation.
     """
+
+
+@dataclass
+class StableDiffusionXLOut:
+    outputs: List[StableDiffusionImage]
+
+
+@dataclass
+class StableDiffusionXLIPAdapterIn:
     prompt: str
     """
     Text prompt.
     """
-    output_resolution: Optional[int] = 1024
+    num_images: int
     """
-    Resolution of the output image, in pixels.
+    Number of images to generate.
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
+    image_prompt_uri: Optional[str] = None
     """
-    Selected model.
+    Image prompt.
+    """
+    ip_adapter_scale: Optional[float] = None
+    """
+    Controls the influence of the image prompt on the generated output.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    image_influence: Annotated[Optional[float], Field(ge=0.0, le=10.0)] = 9
-    """
-    Controls the influence of the input image on the generated output.
-    """
-    seed: Optional[int] = None
+    width: Optional[int] = None
     """
-    Seed for deterministic generation. Default is a random seed.
+    Width of output image, in pixels.
     """
-
-
-class ControlledGenerateImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    image_uri: str
+    height: Optional[int] = None
     """
-    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    Height of output image, in pixels.
     """
-    seed: int
+    seeds: Optional[List[int]] = None
     """
-    The random noise seed used for generation.
+    Random noise seeds. Default is random seeds for each generation.
     """
 
 
-class MultiControlledGenerateImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
+@dataclass
+class StableDiffusionXLIPAdapterOut:
+    outputs: List[StableDiffusionImage]
+
 
+@dataclass
+class StableDiffusionXLControlNetIn:
     image_uri: str
     """
     Input image.
     """
     control_method: Literal["edge", "depth", "illusion"]
     """
     Strategy to control generation using the input image.
@@ -339,172 +416,149 @@
     """
     Number of images to generate.
     """
     output_resolution: Optional[int] = 1024
     """
     Resolution of the output image, in pixels.
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
-    """
-    Selected model.
-    """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    image_influence: Annotated[Optional[float], Field(ge=0.0, le=10.0)] = 9
+    conditioning_scale: Optional[float] = None
     """
     Controls the influence of the input image on the generated output.
     """
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
-class MultiControlledGenerateImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    outputs: List[ControlledGenerateImageOut]
+@dataclass
+class StableDiffusionXLControlNetOut:
+    outputs: List[StableDiffusionImage]
 
 
-class GenerativeEditImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class GenerativeEditImageIn:
     image_uri: str
     """
     Original image.
     """
     prompt: str
     """
     Text prompt.
     """
     mask_image_uri: Optional[str] = None
     """
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
-    image_prompt_uri: Optional[str] = None
+    store: Optional[str] = None
     """
-    Image prompt.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    output_resolution: Optional[int] = 1024
+    node: Optional[Literal["StableDiffusionXLInpaint"]] = "StableDiffusionXLInpaint"
     """
-    Resolution of the output image, in pixels.
+    Selected node.
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
+
+
+@dataclass
+class GenerativeEditImageOut:
+    image_uri: str
     """
-    Selected model.
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
-    strength: Annotated[Optional[float], Field(ge=0.0, le=10.0)] = 8
+
+
+@dataclass
+class MultiGenerativeEditImageIn:
+    image_uri: str
     """
-    Controls the strength of the generation process.
+    Original image.
     """
-    image_prompt_influence: Annotated[Optional[float], Field(ge=0.0, le=10.0)] = 5
+    prompt: str
     """
-    Controls the influence of the image prompt on the generated output.
+    Text prompt.
     """
-    negative_prompt: Optional[str] = None
+    num_images: int
     """
-    Negative input prompt.
+    Number of images to generate.
+    """
+    mask_image_uri: Optional[str] = None
+    """
+    Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    seed: Optional[int] = None
+    node: Optional[Literal["StableDiffusionXLInpaint"]] = "StableDiffusionXLInpaint"
     """
-    Seed for deterministic generation. Default is a random seed.
+    Selected node.
     """
 
 
-class GenerativeEditImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    image_uri: str
-    """
-    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
-    """
-    seed: int
-    """
-    The random noise seed used for generation.
-    """
-
+@dataclass
+class MultiGenerativeEditImageOut:
+    outputs: List[GenerativeEditImageOut]
 
-class MultiGenerativeEditImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
 
+@dataclass
+class StableDiffusionXLInpaintIn:
     image_uri: str
     """
     Original image.
     """
     prompt: str
     """
     Text prompt.
     """
-    mask_image_uri: Optional[str] = None
-    """
-    Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
-    """
-    image_prompt_uri: Optional[str] = None
-    """
-    Image prompt.
-    """
     num_images: int
     """
     Number of images to generate.
     """
-    output_resolution: Optional[int] = 1024
+    mask_image_uri: Optional[str] = None
     """
-    Resolution of the output image, in pixels.
+    Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
+    output_resolution: Optional[int] = 1024
     """
-    Selected model.
+    Resolution of the output image, in pixels.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    strength: Annotated[Optional[float], Field(ge=0.0, le=10.0)] = 8
+    strength: Optional[float] = 0.5
     """
     Controls the strength of the generation process.
     """
-    image_prompt_influence: Annotated[Optional[float], Field(ge=0.0, le=10.0)] = 5
-    """
-    Controls the influence of the image prompt on the generated output.
-    """
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
-class MultiGenerativeEditImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    outputs: List[GenerativeEditImageOut]
-
+@dataclass
+class StableDiffusionXLInpaintOut:
+    outputs: List[StableDiffusionImage]
 
-class BoundingBox(BaseModel):
-    class Config:
-        extra = Extra.allow
 
+@dataclass
+class BoundingBox:
     x1: float
     """
     Top left corner x.
     """
     y1: float
     """
     Top left corner y.
@@ -515,32 +569,28 @@
     """
     y2: float
     """
     Bottom right corner y.
     """
 
 
-class Point(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class Point:
     x: int
     """
     X position.
     """
     y: int
     """
     Y position.
     """
 
 
-class FillMaskIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class FillMaskIn:
     image_uri: str
     """
     Input image.
     """
     mask_image_uri: str
     """
     Mask image that controls which pixels are inpainted.
@@ -551,28 +601,24 @@
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class FillMaskOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class FillMaskOut:
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
-class RemoveBackgroundIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class RemoveBackgroundIn:
     image_uri: str
     """
     Input image.
     """
     return_mask: Optional[bool] = None
     """
     Return a mask image instead of the original content.
@@ -587,92 +633,80 @@
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class RemoveBackgroundOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class RemoveBackgroundOut:
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
-class UpscaleImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class UpscaleImageIn:
     image_uri: str
     """
     Input image.
     """
     model: Optional[Literal["real-esrgan-x4"]] = "real-esrgan-x4"
     """
     Selected model.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class UpscaleImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class UpscaleImageOut:
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
-class DetectSegmentsIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class DetectSegmentsIn:
     image_uri: str
     """
     Input image.
     """
     point_prompts: Optional[List[Point]] = None
     """
-    Point prompts, to detect a segment under the point. One of `point_prompt` or `box_prompt` must be set.
+    Point prompts, to detect a segment under the point. One of `point_prompts` or `box_prompts` must be set.
     """
     box_prompts: Optional[List[BoundingBox]] = None
     """
-    Box prompts, to detect a segment within the bounding box. One of `point_prompt` or `box_prompt` must be set.
+    Box prompts, to detect a segment within the bounding box. One of `point_prompts` or `box_prompts` must be set.
     """
     model: Optional[Literal["segment-anything"]] = "segment-anything"
     """
     Selected model.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class DetectSegmentsOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class DetectSegmentsOut:
     mask_image_uri: str
     """
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
-class TranscribeMediaIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class TranscribeMediaIn:
     audio_uri: str
     """
     Input audio.
     """
     prompt: Optional[str] = None
     """
     Prompt to guide model on the content and context of input audio.
@@ -695,18 +729,16 @@
     """
     suggest_chapters: Optional[bool] = False
     """
     Suggest automatic chapter markers.
     """
 
 
-class TranscribedWord(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class TranscribedWord:
     word: str
     """
     Text of word.
     """
     start: Optional[float] = None
     """
     Start time of word, in seconds.
@@ -717,18 +749,16 @@
     """
     speaker: Optional[str] = None
     """
     ID of speaker, if `diarize` is enabled.
     """
 
 
-class TranscribedSegment(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class TranscribedSegment:
     text: str
     """
     Text of segment.
     """
     start: float
     """
     Start time of segment, in seconds.
@@ -743,50 +773,44 @@
     """
     words: Optional[List[TranscribedWord]] = None
     """
     Aligned words, if `align` is enabled.
     """
 
 
-class ChapterMarker(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class ChapterMarker:
     title: str
     """
     Chapter title.
     """
     start: float
     """
     Start time of chapter, in seconds.
     """
 
 
-class TranscribeMediaOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class TranscribeMediaOut:
     text: str
     """
     Transcribed text.
     """
     segments: Optional[List[TranscribedSegment]] = None
     """
     Transcribed segments, if `segment` is enabled.
     """
     chapters: Optional[List[ChapterMarker]] = None
     """
     Chapter markers, if `suggest_chapters` is enabled.
     """
 
 
-class GenerateSpeechIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class GenerateSpeechIn:
     text: str
     """
     Input text.
     """
     audio_uri: Optional[str] = None
     """
     Reference audio used to synthesize the speaker. If unset, a default speaker voice will be used.
@@ -797,372 +821,392 @@
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
-class GenerateSpeechOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class GenerateSpeechOut:
     audio_uri: str
     """
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
     """
 
 
-class Embedding(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class Embedding:
     vector: List[float]
     """
     Embedding vector.
     """
-    document_id: Optional[str] = None
+    doc_id: Optional[str] = None
     """
     Vector store document ID.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     Vector store document metadata.
     """
 
 
-class EmbedTextIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class EmbedTextIn:
     text: str
     """
     Text to embed.
     """
-    model: Optional[Literal["jina-v2", "clip"]] = "jina-v2"
-    """
-    Selected model.
-    """
     store: Optional[str] = None
     """
     [Vector store](/docs/vector-stores) identifier.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     Metadata that can be used to query the vector store. Ignored if `store` is unset.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     Choose keys from `metadata` to embed with text.
     """
-    document_id: Optional[str] = None
+    doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
+    node: Optional[Literal["JinaV2", "CLIP"]] = "JinaV2"
+    """
+    Selected node.
+    """
 
 
-class EmbedTextOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class EmbedTextOut:
     embedding: Embedding
     """
     Generated embedding.
     """
 
 
-class EmbedTextItem(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class EmbedTextItem:
     text: str
     """
     Text to embed.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     Metadata that can be used to query the vector store. Ignored if `store` is unset.
     """
-    document_id: Optional[str] = None
+    doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
 
 
-class MultiEmbedTextIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class MultiEmbedTextIn:
     items: List[EmbedTextItem]
     """
     Items to embed.
     """
-    model: Optional[Literal["jina-v2", "clip"]] = "jina-v2"
+    store: Optional[str] = None
     """
-    Selected model.
+    [Vector store](/docs/vector-stores) identifier.
+    """
+    embedded_metadata_keys: Optional[List[str]] = None
+    """
+    Choose keys from `metadata` to embed with text.
+    """
+    node: Optional[Literal["JinaV2", "CLIP"]] = "JinaV2"
+    """
+    Selected node.
+    """
+
+
+@dataclass
+class MultiEmbedTextOut:
+    embeddings: List[Embedding]
+    """
+    Generated embeddings.
+    """
+
+
+@dataclass
+class JinaV2In:
+    items: List[EmbedTextItem]
+    """
+    Items to embed.
     """
     store: Optional[str] = None
     """
     [Vector store](/docs/vector-stores) identifier.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     Choose keys from `metadata` to embed with text.
     """
 
 
-class MultiEmbedTextOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class JinaV2Out:
     embeddings: List[Embedding]
     """
     Generated embeddings.
     """
 
 
-class EmbedImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class EmbedImageIn:
     image_uri: str
     """
     Image to embed.
     """
-    model: Optional[Literal["clip"]] = "clip"
-    """
-    Selected model.
-    """
     store: Optional[str] = None
     """
     [Vector store](/docs/vector-stores) identifier.
     """
-    document_id: Optional[str] = None
+    doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
+    node: Optional[Literal["CLIP"]] = "CLIP"
+    """
+    Selected node.
+    """
 
 
-class EmbedImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class EmbedImageOut:
     embedding: Embedding
     """
     Generated embedding.
     """
 
 
-class EmbedImageItem(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class EmbedImageItem:
     image_uri: str
     """
     Image to embed.
     """
-    document_id: Optional[str] = None
+    doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
 
 
-class MultiEmbedImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
+@dataclass
+class EmbedTextOrImageItem:
+    image_uri: Optional[str] = None
+    """
+    Image to embed.
+    """
+    text: Optional[str] = None
+    """
+    Text to embed.
+    """
+    metadata: Optional[Dict[str, Any]] = None
+    """
+    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    """
+    doc_id: Optional[str] = None
+    """
+    Vector store document ID. Ignored if `store` is unset.
+    """
+
 
+@dataclass
+class MultiEmbedImageIn:
     items: List[EmbedImageItem]
     """
     Items to embed.
     """
     store: Optional[str] = None
     """
     [Vector store](/docs/vector-stores) identifier.
     """
-    model: Optional[Literal["clip"]] = "clip"
+    node: Optional[Literal["CLIP"]] = "CLIP"
     """
-    Selected model.
+    Selected node.
     """
 
 
-class MultiEmbedImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class MultiEmbedImageOut:
     embeddings: List[Embedding]
     """
     Generated embeddings.
     """
 
 
-class VectorStoreParams(BaseModel):
+@dataclass
+class CLIPIn:
+    items: List[EmbedTextOrImageItem]
+    """
+    Items to embed.
+    """
+    embedded_metadata_keys: Optional[List[str]] = None
+    """
+    Choose keys from `metadata` to embed with text, when embedding and storing text documents.
+    """
+    store: Optional[str] = None
+    """
+    [Vector store](/docs/vector-stores) identifier.
+    """
+
+
+@dataclass
+class CLIPOut:
+    embeddings: List[Embedding]
     """
-    Fields describing a vector store and its associated index.
+    Generated embeddings.
     """
 
-    class Config:
-        extra = Extra.allow
 
-    name: Annotated[str, Field(max_length=63, min_length=1)]
+@dataclass
+class VectorStoreParams:
+    name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
     """
-    m: Annotated[Optional[int], Field(ge=1, le=64)] = 16
+    m: Optional[int] = 16
     """
     The max number of connections per layer for the index.
     """
-    ef_construction: Annotated[Optional[int], Field(ge=1, le=128)] = 64
+    ef_construction: Optional[int] = 64
     """
     The size of the dynamic candidate list for constructing the index graph.
     """
     metric: Optional[Literal["cosine", "l2", "inner"]] = "inner"
     """
     The distance metric to construct the index with.
     """
 
 
-class DeleteVectorStoreParams(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class DeleteVectorStoreParams:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
     """
 
 
-class Vector(BaseModel):
+@dataclass
+class Vector:
     """
     Canonical representation of document with embedding vector.
     """
 
-    class Config:
-        extra = Extra.allow
-
     id: str
     """
     Document ID.
     """
     vector: List[float]
     """
     Embedding vector.
     """
     metadata: Dict[str, Any]
     """
     Document metadata.
     """
 
 
-class GetVectorsParams(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class GetVectorsParams:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
     """
-    ids: Annotated[List[str], Field(max_items=100)]
+    ids: List[str]
     """
     Document IDs to retrieve.
     """
 
 
-class GetVectorsResponse(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class GetVectorsResponse:
     vectors: List[Vector]
     """
     Retrieved vectors.
     """
 
 
-class VectorUpdateCountResponse(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class VectorUpdateCountResponse:
     count: int
     """
     Number of vectors modified.
     """
 
 
-class UpdateVectorParams(BaseModel):
+@dataclass
+class UpdateVectorParams:
     """
     Document to update.
     """
 
-    class Config:
-        extra = Extra.allow
-
     id: str
     """
     Document ID.
     """
     vector: Optional[List[float]] = None
     """
     Embedding vector.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     Document metadata.
     """
 
 
-class UpdateVectorsParams(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class UpdateVectorsParams:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
     """
-    vectors: Annotated[List[UpdateVectorParams], Field(max_items=100)]
+    vectors: List[UpdateVectorParams]
     """
     Vectors to upsert.
     """
 
 
-class DeleteVectorsParams(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class DeleteVectorsParams:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
     """
-    ids: Annotated[List[str], Field(max_items=100)]
+    ids: List[str]
     """
     Document IDs to delete.
     """
 
 
-class QueryVectorStoreParams(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class QueryVectorStoreParams:
     name: str
     """
     Vector store to query against.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
@@ -1179,19 +1223,19 @@
     """
     Vector to use for the query.
     """
     query_strings: Optional[List[str]] = None
     """
     Texts to embed and use for the query.
     """
-    top_k: Annotated[Optional[int], Field(ge=1, le=1000)] = 10
+    top_k: Optional[int] = 10
     """
     Number of results to return.
     """
-    ef_search: Annotated[Optional[int], Field(ge=1, le=1000)] = 40
+    ef_search: Optional[int] = 40
     """
     The size of the dynamic candidate list for searching the index graph.
     """
     include_values: Optional[bool] = False
     """
     Include the values of the vectors in the response.
     """
@@ -1201,18 +1245,16 @@
     """
     filters: Optional[Dict[str, Any]] = None
     """
     Filter metadata by key-value pairs.
     """
 
 
-class VectorStoreQueryResult(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class VectorStoreQueryResult:
     id: str
     """
     Document ID.
     """
     distance: float
     """
     Similarity score.
@@ -1223,18 +1265,16 @@
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     Document metadata.
     """
 
 
-class QueryVectorStoreResponse(BaseModel):
-    class Config:
-        extra = Extra.allow
-
+@dataclass
+class QueryVectorStoreResponse:
     results: List[List[VectorStoreQueryResult]]
     """
     Query results.
     """
     name: Optional[str] = None
     """
     Vector store name.
```

### Comparing `substrate-120240315.0.1/substrate/core/sb.py` & `substrate-120240403.0.1/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-120240315.0.1/substrate/future_dataclass_models.py` & `substrate-120240403.0.1/substrate/future_dataclass_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,62 +27,98 @@
     """
     (Future reference)
     A message providing more details about the error.
     """
 
 
 @dataclass
-class ResponseFormat:
+class FutureGenerateTextIn:
     """
     (Future reference)
     """
 
-    type: Literal["json_object", "text"]
+    prompt: str
     """
     (Future reference)
-    Type of response.
+    Input prompt.
     """
-    json_schema: Optional[Dict[str, Any]] = None
+    temperature: Optional[int] = 4
     """
     (Future reference)
-    JSON schema to guide `json_object` response.
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    (Future reference)
+    Maximum number of tokens to generate.
+    """
+    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    """
+    (Future reference)
+    Selected node.
     """
 
 
 @dataclass
-class FutureGenerateTextIn:
+class FutureGenerateTextOut:
     """
     (Future reference)
     """
 
-    prompt: str
+    text: Optional[str] = None
     """
     (Future reference)
-    Input prompt.
+    Text response.
     """
-    model: Optional[Literal["mistral-7b-instruct"]] = "mistral-7b-instruct"
+
+
+@dataclass
+class FutureGenerateJSONIn:
     """
     (Future reference)
-    Selected model.
     """
-    response_format: Optional[ResponseFormat] = None
+
+    prompt: str
     """
     (Future reference)
-    Format of the response.
+    Input prompt.
+    """
+    json_schema: Dict[str, Any]
+    """
+    (Future reference)
+    JSON schema to guide `json_object` response.
     """
     temperature: Optional[int] = 4
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
-    max_tokens: Optional[int] = 800
+    max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
+    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    """
+    (Future reference)
+    Selected node.
+    """
+
+
+@dataclass
+class FutureGenerateJSONOut:
+    """
+    (Future reference)
+    """
+
+    json_object: Optional[Dict[str, Any]] = None
+    """
+    (Future reference)
+    JSON response.
+    """
 
 
 @dataclass
 class FutureMultiGenerateTextIn:
     """
     (Future reference)
     """
@@ -93,94 +129,178 @@
     Input prompt.
     """
     num_choices: int
     """
     (Future reference)
     Number of choices to generate.
     """
-    model: Optional[Literal["mistral-7b-instruct"]] = "mistral-7b-instruct"
+    temperature: Optional[int] = 4
     """
     (Future reference)
-    Selected model.
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
-    response_format: Optional[ResponseFormat] = None
+    max_tokens: Optional[int] = None
     """
     (Future reference)
-    Format of the response.
+    Maximum number of tokens to generate.
+    """
+    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    """
+    (Future reference)
+    Selected node.
+    """
+
+
+@dataclass
+class FutureMultiGenerateTextOut:
+    """
+    (Future reference)
+    """
+
+    choices: List[FutureGenerateTextOut]
+
+
+@dataclass
+class FutureMultiGenerateJSONIn:
+    """
+    (Future reference)
+    """
+
+    prompt: str
+    """
+    (Future reference)
+    Input prompt.
+    """
+    json_schema: Dict[str, Any]
+    """
+    (Future reference)
+    JSON schema to guide `json_object` response.
+    """
+    num_choices: int
+    """
+    (Future reference)
+    Number of choices to generate.
     """
     temperature: Optional[int] = 4
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
-    max_tokens: Optional[int] = 800
+    max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
+    node: Optional[Literal["Mistral7BInstruct"]] = "Mistral7BInstruct"
+    """
+    (Future reference)
+    Selected node.
+    """
 
 
 @dataclass
-class FutureGenerateTextOut:
+class FutureMultiGenerateJSONOut:
+    """
+    (Future reference)
+    """
+
+    choices: List[FutureGenerateJSONOut]
+
+
+@dataclass
+class FutureMistral7BInstructIn:
+    """
+    (Future reference)
+    """
+
+    prompt: str
+    """
+    (Future reference)
+    Input prompt.
+    """
+    num_choices: int
+    """
+    (Future reference)
+    Number of choices to generate.
+    """
+    json_schema: Optional[Dict[str, Any]] = None
+    """
+    (Future reference)
+    JSON schema to guide response.
+    """
+    temperature: Optional[float] = None
+    """
+    (Future reference)
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    (Future reference)
+    Maximum number of tokens to generate.
+    """
+
+
+@dataclass
+class Mistral7BInstructChoice:
     """
     (Future reference)
     """
 
     text: Optional[str] = None
     """
     (Future reference)
-    Text response.
+    Text response, if `json_schema` was not provided.
     """
     json_object: Optional[Dict[str, Any]] = None
     """
     (Future reference)
-    JSON response.
+    JSON response, if `json_schema` was provided.
     """
 
 
 @dataclass
-class FutureMultiGenerateTextOut:
+class FutureMistral7BInstructOut:
     """
     (Future reference)
     """
 
-    choices: List[FutureGenerateTextOut]
+    choices: List[Mistral7BInstructChoice]
 
 
 @dataclass
 class FutureGenerateTextVisionIn:
     """
     (Future reference)
     """
 
     prompt: str
     """
     (Future reference)
     Text prompt.
     """
-    image_uris: Optional[List[str]] = None
+    image_uris: List[str]
     """
     (Future reference)
     Image prompts.
     """
-    model: Optional[Literal["firellava-13b"]] = "firellava-13b"
-    """
-    (Future reference)
-    Selected model.
-    """
     temperature: Optional[int] = 4
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = 800
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
+    node: Optional[Literal["Firellava13B"]] = "Firellava13B"
+    """
+    (Future reference)
+    Selected node.
+    """
 
 
 @dataclass
 class FutureGenerateTextVisionOut:
     """
     (Future reference)
     """
@@ -189,82 +309,88 @@
     """
     (Future reference)
     Text response.
     """
 
 
 @dataclass
-class FutureGenerateImageIn:
+class FutureFirellava13BIn:
     """
     (Future reference)
     """
 
     prompt: str
     """
     (Future reference)
     Text prompt.
     """
-    image_prompt_uri: Optional[str] = None
+    image_uris: List[str]
     """
     (Future reference)
-    Image prompt.
+    Image prompts.
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
+    temperature: Optional[float] = None
     """
     (Future reference)
-    Selected model.
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
-    image_influence: Optional[float] = 5
+    max_tokens: Optional[int] = 800
     """
     (Future reference)
-    Controls the influence of the image prompt on the generated output.
+    Maximum number of tokens to generate.
     """
-    negative_prompt: Optional[str] = None
+
+
+@dataclass
+class FutureFirellava13BOut:
     """
     (Future reference)
-    Negative input prompt.
     """
-    store: Optional[str] = None
+
+    text: str
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Text response.
     """
-    width: Optional[int] = None
+
+
+@dataclass
+class FutureGenerateImageIn:
     """
     (Future reference)
-    Width of output image, in pixels.
     """
-    height: Optional[int] = None
+
+    prompt: str
     """
     (Future reference)
-    Height of output image, in pixels.
+    Text prompt.
+    """
+    store: Optional[str] = None
+    """
+    (Future reference)
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    seed: Optional[int] = None
+    node: Optional[Literal["StableDiffusionXL"]] = "StableDiffusionXL"
     """
     (Future reference)
-    Seed for deterministic generation. Default is a random seed.
+    Selected node.
     """
 
 
 @dataclass
 class FutureGenerateImageOut:
     """
     (Future reference)
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
-    seed: int
-    """
-    (Future reference)
-    The random noise seed used for generation.
-    """
 
 
 @dataclass
 class FutureMultiGenerateImageIn:
     """
     (Future reference)
     """
@@ -275,138 +401,179 @@
     Text prompt.
     """
     num_images: int
     """
     (Future reference)
     Number of images to generate.
     """
-    image_prompt_uri: Optional[str] = None
+    store: Optional[str] = None
     """
     (Future reference)
-    Image prompt.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
+    node: Optional[Literal["StableDiffusionXL"]] = "StableDiffusionXL"
     """
     (Future reference)
-    Selected model.
+    Selected node.
+    """
+
+
+@dataclass
+class FutureMultiGenerateImageOut:
     """
-    image_influence: Optional[float] = 5
+    (Future reference)
+    """
+
+    outputs: List[FutureGenerateImageOut]
+
+
+@dataclass
+class FutureStableDiffusionXLIn:
     """
     (Future reference)
-    Controls the influence of the image prompt on the generated output.
+    """
+
+    prompt: str
+    """
+    (Future reference)
+    Text prompt.
     """
     negative_prompt: Optional[str] = None
     """
     (Future reference)
     Negative input prompt.
     """
+    steps: Optional[int] = None
+    """
+    (Future reference)
+    Number of diffusion steps.
+    """
+    num_images: Optional[int] = None
+    """
+    (Future reference)
+    Number of images to generate.
+    """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
+    height: Optional[int] = None
+    """
+    (Future reference)
+    Height of output image, in pixels.
+    """
     width: Optional[int] = None
     """
     (Future reference)
     Width of output image, in pixels.
     """
-    height: Optional[int] = None
+    seeds: Optional[int] = None
     """
     (Future reference)
-    Height of output image, in pixels.
+    Seeds for deterministic generation. Default is a random seed.
     """
-    seeds: Optional[List[int]] = None
+    guidance_scale: Optional[float] = 5
     """
     (Future reference)
-    Random noise seeds. Default is random seeds for each generation.
+    Higher values adhere to the text prompt more strongly, typically at the expense of image quality.
     """
 
 
 @dataclass
-class FutureMultiGenerateImageOut:
+class StableDiffusionImage:
     """
     (Future reference)
     """
 
-    outputs: List[FutureGenerateImageOut]
+    image_uri: str
+    """
+    (Future reference)
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+    seed: int
+    """
+    (Future reference)
+    The random noise seed used for generation.
+    """
 
 
 @dataclass
-class FutureControlledGenerateImageIn:
+class FutureStableDiffusionXLOut:
     """
     (Future reference)
     """
 
-    image_uri: str
+    outputs: List[StableDiffusionImage]
+
+
+@dataclass
+class FutureStableDiffusionXLIPAdapterIn:
     """
     (Future reference)
-    Input image.
     """
-    control_method: Literal["edge", "depth", "illusion"]
+
+    prompt: str
     """
     (Future reference)
-    Strategy to control generation using the input image.
+    Text prompt.
     """
-    prompt: str
+    num_images: int
     """
     (Future reference)
-    Text prompt.
+    Number of images to generate.
     """
-    output_resolution: Optional[int] = 1024
+    image_prompt_uri: Optional[str] = None
     """
     (Future reference)
-    Resolution of the output image, in pixels.
+    Image prompt.
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
+    ip_adapter_scale: Optional[float] = None
     """
     (Future reference)
-    Selected model.
+    Controls the influence of the image prompt on the generated output.
     """
     negative_prompt: Optional[str] = None
     """
     (Future reference)
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    image_influence: Optional[float] = 9
+    width: Optional[int] = None
     """
     (Future reference)
-    Controls the influence of the input image on the generated output.
+    Width of output image, in pixels.
     """
-    seed: Optional[int] = None
+    height: Optional[int] = None
     """
     (Future reference)
-    Seed for deterministic generation. Default is a random seed.
+    Height of output image, in pixels.
     """
-
-
-@dataclass
-class FutureControlledGenerateImageOut:
+    seeds: Optional[List[int]] = None
     """
     (Future reference)
+    Random noise seeds. Default is random seeds for each generation.
     """
 
-    image_uri: str
-    """
-    (Future reference)
-    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
-    """
-    seed: int
+
+@dataclass
+class FutureStableDiffusionXLIPAdapterOut:
     """
     (Future reference)
-    The random noise seed used for generation.
     """
 
+    outputs: List[StableDiffusionImage]
+
 
 @dataclass
-class FutureMultiControlledGenerateImageIn:
+class FutureStableDiffusionXLControlNetIn:
     """
     (Future reference)
     """
 
     image_uri: str
     """
     (Future reference)
@@ -428,48 +595,43 @@
     Number of images to generate.
     """
     output_resolution: Optional[int] = 1024
     """
     (Future reference)
     Resolution of the output image, in pixels.
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
-    """
-    (Future reference)
-    Selected model.
-    """
     negative_prompt: Optional[str] = None
     """
     (Future reference)
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    image_influence: Optional[float] = 9
+    conditioning_scale: Optional[float] = None
     """
     (Future reference)
     Controls the influence of the input image on the generated output.
     """
     seeds: Optional[List[int]] = None
     """
     (Future reference)
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 @dataclass
-class FutureMultiControlledGenerateImageOut:
+class FutureStableDiffusionXLControlNetOut:
     """
     (Future reference)
     """
 
-    outputs: List[FutureControlledGenerateImageOut]
+    outputs: List[StableDiffusionImage]
 
 
 @dataclass
 class FutureGenerativeEditImageIn:
     """
     (Future reference)
     """
@@ -485,76 +647,88 @@
     Text prompt.
     """
     mask_image_uri: Optional[str] = None
     """
     (Future reference)
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
-    image_prompt_uri: Optional[str] = None
+    store: Optional[str] = None
     """
     (Future reference)
-    Image prompt.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    output_resolution: Optional[int] = 1024
+    node: Optional[Literal["StableDiffusionXLInpaint"]] = "StableDiffusionXLInpaint"
     """
     (Future reference)
-    Resolution of the output image, in pixels.
+    Selected node.
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
+
+
+@dataclass
+class FutureGenerativeEditImageOut:
     """
     (Future reference)
-    Selected model.
     """
-    strength: Optional[float] = 8
+
+    image_uri: str
     """
     (Future reference)
-    Controls the strength of the generation process.
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
-    image_prompt_influence: Optional[float] = 5
+
+
+@dataclass
+class FutureMultiGenerativeEditImageIn:
     """
     (Future reference)
-    Controls the influence of the image prompt on the generated output.
     """
-    negative_prompt: Optional[str] = None
+
+    image_uri: str
     """
     (Future reference)
-    Negative input prompt.
+    Original image.
     """
-    store: Optional[str] = None
+    prompt: str
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Text prompt.
     """
-    seed: Optional[int] = None
+    num_images: int
     """
     (Future reference)
-    Seed for deterministic generation. Default is a random seed.
+    Number of images to generate.
     """
-
-
-@dataclass
-class FutureGenerativeEditImageOut:
+    mask_image_uri: Optional[str] = None
     """
     (Future reference)
+    Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
-
-    image_uri: str
+    store: Optional[str] = None
     """
     (Future reference)
-    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    seed: int
+    node: Optional[Literal["StableDiffusionXLInpaint"]] = "StableDiffusionXLInpaint"
     """
     (Future reference)
-    The random noise seed used for generation.
+    Selected node.
     """
 
 
 @dataclass
-class FutureMultiGenerativeEditImageIn:
+class FutureMultiGenerativeEditImageOut:
+    """
+    (Future reference)
+    """
+
+    outputs: List[FutureGenerativeEditImageOut]
+
+
+@dataclass
+class FutureStableDiffusionXLInpaintIn:
     """
     (Future reference)
     """
 
     image_uri: str
     """
     (Future reference)
@@ -571,63 +745,48 @@
     Number of images to generate.
     """
     mask_image_uri: Optional[str] = None
     """
     (Future reference)
     Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
-    image_prompt_uri: Optional[str] = None
-    """
-    (Future reference)
-    Image prompt.
-    """
     output_resolution: Optional[int] = 1024
     """
     (Future reference)
     Resolution of the output image, in pixels.
     """
-    model: Optional[Literal["stablediffusion-xl"]] = "stablediffusion-xl"
-    """
-    (Future reference)
-    Selected model.
-    """
     negative_prompt: Optional[str] = None
     """
     (Future reference)
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    strength: Optional[float] = 8
+    strength: Optional[float] = 0.5
     """
     (Future reference)
     Controls the strength of the generation process.
     """
-    image_prompt_influence: Optional[float] = 5
-    """
-    (Future reference)
-    Controls the influence of the image prompt on the generated output.
-    """
     seeds: Optional[List[int]] = None
     """
     (Future reference)
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 @dataclass
-class FutureMultiGenerativeEditImageOut:
+class FutureStableDiffusionXLInpaintOut:
     """
     (Future reference)
     """
 
-    outputs: List[FutureGenerativeEditImageOut]
+    outputs: List[StableDiffusionImage]
 
 
 @dataclass
 class BoundingBox:
     """
     (Future reference)
     """
@@ -805,20 +964,20 @@
     """
     (Future reference)
     Input image.
     """
     point_prompts: Optional[List[Point]] = None
     """
     (Future reference)
-    Point prompts, to detect a segment under the point. One of `point_prompt` or `box_prompt` must be set.
+    Point prompts, to detect a segment under the point. One of `point_prompts` or `box_prompts` must be set.
     """
     box_prompts: Optional[List[BoundingBox]] = None
     """
     (Future reference)
-    Box prompts, to detect a segment within the bounding box. One of `point_prompt` or `box_prompt` must be set.
+    Box prompts, to detect a segment within the bounding box. One of `point_prompts` or `box_prompts` must be set.
     """
     model: Optional[Literal["segment-anything"]] = "segment-anything"
     """
     (Future reference)
     Selected model.
     """
     store: Optional[str] = None
@@ -1034,15 +1193,15 @@
     """
 
     vector: List[float]
     """
     (Future reference)
     Embedding vector.
     """
-    document_id: Optional[str] = None
+    doc_id: Optional[str] = None
     """
     (Future reference)
     Vector store document ID.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     (Future reference)
@@ -1057,19 +1216,14 @@
     """
 
     text: str
     """
     (Future reference)
     Text to embed.
     """
-    model: Optional[Literal["jina-v2", "clip"]] = "jina-v2"
-    """
-    (Future reference)
-    Selected model.
-    """
     store: Optional[str] = None
     """
     (Future reference)
     [Vector store](/docs/vector-stores) identifier.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
@@ -1077,19 +1231,24 @@
     Metadata that can be used to query the vector store. Ignored if `store` is unset.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     (Future reference)
     Choose keys from `metadata` to embed with text.
     """
-    document_id: Optional[str] = None
+    doc_id: Optional[str] = None
     """
     (Future reference)
     Vector store document ID. Ignored if `store` is unset.
     """
+    node: Optional[Literal["JinaV2", "CLIP"]] = "JinaV2"
+    """
+    (Future reference)
+    Selected node.
+    """
 
 
 @dataclass
 class FutureEmbedTextOut:
     """
     (Future reference)
     """
@@ -1113,15 +1272,15 @@
     Text to embed.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     (Future reference)
     Metadata that can be used to query the vector store. Ignored if `store` is unset.
     """
-    document_id: Optional[str] = None
+    doc_id: Optional[str] = None
     """
     (Future reference)
     Vector store document ID. Ignored if `store` is unset.
     """
 
 
 @dataclass
@@ -1131,33 +1290,69 @@
     """
 
     items: List[EmbedTextItem]
     """
     (Future reference)
     Items to embed.
     """
-    model: Optional[Literal["jina-v2", "clip"]] = "jina-v2"
+    store: Optional[str] = None
+    """
+    (Future reference)
+    [Vector store](/docs/vector-stores) identifier.
+    """
+    embedded_metadata_keys: Optional[List[str]] = None
+    """
+    (Future reference)
+    Choose keys from `metadata` to embed with text.
+    """
+    node: Optional[Literal["JinaV2", "CLIP"]] = "JinaV2"
+    """
+    (Future reference)
+    Selected node.
+    """
+
+
+@dataclass
+class FutureMultiEmbedTextOut:
     """
     (Future reference)
-    Selected model.
+    """
+
+    embeddings: List[Embedding]
+    """
+    (Future reference)
+    Generated embeddings.
+    """
+
+
+@dataclass
+class FutureJinaV2In:
+    """
+    (Future reference)
+    """
+
+    items: List[EmbedTextItem]
+    """
+    (Future reference)
+    Items to embed.
     """
     store: Optional[str] = None
     """
     (Future reference)
     [Vector store](/docs/vector-stores) identifier.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     (Future reference)
     Choose keys from `metadata` to embed with text.
     """
 
 
 @dataclass
-class FutureMultiEmbedTextOut:
+class FutureJinaV2Out:
     """
     (Future reference)
     """
 
     embeddings: List[Embedding]
     """
     (Future reference)
@@ -1172,29 +1367,29 @@
     """
 
     image_uri: str
     """
     (Future reference)
     Image to embed.
     """
-    model: Optional[Literal["clip"]] = "clip"
-    """
-    (Future reference)
-    Selected model.
-    """
     store: Optional[str] = None
     """
     (Future reference)
     [Vector store](/docs/vector-stores) identifier.
     """
-    document_id: Optional[str] = None
+    doc_id: Optional[str] = None
     """
     (Future reference)
     Vector store document ID. Ignored if `store` is unset.
     """
+    node: Optional[Literal["CLIP"]] = "CLIP"
+    """
+    (Future reference)
+    Selected node.
+    """
 
 
 @dataclass
 class FutureEmbedImageOut:
     """
     (Future reference)
     """
@@ -1213,15 +1408,43 @@
     """
 
     image_uri: str
     """
     (Future reference)
     Image to embed.
     """
-    document_id: Optional[str] = None
+    doc_id: Optional[str] = None
+    """
+    (Future reference)
+    Vector store document ID. Ignored if `store` is unset.
+    """
+
+
+@dataclass
+class EmbedTextOrImageItem:
+    """
+    (Future reference)
+    """
+
+    image_uri: Optional[str] = None
+    """
+    (Future reference)
+    Image to embed.
+    """
+    text: Optional[str] = None
+    """
+    (Future reference)
+    Text to embed.
+    """
+    metadata: Optional[Dict[str, Any]] = None
+    """
+    (Future reference)
+    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    """
+    doc_id: Optional[str] = None
     """
     (Future reference)
     Vector store document ID. Ignored if `store` is unset.
     """
 
 
 @dataclass
@@ -1236,18 +1459,18 @@
     Items to embed.
     """
     store: Optional[str] = None
     """
     (Future reference)
     [Vector store](/docs/vector-stores) identifier.
     """
-    model: Optional[Literal["clip"]] = "clip"
+    node: Optional[Literal["CLIP"]] = "CLIP"
     """
     (Future reference)
-    Selected model.
+    Selected node.
     """
 
 
 @dataclass
 class FutureMultiEmbedImageOut:
     """
     (Future reference)
@@ -1257,18 +1480,53 @@
     """
     (Future reference)
     Generated embeddings.
     """
 
 
 @dataclass
+class FutureCLIPIn:
+    """
+    (Future reference)
+    """
+
+    items: List[EmbedTextOrImageItem]
+    """
+    (Future reference)
+    Items to embed.
+    """
+    embedded_metadata_keys: Optional[List[str]] = None
+    """
+    (Future reference)
+    Choose keys from `metadata` to embed with text, when embedding and storing text documents.
+    """
+    store: Optional[str] = None
+    """
+    (Future reference)
+    [Vector store](/docs/vector-stores) identifier.
+    """
+
+
+@dataclass
+class FutureCLIPOut:
+    """
+    (Future reference)
+    """
+
+    embeddings: List[Embedding]
+    """
+    (Future reference)
+    Generated embeddings.
+    """
+
+
+@dataclass
 class VectorStoreParams:
     """
     (Future reference)
-    Fields describing a vector store and its associated index.
     """
 
     name: str
     """
     (Future reference)
     Vector store name.
     """
```

### Comparing `substrate-120240315.0.1/substrate/nodes.py` & `substrate-120240403.0.1/substrate/nodes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,103 +1,127 @@
 """
 ꩜ Substrate
 @GENERATED FILE
-20240315.20240321
+20240403.20240403
 """
 
 from .substrate import SubstrateResponse
 from .core.corenode import CoreNode
 from .dataclass_models import (
+    CLIPOut,
+    JinaV2Out,
     FillMaskOut,
     EmbedTextOut,
     EmbedImageOut,
+    Firellava13BOut,
+    GenerateJSONOut,
     GenerateTextOut,
     UpscaleImageOut,
     GenerateImageOut,
     DetectSegmentsOut,
     GenerateSpeechOut,
     MultiEmbedTextOut,
     MultiEmbedImageOut,
     TranscribeMediaOut,
     RemoveBackgroundOut,
+    Mistral7BInstructOut,
+    MultiGenerateJSONOut,
     MultiGenerateTextOut,
+    StableDiffusionXLOut,
     GenerateTextVisionOut,
     MultiGenerateImageOut,
     GenerativeEditImageOut,
-    ControlledGenerateImageOut,
     MultiGenerativeEditImageOut,
-    MultiControlledGenerateImageOut,
+    StableDiffusionXLInpaintOut,
+    StableDiffusionXLIPAdapterOut,
+    StableDiffusionXLControlNetOut,
 )
 from .typeddict_models import (
+    CLIPIn,
+    JinaV2In,
     FillMaskIn,
     EmbedTextIn,
     EmbedImageIn,
+    Firellava13BIn,
+    GenerateJSONIn,
     GenerateTextIn,
     UpscaleImageIn,
     GenerateImageIn,
     DetectSegmentsIn,
     GenerateSpeechIn,
     MultiEmbedTextIn,
     MultiEmbedImageIn,
     TranscribeMediaIn,
     RemoveBackgroundIn,
+    Mistral7BInstructIn,
+    MultiGenerateJSONIn,
     MultiGenerateTextIn,
+    StableDiffusionXLIn,
     GenerateTextVisionIn,
     MultiGenerateImageIn,
     GenerativeEditImageIn,
-    ControlledGenerateImageIn,
     MultiGenerativeEditImageIn,
-    MultiControlledGenerateImageIn,
+    StableDiffusionXLInpaintIn,
+    StableDiffusionXLIPAdapterIn,
+    StableDiffusionXLControlNetIn,
 )
 from .future_dataclass_models import (
+    FutureCLIPOut,
+    FutureJinaV2Out,
     FutureFillMaskOut,
     FutureEmbedTextOut,
     FutureEmbedImageOut,
+    FutureFirellava13BOut,
+    FutureGenerateJSONOut,
     FutureGenerateTextOut,
     FutureUpscaleImageOut,
     FutureGenerateImageOut,
     FutureDetectSegmentsOut,
     FutureGenerateSpeechOut,
     FutureMultiEmbedTextOut,
     FutureMultiEmbedImageOut,
     FutureTranscribeMediaOut,
     FutureRemoveBackgroundOut,
+    FutureMistral7BInstructOut,
+    FutureMultiGenerateJSONOut,
     FutureMultiGenerateTextOut,
+    FutureStableDiffusionXLOut,
     FutureGenerateTextVisionOut,
     FutureMultiGenerateImageOut,
     FutureGenerativeEditImageOut,
-    FutureControlledGenerateImageOut,
     FutureMultiGenerativeEditImageOut,
-    FutureMultiControlledGenerateImageOut,
+    FutureStableDiffusionXLInpaintOut,
+    FutureStableDiffusionXLIPAdapterOut,
+    FutureStableDiffusionXLControlNetOut,
 )
 
 
 class GenerateText(CoreNode):
     """
     Generate text using a language model.
 
     https://substrate.run/library#GenerateText
     """
 
     def __init__(self, args: GenerateTextIn):
         """
-        Input arguments: `prompt`, `model` (optional), `response_format` (optional), `temperature` (optional), `max_tokens` (optional)
+        Input arguments: `prompt`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
-        Output fields: `future.text` (optional), `future.json_object` (optional)
+        Output fields: `future.text` (optional)
 
         https://substrate.run/library#GenerateText
         """
         super().__init__(**args)
         self.node = "GenerateText"
 
     def output(self, response: SubstrateResponse) -> GenerateTextOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.text` (optional), `future.json_object` (optional)
+        Output fields: `future.text` (optional)
 
         https://substrate.run/library#GenerateText
         """
         klass = GenerateTextOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
@@ -107,15 +131,15 @@
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
     def future(self) -> FutureGenerateTextOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.text` (optional), `future.json_object` (optional)
+        Output fields: `future.text` (optional)
 
         https://substrate.run/library#GenerateText
         """
         return super().future  # type: ignore
 
 
 class MultiGenerateText(CoreNode):
@@ -123,15 +147,15 @@
     Generate multiple text choices using a language model.
 
     https://substrate.run/library#MultiGenerateText
     """
 
     def __init__(self, args: MultiGenerateTextIn):
         """
-        Input arguments: `prompt`, `num_choices`, `model` (optional), `response_format` (optional), `temperature` (optional), `max_tokens` (optional)
+        Input arguments: `prompt`, `num_choices`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
         Output fields: `future.choices`
 
         https://substrate.run/library#MultiGenerateText
         """
         super().__init__(**args)
         self.node = "MultiGenerateText"
@@ -161,24 +185,118 @@
         Output fields: `future.choices`
 
         https://substrate.run/library#MultiGenerateText
         """
         return super().future  # type: ignore
 
 
+class GenerateJSON(CoreNode):
+    """
+    Generate JSON using a language model.
+
+    https://substrate.run/library#GenerateJSON
+    """
+
+    def __init__(self, args: GenerateJSONIn):
+        """
+        Input arguments: `prompt`, `json_schema`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
+
+        Output fields: `future.json_object` (optional)
+
+        https://substrate.run/library#GenerateJSON
+        """
+        super().__init__(**args)
+        self.node = "GenerateJSON"
+
+    def output(self, response: SubstrateResponse) -> GenerateJSONOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.json_object` (optional)
+
+        https://substrate.run/library#GenerateJSON
+        """
+        klass = GenerateJSONOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureGenerateJSONOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.json_object` (optional)
+
+        https://substrate.run/library#GenerateJSON
+        """
+        return super().future  # type: ignore
+
+
+class MultiGenerateJSON(CoreNode):
+    """
+    Generate multiple JSON choices using a language model.
+
+    https://substrate.run/library#MultiGenerateJSON
+    """
+
+    def __init__(self, args: MultiGenerateJSONIn):
+        """
+        Input arguments: `prompt`, `json_schema`, `num_choices`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#MultiGenerateJSON
+        """
+        super().__init__(**args)
+        self.node = "MultiGenerateJSON"
+
+    def output(self, response: SubstrateResponse) -> MultiGenerateJSONOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#MultiGenerateJSON
+        """
+        klass = MultiGenerateJSONOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureMultiGenerateJSONOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#MultiGenerateJSON
+        """
+        return super().future  # type: ignore
+
+
 class GenerateTextVision(CoreNode):
     """
-    Generate text by prompting with text and images using a vision-language model.
+    Generate text with image input.
 
     https://substrate.run/library#GenerateTextVision
     """
 
     def __init__(self, args: GenerateTextVisionIn):
         """
-        Input arguments: `prompt`, `image_uris` (optional), `model` (optional), `temperature` (optional), `max_tokens` (optional)
+        Input arguments: `prompt`, `image_uris`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
         Output fields: `future.text`
 
         https://substrate.run/library#GenerateTextVision
         """
         super().__init__(**args)
         self.node = "GenerateTextVision"
@@ -208,37 +326,131 @@
         Output fields: `future.text`
 
         https://substrate.run/library#GenerateTextVision
         """
         return super().future  # type: ignore
 
 
+class Mistral7BInstruct(CoreNode):
+    """
+    Generate text using Mistral 7B Instruct.
+
+    https://substrate.run/library#Mistral7BInstruct
+    """
+
+    def __init__(self, args: Mistral7BInstructIn):
+        """
+        Input arguments: `prompt`, `num_choices`, `json_schema` (optional), `temperature` (optional), `max_tokens` (optional)
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#Mistral7BInstruct
+        """
+        super().__init__(**args)
+        self.node = "Mistral7BInstruct"
+
+    def output(self, response: SubstrateResponse) -> Mistral7BInstructOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#Mistral7BInstruct
+        """
+        klass = Mistral7BInstructOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureMistral7BInstructOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#Mistral7BInstruct
+        """
+        return super().future  # type: ignore
+
+
+class Firellava13B(CoreNode):
+    """
+    Generate text with image input using FireLLaVA 13B.
+
+    https://substrate.run/library#Firellava13B
+    """
+
+    def __init__(self, args: Firellava13BIn):
+        """
+        Input arguments: `prompt`, `image_uris`, `temperature` (optional), `max_tokens` (optional)
+
+        Output fields: `future.text`
+
+        https://substrate.run/library#Firellava13B
+        """
+        super().__init__(**args)
+        self.node = "Firellava13B"
+
+    def output(self, response: SubstrateResponse) -> Firellava13BOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.text`
+
+        https://substrate.run/library#Firellava13B
+        """
+        klass = Firellava13BOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureFirellava13BOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.text`
+
+        https://substrate.run/library#Firellava13B
+        """
+        return super().future  # type: ignore
+
+
 class GenerateImage(CoreNode):
     """
     Generate an image.
 
     https://substrate.run/library#GenerateImage
     """
 
     def __init__(self, args: GenerateImageIn):
         """
-        Input arguments: `prompt`, `image_prompt_uri` (optional), `model` (optional), `image_influence` (optional), `negative_prompt` (optional), `store` (optional), `width` (optional), `height` (optional), `seed` (optional)
+        Input arguments: `prompt`, `store` (optional), `node` (optional)
 
-        Output fields: `future.image_uri`, `future.seed`
+        Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerateImage
         """
         super().__init__(**args)
         self.node = "GenerateImage"
 
     def output(self, response: SubstrateResponse) -> GenerateImageOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.image_uri`, `future.seed`
+        Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerateImage
         """
         klass = GenerateImageOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
@@ -248,15 +460,15 @@
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
     def future(self) -> FutureGenerateImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.image_uri`, `future.seed`
+        Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerateImage
         """
         return super().future  # type: ignore
 
 
 class MultiGenerateImage(CoreNode):
@@ -264,15 +476,15 @@
     Generate multiple images.
 
     https://substrate.run/library#MultiGenerateImage
     """
 
     def __init__(self, args: MultiGenerateImageIn):
         """
-        Input arguments: `prompt`, `image_prompt_uri` (optional), `num_images`, `model` (optional), `image_influence` (optional), `negative_prompt` (optional), `store` (optional), `width` (optional), `height` (optional), `seeds` (optional)
+        Input arguments: `prompt`, `num_images`, `store` (optional), `node` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateImage
         """
         super().__init__(**args)
         self.node = "MultiGenerateImage"
@@ -302,198 +514,292 @@
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateImage
         """
         return super().future  # type: ignore
 
 
-class ControlledGenerateImage(CoreNode):
+class GenerativeEditImage(CoreNode):
     """
-    Generate an image with generation controlled by an input image.
+    Edit an image using image generation.
 
-    https://substrate.run/library#ControlledGenerateImage
+    https://substrate.run/library#GenerativeEditImage
     """
 
-    def __init__(self, args: ControlledGenerateImageIn):
+    def __init__(self, args: GenerativeEditImageIn):
         """
-        Input arguments: `image_uri`, `control_method`, `prompt`, `output_resolution` (optional), `model` (optional), `negative_prompt` (optional), `store` (optional), `image_influence` (optional), `seed` (optional)
+        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `store` (optional), `node` (optional)
 
-        Output fields: `future.image_uri`, `future.seed`
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#ControlledGenerateImage
+        https://substrate.run/library#GenerativeEditImage
         """
         super().__init__(**args)
-        self.node = "ControlledGenerateImage"
+        self.node = "GenerativeEditImage"
 
-    def output(self, response: SubstrateResponse) -> ControlledGenerateImageOut:
+    def output(self, response: SubstrateResponse) -> GenerativeEditImageOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.image_uri`, `future.seed`
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#ControlledGenerateImage
+        https://substrate.run/library#GenerativeEditImage
         """
-        klass = ControlledGenerateImageOut
+        klass = GenerativeEditImageOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureControlledGenerateImageOut:  # type: ignore
+    def future(self) -> FutureGenerativeEditImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.image_uri`, `future.seed`
+        Output fields: `future.image_uri`
 
-        https://substrate.run/library#ControlledGenerateImage
+        https://substrate.run/library#GenerativeEditImage
         """
         return super().future  # type: ignore
 
 
-class MultiControlledGenerateImage(CoreNode):
+class MultiGenerativeEditImage(CoreNode):
     """
-    Generate multiple image outputs with generation controlled by an input image.
+    Edit multiple images using image generation.
 
-    https://substrate.run/library#MultiControlledGenerateImage
+    https://substrate.run/library#MultiGenerativeEditImage
     """
 
-    def __init__(self, args: MultiControlledGenerateImageIn):
+    def __init__(self, args: MultiGenerativeEditImageIn):
         """
-        Input arguments: `image_uri`, `control_method`, `prompt`, `num_images`, `output_resolution` (optional), `model` (optional), `negative_prompt` (optional), `store` (optional), `image_influence` (optional), `seeds` (optional)
+        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `store` (optional), `node` (optional)
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#MultiControlledGenerateImage
+        https://substrate.run/library#MultiGenerativeEditImage
         """
         super().__init__(**args)
-        self.node = "MultiControlledGenerateImage"
+        self.node = "MultiGenerativeEditImage"
 
-    def output(self, response: SubstrateResponse) -> MultiControlledGenerateImageOut:
+    def output(self, response: SubstrateResponse) -> MultiGenerativeEditImageOut:
         """
         Retrieve this node's output from a response.
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#MultiControlledGenerateImage
+        https://substrate.run/library#MultiGenerativeEditImage
         """
-        klass = MultiControlledGenerateImageOut
+        klass = MultiGenerativeEditImageOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureMultiControlledGenerateImageOut:  # type: ignore
+    def future(self) -> FutureMultiGenerativeEditImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#MultiControlledGenerateImage
+        https://substrate.run/library#MultiGenerativeEditImage
         """
         return super().future  # type: ignore
 
 
-class GenerativeEditImage(CoreNode):
+class StableDiffusionXL(CoreNode):
     """
-    Edit an image with a generative model.
+    Generate an image using Stable Diffusion XL.
 
-    https://substrate.run/library#GenerativeEditImage
+    https://substrate.run/library#StableDiffusionXL
     """
 
-    def __init__(self, args: GenerativeEditImageIn):
+    def __init__(self, args: StableDiffusionXLIn):
         """
-        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `image_prompt_uri` (optional), `output_resolution` (optional), `model` (optional), `strength` (optional), `image_prompt_influence` (optional), `negative_prompt` (optional), `store` (optional), `seed` (optional)
+        Input arguments: `prompt`, `negative_prompt` (optional), `steps` (optional), `num_images` (optional), `store` (optional), `height` (optional), `width` (optional), `seeds` (optional), `guidance_scale` (optional)
 
-        Output fields: `future.image_uri`, `future.seed`
+        Output fields: `future.outputs`
 
-        https://substrate.run/library#GenerativeEditImage
+        https://substrate.run/library#StableDiffusionXL
         """
         super().__init__(**args)
-        self.node = "GenerativeEditImage"
+        self.node = "StableDiffusionXL"
 
-    def output(self, response: SubstrateResponse) -> GenerativeEditImageOut:
+    def output(self, response: SubstrateResponse) -> StableDiffusionXLOut:
         """
         Retrieve this node's output from a response.
 
-        Output fields: `future.image_uri`, `future.seed`
+        Output fields: `future.outputs`
 
-        https://substrate.run/library#GenerativeEditImage
+        https://substrate.run/library#StableDiffusionXL
         """
-        klass = GenerativeEditImageOut
+        klass = StableDiffusionXLOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureGenerativeEditImageOut:  # type: ignore
+    def future(self) -> FutureStableDiffusionXLOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.image_uri`, `future.seed`
+        Output fields: `future.outputs`
 
-        https://substrate.run/library#GenerativeEditImage
+        https://substrate.run/library#StableDiffusionXL
         """
         return super().future  # type: ignore
 
 
-class MultiGenerativeEditImage(CoreNode):
+class StableDiffusionXLInpaint(CoreNode):
     """
-    Generate multiple image outputs modifying part of an image using a mask.
+    Inpaint an image using Stable Diffusion XL.
 
-    https://substrate.run/library#MultiGenerativeEditImage
+    https://substrate.run/library#StableDiffusionXLInpaint
     """
 
-    def __init__(self, args: MultiGenerativeEditImageIn):
+    def __init__(self, args: StableDiffusionXLInpaintIn):
         """
-        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `image_prompt_uri` (optional), `num_images`, `output_resolution` (optional), `model` (optional), `negative_prompt` (optional), `store` (optional), `strength` (optional), `image_prompt_influence` (optional), `seeds` (optional)
+        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `output_resolution` (optional), `negative_prompt` (optional), `store` (optional), `strength` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#MultiGenerativeEditImage
+        https://substrate.run/library#StableDiffusionXLInpaint
         """
         super().__init__(**args)
-        self.node = "MultiGenerativeEditImage"
+        self.node = "StableDiffusionXLInpaint"
 
-    def output(self, response: SubstrateResponse) -> MultiGenerativeEditImageOut:
+    def output(self, response: SubstrateResponse) -> StableDiffusionXLInpaintOut:
         """
         Retrieve this node's output from a response.
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#MultiGenerativeEditImage
+        https://substrate.run/library#StableDiffusionXLInpaint
         """
-        klass = MultiGenerativeEditImageOut
+        klass = StableDiffusionXLInpaintOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureMultiGenerativeEditImageOut:  # type: ignore
+    def future(self) -> FutureStableDiffusionXLInpaintOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#MultiGenerativeEditImage
+        https://substrate.run/library#StableDiffusionXLInpaint
+        """
+        return super().future  # type: ignore
+
+
+class StableDiffusionXLIPAdapter(CoreNode):
+    """
+    Generate an image using Stable Diffusion XL with an image prompt.
+
+    https://substrate.run/library#StableDiffusionXLIPAdapter
+    """
+
+    def __init__(self, args: StableDiffusionXLIPAdapterIn):
+        """
+        Input arguments: `prompt`, `image_prompt_uri` (optional), `num_images`, `ip_adapter_scale` (optional), `negative_prompt` (optional), `store` (optional), `width` (optional), `height` (optional), `seeds` (optional)
+
+        Output fields: `future.outputs`
+
+        https://substrate.run/library#StableDiffusionXLIPAdapter
+        """
+        super().__init__(**args)
+        self.node = "StableDiffusionXLIPAdapter"
+
+    def output(self, response: SubstrateResponse) -> StableDiffusionXLIPAdapterOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.outputs`
+
+        https://substrate.run/library#StableDiffusionXLIPAdapter
+        """
+        klass = StableDiffusionXLIPAdapterOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureStableDiffusionXLIPAdapterOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.outputs`
+
+        https://substrate.run/library#StableDiffusionXLIPAdapter
+        """
+        return super().future  # type: ignore
+
+
+class StableDiffusionXLControlNet(CoreNode):
+    """
+    Generate an image using Stable Diffusion XL structuring generation with an input image.
+
+    https://substrate.run/library#StableDiffusionXLControlNet
+    """
+
+    def __init__(self, args: StableDiffusionXLControlNetIn):
+        """
+        Input arguments: `image_uri`, `control_method`, `prompt`, `num_images`, `output_resolution` (optional), `negative_prompt` (optional), `store` (optional), `conditioning_scale` (optional), `seeds` (optional)
+
+        Output fields: `future.outputs`
+
+        https://substrate.run/library#StableDiffusionXLControlNet
+        """
+        super().__init__(**args)
+        self.node = "StableDiffusionXLControlNet"
+
+    def output(self, response: SubstrateResponse) -> StableDiffusionXLControlNetOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.outputs`
+
+        https://substrate.run/library#StableDiffusionXLControlNet
+        """
+        klass = StableDiffusionXLControlNetOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureStableDiffusionXLControlNetOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.outputs`
+
+        https://substrate.run/library#StableDiffusionXLControlNet
         """
         return super().future  # type: ignore
 
 
 class FillMask(CoreNode):
     """
     Edit an image with a generative model.
@@ -774,22 +1080,22 @@
         https://substrate.run/library#GenerateSpeech
         """
         return super().future  # type: ignore
 
 
 class EmbedText(CoreNode):
     """
-    Generate vector embedding for a text document.
+    Generate embedding for a text document.
 
     https://substrate.run/library#EmbedText
     """
 
     def __init__(self, args: EmbedTextIn):
         """
-        Input arguments: `text`, `model` (optional), `store` (optional), `metadata` (optional), `embedded_metadata_keys` (optional), `document_id` (optional)
+        Input arguments: `text`, `store` (optional), `metadata` (optional), `embedded_metadata_keys` (optional), `doc_id` (optional), `node` (optional)
 
         Output fields: `future.embedding`
 
         https://substrate.run/library#EmbedText
         """
         super().__init__(**args)
         self.node = "EmbedText"
@@ -821,22 +1127,22 @@
         https://substrate.run/library#EmbedText
         """
         return super().future  # type: ignore
 
 
 class MultiEmbedText(CoreNode):
     """
-    Generate vector embeddings for multiple text documents.
+    Generate embeddings for multiple text documents.
 
     https://substrate.run/library#MultiEmbedText
     """
 
     def __init__(self, args: MultiEmbedTextIn):
         """
-        Input arguments: `items`, `model` (optional), `store` (optional), `embedded_metadata_keys` (optional)
+        Input arguments: `items`, `store` (optional), `embedded_metadata_keys` (optional), `node` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedText
         """
         super().__init__(**args)
         self.node = "MultiEmbedText"
@@ -868,22 +1174,22 @@
         https://substrate.run/library#MultiEmbedText
         """
         return super().future  # type: ignore
 
 
 class EmbedImage(CoreNode):
     """
-    Generate vector embedding for an image, and optionally store the embedding.
+    Generate embedding for an image.
 
     https://substrate.run/library#EmbedImage
     """
 
     def __init__(self, args: EmbedImageIn):
         """
-        Input arguments: `image_uri`, `model` (optional), `store` (optional), `document_id` (optional)
+        Input arguments: `image_uri`, `store` (optional), `doc_id` (optional), `node` (optional)
 
         Output fields: `future.embedding`
 
         https://substrate.run/library#EmbedImage
         """
         super().__init__(**args)
         self.node = "EmbedImage"
@@ -915,22 +1221,22 @@
         https://substrate.run/library#EmbedImage
         """
         return super().future  # type: ignore
 
 
 class MultiEmbedImage(CoreNode):
     """
-    Generate vector embeddings for multiple images, and optionally store the embeddings.
+    Generate embeddings for multiple images.
 
     https://substrate.run/library#MultiEmbedImage
     """
 
     def __init__(self, args: MultiEmbedImageIn):
         """
-        Input arguments: `items`, `store` (optional), `model` (optional)
+        Input arguments: `items`, `store` (optional), `node` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedImage
         """
         super().__init__(**args)
         self.node = "MultiEmbedImage"
@@ -958,7 +1264,101 @@
         Future reference to this node's output.
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedImage
         """
         return super().future  # type: ignore
+
+
+class JinaV2(CoreNode):
+    """
+    Generate embeddings for multiple text documents using Jina V2.
+
+    https://substrate.run/library#JinaV2
+    """
+
+    def __init__(self, args: JinaV2In):
+        """
+        Input arguments: `items`, `store` (optional), `embedded_metadata_keys` (optional)
+
+        Output fields: `future.embeddings`
+
+        https://substrate.run/library#JinaV2
+        """
+        super().__init__(**args)
+        self.node = "JinaV2"
+
+    def output(self, response: SubstrateResponse) -> JinaV2Out:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.embeddings`
+
+        https://substrate.run/library#JinaV2
+        """
+        klass = JinaV2Out
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureJinaV2Out:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.embeddings`
+
+        https://substrate.run/library#JinaV2
+        """
+        return super().future  # type: ignore
+
+
+class CLIP(CoreNode):
+    """
+    Generate embeddings for text or images using CLIP.
+
+    https://substrate.run/library#CLIP
+    """
+
+    def __init__(self, args: CLIPIn):
+        """
+        Input arguments: `items`, `embedded_metadata_keys` (optional), `store` (optional)
+
+        Output fields: `future.embeddings`
+
+        https://substrate.run/library#CLIP
+        """
+        super().__init__(**args)
+        self.node = "CLIP"
+
+    def output(self, response: SubstrateResponse) -> CLIPOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.embeddings`
+
+        https://substrate.run/library#CLIP
+        """
+        klass = CLIPOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureCLIPOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.embeddings`
+
+        https://substrate.run/library#CLIP
+        """
+        return super().future  # type: ignore
```

### Comparing `substrate-120240315.0.1/substrate/substrate.py` & `substrate-120240403.0.1/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `substrate-120240315.0.1/substrate/typeddict_models.py` & `substrate-120240403.0.1/substrate/typeddict_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,268 +18,365 @@
     """
     message: NotRequired[str]
     """
     A message providing more details about the error.
     """
 
 
-class ResponseFormat(TypedDict):
-    type: NotRequired[Literal["json_object", "text"]]
+class GenerateTextIn(TypedDict):
+    prompt: NotRequired[str]
+    """
+    Input prompt.
     """
-    Type of response.
+    temperature: NotRequired[int]
     """
-    json_schema: NotRequired[Dict[str, Any]]
+    (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: NotRequired[int]
+    """
+    (Optional) Maximum number of tokens to generate.
     """
-    (Optional) JSON schema to guide `json_object` response.
+    node: NotRequired[Literal["Mistral7BInstruct"]]
+    """
+    (Optional) Selected node.
     """
 
 
-class GenerateTextIn(TypedDict):
-    prompt: NotRequired[str]
+class GenerateTextOut(TypedDict):
+    text: NotRequired[str]
     """
-    Input prompt.
+    (Optional) Text response.
     """
-    model: NotRequired[Literal["mistral-7b-instruct"]]
+
+
+class GenerateJSONIn(TypedDict):
+    prompt: NotRequired[str]
     """
-    (Optional) Selected model.
+    Input prompt.
     """
-    response_format: NotRequired[ResponseFormat]
+    json_schema: NotRequired[Dict[str, Any]]
     """
-    (Optional) Format of the response.
+    JSON schema to guide `json_object` response.
     """
     temperature: NotRequired[int]
     """
     (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     (Optional) Maximum number of tokens to generate.
     """
+    node: NotRequired[Literal["Mistral7BInstruct"]]
+    """
+    (Optional) Selected node.
+    """
+
+
+class GenerateJSONOut(TypedDict):
+    json_object: NotRequired[Dict[str, Any]]
+    """
+    (Optional) JSON response.
+    """
 
 
 class MultiGenerateTextIn(TypedDict):
     prompt: NotRequired[str]
     """
     Input prompt.
     """
     num_choices: NotRequired[int]
     """
     Number of choices to generate.
     """
-    model: NotRequired[Literal["mistral-7b-instruct"]]
+    temperature: NotRequired[int]
     """
-    (Optional) Selected model.
+    (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: NotRequired[int]
+    """
+    (Optional) Maximum number of tokens to generate.
     """
-    response_format: NotRequired[ResponseFormat]
+    node: NotRequired[Literal["Mistral7BInstruct"]]
     """
-    (Optional) Format of the response.
+    (Optional) Selected node.
+    """
+
+
+class MultiGenerateTextOut(TypedDict):
+    choices: NotRequired[List[GenerateTextOut]]
+
+
+class MultiGenerateJSONIn(TypedDict):
+    prompt: NotRequired[str]
+    """
+    Input prompt.
+    """
+    json_schema: NotRequired[Dict[str, Any]]
+    """
+    JSON schema to guide `json_object` response.
+    """
+    num_choices: NotRequired[int]
+    """
+    Number of choices to generate.
     """
     temperature: NotRequired[int]
     """
     (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     (Optional) Maximum number of tokens to generate.
     """
+    node: NotRequired[Literal["Mistral7BInstruct"]]
+    """
+    (Optional) Selected node.
+    """
 
 
-class GenerateTextOut(TypedDict):
+class MultiGenerateJSONOut(TypedDict):
+    choices: NotRequired[List[GenerateJSONOut]]
+
+
+class Mistral7BInstructIn(TypedDict):
+    prompt: NotRequired[str]
+    """
+    Input prompt.
+    """
+    num_choices: NotRequired[int]
+    """
+    Number of choices to generate.
+    """
+    json_schema: NotRequired[Dict[str, Any]]
+    """
+    (Optional) JSON schema to guide response.
+    """
+    temperature: NotRequired[float]
+    """
+    (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: NotRequired[int]
+    """
+    (Optional) Maximum number of tokens to generate.
+    """
+
+
+class Mistral7BInstructChoice(TypedDict):
     text: NotRequired[str]
     """
-    (Optional) Text response.
+    (Optional) Text response, if `json_schema` was not provided.
     """
     json_object: NotRequired[Dict[str, Any]]
     """
-    (Optional) JSON response.
+    (Optional) JSON response, if `json_schema` was provided.
     """
 
 
-class MultiGenerateTextOut(TypedDict):
-    choices: NotRequired[List[GenerateTextOut]]
+class Mistral7BInstructOut(TypedDict):
+    choices: NotRequired[List[Mistral7BInstructChoice]]
 
 
 class GenerateTextVisionIn(TypedDict):
     prompt: NotRequired[str]
     """
     Text prompt.
     """
     image_uris: NotRequired[List[str]]
     """
-    (Optional) Image prompts.
-    """
-    model: NotRequired[Literal["firellava-13b"]]
-    """
-    (Optional) Selected model.
+    Image prompts.
     """
     temperature: NotRequired[int]
     """
     (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     (Optional) Maximum number of tokens to generate.
     """
+    node: NotRequired[Literal["Firellava13B"]]
+    """
+    (Optional) Selected node.
+    """
 
 
 class GenerateTextVisionOut(TypedDict):
     text: NotRequired[str]
     """
     Text response.
     """
 
 
-class GenerateImageIn(TypedDict):
+class Firellava13BIn(TypedDict):
     prompt: NotRequired[str]
     """
     Text prompt.
     """
-    image_prompt_uri: NotRequired[str]
-    """
-    (Optional) Image prompt.
-    """
-    model: NotRequired[Literal["stablediffusion-xl"]]
+    image_uris: NotRequired[List[str]]
     """
-    (Optional) Selected model.
+    Image prompts.
     """
-    image_influence: NotRequired[float]
+    temperature: NotRequired[float]
     """
-    (Optional) Controls the influence of the image prompt on the generated output.
+    (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
-    negative_prompt: NotRequired[str]
+    max_tokens: NotRequired[int]
     """
-    (Optional) Negative input prompt.
+    (Optional) Maximum number of tokens to generate.
     """
-    store: NotRequired[str]
+
+
+class Firellava13BOut(TypedDict):
+    text: NotRequired[str]
     """
-    (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Text response.
     """
-    width: NotRequired[int]
+
+
+class GenerateImageIn(TypedDict):
+    prompt: NotRequired[str]
     """
-    (Optional) Width of output image, in pixels.
+    Text prompt.
     """
-    height: NotRequired[int]
+    store: NotRequired[str]
     """
-    (Optional) Height of output image, in pixels.
+    (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    seed: NotRequired[int]
+    node: NotRequired[Literal["StableDiffusionXL"]]
     """
-    (Optional) Seed for deterministic generation. Default is a random seed.
+    (Optional) Selected node.
     """
 
 
 class GenerateImageOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
-    seed: NotRequired[int]
-    """
-    The random noise seed used for generation.
-    """
 
 
 class MultiGenerateImageIn(TypedDict):
     prompt: NotRequired[str]
     """
     Text prompt.
     """
-    image_prompt_uri: NotRequired[str]
-    """
-    (Optional) Image prompt.
-    """
     num_images: NotRequired[int]
     """
     Number of images to generate.
     """
-    model: NotRequired[Literal["stablediffusion-xl"]]
+    store: NotRequired[str]
     """
-    (Optional) Selected model.
+    (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    image_influence: NotRequired[float]
+    node: NotRequired[Literal["StableDiffusionXL"]]
     """
-    (Optional) Controls the influence of the image prompt on the generated output.
+    (Optional) Selected node.
+    """
+
+
+class MultiGenerateImageOut(TypedDict):
+    outputs: NotRequired[List[GenerateImageOut]]
+
+
+class StableDiffusionXLIn(TypedDict):
+    prompt: NotRequired[str]
+    """
+    Text prompt.
     """
     negative_prompt: NotRequired[str]
     """
     (Optional) Negative input prompt.
     """
+    steps: NotRequired[int]
+    """
+    (Optional) Number of diffusion steps.
+    """
+    num_images: NotRequired[int]
+    """
+    (Optional) Number of images to generate.
+    """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
+    height: NotRequired[int]
+    """
+    (Optional) Height of output image, in pixels.
+    """
     width: NotRequired[int]
     """
     (Optional) Width of output image, in pixels.
     """
-    height: NotRequired[int]
+    seeds: NotRequired[int]
     """
-    (Optional) Height of output image, in pixels.
+    (Optional) Seeds for deterministic generation. Default is a random seed.
     """
-    seeds: NotRequired[List[int]]
+    guidance_scale: NotRequired[float]
     """
-    (Optional) Random noise seeds. Default is random seeds for each generation.
+    (Optional) Higher values adhere to the text prompt more strongly, typically at the expense of image quality.
     """
 
 
-class MultiGenerateImageOut(TypedDict):
-    outputs: NotRequired[List[GenerateImageOut]]
-
-
-class ControlledGenerateImageIn(TypedDict):
+class StableDiffusionImage(TypedDict):
     image_uri: NotRequired[str]
     """
-    Input image.
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
-    control_method: NotRequired[Literal["edge", "depth", "illusion"]]
+    seed: NotRequired[int]
     """
-    Strategy to control generation using the input image.
+    The random noise seed used for generation.
     """
+
+
+class StableDiffusionXLOut(TypedDict):
+    outputs: NotRequired[List[StableDiffusionImage]]
+
+
+class StableDiffusionXLIPAdapterIn(TypedDict):
     prompt: NotRequired[str]
     """
     Text prompt.
     """
-    output_resolution: NotRequired[int]
+    image_prompt_uri: NotRequired[str]
     """
-    (Optional) Resolution of the output image, in pixels.
+    (Optional) Image prompt.
     """
-    model: NotRequired[Literal["stablediffusion-xl"]]
+    num_images: NotRequired[int]
     """
-    (Optional) Selected model.
+    Number of images to generate.
+    """
+    ip_adapter_scale: NotRequired[float]
+    """
+    (Optional) Controls the influence of the image prompt on the generated output.
     """
     negative_prompt: NotRequired[str]
     """
     (Optional) Negative input prompt.
     """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    image_influence: NotRequired[float]
-    """
-    (Optional) Controls the influence of the input image on the generated output.
-    """
-    seed: NotRequired[int]
+    width: NotRequired[int]
     """
-    (Optional) Seed for deterministic generation. Default is a random seed.
+    (Optional) Width of output image, in pixels.
     """
-
-
-class ControlledGenerateImageOut(TypedDict):
-    image_uri: NotRequired[str]
+    height: NotRequired[int]
     """
-    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    (Optional) Height of output image, in pixels.
     """
-    seed: NotRequired[int]
+    seeds: NotRequired[List[int]]
     """
-    The random noise seed used for generation.
+    (Optional) Random noise seeds. Default is random seeds for each generation.
     """
 
 
-class MultiControlledGenerateImageIn(TypedDict):
+class StableDiffusionXLIPAdapterOut(TypedDict):
+    outputs: NotRequired[List[StableDiffusionImage]]
+
+
+class StableDiffusionXLControlNetIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Input image.
     """
     control_method: NotRequired[Literal["edge", "depth", "illusion"]]
     """
     Strategy to control generation using the input image.
@@ -292,38 +389,34 @@
     """
     Number of images to generate.
     """
     output_resolution: NotRequired[int]
     """
     (Optional) Resolution of the output image, in pixels.
     """
-    model: NotRequired[Literal["stablediffusion-xl"]]
-    """
-    (Optional) Selected model.
-    """
     negative_prompt: NotRequired[str]
     """
     (Optional) Negative input prompt.
     """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    image_influence: NotRequired[float]
+    conditioning_scale: NotRequired[float]
     """
     (Optional) Controls the influence of the input image on the generated output.
     """
     seeds: NotRequired[List[int]]
     """
     (Optional) Random noise seeds. Default is random seeds for each generation.
     """
 
 
-class MultiControlledGenerateImageOut(TypedDict):
-    outputs: NotRequired[List[ControlledGenerateImageOut]]
+class StableDiffusionXLControlNetOut(TypedDict):
+    outputs: NotRequired[List[StableDiffusionImage]]
 
 
 class GenerativeEditImageIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Original image.
     """
@@ -331,112 +424,103 @@
     """
     Text prompt.
     """
     mask_image_uri: NotRequired[str]
     """
     (Optional) Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
-    image_prompt_uri: NotRequired[str]
+    store: NotRequired[str]
     """
-    (Optional) Image prompt.
+    (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    output_resolution: NotRequired[int]
+    node: NotRequired[Literal["StableDiffusionXLInpaint"]]
     """
-    (Optional) Resolution of the output image, in pixels.
+    (Optional) Selected node.
     """
-    model: NotRequired[Literal["stablediffusion-xl"]]
+
+
+class GenerativeEditImageOut(TypedDict):
+    image_uri: NotRequired[str]
     """
-    (Optional) Selected model.
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
-    strength: NotRequired[float]
+
+
+class MultiGenerativeEditImageIn(TypedDict):
+    image_uri: NotRequired[str]
     """
-    (Optional) Controls the strength of the generation process.
+    Original image.
     """
-    image_prompt_influence: NotRequired[float]
+    prompt: NotRequired[str]
     """
-    (Optional) Controls the influence of the image prompt on the generated output.
+    Text prompt.
     """
-    negative_prompt: NotRequired[str]
+    mask_image_uri: NotRequired[str]
     """
-    (Optional) Negative input prompt.
+    (Optional) Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
+    """
+    num_images: NotRequired[int]
+    """
+    Number of images to generate.
     """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    seed: NotRequired[int]
+    node: NotRequired[Literal["StableDiffusionXLInpaint"]]
     """
-    (Optional) Seed for deterministic generation. Default is a random seed.
+    (Optional) Selected node.
     """
 
 
-class GenerativeEditImageOut(TypedDict):
-    image_uri: NotRequired[str]
-    """
-    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
-    """
-    seed: NotRequired[int]
-    """
-    The random noise seed used for generation.
-    """
+class MultiGenerativeEditImageOut(TypedDict):
+    outputs: NotRequired[List[GenerativeEditImageOut]]
 
 
-class MultiGenerativeEditImageIn(TypedDict):
+class StableDiffusionXLInpaintIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Original image.
     """
     prompt: NotRequired[str]
     """
     Text prompt.
     """
     mask_image_uri: NotRequired[str]
     """
     (Optional) Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
-    image_prompt_uri: NotRequired[str]
-    """
-    (Optional) Image prompt.
-    """
     num_images: NotRequired[int]
     """
     Number of images to generate.
     """
     output_resolution: NotRequired[int]
     """
     (Optional) Resolution of the output image, in pixels.
     """
-    model: NotRequired[Literal["stablediffusion-xl"]]
-    """
-    (Optional) Selected model.
-    """
     negative_prompt: NotRequired[str]
     """
     (Optional) Negative input prompt.
     """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
     strength: NotRequired[float]
     """
     (Optional) Controls the strength of the generation process.
     """
-    image_prompt_influence: NotRequired[float]
-    """
-    (Optional) Controls the influence of the image prompt on the generated output.
-    """
     seeds: NotRequired[List[int]]
     """
     (Optional) Random noise seeds. Default is random seeds for each generation.
     """
 
 
-class MultiGenerativeEditImageOut(TypedDict):
-    outputs: NotRequired[List[GenerativeEditImageOut]]
+class StableDiffusionXLInpaintOut(TypedDict):
+    outputs: NotRequired[List[StableDiffusionImage]]
 
 
 class BoundingBox(TypedDict):
     x1: NotRequired[float]
     """
     Top left corner x.
     """
@@ -546,19 +630,19 @@
 class DetectSegmentsIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Input image.
     """
     point_prompts: NotRequired[List[Point]]
     """
-    (Optional) Point prompts, to detect a segment under the point. One of `point_prompt` or `box_prompt` must be set.
+    (Optional) Point prompts, to detect a segment under the point. One of `point_prompts` or `box_prompts` must be set.
     """
     box_prompts: NotRequired[List[BoundingBox]]
     """
-    (Optional) Box prompts, to detect a segment within the bounding box. One of `point_prompt` or `box_prompt` must be set.
+    (Optional) Box prompts, to detect a segment within the bounding box. One of `point_prompts` or `box_prompts` must be set.
     """
     model: NotRequired[Literal["segment-anything"]]
     """
     (Optional) Selected model.
     """
     store: NotRequired[str]
     """
@@ -699,49 +783,49 @@
 
 
 class Embedding(TypedDict):
     vector: NotRequired[List[float]]
     """
     Embedding vector.
     """
-    document_id: NotRequired[str]
+    doc_id: NotRequired[str]
     """
     (Optional) Vector store document ID.
     """
     metadata: NotRequired[Dict[str, Any]]
     """
     (Optional) Vector store document metadata.
     """
 
 
 class EmbedTextIn(TypedDict):
     text: NotRequired[str]
     """
     Text to embed.
     """
-    model: NotRequired[Literal["jina-v2", "clip"]]
-    """
-    (Optional) Selected model.
-    """
     store: NotRequired[str]
     """
     (Optional) [Vector store](/docs/vector-stores) identifier.
     """
     metadata: NotRequired[Dict[str, Any]]
     """
     (Optional) Metadata that can be used to query the vector store. Ignored if `store` is unset.
     """
     embedded_metadata_keys: NotRequired[List[str]]
     """
     (Optional) Choose keys from `metadata` to embed with text.
     """
-    document_id: NotRequired[str]
+    doc_id: NotRequired[str]
     """
     (Optional) Vector store document ID. Ignored if `store` is unset.
     """
+    node: NotRequired[Literal["JinaV2", "CLIP"]]
+    """
+    (Optional) Selected node.
+    """
 
 
 class EmbedTextOut(TypedDict):
     embedding: NotRequired[Embedding]
     """
     Generated embedding.
     """
@@ -752,110 +836,169 @@
     """
     Text to embed.
     """
     metadata: NotRequired[Dict[str, Any]]
     """
     (Optional) Metadata that can be used to query the vector store. Ignored if `store` is unset.
     """
-    document_id: NotRequired[str]
+    doc_id: NotRequired[str]
     """
     (Optional) Vector store document ID. Ignored if `store` is unset.
     """
 
 
 class MultiEmbedTextIn(TypedDict):
     items: NotRequired[List[EmbedTextItem]]
     """
     Items to embed.
     """
-    model: NotRequired[Literal["jina-v2", "clip"]]
+    store: NotRequired[str]
     """
-    (Optional) Selected model.
+    (Optional) [Vector store](/docs/vector-stores) identifier.
+    """
+    embedded_metadata_keys: NotRequired[List[str]]
+    """
+    (Optional) Choose keys from `metadata` to embed with text.
+    """
+    node: NotRequired[Literal["JinaV2", "CLIP"]]
+    """
+    (Optional) Selected node.
+    """
+
+
+class MultiEmbedTextOut(TypedDict):
+    embeddings: NotRequired[List[Embedding]]
+    """
+    Generated embeddings.
+    """
+
+
+class JinaV2In(TypedDict):
+    items: NotRequired[List[EmbedTextItem]]
+    """
+    Items to embed.
     """
     store: NotRequired[str]
     """
     (Optional) [Vector store](/docs/vector-stores) identifier.
     """
     embedded_metadata_keys: NotRequired[List[str]]
     """
     (Optional) Choose keys from `metadata` to embed with text.
     """
 
 
-class MultiEmbedTextOut(TypedDict):
+class JinaV2Out(TypedDict):
     embeddings: NotRequired[List[Embedding]]
     """
     Generated embeddings.
     """
 
 
 class EmbedImageIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Image to embed.
     """
-    model: NotRequired[Literal["clip"]]
-    """
-    (Optional) Selected model.
-    """
     store: NotRequired[str]
     """
     (Optional) [Vector store](/docs/vector-stores) identifier.
     """
-    document_id: NotRequired[str]
+    doc_id: NotRequired[str]
     """
     (Optional) Vector store document ID. Ignored if `store` is unset.
     """
+    node: NotRequired[Literal["CLIP"]]
+    """
+    (Optional) Selected node.
+    """
 
 
 class EmbedImageOut(TypedDict):
     embedding: NotRequired[Embedding]
     """
     Generated embedding.
     """
 
 
 class EmbedImageItem(TypedDict):
     image_uri: NotRequired[str]
     """
     Image to embed.
     """
-    document_id: NotRequired[str]
+    doc_id: NotRequired[str]
+    """
+    (Optional) Vector store document ID. Ignored if `store` is unset.
+    """
+
+
+class EmbedTextOrImageItem(TypedDict):
+    image_uri: NotRequired[str]
+    """
+    (Optional) Image to embed.
+    """
+    text: NotRequired[str]
+    """
+    (Optional) Text to embed.
+    """
+    metadata: NotRequired[Dict[str, Any]]
+    """
+    (Optional) Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    """
+    doc_id: NotRequired[str]
     """
     (Optional) Vector store document ID. Ignored if `store` is unset.
     """
 
 
 class MultiEmbedImageIn(TypedDict):
     items: NotRequired[List[EmbedImageItem]]
     """
     Items to embed.
     """
     store: NotRequired[str]
     """
     (Optional) [Vector store](/docs/vector-stores) identifier.
     """
-    model: NotRequired[Literal["clip"]]
+    node: NotRequired[Literal["CLIP"]]
     """
-    (Optional) Selected model.
+    (Optional) Selected node.
     """
 
 
 class MultiEmbedImageOut(TypedDict):
     embeddings: NotRequired[List[Embedding]]
     """
     Generated embeddings.
     """
 
 
-class VectorStoreParams(TypedDict):
+class CLIPIn(TypedDict):
+    items: NotRequired[List[EmbedTextOrImageItem]]
+    """
+    Items to embed.
+    """
+    embedded_metadata_keys: NotRequired[List[str]]
+    """
+    (Optional) Choose keys from `metadata` to embed with text, when embedding and storing text documents.
+    """
+    store: NotRequired[str]
+    """
+    (Optional) [Vector store](/docs/vector-stores) identifier.
+    """
+
+
+class CLIPOut(TypedDict):
+    embeddings: NotRequired[List[Embedding]]
     """
-    Fields describing a vector store and its associated index.
+    Generated embeddings.
     """
 
+
+class VectorStoreParams(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model
```

### Comparing `substrate-120240315.0.1/PKG-INFO` & `substrate-120240403.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 120240315.0.1
+Version: 120240403.0.1
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

