# Comparing `tmp/crewai_tools-0.1.1.tar.gz` & `tmp/crewai_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewai_tools-0.1.1.tar", max compression
+gzip compressed data, was "crewai_tools-0.1.2.tar", max compression
```

## Comparing `crewai_tools-0.1.1.tar` & `crewai_tools-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.1.1/LICENSE
--rw-r--r--   0        0        0     3550 2024-02-26 00:09:39.177886 crewai_tools-0.1.1/README.md
--rw-r--r--   0        0        0      470 2024-03-03 02:54:55.157064 crewai_tools-0.1.1/crewai_tools/__init__.py
--rw-r--r--   0        0        0      429 2024-02-19 18:49:52.166367 crewai_tools-0.1.1/crewai_tools/adapters/embedchain_adapter.py
--rw-r--r--   0        0        0     1578 2024-02-15 17:02:16.898153 crewai_tools-0.1.1/crewai_tools/adapters/lancedb_adapter.py
--rw-r--r--   0        0        0     1410 2024-03-03 02:54:59.436707 crewai_tools-0.1.1/crewai_tools/tools/__init__.py
--rw-r--r--   0        0        0     3943 2024-03-27 18:00:56.574243 crewai_tools-0.1.1/crewai_tools/tools/base_tool.py
--rw-r--r--   0        0        0     1565 2024-03-04 01:02:54.866445 crewai_tools-0.1.1/crewai_tools/tools/code_docs_search_tool/README.md
--rw-r--r--   0        0        0     1453 2024-02-29 06:10:11.672785 crewai_tools-0.1.1/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
--rw-r--r--   0        0        0     1138 2024-03-04 01:07:57.443721 crewai_tools-0.1.1/crewai_tools/tools/csv_search_tool/README.md
--rw-r--r--   0        0        0     1331 2024-03-03 15:29:12.068295 crewai_tools-0.1.1/crewai_tools/tools/csv_search_tool/csv_search_tool.py
--rw-r--r--   0        0        0     2258 2024-03-04 01:05:53.487986 crewai_tools-0.1.1/crewai_tools/tools/directory_read_tool/README.md
--rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.1.1/crewai_tools/tools/directory_read_tool/directory_read_tool.py
--rw-r--r--   0        0        0     1314 2024-03-04 00:35:07.074998 crewai_tools-0.1.1/crewai_tools/tools/directory_search_tool/README.md
--rw-r--r--   0        0        0     1532 2024-02-29 06:10:11.673860 crewai_tools-0.1.1/crewai_tools/tools/directory_search_tool/directory_search_tool.py
--rw-r--r--   0        0        0     1258 2024-03-04 00:29:09.058885 crewai_tools-0.1.1/crewai_tools/tools/docx_search_tool/README.md
--rw-r--r--   0        0        0     1356 2024-02-29 06:10:11.674025 crewai_tools-0.1.1/crewai_tools/tools/docx_search_tool/docx_search_tool.py
--rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.1.1/crewai_tools/tools/file_read_tool/README.md
--rw-r--r--   0        0        0     1056 2024-02-29 06:10:11.674186 crewai_tools-0.1.1/crewai_tools/tools/file_read_tool/file_read_tool.py
--rw-r--r--   0        0        0     1989 2024-03-04 00:39:53.329530 crewai_tools-0.1.1/crewai_tools/tools/github_search_tool/README.md
--rw-r--r--   0        0        0     1793 2024-02-29 06:10:11.674317 crewai_tools-0.1.1/crewai_tools/tools/github_search_tool/github_search_tool.py
--rw-r--r--   0        0        0     1408 2024-03-04 00:31:06.781039 crewai_tools-0.1.1/crewai_tools/tools/json_search_tool/README.md
--rw-r--r--   0        0        0     1406 2024-02-29 06:10:11.674477 crewai_tools-0.1.1/crewai_tools/tools/json_search_tool/json_search_tool.py
--rw-r--r--   0        0        0     1239 2024-03-04 01:13:20.542050 crewai_tools-0.1.1/crewai_tools/tools/mdx_seach_tool/README.md
--rw-r--r--   0        0        0     1331 2024-02-29 06:10:11.674631 crewai_tools-0.1.1/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
--rw-r--r--   0        0        0     1170 2024-03-04 00:58:59.103102 crewai_tools-0.1.1/crewai_tools/tools/pdf_search_tool/README.md
--rw-r--r--   0        0        0     1308 2024-03-07 23:29:34.084694 crewai_tools-0.1.1/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
--rw-r--r--   0        0        0     1514 2024-03-04 00:32:22.700352 crewai_tools-0.1.1/crewai_tools/tools/pg_seach_tool/README.md
--rw-r--r--   0        0        0     1623 2024-02-29 06:10:11.674950 crewai_tools-0.1.1/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
--rw-r--r--   0        0        0     2025 2024-03-04 00:43:27.494777 crewai_tools-0.1.1/crewai_tools/tools/rag/README.md
--rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.1.1/crewai_tools/tools/rag/__init__.py
--rw-r--r--   0        0        0     1363 2024-02-22 15:03:25.187705 crewai_tools-0.1.1/crewai_tools/tools/rag/rag_tool.py
--rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.1.1/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
--rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.1.1/crewai_tools/tools/scrape_website_tool/README.md
--rw-r--r--   0        0        0     2107 2024-03-02 15:41:34.656120 crewai_tools-0.1.1/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
--rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.1.1/crewai_tools/tools/selenium_scraping_tool/README.md
--rw-r--r--   0        0        0     2558 2024-02-29 06:10:11.665178 crewai_tools-0.1.1/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
--rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.1.1/crewai_tools/tools/serper_dev_tool/README.md
--rw-r--r--   0        0        0     1365 2024-03-03 02:55:52.486790 crewai_tools-0.1.1/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
--rw-r--r--   0        0        0     1574 2024-03-04 00:49:03.619139 crewai_tools-0.1.1/crewai_tools/tools/txt_search_tool/README.md
--rw-r--r--   0        0        0     1336 2024-02-29 06:10:11.675422 crewai_tools-0.1.1/crewai_tools/tools/txt_search_tool/txt_search_tool.py
--rw-r--r--   0        0        0     1458 2024-03-04 00:50:22.840678 crewai_tools-0.1.1/crewai_tools/tools/website_search/README.md
--rw-r--r--   0        0        0     1441 2024-02-29 06:10:11.675559 crewai_tools-0.1.1/crewai_tools/tools/website_search/website_search_tool.py
--rw-r--r--   0        0        0     1518 2024-03-04 01:02:02.859522 crewai_tools-0.1.1/crewai_tools/tools/xml_search_tool/README.md
--rw-r--r--   0        0        0     1331 2024-02-29 06:10:11.675704 crewai_tools-0.1.1/crewai_tools/tools/xml_search_tool/xml_search_tool.py
--rw-r--r--   0        0        0     1609 2024-03-04 00:57:27.654128 crewai_tools-0.1.1/crewai_tools/tools/youtube_channel_search_tool/README.md
--rw-r--r--   0        0        0     1809 2024-02-29 06:10:11.675978 crewai_tools-0.1.1/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
--rw-r--r--   0        0        0     1828 2024-03-04 01:04:20.171207 crewai_tools-0.1.1/crewai_tools/tools/youtube_video_search_tool/README.md
--rw-r--r--   0        0        0     1613 2024-02-29 06:10:11.676133 crewai_tools-0.1.1/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
--rw-r--r--   0        0        0      730 2024-03-27 18:01:03.044679 crewai_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 crewai_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3550 2024-02-26 00:09:39.177886 crewai_tools-0.1.2/README.md
+-rw-r--r--   0        0        0      470 2024-03-03 02:54:55.157064 crewai_tools-0.1.2/crewai_tools/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.1.2/crewai_tools/adapters/embedchain_adapter.py
+-rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.1.2/crewai_tools/adapters/lancedb_adapter.py
+-rw-r--r--   0        0        0     1410 2024-03-03 02:54:59.436707 crewai_tools-0.1.2/crewai_tools/tools/__init__.py
+-rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.1.2/crewai_tools/tools/base_tool.py
+-rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.1.2/crewai_tools/tools/code_docs_search_tool/README.md
+-rw-r--r--   0        0        0     1541 2024-03-27 18:04:45.820264 crewai_tools-0.1.2/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
+-rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.1.2/crewai_tools/tools/csv_search_tool/README.md
+-rw-r--r--   0        0        0     1439 2024-03-27 18:04:45.821112 crewai_tools-0.1.2/crewai_tools/tools/csv_search_tool/csv_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.1.2/crewai_tools/tools/directory_read_tool/README.md
+-rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.1.2/crewai_tools/tools/directory_read_tool/directory_read_tool.py
+-rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.1.2/crewai_tools/tools/directory_search_tool/README.md
+-rw-r--r--   0        0        0     1598 2024-03-27 18:04:45.822270 crewai_tools-0.1.2/crewai_tools/tools/directory_search_tool/directory_search_tool.py
+-rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.1.2/crewai_tools/tools/docx_search_tool/README.md
+-rw-r--r--   0        0        0     1460 2024-03-27 18:04:45.823331 crewai_tools-0.1.2/crewai_tools/tools/docx_search_tool/docx_search_tool.py
+-rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.1.2/crewai_tools/tools/file_read_tool/README.md
+-rw-r--r--   0        0        0     1056 2024-02-29 06:10:11.674186 crewai_tools-0.1.2/crewai_tools/tools/file_read_tool/file_read_tool.py
+-rw-r--r--   0        0        0     2733 2024-03-27 18:04:45.823902 crewai_tools-0.1.2/crewai_tools/tools/github_search_tool/README.md
+-rw-r--r--   0        0        0     1854 2024-03-27 18:04:45.824045 crewai_tools-0.1.2/crewai_tools/tools/github_search_tool/github_search_tool.py
+-rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.1.2/crewai_tools/tools/json_search_tool/README.md
+-rw-r--r--   0        0        0     1495 2024-03-27 18:04:45.824458 crewai_tools-0.1.2/crewai_tools/tools/json_search_tool/json_search_tool.py
+-rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.1.2/crewai_tools/tools/mdx_seach_tool/README.md
+-rw-r--r--   0        0        0     1439 2024-03-27 18:04:45.825044 crewai_tools-0.1.2/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
+-rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.1.2/crewai_tools/tools/pdf_search_tool/README.md
+-rw-r--r--   0        0        0     1421 2024-03-27 18:04:45.826870 crewai_tools-0.1.2/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
+-rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.1.2/crewai_tools/tools/pg_seach_tool/README.md
+-rw-r--r--   0        0        0     1246 2024-03-27 18:04:45.827249 crewai_tools-0.1.2/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
+-rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.1.2/crewai_tools/tools/rag/README.md
+-rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.1.2/crewai_tools/tools/rag/__init__.py
+-rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.1.2/crewai_tools/tools/rag/rag_tool.py
+-rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.1.2/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
+-rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.1.2/crewai_tools/tools/scrape_website_tool/README.md
+-rw-r--r--   0        0        0     2107 2024-03-02 15:41:34.656120 crewai_tools-0.1.2/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
+-rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.1.2/crewai_tools/tools/selenium_scraping_tool/README.md
+-rw-r--r--   0        0        0     2558 2024-02-29 06:10:11.665178 crewai_tools-0.1.2/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
+-rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.1.2/crewai_tools/tools/serper_dev_tool/README.md
+-rw-r--r--   0        0        0     1365 2024-03-03 02:55:52.486790 crewai_tools-0.1.2/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
+-rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.1.2/crewai_tools/tools/txt_search_tool/README.md
+-rw-r--r--   0        0        0     1445 2024-03-27 18:04:45.828786 crewai_tools-0.1.2/crewai_tools/tools/txt_search_tool/txt_search_tool.py
+-rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.1.2/crewai_tools/tools/website_search/README.md
+-rw-r--r--   0        0        0     1531 2024-03-27 18:04:45.829385 crewai_tools-0.1.2/crewai_tools/tools/website_search/website_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.1.2/crewai_tools/tools/xml_search_tool/README.md
+-rw-r--r--   0        0        0     1439 2024-03-27 18:04:45.829923 crewai_tools-0.1.2/crewai_tools/tools/xml_search_tool/xml_search_tool.py
+-rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.1.2/crewai_tools/tools/youtube_channel_search_tool/README.md
+-rw-r--r--   0        0        0     1889 2024-03-27 18:04:45.830546 crewai_tools-0.1.2/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
+-rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.1.2/crewai_tools/tools/youtube_video_search_tool/README.md
+-rw-r--r--   0        0        0     1663 2024-03-27 18:04:45.830891 crewai_tools-0.1.2/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
+-rw-r--r--   0        0        0      730 2024-04-03 09:02:15.231634 crewai_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 crewai_tools-0.1.2/PKG-INFO
```

### Comparing `crewai_tools-0.1.1/LICENSE` & `crewai_tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/README.md` & `crewai_tools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/adapters/lancedb_adapter.py` & `crewai_tools-0.1.2/crewai_tools/adapters/lancedb_adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,19 +31,26 @@
     _db: LanceDBConnection = PrivateAttr()
     _table: LanceDBTable = PrivateAttr()
 
     def model_post_init(self, __context: Any) -> None:
         self._db = lancedb_connect(self.uri)
         self._table = self._db.open_table(self.table_name)
 
-        return super().model_post_init(__context)
+        super().model_post_init(__context)
 
     def query(self, question: str) -> str:
         query = self.embedding_function([question])[0]
         results = (
             self._table.search(query, vector_column_name=self.vector_column_name)
             .limit(self.top_k)
             .select([self.text_column_name])
             .to_list()
         )
         values = [result[self.text_column_name] for result in results]
         return "\n".join(values)
+
+    def add(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        self._table.add(*args, **kwargs)
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/__init__.py` & `crewai_tools-0.1.2/crewai_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/base_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/base_tool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Optional, Type
 
-from pydantic import BaseModel, model_validator
+from langchain_core.tools import StructuredTool
+from pydantic import BaseModel, ConfigDict, Field, validator
 from pydantic.v1 import BaseModel as V1BaseModel
 
-from langchain_core.tools import StructuredTool
 
 class BaseTool(BaseModel, ABC):
+    class _ArgsSchemaPlaceholder(V1BaseModel):
+        pass
+
+    model_config = ConfigDict()
+
     name: str
     """The unique name of the tool that clearly communicates its purpose."""
     description: str
     """Used to tell the model how/when/why to use the tool."""
-    args_schema: Optional[Type[V1BaseModel]] = None
+    args_schema: Type[V1BaseModel] = Field(default_factory=_ArgsSchemaPlaceholder)
     """The schema for the arguments that the tool accepts."""
     description_updated: bool = False
     """Flag to check if the description has been updated."""
     cache_function: Optional[Callable] = lambda _args, _result: True
     """Function that will be used to determine if the tool should be cached, should return a boolean. If None, the tool will be cached."""
 
-    @model_validator(mode="after")
-    def _check_args_schema(self):
-        self._set_args_schema()
+    @validator("args_schema", always=True, pre=True)
+    def _default_args_schema(cls, v: Type[V1BaseModel]) -> Type[V1BaseModel]:
+        if not isinstance(v, cls._ArgsSchemaPlaceholder):
+            return v
+
+        return type(
+            f"{cls.__name__}Schema",
+            (V1BaseModel,),
+            {
+                "__annotations__": {
+                    k: v for k, v in cls._run.__annotations__.items() if k != "return"
+                },
+            },
+        )
+
+    def model_post_init(self, __context: Any) -> None:
         self._generate_description()
-        return self
+
+        super().model_post_init(__context)
 
     def run(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> Any:
         print(f"Using Tool: {self.name}")
@@ -53,24 +72,28 @@
         if self.args_schema is None:
             class_name = f"{self.__class__.__name__}Schema"
             self.args_schema = type(
                 class_name,
                 (V1BaseModel,),
                 {
                     "__annotations__": {
-                        k: v for k, v in self._run.__annotations__.items() if k != 'return'
+                        k: v
+                        for k, v in self._run.__annotations__.items()
+                        if k != "return"
                     },
                 },
             )
+
     def _generate_description(self):
         args = []
-        for arg, attribute in self.args_schema.schema()['properties'].items():
-            args.append(f"{arg}: '{attribute['type']}'")
+        for arg, attribute in self.args_schema.schema()["properties"].items():
+            if "type" in attribute:
+                args.append(f"{arg}: '{attribute['type']}'")
 
-        description = self.description.replace('\n', ' ')
+        description = self.description.replace("\n", " ")
         self.description = f"{self.name}({', '.join(args)}) - {description}"
 
 
 class Tool(BaseTool):
     func: Callable
     """The function that will be executed when the tool is called."""
 
@@ -89,35 +112,35 @@
     Decorator to create a tool from a function.
     """
 
     def _make_with_name(tool_name: str) -> Callable:
         def _make_tool(f: Callable) -> BaseTool:
             if f.__doc__ is None:
                 raise ValueError("Function must have a docstring")
+            if f.__annotations__ is None:
+                raise ValueError("Function must have type annotations")
 
-            args_schema = None
-            if f.__annotations__:
-                class_name = "".join(tool_name.split()).title()
-                args_schema = type(
-                    class_name,
-                    (V1BaseModel,),
-                    {
-                        "__annotations__": {
-                            k: v for k, v in f.__annotations__.items() if k != 'return'
-                        },
+            class_name = "".join(tool_name.split()).title()
+            args_schema = type(
+                class_name,
+                (V1BaseModel,),
+                {
+                    "__annotations__": {
+                        k: v for k, v in f.__annotations__.items() if k != "return"
                     },
-                )
+                },
+            )
 
             return Tool(
                 name=tool_name,
                 description=f.__doc__,
                 func=f,
                 args_schema=args_schema,
             )
 
         return _make_tool
 
     if len(args) == 1 and callable(args[0]):
         return _make_with_name(args[0].__name__)(args[0])
     if len(args) == 1 and isinstance(args[0], str):
         return _make_with_name(args[0])
-    raise ValueError("Invalid arguments")
+    raise ValueError("Invalid arguments")
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,52 @@
-from typing import Optional, Type, Any
-from pydantic.v1 import BaseModel, Field
+from typing import Any, Optional, Type
 
-from embedchain import App
 from embedchain.models.data_type import DataType
+from pydantic.v1 import BaseModel, Field
 
 from ..rag.rag_tool import RagTool
 
 
 class FixedCodeDocsSearchToolSchema(BaseModel):
-	"""Input for CodeDocsSearchTool."""
-	search_query: str = Field(..., description="Mandatory search query you want to use to search the Code Docs content")
+    """Input for CodeDocsSearchTool."""
+
+    search_query: str = Field(
+        ...,
+        description="Mandatory search query you want to use to search the Code Docs content",
+    )
+
 
 class CodeDocsSearchToolSchema(FixedCodeDocsSearchToolSchema):
-	"""Input for CodeDocsSearchTool."""
-	docs_url: str = Field(..., description="Mandatory docs_url path you want to search")
+    """Input for CodeDocsSearchTool."""
+
+    docs_url: str = Field(..., description="Mandatory docs_url path you want to search")
+
 
 class CodeDocsSearchTool(RagTool):
-	name: str = "Search a Code Docs content"
-	description: str = "A tool that can be used to semantic search a query from a Code Docs content."
-	summarize: bool = False
-	args_schema: Type[BaseModel] = CodeDocsSearchToolSchema
-	docs_url: Optional[str] = None
-
-	def __init__(self, docs_url: Optional[str] = None, **kwargs):
-		super().__init__(**kwargs)
-		if docs_url is not None:
-			self.docs_url = docs_url
-			self.description = f"A tool that can be used to semantic search a query the {docs_url} Code Docs content."
-			self.args_schema = FixedCodeDocsSearchToolSchema
-			self._generate_description()
-
-	def _run(
-		self,
-		search_query: str,
-		**kwargs: Any,
-	) -> Any:
-		docs_url = kwargs.get('docs_url', self.docs_url)
-		self.app = App()
-		self.app.add(docs_url, data_type=DataType.DOCS_SITE)
-		return super()._run(query=search_query)
+    name: str = "Search a Code Docs content"
+    description: str = (
+        "A tool that can be used to semantic search a query from a Code Docs content."
+    )
+    args_schema: Type[BaseModel] = CodeDocsSearchToolSchema
+
+    def __init__(self, docs_url: Optional[str] = None, **kwargs):
+        super().__init__(**kwargs)
+        if docs_url is not None:
+            self.add(docs_url)
+            self.description = f"A tool that can be used to semantic search a query the {docs_url} Code Docs content."
+            self.args_schema = FixedCodeDocsSearchToolSchema
+
+    def add(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        kwargs["data_type"] = DataType.DOCS_SITE
+        super().add(*args, **kwargs)
+
+    def _before_run(
+        self,
+        query: str,
+        **kwargs: Any,
+    ) -> Any:
+        if "docs_url" in kwargs:
+            self.add(kwargs["docs_url"])
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/directory_read_tool/README.md` & `crewai_tools-0.1.2/crewai_tools/tools/directory_read_tool/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -135,8 +135,8 @@
 00000860: 6172 6974 792c 2063 6f6e 7369 7374 656e  arity, consisten
 00000870: 6379 2c20 616e 6420 6164 6865 7265 6e63  cy, and adherenc
 00000880: 6520 746f 2074 6865 2068 6967 682d 7175  e to the high-qu
 00000890: 616c 6974 7920 7374 616e 6461 7264 7320  ality standards 
 000008a0: 6578 656d 706c 6966 6965 6420 696e 2074  exemplified in t
 000008b0: 6865 2070 726f 7669 6465 6420 646f 6375  he provided docu
 000008c0: 6d65 6e74 6174 696f 6e20 6578 616d 706c  mentation exampl
-000008d0: 652e                                     e.
+000008d0: 652e 0a                                  e..
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/directory_read_tool/directory_read_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/directory_read_tool/directory_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/directory_search_tool/directory_search_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/directory_search_tool/directory_search_tool.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,52 @@
-from typing import Optional, Type, Any
-from pydantic.v1 import BaseModel, Field
+from typing import Any, Optional, Type
 
-from embedchain import App
 from embedchain.loaders.directory_loader import DirectoryLoader
+from pydantic.v1 import BaseModel, Field
 
 from ..rag.rag_tool import RagTool
 
 
 class FixedDirectorySearchToolSchema(BaseModel):
-	"""Input for DirectorySearchTool."""
-	search_query: str = Field(..., description="Mandatory search query you want to use to search the directory's content")
+    """Input for DirectorySearchTool."""
+
+    search_query: str = Field(
+        ...,
+        description="Mandatory search query you want to use to search the directory's content",
+    )
+
 
 class DirectorySearchToolSchema(FixedDirectorySearchToolSchema):
-	"""Input for DirectorySearchTool."""
-	directory: str = Field(..., description="Mandatory directory you want to search")
+    """Input for DirectorySearchTool."""
+
+    directory: str = Field(..., description="Mandatory directory you want to search")
+
 
 class DirectorySearchTool(RagTool):
-	name: str = "Search a directory's content"
-	description: str = "A tool that can be used to semantic search a query from a directory's content."
-	summarize: bool = False
-	args_schema: Type[BaseModel] = DirectorySearchToolSchema
-	directory: Optional[str] = None
-
-	def __init__(self, directory: Optional[str] = None, **kwargs):
-		super().__init__(**kwargs)
-		if directory is not None:
-			self.directory = directory
-			self.description = f"A tool that can be used to semantic search a query the {directory} directory's content."
-			self.args_schema = FixedDirectorySearchToolSchema
-			self._generate_description()
-
-	def _run(
-		self,
-		search_query: str,
-		**kwargs: Any,
-	) -> Any:
-		directory = kwargs.get('directory', self.directory)
-		loader = DirectoryLoader(config=dict(recursive=True))
-		self.app = App()
-		self.app.add(directory, loader=loader)
-		return super()._run(query=search_query)
+    name: str = "Search a directory's content"
+    description: str = (
+        "A tool that can be used to semantic search a query from a directory's content."
+    )
+    args_schema: Type[BaseModel] = DirectorySearchToolSchema
+
+    def __init__(self, directory: Optional[str] = None, **kwargs):
+        super().__init__(**kwargs)
+        if directory is not None:
+            self.add(directory)
+            self.description = f"A tool that can be used to semantic search a query the {directory} directory's content."
+            self.args_schema = FixedDirectorySearchToolSchema
+
+    def add(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        kwargs["loader"] = DirectoryLoader(config=dict(recursive=True))
+        super().add(*args, **kwargs)
+
+    def _before_run(
+        self,
+        query: str,
+        **kwargs: Any,
+    ) -> Any:
+        if "directory" in kwargs:
+            self.add(kwargs["directory"])
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/file_read_tool/README.md` & `crewai_tools-0.1.2/crewai_tools/tools/file_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/file_read_tool/file_read_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/file_read_tool/file_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/github_search_tool/README.md` & `crewai_tools-0.1.2/crewai_tools/tools/github_search_tool/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -30,7 +30,35 @@
 	content_types=['code', 'issue'] # Options: code, repo, pr, issue
 )
 ```
 
 ## Arguments
 - `github_repo` : The URL of the GitHub repository where the search will be conducted. This is a mandatory field and specifies the target repository for your search.
 - `content_types` : Specifies the types of content to include in your search. You must provide a list of content types from the following options: `code` for searching within the code, `repo` for searching within the repository's general information, `pr` for searching within pull requests, and `issue` for searching within issues. This field is mandatory and allows tailoring the search to specific content types within the GitHub repository.
+
+## Custom model and embeddings
+
+By default, the tool uses OpenAI for both embeddings and summarization. To customize the model, you can use a config dictionary as follows:
+
+```python
+tool = GitHubSearchTool(
+    config=dict(
+        llm=dict(
+            provider="ollama", # or google, openai, anthropic, llama2, ...
+            config=dict(
+                model="llama2",
+                # temperature=0.5,
+                # top_p=1,
+                # stream=true,
+            ),
+        ),
+        embedder=dict(
+            provider="google",
+            config=dict(
+                model="models/embedding-001",
+                task_type="retrieval_document",
+                # title="Embeddings",
+            ),
+        ),
+    )
+)
+```
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/github_search_tool/github_search_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/github_search_tool/github_search_tool.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,58 @@
-from typing import Optional, Type, List, Any
-from pydantic.v1 import BaseModel, Field
+from typing import Any, List, Optional, Type
 
-from embedchain import App
 from embedchain.loaders.github import GithubLoader
+from pydantic.v1 import BaseModel, Field
 
 from ..rag.rag_tool import RagTool
 
 
 class FixedGithubSearchToolSchema(BaseModel):
-	"""Input for GithubSearchTool."""
-	search_query: str = Field(..., description="Mandatory search query you want to use to search the github repo's content")
+    """Input for GithubSearchTool."""
+
+    search_query: str = Field(
+        ...,
+        description="Mandatory search query you want to use to search the github repo's content",
+    )
+
 
 class GithubSearchToolSchema(FixedGithubSearchToolSchema):
-	"""Input for GithubSearchTool."""
-	github_repo: str = Field(..., description="Mandatory github you want to search")
-	content_types: List[str] = Field(..., description="Mandatory content types you want to be inlcuded search, options: [code, repo, pr, issue]")
+    """Input for GithubSearchTool."""
+
+    github_repo: str = Field(..., description="Mandatory github you want to search")
+    content_types: List[str] = Field(
+        ...,
+        description="Mandatory content types you want to be inlcuded search, options: [code, repo, pr, issue]",
+    )
+
 
 class GithubSearchTool(RagTool):
-	name: str = "Search a github repo's content"
-	description: str = "A tool that can be used to semantic search a query from a github repo's content."
-	summarize: bool = False
-	gh_token: str = None
-	args_schema: Type[BaseModel] = GithubSearchToolSchema
-	github_repo: Optional[str] = None
-	content_types: List[str]
-
-	def __init__(self, github_repo: Optional[str] = None, **kwargs):
-		super().__init__(**kwargs)
-		if github_repo is not None:
-			self.github_repo = github_repo
-			self.description = f"A tool that can be used to semantic search a query the {github_repo} github repo's content."
-			self.args_schema = FixedGithubSearchToolSchema
-			self._generate_description()
-
-	def _run(
-		self,
-		search_query: str,
-		**kwargs: Any,
-	) -> Any:
-		github_repo = kwargs.get('github_repo', self.github_repo)
-		loader = GithubLoader(config={"token": self.gh_token})
-		app = App()
-		app.add(f"repo:{github_repo} type:{','.join(self.content_types)}", data_type="github", loader=loader)
-		self.app = app
-		return super()._run(query=search_query)
+    name: str = "Search a github repo's content"
+    description: str = "A tool that can be used to semantic search a query from a github repo's content."
+    summarize: bool = False
+    gh_token: str
+    args_schema: Type[BaseModel] = GithubSearchToolSchema
+    content_types: List[str]
+
+    def __init__(self, github_repo: Optional[str] = None, **kwargs):
+        super().__init__(**kwargs)
+        if github_repo is not None:
+            self.add(github_repo)
+            self.description = f"A tool that can be used to semantic search a query the {github_repo} github repo's content."
+            self.args_schema = FixedGithubSearchToolSchema
+
+    def add(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        kwargs["data_type"] = "github"
+        kwargs["loader"] = GithubLoader(config={"token": self.gh_token})
+        super().add(*args, **kwargs)
+
+    def _before_run(
+        self,
+        query: str,
+        **kwargs: Any,
+    ) -> Any:
+        if "github_repo" in kwargs:
+            self.add(kwargs["github_repo"])
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,51 @@
-from typing import Optional, Type, Any
-from pydantic.v1 import BaseModel, Field
+from typing import Any, Optional, Type
 
-from embedchain import App
 from embedchain.models.data_type import DataType
+from pydantic.v1 import BaseModel, Field
 
 from ..rag.rag_tool import RagTool
 
 
-class FixedMDXSearchToolSchema(BaseModel):
-	"""Input for MDXSearchTool."""
-	search_query: str = Field(..., description="Mandatory search query you want to use to search the MDX's content")
-
-class MDXSearchToolSchema(FixedMDXSearchToolSchema):
-	"""Input for MDXSearchTool."""
-	mdx: str = Field(..., description="Mandatory mdx path you want to search")
-
-class MDXSearchTool(RagTool):
-	name: str = "Search a MDX's content"
-	description: str = "A tool that can be used to semantic search a query from a MDX's content."
-	summarize: bool = False
-	args_schema: Type[BaseModel] = MDXSearchToolSchema
-	mdx: Optional[str] = None
-
-	def __init__(self, mdx: Optional[str] = None, **kwargs):
-		super().__init__(**kwargs)
-		if mdx is not None:
-			self.mdx = mdx
-			self.description = f"A tool that can be used to semantic search a query the {mdx} MDX's content."
-			self.args_schema = FixedMDXSearchToolSchema
-			self._generate_description()
-
-	def _run(
-		self,
-		search_query: str,
-		**kwargs: Any,
-	) -> Any:
-		mdx = kwargs.get('mdx', self.mdx)
-		self.app = App()
-		self.app.add(mdx, data_type=DataType.MDX)
-		return super()._run(query=search_query)
+class FixedPDFSearchToolSchema(BaseModel):
+    """Input for PDFSearchTool."""
+
+    query: str = Field(
+        ..., description="Mandatory query you want to use to search the PDF's content"
+    )
+
+
+class PDFSearchToolSchema(FixedPDFSearchToolSchema):
+    """Input for PDFSearchTool."""
+
+    pdf: str = Field(..., description="Mandatory pdf path you want to search")
+
+
+class PDFSearchTool(RagTool):
+    name: str = "Search a PDF's content"
+    description: str = (
+        "A tool that can be used to semantic search a query from a PDF's content."
+    )
+    args_schema: Type[BaseModel] = PDFSearchToolSchema
+
+    def __init__(self, pdf: Optional[str] = None, **kwargs):
+        super().__init__(**kwargs)
+        if pdf is not None:
+            self.add(pdf)
+            self.description = f"A tool that can be used to semantic search a query the {pdf} PDF's content."
+            self.args_schema = FixedPDFSearchToolSchema
+
+    def add(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        kwargs["data_type"] = DataType.PDF_FILE
+        super().add(*args, **kwargs)
+
+    def _before_run(
+        self,
+        query: str,
+        **kwargs: Any,
+    ) -> Any:
+        if "pdf" in kwargs:
+            self.add(kwargs["pdf"])
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/rag/README.md` & `crewai_tools-0.1.2/crewai_tools/tools/rag/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -44,21 +44,18 @@
 rag_tool = RagTool().from_file('path/to/your/file.txt')
 
 # Example: Loading from a directory
 rag_tool = RagTool().from_directory('path/to/your/directory')
 
 # Example: Loading from a web page
 rag_tool = RagTool().from_web_page('https://example.com')
-
-# Example: Loading from an Embedchain configuration
-rag_tool = RagTool().from_embedchain('path/to/your/config.json')
 ```
 
 ## **Contribution**
 
 Contributions to RagTool and the broader CrewAI tools ecosystem are welcome. To contribute, please follow the standard GitHub workflow for forking the repository, making changes, and submitting a pull request.
 
 ## **License**
 
 RagTool is open-source and available under the MIT license.
 
-Thank you for considering RagTool for your knowledge base needs. Your contributions and feedback are invaluable to making RagTool even better.
+Thank you for considering RagTool for your knowledge base needs. Your contributions and feedback are invaluable to making RagTool even better.
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py` & `crewai_tools-0.1.2/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/scrape_website_tool/README.md` & `crewai_tools-0.1.2/crewai_tools/tools/scrape_website_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/selenium_scraping_tool/README.md` & `crewai_tools-0.1.2/crewai_tools/tools/selenium_scraping_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/serper_dev_tool/README.md` & `crewai_tools-0.1.2/crewai_tools/tools/serper_dev_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/txt_search_tool/txt_search_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/txt_search_tool/txt_search_tool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,52 @@
-from typing import Optional, Type, Any
-from pydantic.v1 import BaseModel, Field
+from typing import Any, Optional, Type
 
-from embedchain import App
 from embedchain.models.data_type import DataType
+from pydantic.v1 import BaseModel, Field
 
 from ..rag.rag_tool import RagTool
 
+
 class FixedTXTSearchToolSchema(BaseModel):
-	"""Input for TXTSearchTool."""
-	search_query: str = Field(..., description="Mandatory search query you want to use to search the txt's content")
+    """Input for TXTSearchTool."""
+
+    search_query: str = Field(
+        ...,
+        description="Mandatory search query you want to use to search the txt's content",
+    )
+
 
 class TXTSearchToolSchema(FixedTXTSearchToolSchema):
-	"""Input for TXTSearchTool."""
-	txt: str = Field(..., description="Mandatory txt path you want to search")
+    """Input for TXTSearchTool."""
+
+    txt: str = Field(..., description="Mandatory txt path you want to search")
+
 
 class TXTSearchTool(RagTool):
-	name: str = "Search a txt's content"
-	description: str = "A tool that can be used to semantic search a query from a txt's content."
-	summarize: bool = False
-	args_schema: Type[BaseModel] = TXTSearchToolSchema
-	txt: Optional[str] = None
-
-	def __init__(self, txt: Optional[str] = None, **kwargs):
-		super().__init__(**kwargs)
-		if txt is not None:
-			self.txt = txt
-			self.description = f"A tool that can be used to semantic search a query the {txt} txt's content."
-			self.args_schema = FixedTXTSearchToolSchema
-			self._generate_description()
-
-	def _run(
-		self,
-		search_query: str,
-		**kwargs: Any,
-	) -> Any:
-		txt = kwargs.get('txt', self.txt)
-		self.app = App()
-		self.app.add(txt, data_type=DataType.TEXT_FILE)
-		return super()._run(query=search_query)
+    name: str = "Search a txt's content"
+    description: str = (
+        "A tool that can be used to semantic search a query from a txt's content."
+    )
+    args_schema: Type[BaseModel] = TXTSearchToolSchema
+
+    def __init__(self, txt: Optional[str] = None, **kwargs):
+        super().__init__(**kwargs)
+        if txt is not None:
+            self.add(txt)
+            self.description = f"A tool that can be used to semantic search a query the {txt} txt's content."
+            self.args_schema = FixedTXTSearchToolSchema
+
+    def add(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        kwargs["data_type"] = DataType.TEXT_FILE
+        super().add(*args, **kwargs)
+
+    def _before_run(
+        self,
+        query: str,
+        **kwargs: Any,
+    ) -> Any:
+        if "txt" in kwargs:
+            self.add(kwargs["txt"])
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/website_search/website_search_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/website_search/website_search_tool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,52 @@
-from typing import Optional, Type, Any
-from pydantic.v1 import BaseModel, Field
+from typing import Any, Optional, Type
 
-from embedchain import App
 from embedchain.models.data_type import DataType
+from pydantic.v1 import BaseModel, Field
 
 from ..rag.rag_tool import RagTool
 
 
 class FixedWebsiteSearchToolSchema(BaseModel):
-	"""Input for WebsiteSearchTool."""
-	search_query: str = Field(..., description="Mandatory search query you want to use to search a specific website")
+    """Input for WebsiteSearchTool."""
+
+    search_query: str = Field(
+        ...,
+        description="Mandatory search query you want to use to search a specific website",
+    )
+
 
 class WebsiteSearchToolSchema(FixedWebsiteSearchToolSchema):
-	"""Input for WebsiteSearchTool."""
-	website: str = Field(..., description="Mandatory valid website URL you want to search on")
+    """Input for WebsiteSearchTool."""
+
+    website: str = Field(
+        ..., description="Mandatory valid website URL you want to search on"
+    )
+
 
 class WebsiteSearchTool(RagTool):
-	name: str = "Search in a specific website"
-	description: str = "A tool that can be used to semantic search a query from a specific URL content."
-	summarize: bool = False
-	args_schema: Type[BaseModel] = WebsiteSearchToolSchema
-	website: Optional[str] = None
-
-	def __init__(self, website: Optional[str] = None, **kwargs):
-		super().__init__(**kwargs)
-		if website is not None:
-			self.website = website
-			self.description = f"A tool that can be used to semantic search a query from {website} website content."
-			self.args_schema = FixedWebsiteSearchToolSchema
-			self._generate_description()
-
-	def _run(
-		self,
-		search_query: str,
-		**kwargs: Any,
-	) -> Any:
-		website = kwargs.get('website', self.website)
-		self.app = App()
-		self.app.add(website, data_type=DataType.WEB_PAGE)
-		return super()._run(query=search_query)
+    name: str = "Search in a specific website"
+    description: str = "A tool that can be used to semantic search a query from a specific URL content."
+    args_schema: Type[BaseModel] = WebsiteSearchToolSchema
+
+    def __init__(self, website: Optional[str] = None, **kwargs):
+        super().__init__(**kwargs)
+        if website is not None:
+            self.add(website)
+            self.description = f"A tool that can be used to semantic search a query from {website} website content."
+            self.args_schema = FixedWebsiteSearchToolSchema
+
+    def add(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        kwargs["data_type"] = DataType.WEB_PAGE
+        super().add(*args, **kwargs)
+
+    def _before_run(
+        self,
+        query: str,
+        **kwargs: Any,
+    ) -> Any:
+        if "website" in kwargs:
+            self.add(kwargs["website"])
```

### Comparing `crewai_tools-0.1.1/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py` & `crewai_tools-0.1.2/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,55 @@
-from typing import Optional, Type, Any
-from pydantic.v1 import BaseModel, Field
+from typing import Any, Optional, Type
 
-from embedchain import App
 from embedchain.models.data_type import DataType
+from pydantic.v1 import BaseModel, Field
 
 from ..rag.rag_tool import RagTool
 
 
 class FixedYoutubeChannelSearchToolSchema(BaseModel):
-	"""Input for YoutubeChannelSearchTool."""
-	search_query: str = Field(..., description="Mandatory search query you want to use to search the Youtube Channels content")
+    """Input for YoutubeChannelSearchTool."""
+
+    search_query: str = Field(
+        ...,
+        description="Mandatory search query you want to use to search the Youtube Channels content",
+    )
+
 
 class YoutubeChannelSearchToolSchema(FixedYoutubeChannelSearchToolSchema):
-	"""Input for YoutubeChannelSearchTool."""
-	youtube_channel_handle: str = Field(..., description="Mandatory youtube_channel_handle path you want to search")
+    """Input for YoutubeChannelSearchTool."""
+
+    youtube_channel_handle: str = Field(
+        ..., description="Mandatory youtube_channel_handle path you want to search"
+    )
+
 
 class YoutubeChannelSearchTool(RagTool):
-	name: str = "Search a Youtube Channels content"
-	description: str = "A tool that can be used to semantic search a query from a Youtube Channels content."
-	summarize: bool = False
-	args_schema: Type[BaseModel] = YoutubeChannelSearchToolSchema
-	youtube_channel_handle: Optional[str] = None
-
-	def __init__(self, youtube_channel_handle: Optional[str] = None, **kwargs):
-		super().__init__(**kwargs)
-		if youtube_channel_handle is not None:
-			self.youtube_channel_handle = youtube_channel_handle
-			self.description = f"A tool that can be used to semantic search a query the {youtube_channel_handle} Youtube Channels content."
-			self.args_schema = FixedYoutubeChannelSearchToolSchema
-			self._generate_description()
-
-	def _run(
-		self,
-		search_query: str,
-		**kwargs: Any,
-	) -> Any:
-		youtube_channel_handle = kwargs.get('youtube_channel_handle', self.youtube_channel_handle)
-		if not youtube_channel_handle.startswith("@"):
-			youtube_channel_handle = f"@{youtube_channel_handle}"
-		self.app = App()
-		self.app.add(youtube_channel_handle, data_type=DataType.YOUTUBE_CHANNEL)
-		return super()._run(query=search_query)
+    name: str = "Search a Youtube Channels content"
+    description: str = "A tool that can be used to semantic search a query from a Youtube Channels content."
+    args_schema: Type[BaseModel] = YoutubeChannelSearchToolSchema
+
+    def __init__(self, youtube_channel_handle: Optional[str] = None, **kwargs):
+        super().__init__(**kwargs)
+        if youtube_channel_handle is not None:
+            self.add(youtube_channel_handle)
+            self.description = f"A tool that can be used to semantic search a query the {youtube_channel_handle} Youtube Channels content."
+            self.args_schema = FixedYoutubeChannelSearchToolSchema
+
+    def add(
+        self,
+        youtube_channel_handle: str,
+        **kwargs: Any,
+    ) -> None:
+        if not youtube_channel_handle.startswith("@"):
+            youtube_channel_handle = f"@{youtube_channel_handle}"
+
+        kwargs["data_type"] = DataType.YOUTUBE_CHANNEL
+        super().add(youtube_channel_handle, **kwargs)
+
+    def _before_run(
+        self,
+        query: str,
+        **kwargs: Any,
+    ) -> Any:
+        if "youtube_channel_handle" in kwargs:
+            self.add(kwargs["youtube_channel_handle"])
```

### Comparing `crewai_tools-0.1.1/pyproject.toml` & `crewai_tools-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crewai-tools"
-version = "0.1.1"
+version = "0.1.2"
 description = "Set of tools for the crewAI framework"
 authors = ["João Moura <joaomdmoura@mgail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.13"
 pydantic = "^2.6.1"
```

### Comparing `crewai_tools-0.1.1/PKG-INFO` & `crewai_tools-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crewai-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Set of tools for the crewAI framework
 Author: João Moura
 Author-email: joaomdmoura@mgail.com
 Requires-Python: >=3.10,<=3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

