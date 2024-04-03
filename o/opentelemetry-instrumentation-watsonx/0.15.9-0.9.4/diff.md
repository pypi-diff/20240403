# Comparing `tmp/opentelemetry_instrumentation_watsonx-0.15.9.tar.gz` & `tmp/opentelemetry_instrumentation_watsonx-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_watsonx-0.15.9.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_watsonx-0.9.4.tar", max compression
```

## Comparing `opentelemetry_instrumentation_watsonx-0.15.9.tar` & `opentelemetry_instrumentation_watsonx-0.9.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1495 2024-04-03 18:13:50.333438 opentelemetry_instrumentation_watsonx-0.15.9/README.md
--rw-r--r--   0        0        0    17250 2024-04-03 18:13:50.333438 opentelemetry_instrumentation_watsonx-0.15.9/opentelemetry/instrumentation/watsonx/__init__.py
--rw-r--r--   0        0        0       23 2024-04-03 18:13:50.333438 opentelemetry_instrumentation_watsonx-0.15.9/opentelemetry/instrumentation/watsonx/version.py
--rw-r--r--   0        0        0     1008 2024-04-03 18:14:27.057462 opentelemetry_instrumentation_watsonx-0.15.9/pyproject.toml
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_watsonx-0.15.9/PKG-INFO
+-rw-r--r--   0        0        0      880 2024-01-22 09:18:14.865253 opentelemetry_instrumentation_watsonx-0.9.4/README.md
+-rw-r--r--   0        0        0     6485 2024-01-22 09:18:14.865487 opentelemetry_instrumentation_watsonx-0.9.4/opentelemetry/instrumentation/watsonx/__init__.py
+-rw-r--r--   0        0        0       22 2024-01-22 09:18:34.075879 opentelemetry_instrumentation_watsonx-0.9.4/opentelemetry/instrumentation/watsonx/version.py
+-rw-r--r--   0        0        0      669 2024-01-22 09:18:34.076307 opentelemetry_instrumentation_watsonx-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_watsonx-0.9.4/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_watsonx-0.15.9/README.md` & `opentelemetry_instrumentation_watsonx-0.9.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,21 @@
 # OpenTelemetry IBM Watsonx Instrumentation
 
-This library allows tracing IBM Watsonx prompts and completions sent with the official [IBM Watson Machine Learning library](https://ibm.github.io/watson-machine-learning-sdk/) and [IBM watsonx.ai library](https://ibm.github.io/watsonx-ai-python-sdk/).
+This library allows tracing IBM Watsonx prompts and completions sent with the official [IBM Watson Machine Learning library](https://ibm.github.io/watson-machine-learning-sdk/).
 
 ## Installation
 
 ```bash
 pip install opentelemetry-instrumentation-watsonx
 ```
 
-## Example usage
-
-```python
-from opentelemetry.instrumentation.watsonx import WatsonxInstrumentor
-
-WatsonxInstrumentor().instrument()
-```
-
 ## Privacy
 
 **By default, this instrumentation logs prompts, completions, and embeddings to span attributes**. This gives you a clear visibility into how your LLM application is working, and can make it easy to debug and evaluate the quality of the outputs.
 
 However, you may want to disable this logging for privacy reasons, as they may contain highly sensitive data from your users. You may also simply want to reduce the size of your traces.
 
 To disable logging, set the `TRACELOOP_TRACE_CONTENT` environment variable to `false`.
 
 ```bash
 TRACELOOP_TRACE_CONTENT=false
 ```
-
-## SSL Issue
-
-In case of SSL handshake issues (or similar ones) as follows:
-
-```
-E0423 17:04:25.197068000 6150713344 ssl_transport_security.cc:1420]    Handshake failed with fatal error SSL_ERROR_SSL: error:100000f7:SSL routines:OPENSSL_internal:WRONG_VERSION_NUMBER.
-```
-
-You can instruct the exporter with an environment variable to ignore SSL errors:
-
-```bash
-OTEL_EXPORTER_OTLP_INSECURE=true
-```
```

