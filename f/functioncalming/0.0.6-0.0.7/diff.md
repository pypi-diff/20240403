# Comparing `tmp/functioncalming-0.0.6.tar.gz` & `tmp/functioncalming-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functioncalming-0.0.6.tar", max compression
+gzip compressed data, was "functioncalming-0.0.7.tar", max compression
```

## Comparing `functioncalming-0.0.6.tar` & `functioncalming-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1081 2023-12-03 18:19:47.739079 functioncalming-0.0.6/LICENSE
--rw-r--r--   0        0        0     7116 2023-12-05 21:08:31.350633 functioncalming-0.0.6/README.md
--rw-r--r--   0        0        0       90 2023-12-03 18:19:47.744765 functioncalming-0.0.6/functioncalming/__init__.py
--rw-r--r--   0        0        0    16753 2024-03-24 15:48:38.527346 functioncalming-0.0.6/functioncalming/client.py
--rw-r--r--   0        0        0     4308 2024-03-17 18:30:02.836518 functioncalming-0.0.6/functioncalming/distil.py
--rw-r--r--   0        0        0     7004 2024-03-15 11:32:43.170300 functioncalming-0.0.6/functioncalming/utils.py
--rw-r--r--   0        0        0      749 2024-03-24 15:51:25.173851 functioncalming-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     7871 1970-01-01 00:00:00.000000 functioncalming-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-03 13:50:14.359647 functioncalming-0.0.7/LICENSE
+-rw-r--r--   0        0        0     7412 2024-04-03 17:49:36.616998 functioncalming-0.0.7/README.md
+-rw-r--r--   0        0        0       90 2024-04-03 13:50:14.359876 functioncalming-0.0.7/functioncalming/__init__.py
+-rw-r--r--   0        0        0    22304 2024-04-03 17:55:37.039789 functioncalming-0.0.7/functioncalming/client.py
+-rw-r--r--   0        0        0     4308 2024-04-03 13:50:14.360289 functioncalming-0.0.7/functioncalming/distil.py
+-rw-r--r--   0        0        0     7047 2024-04-03 17:22:50.208270 functioncalming-0.0.7/functioncalming/utils.py
+-rw-r--r--   0        0        0      749 2024-04-03 17:55:59.808034 functioncalming-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8167 1970-01-01 00:00:00.000000 functioncalming-0.0.7/PKG-INFO
```

### Comparing `functioncalming-0.0.6/LICENSE` & `functioncalming-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `functioncalming-0.0.6/README.md` & `functioncalming-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 functioncalming comes with support for:
 - Structured responses from the LLM via pydantic models
 - Structured responses from the LLM via plain python function (pydantic argument validation happens under the hood)
 - Parallel function calling, as well as giving the model a choice of multiple different tools
 - Automatically passing function/tool results back to the model
 - Automatic message history re-writing to hide failed function calls that were re-tried
 - Create fine-tuning data to make model better at calling your functions/models with near zero config
-- Create fine-tuning data for distilling a complex pipeline to a simple model via a simple decorator (`@distillery`) 
+- Create fine-tuning data for distilling a complex pipeline to a simple model via a simple decorator (`@distillery`)
+- Reporting the cost of your API requests (using OpenAI pricing as of April 2024)
 
 ## Who is this for?
 Basically, functioncalming provides useful utilities for any case where you find yourself using function calling in OpenAI. 
 However, it particularly shines in use-cases where any of the following are the case:
 - LLM responses are consumed in a mostly machine-facing way (i.e. the output of the LLM is used in a workflow instead of direct conversation with a user)
 - LLMs are used for data extraction, i.e. you just want to extract a possibly complex and nested structured object from an input (rather than just calling e.g. a simple `get_weather()`-style function)
 - The same function(s) are called over and over again, and you want to fine-tune a cheaper model to reach the level of quality that GPT-4 offers
@@ -25,57 +26,60 @@
 
 ```python
 from pydantic import BaseModel
 from functioncalming.client import get_completion
 
 
 class Actor(BaseModel):
-  """
-  A person or non-human actor involved in a situation
-  """
-  name: str
-  adjectives: list[str]
+    """
+    A person or non-human actor involved in a situation
+    """
+    name: str
+    adjectives: list[str]
 
 
 class Situation(BaseModel):
-  """
-  A situation or event involving a number of actors
-  """
-  actors: list[Actor]
-  action: str
+    """
+    A situation or event involving a number of actors
+    """
+    actors: list[Actor]
+    action: str
 
 
 class EmojiTranslation(BaseModel):
-  translation: str
+    translation: str
 
 
 PROMPT = """You help extract cleaned data from unstructured input text 
 and simultaneously (but separately) turn the text into an Emoji-translation.
 You also have a tendency to always make a mistake the first time you call a function, but then do it correctly.
 """
 
 history = [
-  {'role': 'system', 'content': PROMPT},
-  {'role': 'user', 'content': "The quick brown fox jumps over the lazy dog"}
+    {'role': 'system', 'content': PROMPT},
+    {'role': 'user', 'content': "The quick brown fox jumps over the lazy dog"}
 ]
 
 
 async def main():
-  responses, cleaned_history = await get_completion(
-    history=history,
-    tools=[Situation, EmojiTranslation],
-    temperature=0,
-    retries=1,
-    rewrite_log_destination='finetune.jsonl',
-    rewrite_history_in_place=False  # this is on by default, turning it off here so you can see the different histories 
-  )
-  print(responses[0].model_dump_json(
-    indent=4))  # {"actors": [{"name": "fox", "adjectives": ["quick", "brown"]}, {"name": "dog", "adjectives": ["lazy"]}], "action": "jumping over"}
-  print(responses[1].model_dump_json(indent=4))  # {"translation": "🦊↗️🐶"}
-  print(f"Real history: {len(history)} messages. Rewritten history: {len(cleaned_history)} messages.")
+    calm_response = await get_completion(
+        messages=history,
+        tools=[Situation, EmojiTranslation],
+        temperature=0,
+        retries=1,
+        rewrite_log_destination='finetune.jsonl', 
+    )
+    print(calm_response.success)
+    print(calm_response.retries_done)
+    print(calm_response.usage)  # total tokens used 
+    print(calm_response.cost)  # estimated dollar cost of all requests that were done
+    print(calm_response.tool_call_results[0].model_dump_json(
+        indent=4))  # {"actors": [{"name": "fox", "adjectives": ["quick", "brown"]}, {"name": "dog", "adjectives": ["lazy"]}], "action": "jumping over"}
+    print(calm_response.tool_call_results[1].model_dump_json(indent=4))  # {"translation": "🦊↗️🐶"}
+    print(f"Clean, rewritten history: {len(calm_response.messages)} messages. Real history: {len(calm_response.messages_raw)} messages.")
 ```
 ## Generating fine-tuning data for distillation
 functioncalming tries to make it easy to generate data for function distillation - i.e. fine-tuning a cheaper, faster "student" pipeline
 to perform a complex task that can be reliably achieved using a more expensive, slower "teacher" pipeline. The ideas is to track the inputs 
 and outputs of the teacher pipeline and use them to train the student pipeline to perform the task directly.
 
 What functioncalming provides here is a simple interface to "clean up" and augment the message history of the teacher pipeline to
```

### Comparing `functioncalming-0.0.6/functioncalming/client.py` & `functioncalming-0.0.7/functioncalming/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+import dataclasses
 import uuid
 
 import json
 import logging
 import os
 from typing import Callable, TextIO, Awaitable, Literal
+from functools import cached_property
 
+from openai._types import NOT_GIVEN
 from openai.types.chat.chat_completion_message_tool_call import Function
 from pydantic import BaseModel, ValidationError
 from openai import AsyncOpenAI
-from openai._types import NotGiven, NOT_GIVEN
+
 from openai.types.chat import ChatCompletion, ChatCompletionMessage, ChatCompletionMessageToolCall, \
     ChatCompletionToolMessageParam, ChatCompletionSystemMessageParam, ChatCompletionUserMessageParam, \
-    ChatCompletionToolChoiceOptionParam
-
+    ChatCompletionToolChoiceOptionParam, ChatCompletionAssistantMessageParam, ChatCompletionMessageParam
+from openai.types.completion_usage import CompletionUsage
 from functioncalming.utils import Messages, invoke_callback_function, FineTuningData, InnerValidationError, \
-    create_openai_function, OpenAIFunction
+    create_openai_function, OpenAIFunction, ToolCallError
 
 _client = None
 
 
 def get_client():
     global _client
     if not _client:
@@ -34,198 +37,336 @@
     global _client
     _client = client
 
 
 DEFAULT_BEHAVIOR = "default_behavior"
 
 
-type SimpleJsonCompatible = str | int | float | bool | None
-type JsonCompatible = dict[str, JsonCompatible] | list[JsonCompatible] | SimpleJsonCompatible
-type ModelOrJsonCompatible = BaseModel | JsonCompatible
-type BaseModelFunction = Callable[..., ModelOrJsonCompatible] | Callable[..., Awaitable[ModelOrJsonCompatible]]
+type SimpleJsonCompatible = str | int | float | bool
+type JsonCompatible = dict[str, SimpleJsonCompatible | JsonCompatible] | list[SimpleJsonCompatible | JsonCompatible] | SimpleJsonCompatible
+type BaseModelOrJsonCompatible = BaseModel | JsonCompatible
+type BaseModelFunction = Callable[..., BaseModelOrJsonCompatible] | Callable[..., Awaitable[BaseModelOrJsonCompatible]]
+
+
+COSTS_BY_MODEL = {
+    # GPT-4 Turbo
+    "gpt-4-turbo": (0.01, 0.03),
+    "gpt-4-0125-preview": (0.01, 0.03),  # actually a Turbo model
+    "gpt-4-1106-preview": (0.01, 0.03),  # actually a Turbo model
+    "gpt-4-vision-preview": (0.01, 0.03),
+    "gpt-4-1106-vision-preview": (0.01, 0.03),
+    # GPT-4
+    "gpt-4": (0.03, 0.06),
+    "gpt-4-0613": (0.03, 0.06),
+    "gpt-4-32k": (0.06, 0.12),
+    "gpt-4-32k-0613": (0.06, 0.12),
+    # GPT 3.5
+    "gpt-3.5-turbo": (0.0005, 0.0015),
+    "gpt-3.5-turbo-0125": (0.0005, 0.0015),
+    "gpt-3.5-turbo-1106": (0.0005, 0.0015),
+    "gpt-3.5-turbo-0301": (0.0005, 0.0015),  # available in playground but not in docs?
+    "gpt-3.5-turbo-instruct": (0.0015, 0.0020),  # not actually a chat model
+    # deprecated 3.5
+    "gpt-3.5-turbo-0613": (0.0005, 0.0015),
+    "gpt-3.5-turbo-16k-0613": (0.0005, 0.0015),
+    "gpt-3.5-turbo-16k": (0.0005, 0.0015),
+}
+
+
+class ToolCallShortcut:
+    def __init__(self, message: ChatCompletionMessage):
+        self.model = None
+        self.message: ChatCompletionMessage = message
+        self.usage: CompletionUsage = CompletionUsage(
+            completion_tokens=0, prompt_tokens=0, total_tokens=0
+        )
+
+
+@dataclasses.dataclass
+class CalmResponse:
+    success: bool
+    tool_call_results: list[BaseModelOrJsonCompatible]
+    messages: Messages
+    error: Exception | None
+    retries_done: int
+
+    _rewritten_from: int
+    _omitted_messages: Messages
+    _unaltered_first_message: ChatCompletionMessageParam | None
+
+    # multiple completions means there were retries
+    raw_completions: list[ChatCompletion | ToolCallShortcut]
+    """
+    All the ChatCompletion objects returned by OpenAI during this call, ordered chronologically (last is newest).
+    Multiple completions may be returned if retrys were performed.
+    """
+
+    @cached_property
+    def messages_raw(self):
+        """The non-rewritten message history as it was actually performed against the API."""
+        res = self.messages[:self._rewritten_from] + self._omitted_messages
+        if self._unaltered_first_message is not None:
+            res[0] = self._unaltered_first_message
+        return res
+
+    @property
+    def last_message(self) -> ChatCompletionAssistantMessageParam:
+        return self.messages[-1]
+
+    @property
+    def model(self) -> str | None:
+        return self._cost_model_usage[0]
+
+    @property
+    def cost(self) -> float:
+        return self._cost_model_usage[1]
+
+    @property
+    def usage(self) -> CompletionUsage:
+        return self._cost_model_usage[2]
+
+    @cached_property
+    def _cost_model_usage(self) -> tuple[str | None, float, CompletionUsage]:
+        total_cost = 0.
+        model = None
+        usage = CompletionUsage(
+            completion_tokens=0, prompt_tokens=0, total_tokens=0
+        )
+        for completion in self.raw_completions:
+            if completion.model is None:
+                continue
+            # we never switch models between retries for now, not sure if that will ever change
+            model = completion.model
+            prompt_tokens = completion.usage.prompt_tokens
+            completion_tokens = completion.usage.completion_tokens
+            prompt_costs_per_1k, completion_costs_per_1k = COSTS_BY_MODEL[model]
+            usage.completion_tokens += completion_tokens
+            usage.prompt_tokens += prompt_tokens
+            total_cost += (
+                    prompt_costs_per_1k * prompt_tokens / 1000.
+                    + completion_costs_per_1k * completion_tokens / 1000.
+            )
+        usage.total_tokens = usage.prompt_tokens + usage.completion_tokens
+        return model, total_cost, usage
 
 
 async def get_completion(
-        history: Messages | None = None,
+        messages: Messages | None = None,
         system_prompt: str | None = None,
         user_message: str | None = None,
         distil_system_prompt: str | None = None,
         tools: list[type[BaseModel] | BaseModelFunction] | None = None,
         tool_choice: Literal[DEFAULT_BEHAVIOR] | ChatCompletionToolChoiceOptionParam = DEFAULT_BEHAVIOR,
         retries: int = 0,
-        pass_results_to_model: bool = False,
-        rewrite_history_in_place: bool = True,
+        pass_results_to_model: bool = True,
         rewrite_log_destination: str | TextIO | None = None,
         rewrite_log_extra_data: dict | None = None,
         openai_client: AsyncOpenAI | None = None,
-        model_name: Literal["gpt-3.5-turbo", "gpt-4-1106-preview"] | str = None,
+        model: Literal["gpt-3.5-turbo", "gpt-4-1106-preview"] | str = None,
         **kwargs
-) -> tuple[list[BaseModel], Messages]:
+) -> CalmResponse:
     """
     Get a completion with validated function call responses from the chat completions API.
 
-    :param history: Message history. Should be None if system_prompt and/or user_message are set
+    :param messages: Message history. Should be None if system_prompt and/or user_message are set
     :param system_prompt: Initial system message (will be added to the beginning of the history - typically used without a 'history' param)
-        (if set, do not supply a system message in 'history')
+        (if set, do not supply an initial system message in 'history')
     :param user_message: Next user message (will be appended to the history)
     :param distil_system_prompt: If set, the first message of the history will be rewritten to this system message
         (useful for distillation trainng data generation)
     :param tools: list of available tools, given either as BaseModels or functions that return BaseModel instances
     :param tool_choice: By default, forces a tool call if only one tool is available. Otherwise, same as vanilla OpenAI
     :param retries: number of attempts to give the model to fix broken function calls (first try not counted)
-    :param rewrite_history_in_place: If true, the messages list that was passed in will be modified in-place
+    :param rewrite_history_in_place: If true, the history that was passed in will be modified in-place
     :param pass_results_to_model: If true, function results (or created models) are added to the message history
     :param rewrite_log_destination: filename or io handle to log fine-tuning data to
     :param rewrite_log_extra_data: extra data to merge into the jsonl line for this log entry
     :param openai_client: optional AsyncOpenAI client to use (use set_client() to set a default client)
-    :param model_name: Which OpenAI model to use for the completion
+    :param model: Which OpenAI model to use for the completion
     :param kwargs:
     :return: a tuple of (created models or function responses, rewritten message history)
     """
-    history = initialize_and_validate_history(
-        history=history,
+    # make a copy, we do not edit the passed-in message history
+    if messages is not None:
+        messages = messages[:]
+
+    messages = initialize_and_validate_message_history(
+        messages=messages,
         system_prompt=system_prompt,
         user_message=user_message,
         distil_system_prompt=distil_system_prompt
     )
-    rewrite_cutoff = len(history)
+    rewrite_cutoff = len(messages)
     openai_client = openai_client or get_client()
 
-    model_name = model_name or os.environ.get("OPENAI_MODEL")
-    if model_name is None:
+    model = model or os.environ.get("OPENAI_MODEL")
+    if model is None:
         raise ValueError("No model specified and OPENAI_MODEL is not set.")
 
     tools = tools or []
     openai_functions, distillery_openai_functions = process_tool_definitions(tools)
     available_function_names: set[str] = set(openai_functions.keys())
 
     result_instances: list[BaseModel] = []
-    retries_done = -2
+    tries_done = 0  # first try is not a retry
     successful_tool_calls: list[ChatCompletionMessageToolCall] = []
     successful_tool_responses: list[ChatCompletionToolMessageParam] = []
+    last_message_dict = None
 
     errors: list[Exception] | None = []
-    while (retries_done := retries_done + 1) < retries:
+    raw_completions: list[ChatCompletion | ToolCallShortcut] = []
+    while tries_done + 1 <= 1 + retries:
+        tries_done += 1
         if tool_choice == DEFAULT_BEHAVIOR:
             current_tool_choice = get_tool_choice_for_default_behavior(available_function_names)
         else:
             current_tool_choice = tool_choice
 
-        shortcut = await maybe_shortcut_trivial_function_call(available_function_names, openai_functions)
+        shortcut: ChatCompletionMessage | None = await maybe_shortcut_trivial_function_call(
+            available_function_names,
+            openai_functions
+        )
+
         if shortcut is not None:
             last_message = shortcut
+            raw_completions.append(
+                ToolCallShortcut(message=shortcut)
+            )
         else:
             completion: ChatCompletion = await openai_client.chat.completions.create(
-                messages=history,
-                model=model_name,
+                messages=messages,
+                model=model,
                 tools=[openai_functions[name].tool_definition for name in available_function_names] or NOT_GIVEN,
-                tool_choice=current_tool_choice if tools else NOT_GIVEN,
+                tool_choice=current_tool_choice,
                 **kwargs
             )
+            raw_completions.append(completion)
             last_message: ChatCompletionMessage = completion.choices[0].message
-        history.append(last_message.model_dump(exclude_unset=True))  # make sure the history only has dict objects
+
+        messages.append(last_message.model_dump(
+            exclude_unset=True, exclude_none=True
+        ))  # make sure the history only has dict objects
 
         if not last_message.tool_calls:
             break
 
         num_successful = 0
         num_failed = 0
-        current_errors = []
+        current_errors: list[ValidationError | ToolCallError] = []
         new_available_function_names = set()
         for tool_call in last_message.tool_calls:
             function_name = tool_call.function.name
 
             if function_name not in openai_functions:
-                e = ValueError(f"Error: function `{function_name}` does not exist.")
+                e = ToolCallError(f"Error: function `{function_name}` does not exist.")
                 handle_function_calling_error(
-                    e=e, current_errors=current_errors, history=history, tool_call=tool_call
+                    e=e, current_errors=current_errors, history=messages, tool_call=tool_call
                 )
                 new_available_function_names = available_function_names  # could be anything
                 num_failed += 1
                 continue
 
             openai_function = openai_functions[function_name]
-            arguments = json.loads(tool_call.function.arguments)
+            try:
+                arguments = json.loads(tool_call.function.arguments)
+            except json.JSONDecodeError as e:
+                new_available_function_names.add(function_name)  # available for retry
+                handle_function_calling_error(
+                    e=e, current_errors=current_errors, history=messages, tool_call=tool_call
+                )
+                num_failed += 1
+                continue
+
             try:
                 result_instance, result_for_model, maybe_serialized_result = await invoke_callback_function(
                     openai_function,
                     kwargs=arguments,
-                    history=history,
+                    history=messages,
                     serialize_result_for_model=pass_results_to_model
                 )
                 tool_response = ChatCompletionToolMessageParam(
                     role="tool",
                     tool_call_id=tool_call.id,
                     content=result_for_model
                 )
                 if openai_function.is_distillery:
                     distillery_tool = distillery_openai_functions[function_name]
                     tool_call, tool_response = adjust_distillery_call_for_clean_history(
                         new_function_name=distillery_tool.name,
                         serialized_result=maybe_serialized_result,
                         tool_call=tool_call
                     )
-                history.append(tool_response)
+                messages.append(tool_response)
                 result_instances.append(result_instance)
                 successful_tool_calls.append(tool_call)
                 successful_tool_responses.append(tool_response)
                 num_successful += 1
             except InnerValidationError as e:
                 # There is not really a need for any custom handling vs. other exceptions here - we just raise.
-                # I am just making clear that *inner* validation errors should not lead to a retry,
+                # I am just making clear that *inner* validation errors will not lead to a retry,
                 # since the model did fine calling the tool here.
+                # To force a retry due to a semantic error the model should correct, raise a ToolCallError instead
                 raise e
-            except ValidationError as e:
+            except (ValidationError, ToolCallError) as e:
                 new_available_function_names.add(function_name)  # available for retry
                 handle_function_calling_error(
-                    e=e, current_errors=current_errors, history=history, tool_call=tool_call
+                    e=e, current_errors=current_errors, history=messages, tool_call=tool_call
                 )
                 num_failed += 1
 
         if not num_failed:
             errors = []
             break
 
-        logging.debug(f"Attempt {retries_done + 2}/{retries + 1}: {num_failed} errors")
+        logging.debug(f"Attempt {tries_done}/{retries + 1}: {num_failed} errors")
         errors = current_errors
-        history.append({
+        messages.append({
             "role": "system",
             "content": f"{num_failed}/{num_failed + num_successful} tool calls failed. "
                        f"Please carefully recall the function definition(s) and repeat all failed calls "
                        f"(but only repeat the failed calls!)."
         })
         available_function_names = new_available_function_names
 
-    if errors:
-        raise ExceptionGroup("Function calling validation errors", errors)
-
-    rewritten_history = rewrite_history(
-        history=history,
+    unaltered_first_message, omitted_messages = rewrite_message_history(
+        messages=messages,
         rewrite_cutoff=rewrite_cutoff,
-        in_place=rewrite_history_in_place,
         successful_tool_calls=successful_tool_calls,
         successful_tool_responses=successful_tool_responses,
         distil_system_prompt=distil_system_prompt,
     )
 
-    if rewrite_log_destination is not None:
+    final_error = None
+    if errors:
+        final_error = ExceptionGroup("Function calling validation errors", errors)
+    elif rewrite_log_destination is not None:
         functions_coalesced: list[OpenAIFunction] = list({**openai_functions, **distillery_openai_functions}.values())
         log_finetuning_data(
             destination=rewrite_log_destination,
-            messages=rewritten_history,
+            messages=messages,
             functions=functions_coalesced,
             extra_data=rewrite_log_extra_data
         )
 
-    return result_instances, rewritten_history
+    return CalmResponse(
+        success=final_error is None,
+        tool_call_results=result_instances,
+        messages=messages,
+        _rewritten_from=rewrite_cutoff,
+        _omitted_messages=omitted_messages,
+        _unaltered_first_message=unaltered_first_message,
+        error=final_error,
+        retries_done=tries_done - 1,
+        raw_completions=raw_completions
+    )
 
 
 def handle_function_calling_error(
-        e: Exception,
-        current_errors: list[Exception],
+        e: ValidationError | ToolCallError | json.JSONDecodeError,
+        current_errors: list[ValidationError | ToolCallError | json.JSONDecodeError],
         history: Messages,
         tool_call
 ):
     tool_response = ChatCompletionToolMessageParam(
         role="tool",
         tool_call_id=tool_call.id,
         content=f"Error: {e}"
@@ -254,54 +395,54 @@
                         )
                     )
                 ]
             )
     return last_message
 
 
-def initialize_and_validate_history(
-        history: Messages | None, system_prompt, user_message, distil_system_prompt
+def initialize_and_validate_message_history(
+        messages: Messages | None, system_prompt, user_message, distil_system_prompt
 ) -> Messages:
     """
     Initialize and update the history in-place based on the supplied system prompt and user_message.
     After this call, we guarantee that, if a distil_system_prompt was supplied, the first message in the history is a
     system message (which will be replaced with the distillation prompt during history rewriting).
     """
+    messages = messages[:] if messages is not None else []
 
-    history = history if history is not None else []
-    if not (history or system_prompt or user_message):
+    if not (messages or system_prompt or user_message):
         raise ValueError(
             "No input - supply at least 'messages', 'system_prompt' and/or 'user_message'"
         )
 
     if system_prompt:
-        if history:
+        if messages:
             # TODO maybe just raise on this? Is this ever a useful way to call get_completion in practice?
             logging.warning(
                 "Both 'history' and 'system_prompt' were supplied, "
                 "be aware that the system_prompt will be inserted at the beginning of the history."
             )
 
-        if history and history[0].role == "system":
+        if messages and messages[0]["role"] == "system":
             raise ValueError(
                 "First message in history was already a system message! "
                 "Cowardly refusing to replace it / append another one."
             )
-        history.insert(0, ChatCompletionSystemMessageParam(role="system", content=system_prompt))
+        messages.insert(0, ChatCompletionSystemMessageParam(role="system", content=system_prompt))
 
     if user_message:
-        history.append(ChatCompletionUserMessageParam(role="user", content=user_message))
+        messages.append(ChatCompletionUserMessageParam(role="user", content=user_message))
 
-    if distil_system_prompt and history[0]["role"] != "system":
+    if distil_system_prompt and messages[0]["role"] != "system":
         raise ValueError(
             "Cannot use 'distil_system_prompt' if the first message in the history is not a system message. "
             "Either use the 'system_message' param or supply a history that starts with a system message."
         )
 
-    return history
+    return messages
 
 
 def process_tool_definitions(tools_raw):
     openai_functions: dict[str, OpenAIFunction] = {}
     # Note: these are indexed by their original name
     distillery_openai_functions: dict[str, OpenAIFunction] = {}
     for model_or_fn in tools_raw:
@@ -315,15 +456,17 @@
     return openai_functions, distillery_openai_functions
 
 
 def get_tool_choice_for_default_behavior(
         openai_function_names: list[str] | set[str]
 ) -> ChatCompletionToolChoiceOptionParam:
     tool_choice: ChatCompletionToolChoiceOptionParam
-    if len(openai_function_names) == 1:
+    if not openai_function_names:
+        tool_choice = NOT_GIVEN
+    elif len(openai_function_names) == 1:
         tool_choice = {"type": "function", "function": {"name": list(openai_function_names)[0]}}
     else:
         tool_choice = "auto"
     return tool_choice
 
 
 def adjust_distillery_call_for_clean_history(
@@ -344,47 +487,47 @@
         role="tool",
         tool_call_id=tool_call.id,
         content='{"result": "success"}',
     )
     return adjusted_tool_call, adjusted_tool_response
 
 
-def rewrite_history(
+def rewrite_message_history(
         *,
-        history: Messages,
+        messages: Messages,
         rewrite_cutoff: int,
-        in_place: bool,
         successful_tool_calls: list[ChatCompletionMessageToolCall],
         successful_tool_responses: list[ChatCompletionToolMessageParam],
         distil_system_prompt: str | None,
-) -> Messages:
+):
     """
     Rewrite the history by removing all messages (not just the failed calls) and replacing them with a single clean
     multi call and its responses, starting from the cutoff index.
     """
-    if in_place:
-        clean_history = history
-    else:
-        # edit a copy
-        clean_history = [message.copy() for message in history]
-
+    unaltered_first_message = None
+    omitted_messages = messages[rewrite_cutoff:]
     if successful_tool_calls:
         if distil_system_prompt is not None:
-            clean_history[0]["content"] = distil_system_prompt
+            unaltered_first_message = messages[0]
+            assert unaltered_first_message["role"] == "system", "First message must be a system message when using 'distil_system_prompt'"
+            messages[0] = {
+                **messages[0],
+                "content": distil_system_prompt
+            }
 
-        clean_history[rewrite_cutoff:] = [
+        messages[rewrite_cutoff:] = [
             {
                 "role": "assistant",
                 "tool_calls": [tc.model_dump() for tc in successful_tool_calls],
                 "content": None,
             },
             *successful_tool_responses
         ]
+    return unaltered_first_message, omitted_messages
 
-    return clean_history
 
 
 def log_finetuning_data(
         destination: str | TextIO,
         messages: Messages,
         functions: list[OpenAIFunction],
         extra_data: dict | None = None
```

### Comparing `functioncalming-0.0.6/functioncalming/distil.py` & `functioncalming-0.0.7/functioncalming/distil.py`

 * *Files identical despite different names*

### Comparing `functioncalming-0.0.6/functioncalming/utils.py` & `functioncalming-0.0.7/functioncalming/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
 class InnerValidationError(Exception):
     def __init__(self, messages, original_error):
         super().__init__(messages)
         self.original_error = original_error
 
 
+class ToolCallError(ValueError):
+    pass
+
 @dataclasses.dataclass
 class OpenAIFunction:
     name: str
     definition: FunctionDefinition
     callback: Callable[[...], Awaitable[BaseModel]]
     callback_expects_user_message: bool
     callback_expects_args_from_model: bool
```

### Comparing `functioncalming-0.0.6/pyproject.toml` & `functioncalming-0.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "functioncalming"
-version = "0.0.6"
+version = "0.0.7"
 description = "Robust and reliable OpenAI function calling"
 authors = ["Philipp Dowling <phdowling@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/phdowling/functioncalming"
 repository = "https://github.com/phdowling/functioncalming"
 keywords = ["openai", "function-calling", "distillation", "fine-tuning", "pydantic", "validation", "llm"]
```

### Comparing `functioncalming-0.0.6/PKG-INFO` & `functioncalming-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functioncalming
-Version: 0.0.6
+Version: 0.0.7
 Summary: Robust and reliable OpenAI function calling
 Home-page: https://github.com/phdowling/functioncalming
 License: MIT
 Keywords: openai,function-calling,distillation,fine-tuning,pydantic,validation,llm
 Author: Philipp Dowling
 Author-email: phdowling@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
@@ -25,15 +25,16 @@
 functioncalming comes with support for:
 - Structured responses from the LLM via pydantic models
 - Structured responses from the LLM via plain python function (pydantic argument validation happens under the hood)
 - Parallel function calling, as well as giving the model a choice of multiple different tools
 - Automatically passing function/tool results back to the model
 - Automatic message history re-writing to hide failed function calls that were re-tried
 - Create fine-tuning data to make model better at calling your functions/models with near zero config
-- Create fine-tuning data for distilling a complex pipeline to a simple model via a simple decorator (`@distillery`) 
+- Create fine-tuning data for distilling a complex pipeline to a simple model via a simple decorator (`@distillery`)
+- Reporting the cost of your API requests (using OpenAI pricing as of April 2024)
 
 ## Who is this for?
 Basically, functioncalming provides useful utilities for any case where you find yourself using function calling in OpenAI. 
 However, it particularly shines in use-cases where any of the following are the case:
 - LLM responses are consumed in a mostly machine-facing way (i.e. the output of the LLM is used in a workflow instead of direct conversation with a user)
 - LLMs are used for data extraction, i.e. you just want to extract a possibly complex and nested structured object from an input (rather than just calling e.g. a simple `get_weather()`-style function)
 - The same function(s) are called over and over again, and you want to fine-tune a cheaper model to reach the level of quality that GPT-4 offers
@@ -44,57 +45,60 @@
 
 ```python
 from pydantic import BaseModel
 from functioncalming.client import get_completion
 
 
 class Actor(BaseModel):
-  """
-  A person or non-human actor involved in a situation
-  """
-  name: str
-  adjectives: list[str]
+    """
+    A person or non-human actor involved in a situation
+    """
+    name: str
+    adjectives: list[str]
 
 
 class Situation(BaseModel):
-  """
-  A situation or event involving a number of actors
-  """
-  actors: list[Actor]
-  action: str
+    """
+    A situation or event involving a number of actors
+    """
+    actors: list[Actor]
+    action: str
 
 
 class EmojiTranslation(BaseModel):
-  translation: str
+    translation: str
 
 
 PROMPT = """You help extract cleaned data from unstructured input text 
 and simultaneously (but separately) turn the text into an Emoji-translation.
 You also have a tendency to always make a mistake the first time you call a function, but then do it correctly.
 """
 
 history = [
-  {'role': 'system', 'content': PROMPT},
-  {'role': 'user', 'content': "The quick brown fox jumps over the lazy dog"}
+    {'role': 'system', 'content': PROMPT},
+    {'role': 'user', 'content': "The quick brown fox jumps over the lazy dog"}
 ]
 
 
 async def main():
-  responses, cleaned_history = await get_completion(
-    history=history,
-    tools=[Situation, EmojiTranslation],
-    temperature=0,
-    retries=1,
-    rewrite_log_destination='finetune.jsonl',
-    rewrite_history_in_place=False  # this is on by default, turning it off here so you can see the different histories 
-  )
-  print(responses[0].model_dump_json(
-    indent=4))  # {"actors": [{"name": "fox", "adjectives": ["quick", "brown"]}, {"name": "dog", "adjectives": ["lazy"]}], "action": "jumping over"}
-  print(responses[1].model_dump_json(indent=4))  # {"translation": "🦊↗️🐶"}
-  print(f"Real history: {len(history)} messages. Rewritten history: {len(cleaned_history)} messages.")
+    calm_response = await get_completion(
+        messages=history,
+        tools=[Situation, EmojiTranslation],
+        temperature=0,
+        retries=1,
+        rewrite_log_destination='finetune.jsonl', 
+    )
+    print(calm_response.success)
+    print(calm_response.retries_done)
+    print(calm_response.usage)  # total tokens used 
+    print(calm_response.cost)  # estimated dollar cost of all requests that were done
+    print(calm_response.tool_call_results[0].model_dump_json(
+        indent=4))  # {"actors": [{"name": "fox", "adjectives": ["quick", "brown"]}, {"name": "dog", "adjectives": ["lazy"]}], "action": "jumping over"}
+    print(calm_response.tool_call_results[1].model_dump_json(indent=4))  # {"translation": "🦊↗️🐶"}
+    print(f"Clean, rewritten history: {len(calm_response.messages)} messages. Real history: {len(calm_response.messages_raw)} messages.")
 ```
 ## Generating fine-tuning data for distillation
 functioncalming tries to make it easy to generate data for function distillation - i.e. fine-tuning a cheaper, faster "student" pipeline
 to perform a complex task that can be reliably achieved using a more expensive, slower "teacher" pipeline. The ideas is to track the inputs 
 and outputs of the teacher pipeline and use them to train the student pipeline to perform the task directly.
 
 What functioncalming provides here is a simple interface to "clean up" and augment the message history of the teacher pipeline to
```

