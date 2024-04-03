# Comparing `tmp/bpm_ai-1.2.0.tar.gz` & `tmp/bpm_ai-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai-1.2.0.tar", max compression
+gzip compressed data, was "bpm_ai-1.3.0.tar", max compression
```

## Comparing `bpm_ai-1.2.0.tar` & `bpm_ai-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0      932 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/README.md
--rw-r--r--   0        0        0        0 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/common/__init__.py
--rw-r--r--   0        0        0     1131 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/common/json_utils.py
--rw-r--r--   0        0        0     1022 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/common/multimodal.py
--rw-r--r--   0        0        0        0 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/compose/__init__.py
--rw-r--r--   0        0        0     1324 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/compose/compose.openai.prompt
--rw-r--r--   0        0        0     3820 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/compose/compose.py
--rw-r--r--   0        0        0    21191 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/compose/stopwords.py
--rw-r--r--   0        0        0      973 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/compose/util.py
--rw-r--r--   0        0        0        0 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/decide/__init__.py
--rw-r--r--   0        0        0     3374 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/decide/decide.openai.prompt
--rw-r--r--   0        0        0     3469 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/decide/decide.py
--rw-r--r--   0        0        0     1986 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/decide/schema.py
--rw-r--r--   0        0        0        0 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/extract/__init__.py
--rw-r--r--   0        0        0     1275 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/extract/extract.openai.prompt
--rw-r--r--   0        0        0     7619 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/extract/extract.py
--rw-r--r--   0        0        0        0 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/generic/__init__.py
--rw-r--r--   0        0        0      533 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/generic/generic.openai.prompt
--rw-r--r--   0        0        0     1451 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/generic/generic.py
--rw-r--r--   0        0        0        0 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/translate/__init__.py
--rw-r--r--   0        0        0      160 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/translate/schema.py
--rw-r--r--   0        0        0      225 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/translate/translate.openai.prompt
--rw-r--r--   0        0        0     2376 2024-02-19 16:03:31.545497 bpm_ai-1.2.0/bpm_ai/translate/translate.py
--rw-r--r--   0        0        0     1918 2024-02-19 16:03:31.549497 bpm_ai-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 bpm_ai-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      932 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/common/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/common/errors.py
+-rw-r--r--   0        0        0     1034 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/common/multimodal.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/compose/__init__.py
+-rw-r--r--   0        0        0     1509 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/compose/compose.anthropic.prompt
+-rw-r--r--   0        0        0     1369 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/compose/compose.openai.prompt
+-rw-r--r--   0        0        0     3575 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/compose/compose.py
+-rw-r--r--   0        0        0      738 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/compose/util.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/decide/__init__.py
+-rw-r--r--   0        0        0     3316 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/decide/decide.anthropic.prompt
+-rw-r--r--   0        0        0     3385 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/decide/decide.openai.prompt
+-rw-r--r--   0        0        0     4082 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/decide/decide.py
+-rw-r--r--   0        0        0     1986 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/decide/schema.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/extract/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/extract/extract.anthropic.prompt
+-rw-r--r--   0        0        0     1286 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/extract/extract.openai.prompt
+-rw-r--r--   0        0        0     7210 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/extract/extract.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/generic/__init__.py
+-rw-r--r--   0        0        0      616 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/generic/generic.anthropic.prompt
+-rw-r--r--   0        0        0      544 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/generic/generic.openai.prompt
+-rw-r--r--   0        0        0     1486 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/generic/generic.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/translate/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/translate/schema.py
+-rw-r--r--   0        0        0      576 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/translate/translate.anthropic.prompt
+-rw-r--r--   0        0        0      611 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/translate/translate.openai.prompt
+-rw-r--r--   0        0        0     3004 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/translate/translate.py
+-rw-r--r--   0        0        0     1355 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 bpm_ai-1.3.0/PKG-INFO
```

### Comparing `bpm_ai-1.2.0/README.md` & `bpm_ai-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.2.0/bpm_ai/common/multimodal.py` & `bpm_ai-1.3.0/bpm_ai/common/multimodal.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.speech_recognition.asr import ASRModel
-from bpm_ai_core.util.audio import is_supported_audio_file
-from bpm_ai_core.util.image import is_supported_img_file
+from bpm_ai_core.util.file import is_supported_audio_file
+from bpm_ai_core.util.file import is_supported_img_file
 
 
 def prepare_images_for_llm_prompt(input_data: dict):
     """
-    For multi-modal LLMs. Will be turned into PIL Image(s) as part of the prompt processing.
+    For multi-modal LLMs. Will be turned into Blob objects as part of the prompt processing.
     """
     return {
-        k: f"[# image {v} #]"
+        k: f"[# blob {v} #]"
         if (isinstance(v, str) and is_supported_img_file(v))
         else v for k, v in input_data.items()
     }
 
 
-async def ocr_images(input_data: dict, ocr: OCR | None = None):
+async def ocr_documents(input_data: dict, ocr: OCR | None = None):
     return {
-        k: await ocr.images_to_text(v)
+        k: (await ocr.process(v)).full_text
         if (ocr and isinstance(v, str) and is_supported_img_file(v))
         else v for k, v in input_data.items()
     }
 
 
 async def transcribe_audio(input_data: dict, asr: ASRModel | None = None) -> dict:
     return {
-        k: await asr.transcribe(v)
+        k: (await asr.transcribe(v)).text
         if (asr and isinstance(v, str) and is_supported_audio_file(v))
         else v for k, v in input_data.items()
     }
```

### Comparing `bpm_ai-1.2.0/bpm_ai/compose/compose.openai.prompt` & `bpm_ai-1.3.0/bpm_ai/compose/compose.openai.prompt`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [# system #]
 You are a brilliant creative writing AI that loves to compose {{style}} {{type}} that have a {{tone}} tone. You are an expert for writing in {{lang}}.
 
 Your task is to compose text parts for variables (in curly braces) in a text template, using given context information and desired text properties.
 Only use information from the given template, properties and context, do not make something up.
 Do *NOT* use template variables in your generated text parts, the text you generate *must* be directly usable!
-Be mindful of the relative position and the spaces (or lack thereof) between template variables. When the template is formatted with your generated variables, it must have correct spacing and a coherent content!
+Be mindful of the relative position, whitespaces, and punctuation (or lack thereof) between template variables. When the template is formatted with your generated variables, it must have correct spacing and a coherent content!
 
 # TEXT PROPERTIES
 - style: {{style}}
 - tone: {{tone}}
 - length: {{length}}
 - language: {{lang}}
 
 [# user #]
 # CONTEXT
-{{context}}
+{{context | markdown}}
 
 # TEXT TEMPLATE
 """
 {{template}}
 """
 
 Remember to respect the text properties specified above and write in {{lang}}!
-Remember to *NOT* use template variables in your generated text parts and to mind the position and spacing of template variables!
+Remember to *NOT* use template variables in your generated text parts and to mind the position, spacing, and punctuation of template variable texts!
 
 *IMPORTANT*: Generate text for *all* template variables, do not forget anything!
 {% if False %}
 Do *NOT* use any character escaping!
 {% endif %}
 
 Make sure to get this right, this is very important for my career!
```

### Comparing `bpm_ai-1.2.0/bpm_ai/compose/compose.py` & `bpm_ai-1.3.0/bpm_ai/compose/compose.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import re
 from typing import TypedDict, Callable
 
 from bpm_ai_core.llm.common.llm import LLM
-from bpm_ai_core.llm.common.message import ToolCallsMessage
-from bpm_ai_core.llm.common.tool import Tool
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
 from bpm_ai_core.tracing.decorators import trace
 
-from bpm_ai.common.json_utils import json_to_md
-from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_images
-from bpm_ai.compose.util import remove_stop_words, type_to_prompt_type_str, decode_if_needed
+from bpm_ai.common.errors import MissingParameterError
+from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents
+from bpm_ai.compose.util import remove_stop_words, type_to_prompt_type_str
 
 TEMPLATE_VAR_PATTERN = r'\{\s*([^{}\s]+(?:\s*[^{}\s]+)*)\s*\}'
 
 
 class TextProperties(TypedDict):
     style: str
     type: str
@@ -30,64 +28,62 @@
     llm: LLM,
     input_data: dict[str, str | dict],
     template: str,
     properties: TextProperties,
     ocr: OCR | None = None,
     asr: ASRModel | None = None
 ) -> dict:
+    if template is None:
+        raise MissingParameterError("template is required")
+
     def desc_to_var_name(desc: str):
         v = remove_stop_words(desc, separator='_')
         return re.sub(r'[^A-Za-z0-9_\'äöüÄÖÜß]+', '', v).lower()
 
     def format_vars(template: str, f: Callable[[str], str]):
         return re.sub(TEMPLATE_VAR_PATTERN, lambda m: f(m.group(1)), template)
 
-    if llm.supports_images():
+    if not ocr and llm.supports_images():
         input_data = prepare_images_for_llm_prompt(input_data)
     else:
-        input_data = await ocr_images(input_data, ocr)
+        input_data = await ocr_documents(input_data, ocr)
     input_data = await transcribe_audio(input_data, asr)
 
     # all variables found in the template
     template_vars = re.findall(TEMPLATE_VAR_PATTERN, template)
     # map of template variables that are not already in the input and need to be generated
     template_vars_to_generate_dict = {desc_to_var_name(desc): desc for desc in template_vars if
                                       desc not in input_data.keys()}
     # input variables that are not present in the template
     non_template_input_var_dict = {k: v for k, v in input_data.items() if k not in template_vars}
 
     if len(template_vars_to_generate_dict) > 0:
-        tool = Tool.from_callable(
-            "store_text",
-            "Stores composed text parts for template variables.",
-            args_schema=template_vars_to_generate_dict,
-            callable=lambda **x: x
-        )
-
         prompt = Prompt.from_file(
             "compose",
-            context=json_to_md(non_template_input_var_dict),
+            context=non_template_input_var_dict,
             # remove template braces from variables that are already present in the input to not confuse the model what to generate
             # we do not resolve these variables here to avoid sending that data to the API
             template=format_vars(template, lambda v: v if v in input_data.keys() else '{' + v + '}'),
             type=type_to_prompt_type_str(properties.get("type", "letter")),
             style=properties.get("style", "formal"),
             tone=properties.get("tone", "friendly"),
             length=properties.get("length", "adequate"),
             lang=properties.get("language", "English")
         )
 
-        result = await llm.predict(prompt, tools=[tool])
+        compose_schema = {
+            "name": "store_text",
+            "description": "Stores composed text parts for template variables.",
+            "type": "object",
+            "properties": template_vars_to_generate_dict
+        }
+
+        message = await llm.generate_message(prompt, output_schema=compose_schema)
 
-        if isinstance(result, ToolCallsMessage):
-            generated_vars = result.tool_calls[0].invoke()
-            # fix for encoding error in new OpenAI models API
-            generated_vars = {k: decode_if_needed(v) for k, v in generated_vars.items()}
-        else:
-            generated_vars = {}
+        generated_vars = message.content or {}
     else:
         generated_vars = {}
 
     input_vars = {desc_to_var_name(k): v for k, v in input_data.items()}
     all_vars = generated_vars | input_vars
 
     # resolve all template variables using either input or generated values
```

### Comparing `bpm_ai-1.2.0/bpm_ai/decide/decide.openai.prompt` & `bpm_ai-1.3.0/bpm_ai/decide/decide.openai.prompt`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 {"reasoning": {"relevantFacts": ["The season is Fall", "The number of guests is 26", "The occasion is a House Party", "The budget is low"], "deducedInformation": ["Fall season usually calls for warm, hearty meals", "A low budget means we need to choose a dish that is cost-effective", "The number of guests suggests we need a dish that can be easily prepared in large quantities", "The occasion of a house party does not call for a special or extravagant dish."], "reasoningSteps": ["1. Given the Fall season, a warm, hearty meal like Spareribs, Roastbeef, Dry Aged Gourmet Steak or Stew would be appropriate", "2. Considering the low budget, Stew would be more cost-effective than Spareribs, Roastbeef or Dry Aged Gourmet Steak.", "3. Given the number of guests, a dish that can be easily prepared in large quantities like a Stew would be suitable", "4. Considering all factors (warm and hearty for Fall, cost-effective for a low budget, and easily prepared in large quantities for a house party) Stew seems to be the best choice"], "finalReasoning": "Stew is the best choice as it meets all the requirements: it\'s a warm, hearty meal suitable for Fall, it\'s cost-effective, and it can be easily prepared in large quantities for a house party."}, "decision": "Stew"}
 [# tool_result: call_kufP7dqLA3OmtHJD10cZ5Jt1 #]
 Decision stored, continue with next task.
 {% endif %}
 
 [# user #]
 # CONTEXT
-{{context}}
+{{context | markdown}}
 
 # DECISION TASK DESCRIPTION
 {{task}}
 
 {% if possible_values %}
 IMPORTANT: Remember to respect the enum of possible decision values!
 {% endif %}
```

### Comparing `bpm_ai-1.2.0/bpm_ai/decide/schema.py` & `bpm_ai-1.3.0/bpm_ai/decide/schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.2.0/bpm_ai/extract/extract.openai.prompt` & `bpm_ai-1.3.0/bpm_ai/extract/extract.openai.prompt`

 * *Files 7% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 Pay close attention to the type and description of each requested property. Just the name of a property may be too general or even misleading to figure out what to extract. Strictly follow the description of the property!
 Only extract information that is completely contained in the passage directly or indirectly.
 NEVER make anything up or assume information that can't be deduced from the passage.
 If any property or information is not contained in or can't be deduced from the passage, set the property to null. NEVER make up a value!
 
 [# user #]
 """
-{{input}}
+{{input | markdown}}
 """
 
 Remember: set properties to null if they are not present in or can't be deduced from the above passage!
 
 Make sure to get the extraction right, this is very important for my career!
```

### Comparing `bpm_ai-1.2.0/bpm_ai/extract/extract.py` & `bpm_ai-1.3.0/bpm_ai/extract/extract.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,194 +1,171 @@
 import re
 from typing import Callable, Any
 
-from bpm_ai_core.classification.transformers_classifier import TransformersClassifier, DEFAULT_MODEL_MULTI, \
-    DEFAULT_MODEL_EN
+from bpm_ai_core.classification.zero_shot_classifier import ZeroShotClassifier
 from bpm_ai_core.question_answering.question_answering import QuestionAnswering
 from bpm_ai_core.llm.common.llm import LLM
-from bpm_ai_core.llm.common.message import ToolCallsMessage
-from bpm_ai_core.llm.common.tool import Tool
 from bpm_ai_core.ocr.ocr import OCR
-from bpm_ai_core.pos.spacy_pos_tagger import SpacyPOSTagger
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
+from bpm_ai_core.token_classification.zero_shot_token_classifier import ZeroShotTokenClassifier
 from bpm_ai_core.tracing.decorators import trace
-from bpm_ai_core.util.json import expand_simplified_json_schema
-from bpm_ai_core.util.language import indentify_language
+from bpm_ai_core.util.json_schema import expand_simplified_json_schema
+from bpm_ai_core.util.markdown import dict_to_md
 
-from bpm_ai.common.json_utils import json_to_md
-from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_images
+from bpm_ai.common.errors import MissingParameterError
+from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents
 
 
 @trace("bpm-ai-extract", ["llm"])
 async def extract_llm(
     llm: LLM,
-    input_data: dict[str, str | dict],
+    input_data: dict[str, str | dict | None],
     output_schema: dict[str, str | dict],
     multiple: bool = False,
     multiple_description: str = "",
     ocr: OCR | None = None,
     asr: ASRModel | None = None
 ) -> dict | list[dict]:
-    def transform_result(**extracted):
+    if all(value is None for value in input_data.values()):
+        return input_data
+
+    if not ocr and llm.supports_images():
+        input_data = prepare_images_for_llm_prompt(input_data)
+    else:
+        input_data = await ocr_documents(input_data, ocr)
+    input_data = await transcribe_audio(input_data, asr)
+
+    if not output_schema:
+        return input_data
+
+    def transform_result(extracted: dict):
         def empty_to_none(v):
             return None if v in ["", "null"] else v
 
         if multiple and "entities" in extracted.keys():
             extracted = extracted["entities"]
 
         if isinstance(extracted, list):
-            return [transform_result(**d) for d in extracted]
+            return [transform_result(d) for d in extracted]
         else:
             return {k: empty_to_none(v) for k, v in extracted.items()}
 
-    tool = Tool.from_callable(
-        "information_extraction",
-        f"Extracts the relevant {'entities' if multiple else 'information'} from the passage.",
-        args_schema={
-            "entities": {"type": "array", "description": multiple_description, "items": output_schema}
-        } if multiple else output_schema,
-        callable=transform_result
-    )
-    if llm.supports_images():
-        input_data = prepare_images_for_llm_prompt(input_data)
-    else:
-        input_data = await ocr_images(input_data, ocr)
-    input_data = await transcribe_audio(input_data, asr)
-    input_md = json_to_md(input_data).strip()
-
-    prompt = Prompt.from_file("extract", input=input_md)
+    prompt = Prompt.from_file("extract", input=input_data)
 
-    result = await llm.predict(prompt, tools=[tool])
-
-    if isinstance(result, ToolCallsMessage):
-        return result.tool_calls[0].invoke()
-    else:
-        return {}
+    extract_schema = {
+        "name": "information_extraction",
+        "description": f"Extracts the relevant {'entities' if multiple else 'information'} from the passage.",
+        "type": "object",
+        "properties": output_schema if not multiple else {
+            "entities": {"type": "array", "description": multiple_description, "items": output_schema}
+        }
+    }
 
+    message = await llm.generate_message(prompt, output_schema=extract_schema)
 
-def create_json_object(target: str, schema, get_value: Callable, current_obj=None, root_obj=None, parent_key='', prefix=''):
-    if current_obj is None:
-        current_obj = {}
-        root_obj = {}
-
-    for name, properties in schema.items():
-        full_key = f'{parent_key}.{name}' if parent_key else name
-        if properties['type'] == 'object':
-            current_obj[name] = create_json_object(target, properties['properties'], get_value, {}, root_obj, full_key)
-        else:
-            description = properties.get('description')
-            if prefix:
-                description = prefix + (description[:1].lower() + description[1:])
-            value = get_value(target, full_key, properties['type'], description, root_obj)
-            current_obj[name] = value
-            root_obj[full_key] = value
-
-    return current_obj
-
-
-def filter_and_join(tags, tags_to_join=['NOUN', 'PROPN', 'NUM', 'SYM', 'X']):
-    result = []
-    current_word = ""
-    prev_tag = None
-
-    for token, tag in tags:
-        if tag in tags_to_join:
-            if prev_tag not in tags_to_join and current_word:
-                result.append(current_word.strip())
-                current_word = ""
-            current_word += token
-        else:
-            if current_word:
-                result.append(current_word.strip())
-                current_word = ""
-        prev_tag = tag
-
-    if current_word:
-        result.append(current_word.strip())
-    return result
-
-
-def strip_non_numeric_chars(s):
-    while len(s) > 0 and not s[0].isdigit():
-        s = s[1:]
-    while len(s) > 0 and not s[-1].isdigit():
-        s = s[:-1]
-    return s
+    return transform_result(message.content or {})
 
 
 @trace("bpm-ai-extract", ["extractive-qa"])
 async def extract_qa(
     qa: QuestionAnswering,
-    input_data: dict[str, str | dict],
+    classifier: ZeroShotClassifier,
+    token_classifier: ZeroShotTokenClassifier,
+    input_data: dict[str, str | dict | None],
     output_schema: dict[str, str | dict],
     multiple: bool = False,
     multiple_description: str = "",
     ocr: OCR | None = None,
     asr: ASRModel | None = None
 ) -> dict | list[dict]:
-    input_data = await ocr_images(input_data, ocr)
+    if all(value is None for value in input_data.values()):
+        return input_data
+
+    input_data = await ocr_documents(input_data, ocr)
     input_data = await transcribe_audio(input_data, asr)
 
-    input_md = json_to_md(input_data).strip()
+    if not output_schema:
+        return input_data
+
+    input_md = dict_to_md(input_data).strip()
     output_schema = expand_simplified_json_schema(output_schema)["properties"]
 
-    def extract_value(text: str, field_name: str, field_type: str, description: str, existing_values: dict) -> Any:
+    def strip_non_numeric_chars(s):
+        while len(s) > 0 and not s[0].isdigit():
+            s = s[1:]
+        while len(s) > 0 and not s[-1].isdigit():
+            s = s[:-1]
+        return s
+
+    async def create_json_object(target: str, schema, get_value: Callable, current_obj=None, root_obj=None, parent_key='', prefix=''):
+        if current_obj is None:
+            current_obj = {}
+            root_obj = {}
+
+        for name, properties in schema.items():
+            full_key = f'{parent_key}.{name}' if parent_key else name
+            if properties['type'] == 'object':
+                current_obj[name] = await create_json_object(target, properties['properties'], get_value, {}, root_obj, full_key)
+            else:
+                description = properties.get('description')
+                enum = properties.get('enum', None)
+                if prefix:
+                    description = prefix + (description[:1].lower() + description[1:])
+                value = await get_value(target, full_key, properties['type'], description, enum, root_obj)
+                current_obj[name] = value
+                root_obj[full_key] = value
+
+        return current_obj
+
+    async def extract_value(text: str, field_name: str, field_type: str, description: str, enum: list, existing_values: dict) -> Any:
         """
         Extract value of type `field_type` from `text` based on `description`.
         `{}` placeholders in `description` will be formatted using `existing_values` dict which has flat dot notation keys
         (e.g. person.age if there is a person object with an age field).
         """
+        if enum:
+            # if an enum of values is given for the field, perform a classification instead of extraction
+            return (await classifier.classify(text, enum)).max_label
+
         question = description + "?" if not description.endswith("?") else description
         question = question.format(**existing_values)
         question = question[:1].upper() + question[1:]  # capitalize first word
 
-        answer = qa.answer(text, question, confidence_threshold=0.01)
+        qa_result = await qa.answer(text, question, confidence_threshold=0.01)
 
-        if answer is None:
+        if qa_result is None:
             return None
 
         if field_type == "integer":
             try:
-                return int(strip_non_numeric_chars(answer))
+                return int(strip_non_numeric_chars(qa_result.answer))
             except ValueError:
                 return None
         elif field_type == "number":
             try:
-                return float(strip_non_numeric_chars(answer))
+                return float(strip_non_numeric_chars(qa_result.answer))
             except ValueError:
                 return None
         else:
-            return answer.strip(" .,;:!?")
+            return qa_result.answer.strip(" .,;:!?")
 
     if not multiple:
-        return create_json_object(input_md, output_schema, extract_value)
+        return await create_json_object(input_md, output_schema, extract_value)
     else:
-        language = indentify_language(input_md)
-        tagger = SpacyPOSTagger(language=language)
-        classifier = TransformersClassifier(model=DEFAULT_MODEL_EN if language == "en" else DEFAULT_MODEL_MULTI)
-
-        pos_tags = tagger.tag(input_md)
-        candidates = filter_and_join(pos_tags)
-
-        if not multiple_description:
-            raise Exception("Description for entity type is required.")
-
-        entities = []
-        for candidate in candidates:
-            true_label = multiple_description.lower()
-            false_label = f"not {true_label}"
-            result = classifier.classify(candidate, [true_label, false_label], confidence_threshold=0.75)
-            if result == true_label:
-                entities.append(candidate)
+        if not multiple_description or multiple_description.isspace():
+            raise MissingParameterError("Description for entity type is required.")
+
+        result = await token_classifier.classify(input_md, classes=[multiple_description], confidence_threshold=0.75)
+        entities = [s.word for s in result.spans]
 
         # to specify the current entity we are interested in, we mark it in the context and prepend a hint to the description
         description_prefix = f"For the {multiple_description} marked by << >>, "
         extracted = [
-            create_json_object(input_md.replace(entity, f"<< {entity} >>"), output_schema, extract_value, prefix=description_prefix)
+            await create_json_object(input_md.replace(entity, f"<< {entity} >>"), output_schema, extract_value, prefix=description_prefix)
             for entity in entities
         ]
 
         def clean_dict_strings(d):
             for key, value in d.items():
                 if isinstance(value, str):
                     d[key] = re.sub(r'<<\s|\s>>', '', value)
```

### Comparing `bpm_ai-1.2.0/bpm_ai/generic/generic.openai.prompt` & `bpm_ai-1.3.0/bpm_ai/generic/generic.openai.prompt`

 * *Files 3% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 Your task is to help users execute their business processes by performing a given task.
 
 You will receive a task description and context information that may help with the task.
 Perform the task based on the description and context information and store the result.
 
 [# user #]
 # CONTEXT
-{{context}}
+{{context | markdown}}
 
 # TASK DESCRIPTION
 {{task}}
 
 Make sure to get this right, this is very important for my career!
```

### Comparing `bpm_ai-1.2.0/bpm_ai/translate/translate.py` & `bpm_ai-1.3.0/bpm_ai/translate/translate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,82 @@
 from bpm_ai_core.llm.common.llm import LLM
-from bpm_ai_core.llm.common.message import ToolCallsMessage
-from bpm_ai_core.llm.common.tool import Tool
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
 from bpm_ai_core.tracing.decorators import trace
 from bpm_ai_core.translation.nmt import NMTModel
 
-from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_images
+from bpm_ai.common.errors import MissingParameterError, LanguageNotFoundError
+from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents
 from bpm_ai.translate.schema import get_translation_output_schema
 
 
 @trace("bpm-ai-translate", ["llm"])
 async def translate_llm(
-    llm: LLM,
-    input_data: dict[str, str | dict],
-    target_language: str,
-    ocr: OCR | None = None,
-    asr: ASRModel | None = None
+        llm: LLM,
+        input_data: dict[str, str | dict | None],
+        target_language: str,
+        ocr: OCR | None = None,
+        asr: ASRModel | None = None
 ) -> dict:
-    tool = Tool.from_callable(
-        "store_translation",
-        f"Stores the finished translation into {target_language}.",
-        args_schema=get_translation_output_schema(input_data, target_language),
-        callable=lambda **x: x
-    )
+    input_items = {k: v for k, v in input_data.items() if v is not None}
+    if not input_items:
+        return input_data
+
+    if not target_language or target_language.isspace():
+        raise MissingParameterError("target language is required")
 
-    if llm.supports_images():
-        input_data = prepare_images_for_llm_prompt(input_data)
+    if not ocr and llm.supports_images():
+        input_items = prepare_images_for_llm_prompt(input_items)
     else:
-        input_data = await ocr_images(input_data, ocr)
-    input_data = await transcribe_audio(input_data, asr)
+        input_items = await ocr_documents(input_items, ocr)
+    input_items = await transcribe_audio(input_items, asr)
 
     prompt = Prompt.from_file(
         "translate",
-        input=input_data,
+        input=input_items,
         lang=target_language
     )
 
-    result = await llm.predict(prompt, tools=[tool])
+    compose_schema = {
+        "name": "store_translation",
+        "description": f"Stores the finished translation into {target_language}.",
+        "type": "object",
+        "properties": get_translation_output_schema(input_items, target_language)
+    }
 
-    if isinstance(result, ToolCallsMessage):
-        return result.tool_calls[0].invoke()
-    else:
-        return {}
+    message = await llm.generate_message(prompt, output_schema=compose_schema)
+
+    return {k: message.content.get(k, None) for k in input_data.keys()}
 
 
 @trace("bpm-ai-translate", ["nmt"])
 async def translate_nmt(
-    nmt: NMTModel,
-    input_data: dict[str, str | dict],
-    target_language: str,
-    ocr: OCR | None = None,
-    asr: ASRModel | None = None
+        nmt: NMTModel,
+        input_data: dict[str, str | dict | None],
+        target_language: str,
+        ocr: OCR | None = None,
+        asr: ASRModel | None = None
 ) -> dict:
-    input_data = await ocr_images(input_data, ocr)
-    input_data = await transcribe_audio(input_data, asr)
+    input_items = {k: v for k, v in input_data.items() if v is not None}
+    if not input_items:
+        return input_data
+
+    if not target_language or target_language.isspace():
+        raise MissingParameterError("target language is required")
+
+    input_items = await ocr_documents(input_items, ocr)
+    input_items = await transcribe_audio(input_items, asr)
 
     try:
         import langcodes
         target_language_code = langcodes.find(target_language).language
     except ImportError:
         raise ImportError('langcodes is not installed')
     except LookupError:
-        raise Exception(f"Could not identify target language '{target_language}'.")
-
-    texts_to_translate = list(input_data.values())  # todo handle potential None values
-    translated_texts = nmt.translate(texts_to_translate, target_language_code)
+        raise LanguageNotFoundError(f"Could not identify target language '{target_language}'.")
 
-    return {k: translated_texts[i] for i, k in enumerate(input_data.keys())}
+    texts_to_translate = list(input_items.values())
+    texts_translated = await nmt.translate(texts_to_translate, target_language_code)
+    input_items_translated = {k: texts_translated[i] for i, k in enumerate(input_items.keys())}
 
+    return {k: input_items_translated.get(k, None) for k in input_data.keys()}
```

### Comparing `bpm_ai-1.2.0/PKG-INFO` & `bpm_ai-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: bpm-ai
-Version: 1.2.0
+Version: 1.3.0
 Summary: AI task automation for BPM engines.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: inference
-Requires-Dist: bpm-ai-core (==1.2.0)
-Requires-Dist: faster-whisper (>=0.10.0,<0.11.0) ; extra == "inference"
-Requires-Dist: langcodes[data] (>=3.3.0,<4.0.0) ; extra == "inference"
+Requires-Dist: aiobotocore (>=2.12.1,<3.0.0)
+Requires-Dist: amazon-textract-prettyprinter (>=0.1.9,<0.2.0)
+Requires-Dist: anthropic (>=0.20.0,<0.21.0)
+Requires-Dist: azure-ai-documentintelligence (>=1.0.0b2,<2.0.0)
+Requires-Dist: azure-ai-translation-text (>=1.0.0b1,<2.0.0)
+Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0)
+Requires-Dist: bpm-ai-core (==2.2.0)
 Requires-Dist: langfuse (>=2.13.3,<3.0.0)
-Requires-Dist: lingua-language-detector (>=2.0.2,<3.0.0) ; extra == "inference"
-Requires-Dist: nltk (>=3.8.1,<4.0.0) ; extra == "inference"
 Requires-Dist: openai (>=1.11.0,<2.0.0)
-Requires-Dist: pytesseract (>=0.3.10,<0.4.0) ; extra == "inference"
-Requires-Dist: sacremoses (>=0.1.1,<0.2.0) ; extra == "inference"
-Requires-Dist: sentencepiece (>=0.1.99,<0.2.0) ; extra == "inference"
-Requires-Dist: transformers (>=4.37.2,<5.0.0) ; extra == "inference"
 Project-URL: Repository, https://github.com/holunda-io/bpm-ai
 Description-Content-Type: text/markdown
 
 # bpm-ai
 _AI task automation for BPM engines._
 
 See [camunda-8-connector-gpt](https://github.com/holunda-io/camunda-8-connector-gpt) for actual integration with the Camunda Platform 8 BPM engine using custom BPMN elements (Connectors).
```

