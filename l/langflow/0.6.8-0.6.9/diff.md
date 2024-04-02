# Comparing `tmp/langflow-0.6.8.tar.gz` & `tmp/langflow-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-0.6.8.tar", max compression
+gzip compressed data, was "langflow-0.6.9.tar", max compression
```

## Comparing `langflow-0.6.8.tar` & `langflow-0.6.9.tar`

### file list

```diff
@@ -1,339 +1,339 @@
--rw-r--r--   0        0        0     1065 2024-02-28 16:19:17.911800 langflow-0.6.8/LICENSE
--rw-r--r--   0        0        0     9292 2024-02-28 16:19:17.911800 langflow-0.6.8/README.md
--rw-r--r--   0        0        0     4312 2024-02-28 16:19:18.331802 langflow-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      542 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/__init__.py
--rw-r--r--   0        0        0    11899 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/__main__.py
--rw-r--r--   0        0        0       38 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/README
--rw-r--r--   0        0        0     2225 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/env.py
--rw-r--r--   0        0        0      651 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/script.py.mako
--rw-r--r--   0        0        0     1618 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/006b3990db50_add_unique_constraints.py
--rw-r--r--   0        0        0     2551 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/0b8757876a7c_.py
--rw-r--r--   0        0        0     1174 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/1ef9c4f3765d_.py
--rw-r--r--   0        0        0     7482 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/260dbcc8b680_adds_tables.py
--rw-r--r--   0        0        0     1467 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/2ac71eb9c3ae_adds_credential_table.py
--rw-r--r--   0        0        0     1580 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/67cc006d50bf_add_profile_image_column.py
--rw-r--r--   0        0        0     1475 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/7843803a87b5_store_updates.py
--rw-r--r--   0        0        0     3416 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/7d2162acc8b2_adds_updated_at_and_folder_cols.py
--rw-r--r--   0        0        0     2273 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/b2fa308044b5_add_unique_constraints.py
--rw-r--r--   0        0        0     1837 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/bc2f01c40e4a_new_fixes.py
--rw-r--r--   0        0        0     3101 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/eb5866d51fd2_change_columns_to_be_nullable.py
--rw-r--r--   0        0        0     1208 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/f5ee9749d1a6_user_id_can_be_null_in_flow.py
--rw-r--r--   0        0        0     1116 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic/versions/fd531f8868b1_fix_credential_table.py
--rw-r--r--   0        0        0     3503 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/alembic.ini
--rw-r--r--   0        0        0       61 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/__init__.py
--rw-r--r--   0        0        0      644 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/router.py
--rw-r--r--   0        0        0     7064 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/utils.py
--rw-r--r--   0        0        0      749 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/__init__.py
--rw-r--r--   0        0        0     3031 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/api_key.py
--rw-r--r--   0        0        0     4904 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/base.py
--rw-r--r--   0        0        0     5089 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/callback.py
--rw-r--r--   0        0        0    10000 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/chat.py
--rw-r--r--   0        0        0     3422 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/credential.py
--rw-r--r--   0        0        0    14797 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/endpoints.py
--rw-r--r--   0        0        0     5206 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/flows.py
--rw-r--r--   0        0        0     4071 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/login.py
--rw-r--r--   0        0        0     4332 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/schemas.py
--rw-r--r--   0        0        0     7032 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/store.py
--rw-r--r--   0        0        0     4834 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/users.py
--rw-r--r--   0        0        0     4900 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/api/v1/validate.py
--rw-r--r--   0        0        0      103 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/__init__.py
--rw-r--r--   0        0        0     1825 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/agents/AgentInitializer.py
--rw-r--r--   0        0        0      891 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/agents/CSVAgent.py
--rw-r--r--   0        0        0      701 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/agents/JsonAgent.py
--rw-r--r--   0        0        0     3468 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/agents/OpenAIConversationalAgent.py
--rw-r--r--   0        0        0     1061 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/agents/SQLAgent.py
--rw-r--r--   0        0        0      833 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/agents/VectorStoreAgent.py
--rw-r--r--   0        0        0      839 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/agents/VectorStoreRouterAgent.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/agents/__init__.py
--rw-r--r--   0        0        0     1027 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/chains/ConversationChain.py
--rw-r--r--   0        0        0      848 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/chains/LLMChain.py
--rw-r--r--   0        0        0      624 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/chains/LLMCheckerChain.py
--rw-r--r--   0        0        0     1161 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/chains/LLMMathChain.py
--rw-r--r--   0        0        0      981 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/chains/PromptRunner.py
--rw-r--r--   0        0        0     1559 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/chains/RetrievalQA.py
--rw-r--r--   0        0        0     1555 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/chains/RetrievalQAWithSourcesChain.py
--rw-r--r--   0        0        0      834 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/chains/SQLDatabaseChain.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/chains/__init__.py
--rw-r--r--   0        0        0      331 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/custom_components/CustomComponent.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/custom_components/__init__.py
--rw-r--r--   0        0        0     1658 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/documentloaders/DirectoryLoader.py
--rw-r--r--   0        0        0     3958 2024-02-28 16:19:18.335802 langflow-0.6.8/src/backend/langflow/components/documentloaders/FileLoader.py
--rw-r--r--   0        0        0     1574 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/documentloaders/UrlLoader.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/documentloaders/__init__.py
--rw-r--r--   0        0        0     1671 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/embeddings/AmazonBedrockEmbeddings.py
--rw-r--r--   0        0        0     2056 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/embeddings/AzureOpenAIEmbeddings.py
--rw-r--r--   0        0        0     1313 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/embeddings/CohereEmbeddings.py
--rw-r--r--   0        0        0     1490 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/embeddings/HuggingFaceEmbeddings.py
--rw-r--r--   0        0        0     1802 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/embeddings/HuggingFaceInferenceAPIEmbeddings.py
--rw-r--r--   0        0        0     1256 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/embeddings/OllamaEmbeddings.py
--rw-r--r--   0        0        0     5268 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/embeddings/OpenAIEmbeddings.py
--rw-r--r--   0        0        0     2608 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/embeddings/VertexAIEmbeddings.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/embeddings/__init__.py
--rw-r--r--   0        0        0     2209 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/AmazonBedrock.py
--rw-r--r--   0        0        0     1433 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/Anthropic.py
--rw-r--r--   0        0        0     2571 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/AnthropicLLM.py
--rw-r--r--   0        0        0     3164 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/AzureChatOpenAI.py
--rw-r--r--   0        0        0     3597 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/BaiduQianfanChatEndpoints.py
--rw-r--r--   0        0        0     3497 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/BaiduQianfanLLMEndpoints.py
--rw-r--r--   0        0        0     1455 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/CTransformers.py
--rw-r--r--   0        0        0     1618 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/ChatAnthropic.py
--rw-r--r--   0        0        0     4625 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/ChatLiteLLM.py
--rw-r--r--   0        0        0     9925 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/ChatOllamaEndpoint.py
--rw-r--r--   0        0        0     2911 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/ChatOpenAI.py
--rw-r--r--   0        0        0     2658 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/ChatVertexAI.py
--rw-r--r--   0        0        0     1020 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/Cohere.py
--rw-r--r--   0        0        0     2890 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/GoogleGenerativeAI.py
--rw-r--r--   0        0        0     1552 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/HuggingFaceEndpoints.py
--rw-r--r--   0        0        0     5575 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/LlamaCpp.py
--rw-r--r--   0        0        0     5739 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/OllamaLLM.py
--rw-r--r--   0        0        0     4762 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/VertexAI.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/llms/__init__.py
--rw-r--r--   0        0        0     1748 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/retrievers/AmazonKendra.py
--rw-r--r--   0        0        0     1081 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/retrievers/MetalRetriever.py
--rw-r--r--   0        0        0     2239 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/retrievers/MultiQueryRetriever.py
--rw-r--r--   0        0        0     2475 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/retrievers/VectaraSelfQueryRetriver.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/retrievers/__init__.py
--rw-r--r--   0        0        0     1090 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/textsplitters/CharacterTextSplitter.py
--rw-r--r--   0        0        0     2883 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/textsplitters/LanguageRecursiveTextSplitter.py
--rw-r--r--   0        0        0     2968 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/textsplitters/RecursiveCharacterTextSplitter.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/textsplitters/__init__.py
--rw-r--r--   0        0        0      519 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/toolkits/JsonToolkit.py
--rw-r--r--   0        0        0     1800 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/toolkits/Metaphor.py
--rw-r--r--   0        0        0      809 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/toolkits/OpenAPIToolkit.py
--rw-r--r--   0        0        0      836 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/toolkits/VectorStoreInfo.py
--rw-r--r--   0        0        0      911 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/toolkits/VectorStoreRouterToolkit.py
--rw-r--r--   0        0        0      889 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/toolkits/VectorStoreToolkit.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/toolkits/__init__.py
--rw-r--r--   0        0        0     1559 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/tools/SearchApi.py
--rw-r--r--   0        0        0     1245 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/BingSearchAPIWrapper.py
--rw-r--r--   0        0        0     2561 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/GetRequest.py
--rw-r--r--   0        0        0      778 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/GoogleSearchAPIWrapper.py
--rw-r--r--   0        0        0     1661 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/GoogleSerperAPIWrapper.py
--rw-r--r--   0        0        0     1580 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/JSONDocumentBuilder.py
--rw-r--r--   0        0        0     2602 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/PostRequest.py
--rw-r--r--   0        0        0     1128 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/SearxSearchWrapper.py
--rw-r--r--   0        0        0     1004 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/SerpAPIWrapper.py
--rw-r--r--   0        0        0     3118 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/UpdateRequest.py
--rw-r--r--   0        0        0     1002 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/WikipediaAPIWrapper.py
--rw-r--r--   0        0        0      700 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/utilities/WolframAlphaAPIWrapper.py
--rw-r--r--   0        0        0     4701 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/Chroma.py
--rw-r--r--   0        0        0      918 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/FAISS.py
--rw-r--r--   0        0        0     1623 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/MongoDBAtlasVectorSearch.py
--rw-r--r--   0        0        0     2527 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/Pinecone.py
--rw-r--r--   0        0        0     4170 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/Qdrant.py
--rw-r--r--   0        0        0     2866 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/Redis.py
--rw-r--r--   0        0        0     1726 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/SupabaseVectorStore.py
--rw-r--r--   0        0        0     2671 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/Vectara.py
--rw-r--r--   0        0        0     3092 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/Weaviate.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/__init__.py
--rw-r--r--   0        0        0     2648 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/components/vectorstores/pgvector.py
--rw-r--r--   0        0        0    13860 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/config.yaml
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/core/__init__.py
--rw-r--r--   0        0        0      351 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/core/celery_app.py
--rw-r--r--   0        0        0      778 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/core/celeryconfig.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/custom/__init__.py
--rw-r--r--   0        0        0     1661 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/custom/customs.py
--rw-r--r--   0        0        0     1441 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/field_typing/__init__.py
--rw-r--r--   0        0        0     1718 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/field_typing/constants.py
--rw-r--r--   0        0        0      568 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/field_typing/range_spec.py
--rw-r--r--   0        0        0   220602 2024-02-28 16:20:24.524063 langflow-0.6.8/src/backend/langflow/frontend/assets/index-c6d7fba2.css
--rw-r--r--   0        0        0  5558933 2024-02-28 16:20:24.532063 langflow-0.6.8/src/backend/langflow/frontend/assets/index-fef5028f.js
--rw-r--r--   0        0        0    23161 2024-02-28 16:20:24.524063 langflow-0.6.8/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png
--rw-r--r--   0        0        0    26806 2024-02-28 16:20:24.524063 langflow-0.6.8/src/backend/langflow/frontend/assets/robot-95e1b00d.png
--rw-r--r--   0        0        0     4310 2024-02-28 16:20:24.524063 langflow-0.6.8/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
--rw-r--r--   0        0        0   104187 2024-02-28 16:20:24.524063 langflow-0.6.8/src/backend/langflow/frontend/favicon.ico
--rw-r--r--   0        0        0      724 2024-02-28 16:20:24.524063 langflow-0.6.8/src/backend/langflow/frontend/index.html
--rw-r--r--   0        0        0      764 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/edge/__init__.py
--rw-r--r--   0        0        0     4568 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/edge/base.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/graph/__init__.py
--rw-r--r--   0        0        0     9691 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/graph/base.py
--rw-r--r--   0        0        0     2725 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/graph/constants.py
--rw-r--r--   0        0        0     8470 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/graph/utils.py
--rw-r--r--   0        0        0      674 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/utils.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/vertex/__init__.py
--rw-r--r--   0        0        0    15149 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/vertex/base.py
--rw-r--r--   0        0        0        1 2024-02-28 16:19:18.339802 langflow-0.6.8/src/backend/langflow/graph/vertex/constants.py
--rw-r--r--   0        0        0    11785 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/graph/vertex/types.py
--rw-r--r--   0        0        0      125 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/graph/vertex/utils.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/__init__.py
--rw-r--r--   0        0        0       84 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/agents/__init__.py
--rw-r--r--   0        0        0     2442 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/agents/base.py
--rw-r--r--   0        0        0     9147 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/agents/custom.py
--rw-r--r--   0        0        0     1458 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/agents/prebuilt.py
--rw-r--r--   0        0        0     4646 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/base.py
--rw-r--r--   0        0        0       84 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/chains/__init__.py
--rw-r--r--   0        0        0     2997 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/chains/base.py
--rw-r--r--   0        0        0     4810 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/chains/custom.py
--rw-r--r--   0        0        0      194 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/__init__.py
--rw-r--r--   0        0        0     1579 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/base.py
--rw-r--r--   0        0        0       62 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/code_parser/__init__.py
--rw-r--r--   0        0        0    11288 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/code_parser/code_parser.py
--rw-r--r--   0        0        0     1143 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/code_parser/utils.py
--rw-r--r--   0        0        0       77 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/custom_component/__init__.py
--rw-r--r--   0        0        0     3740 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/custom_component/component.py
--rw-r--r--   0        0        0     9336 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/custom_component/custom_component.py
--rw-r--r--   0        0        0       77 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/directory_reader/__init__.py
--rw-r--r--   0        0        0    10510 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/directory_reader/directory_reader.py
--rw-r--r--   0        0        0     5476 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/directory_reader/utils.py
--rw-r--r--   0        0        0      583 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/schema.py
--rw-r--r--   0        0        0    14434 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom/utils.py
--rw-r--r--   0        0        0     2378 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/custom_lists.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/document_loaders/__init__.py
--rw-r--r--   0        0        0     1566 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/document_loaders/base.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/embeddings/__init__.py
--rw-r--r--   0        0        0     1532 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/embeddings/base.py
--rw-r--r--   0        0        0      171 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/importing/__init__.py
--rw-r--r--   0        0        0     6354 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/importing/utils.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/initialize/__init__.py
--rw-r--r--   0        0        0      363 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/initialize/llm.py
--rw-r--r--   0        0        0    20463 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/initialize/loading.py
--rw-r--r--   0        0        0     4142 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/initialize/utils.py
--rw-r--r--   0        0        0     9557 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/initialize/vector_store.py
--rw-r--r--   0        0        0      739 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/listing.py
--rw-r--r--   0        0        0       78 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/llms/__init__.py
--rw-r--r--   0        0        0     1442 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/llms/base.py
--rw-r--r--   0        0        0       88 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/memories/__init__.py
--rw-r--r--   0        0        0     2248 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/memories/base.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/output_parsers/__init__.py
--rw-r--r--   0        0        0     2434 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/output_parsers/base.py
--rw-r--r--   0        0        0       87 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/prompts/__init__.py
--rw-r--r--   0        0        0     2546 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/prompts/base.py
--rw-r--r--   0        0        0     2444 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/prompts/custom.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/retrievers/__init__.py
--rw-r--r--   0        0        0     2202 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/retrievers/base.py
--rw-r--r--   0        0        0     2359 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/run.py
--rw-r--r--   0        0        0      106 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/text_splitters/__init__.py
--rw-r--r--   0        0        0     1537 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/text_splitters/base.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/toolkits/__init__.py
--rw-r--r--   0        0        0     2604 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/toolkits/base.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/toolkits/custom.py
--rw-r--r--   0        0        0       81 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/tools/__init__.py
--rw-r--r--   0        0        0     5835 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/tools/base.py
--rw-r--r--   0        0        0      888 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/tools/constants.py
--rw-r--r--   0        0        0     1272 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/tools/custom.py
--rw-r--r--   0        0        0     4168 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/tools/util.py
--rw-r--r--   0        0        0     2550 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/types.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/utilities/__init__.py
--rw-r--r--   0        0        0     2527 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/utilities/base.py
--rw-r--r--   0        0        0     2932 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/utils.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/vector_store/__init__.py
--rw-r--r--   0        0        0     1871 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/vector_store/base.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/wrappers/__init__.py
--rw-r--r--   0        0        0     1515 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/interface/wrappers/base.py
--rw-r--r--   0        0        0     3296 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/main.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/processing/__init__.py
--rw-r--r--   0        0        0     3841 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/processing/base.py
--rw-r--r--   0        0        0     1745 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/processing/load.py
--rw-r--r--   0        0        0    11806 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/processing/process.py
--rw-r--r--   0        0        0      605 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/server.py
--rw-r--r--   0        0        0      115 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/services/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/services/auth/__init__.py
--rw-r--r--   0        0        0      327 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/services/auth/factory.py
--rw-r--r--   0        0        0      329 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/services/auth/service.py
--rw-r--r--   0        0        0    11614 2024-02-28 16:19:18.343802 langflow-0.6.8/src/backend/langflow/services/auth/utils.py
--rw-r--r--   0        0        0      170 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/base.py
--rw-r--r--   0        0        0      156 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/cache/__init__.py
--rw-r--r--   0        0        0     2148 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/cache/base.py
--rw-r--r--   0        0        0     1420 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/cache/factory.py
--rw-r--r--   0        0        0    10129 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/cache/service.py
--rw-r--r--   0        0        0     4752 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/cache/utils.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/chat/__init__.py
--rw-r--r--   0        0        0     4561 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/chat/cache.py
--rw-r--r--   0        0        0       45 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/chat/config.py
--rw-r--r--   0        0        0      340 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/chat/factory.py
--rw-r--r--   0        0        0    10565 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/chat/service.py
--rw-r--r--   0        0        0     1793 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/chat/utils.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/credentials/__init__.py
--rw-r--r--   0        0        0      470 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/credentials/factory.py
--rw-r--r--   0        0        0     1628 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/credentials/service.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/__init__.py
--rw-r--r--   0        0        0      670 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/factory.py
--rw-r--r--   0        0        0      161 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/__init__.py
--rw-r--r--   0        0        0      146 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/api_key/__init__.py
--rw-r--r--   0        0        0     2495 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/api_key/crud.py
--rw-r--r--   0        0        0     1451 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/api_key/model.py
--rw-r--r--   0        0        0      760 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/base.py
--rw-r--r--   0        0        0       88 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/component/__init__.py
--rw-r--r--   0        0        0     1046 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/component/model.py
--rw-r--r--   0        0        0      166 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/credential/__init__.py
--rw-r--r--   0        0        0     1851 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/credential/model.py
--rw-r--r--   0        0        0      202 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/credential/schema.py
--rw-r--r--   0        0        0      118 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/flow/__init__.py
--rw-r--r--   0        0        0     2230 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/flow/model.py
--rw-r--r--   0        0        0      137 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/user/__init__.py
--rw-r--r--   0        0        0     2043 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/user/crud.py
--rw-r--r--   0        0        0     2020 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/models/user/model.py
--rw-r--r--   0        0        0    10727 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/service.py
--rw-r--r--   0        0        0     2643 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/database/utils.py
--rw-r--r--   0        0        0     2240 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/deps.py
--rw-r--r--   0        0        0      292 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/factory.py
--rw-r--r--   0        0        0     4682 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/manager.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/plugins/__init__.py
--rw-r--r--   0        0        0      247 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/plugins/base.py
--rw-r--r--   0        0        0      476 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/plugins/factory.py
--rw-r--r--   0        0        0     2439 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/plugins/langfuse_plugin.py
--rw-r--r--   0        0        0     2453 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/plugins/service.py
--rw-r--r--   0        0        0      551 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/schema.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/session/__init__.py
--rw-r--r--   0        0        0      446 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/session/factory.py
--rw-r--r--   0        0        0     1760 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/session/service.py
--rw-r--r--   0        0        0      516 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/session/utils.py
--rw-r--r--   0        0        0       65 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/settings/__init__.py
--rw-r--r--   0        0        0     4051 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/settings/auth.py
--rw-r--r--   0        0        0     9270 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/settings/base.py
--rw-r--r--   0        0        0       71 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/settings/constants.py
--rw-r--r--   0        0        0      505 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/settings/factory.py
--rw-r--r--   0        0        0     1501 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/settings/service.py
--rw-r--r--   0        0        0     1381 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/settings/utils.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/store/__init__.py
--rw-r--r--   0        0        0      720 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/store/exceptions.py
--rw-r--r--   0        0        0      443 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/store/factory.py
--rw-r--r--   0        0        0     2013 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/store/schema.py
--rw-r--r--   0        0        0    22729 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/store/service.py
--rw-r--r--   0        0        0     2020 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/store/utils.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/task/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/task/backends/__init__.py
--rw-r--r--   0        0        0     2373 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/task/backends/anyio.py
--rw-r--r--   0        0        0      292 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/task/backends/base.py
--rw-r--r--   0        0        0      882 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/task/backends/celery.py
--rw-r--r--   0        0        0      340 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/task/factory.py
--rw-r--r--   0        0        0     2509 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/task/service.py
--rw-r--r--   0        0        0      613 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/task/utils.py
--rw-r--r--   0        0        0     8103 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/services/utils.py
--rw-r--r--   0        0        0     6567 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/settings.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/field/__init__.py
--rw-r--r--   0        0        0     3445 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/field/base.py
--rw-r--r--   0        0        0      423 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/__init__.py
--rw-r--r--   0        0        0     5289 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/agents.py
--rw-r--r--   0        0        0    10322 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/base.py
--rw-r--r--   0        0        0     7831 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/chains.py
--rw-r--r--   0        0        0     1745 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/constants.py
--rw-r--r--   0        0        0     1719 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/custom_components.py
--rw-r--r--   0        0        0     9188 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/documentloaders.py
--rw-r--r--   0        0        0     3702 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/embeddings.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/formatter/__init__.py
--rw-r--r--   0        0        0      297 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/formatter/base.py
--rw-r--r--   0        0        0     5719 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/formatter/field_formatters.py
--rw-r--r--   0        0        0     5274 2024-02-28 16:19:18.347802 langflow-0.6.8/src/backend/langflow/template/frontend_node/llms.py
--rw-r--r--   0        0        0     6534 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/template/frontend_node/memories.py
--rw-r--r--   0        0        0      364 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/template/frontend_node/output_parsers.py
--rw-r--r--   0        0        0     3419 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/template/frontend_node/prompts.py
--rw-r--r--   0        0        0      523 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/template/frontend_node/retrievers.py
--rw-r--r--   0        0        0     2355 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/template/frontend_node/textsplitters.py
--rw-r--r--   0        0        0     3836 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/template/frontend_node/tools.py
--rw-r--r--   0        0        0     1035 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/template/frontend_node/utilities.py
--rw-r--r--   0        0        0    11972 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/template/frontend_node/vectorstores.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/template/template/__init__.py
--rw-r--r--   0        0        0     2495 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/template/template/base.py
--rw-r--r--   0        0        0        0 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/utils/__init__.py
--rw-r--r--   0        0        0     5656 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/utils/constants.py
--rw-r--r--   0        0        0      386 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/utils/lazy_load.py
--rw-r--r--   0        0        0     1988 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/utils/logger.py
--rw-r--r--   0        0        0     3154 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/utils/payload.py
--rw-r--r--   0        0        0       23 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/utils/types.py
--rw-r--r--   0        0        0    13908 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/utils/util.py
--rw-r--r--   0        0        0    10201 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/utils/validate.py
--rw-r--r--   0        0        0     2809 2024-02-28 16:19:18.351802 langflow-0.6.8/src/backend/langflow/worker.py
--rw-r--r--   0        0        0    13644 1970-01-01 00:00:00.000000 langflow-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-02-29 18:31:25.737872 langflow-0.6.9/LICENSE
+-rw-r--r--   0        0        0     9292 2024-02-29 18:31:25.737872 langflow-0.6.9/README.md
+-rw-r--r--   0        0        0     4312 2024-02-29 18:31:26.157870 langflow-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      542 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/__init__.py
+-rw-r--r--   0        0        0    11932 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/__main__.py
+-rw-r--r--   0        0        0       38 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/README
+-rw-r--r--   0        0        0     2562 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/env.py
+-rw-r--r--   0        0        0      872 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/script.py.mako
+-rw-r--r--   0        0        0     2912 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/006b3990db50_add_unique_constraints.py
+-rw-r--r--   0        0        0      648 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/0b8757876a7c_.py
+-rw-r--r--   0        0        0     1141 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/1ef9c4f3765d_.py
+-rw-r--r--   0        0        0     7667 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/260dbcc8b680_adds_tables.py
+-rw-r--r--   0        0        0     1812 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/2ac71eb9c3ae_adds_credential_table.py
+-rw-r--r--   0        0        0     1809 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/67cc006d50bf_add_profile_image_column.py
+-rw-r--r--   0        0        0     1897 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/7843803a87b5_store_updates.py
+-rw-r--r--   0        0        0     2318 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/7d2162acc8b2_adds_updated_at_and_folder_cols.py
+-rw-r--r--   0        0        0     4555 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/b2fa308044b5_add_unique_constraints.py
+-rw-r--r--   0        0        0     2825 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/bc2f01c40e4a_new_fixes.py
+-rw-r--r--   0        0        0      718 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/eb5866d51fd2_change_columns_to_be_nullable.py
+-rw-r--r--   0        0        0     1209 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/f5ee9749d1a6_user_id_can_be_null_in_flow.py
+-rw-r--r--   0        0        0     2056 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic/versions/fd531f8868b1_fix_credential_table.py
+-rw-r--r--   0        0        0     3497 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/alembic.ini
+-rw-r--r--   0        0        0       61 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/__init__.py
+-rw-r--r--   0        0        0      644 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/router.py
+-rw-r--r--   0        0        0     7064 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/utils.py
+-rw-r--r--   0        0        0      749 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/__init__.py
+-rw-r--r--   0        0        0     3031 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/api_key.py
+-rw-r--r--   0        0        0     4904 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/base.py
+-rw-r--r--   0        0        0     5089 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/callback.py
+-rw-r--r--   0        0        0    10043 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/chat.py
+-rw-r--r--   0        0        0     3422 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/credential.py
+-rw-r--r--   0        0        0    14797 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/endpoints.py
+-rw-r--r--   0        0        0     5206 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/flows.py
+-rw-r--r--   0        0        0     4071 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/login.py
+-rw-r--r--   0        0        0     4332 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/schemas.py
+-rw-r--r--   0        0        0     7032 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/store.py
+-rw-r--r--   0        0        0     4834 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/users.py
+-rw-r--r--   0        0        0     4900 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/api/v1/validate.py
+-rw-r--r--   0        0        0      103 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/__init__.py
+-rw-r--r--   0        0        0     1825 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/agents/AgentInitializer.py
+-rw-r--r--   0        0        0      891 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/agents/CSVAgent.py
+-rw-r--r--   0        0        0      701 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/agents/JsonAgent.py
+-rw-r--r--   0        0        0     3468 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/agents/OpenAIConversationalAgent.py
+-rw-r--r--   0        0        0     1061 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/agents/SQLAgent.py
+-rw-r--r--   0        0        0      833 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/agents/VectorStoreAgent.py
+-rw-r--r--   0        0        0      839 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/agents/VectorStoreRouterAgent.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/agents/__init__.py
+-rw-r--r--   0        0        0     1027 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/chains/ConversationChain.py
+-rw-r--r--   0        0        0      848 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/chains/LLMChain.py
+-rw-r--r--   0        0        0      624 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/chains/LLMCheckerChain.py
+-rw-r--r--   0        0        0     1161 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/chains/LLMMathChain.py
+-rw-r--r--   0        0        0      981 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/chains/PromptRunner.py
+-rw-r--r--   0        0        0     1559 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/chains/RetrievalQA.py
+-rw-r--r--   0        0        0     1555 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/chains/RetrievalQAWithSourcesChain.py
+-rw-r--r--   0        0        0      834 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/chains/SQLDatabaseChain.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/chains/__init__.py
+-rw-r--r--   0        0        0      331 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/custom_components/CustomComponent.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/custom_components/__init__.py
+-rw-r--r--   0        0        0     1658 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/documentloaders/DirectoryLoader.py
+-rw-r--r--   0        0        0     3958 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/documentloaders/FileLoader.py
+-rw-r--r--   0        0        0     1574 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/documentloaders/UrlLoader.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.161871 langflow-0.6.9/src/backend/langflow/components/documentloaders/__init__.py
+-rw-r--r--   0        0        0     1671 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/embeddings/AmazonBedrockEmbeddings.py
+-rw-r--r--   0        0        0     2056 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/embeddings/AzureOpenAIEmbeddings.py
+-rw-r--r--   0        0        0     1313 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/embeddings/CohereEmbeddings.py
+-rw-r--r--   0        0        0     1490 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/embeddings/HuggingFaceEmbeddings.py
+-rw-r--r--   0        0        0     1802 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/embeddings/HuggingFaceInferenceAPIEmbeddings.py
+-rw-r--r--   0        0        0     1256 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/embeddings/OllamaEmbeddings.py
+-rw-r--r--   0        0        0     5268 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/embeddings/OpenAIEmbeddings.py
+-rw-r--r--   0        0        0     2608 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/embeddings/VertexAIEmbeddings.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/embeddings/__init__.py
+-rw-r--r--   0        0        0     2209 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/AmazonBedrock.py
+-rw-r--r--   0        0        0     1433 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/Anthropic.py
+-rw-r--r--   0        0        0     2571 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/AnthropicLLM.py
+-rw-r--r--   0        0        0     3164 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/AzureChatOpenAI.py
+-rw-r--r--   0        0        0     3597 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/BaiduQianfanChatEndpoints.py
+-rw-r--r--   0        0        0     3497 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/BaiduQianfanLLMEndpoints.py
+-rw-r--r--   0        0        0     1455 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/CTransformers.py
+-rw-r--r--   0        0        0     1618 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/ChatAnthropic.py
+-rw-r--r--   0        0        0     4625 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/ChatLiteLLM.py
+-rw-r--r--   0        0        0     9925 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/ChatOllamaEndpoint.py
+-rw-r--r--   0        0        0     2911 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/ChatOpenAI.py
+-rw-r--r--   0        0        0     2658 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/ChatVertexAI.py
+-rw-r--r--   0        0        0     1020 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/Cohere.py
+-rw-r--r--   0        0        0     2890 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/GoogleGenerativeAI.py
+-rw-r--r--   0        0        0     1552 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/HuggingFaceEndpoints.py
+-rw-r--r--   0        0        0     5575 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/LlamaCpp.py
+-rw-r--r--   0        0        0     5739 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/OllamaLLM.py
+-rw-r--r--   0        0        0     4762 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/VertexAI.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/llms/__init__.py
+-rw-r--r--   0        0        0     1748 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/retrievers/AmazonKendra.py
+-rw-r--r--   0        0        0     1081 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/retrievers/MetalRetriever.py
+-rw-r--r--   0        0        0     2239 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/retrievers/MultiQueryRetriever.py
+-rw-r--r--   0        0        0     2475 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/retrievers/VectaraSelfQueryRetriver.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/retrievers/__init__.py
+-rw-r--r--   0        0        0     1090 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/textsplitters/CharacterTextSplitter.py
+-rw-r--r--   0        0        0     2883 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/textsplitters/LanguageRecursiveTextSplitter.py
+-rw-r--r--   0        0        0     2968 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/textsplitters/RecursiveCharacterTextSplitter.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/textsplitters/__init__.py
+-rw-r--r--   0        0        0      519 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/toolkits/JsonToolkit.py
+-rw-r--r--   0        0        0     1800 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/toolkits/Metaphor.py
+-rw-r--r--   0        0        0      809 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/toolkits/OpenAPIToolkit.py
+-rw-r--r--   0        0        0      836 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/toolkits/VectorStoreInfo.py
+-rw-r--r--   0        0        0      911 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/toolkits/VectorStoreRouterToolkit.py
+-rw-r--r--   0        0        0      889 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/toolkits/VectorStoreToolkit.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/toolkits/__init__.py
+-rw-r--r--   0        0        0     1559 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/tools/SearchApi.py
+-rw-r--r--   0        0        0     1245 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/BingSearchAPIWrapper.py
+-rw-r--r--   0        0        0     2561 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/GetRequest.py
+-rw-r--r--   0        0        0      778 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/GoogleSearchAPIWrapper.py
+-rw-r--r--   0        0        0     1661 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/GoogleSerperAPIWrapper.py
+-rw-r--r--   0        0        0     1580 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/JSONDocumentBuilder.py
+-rw-r--r--   0        0        0     2602 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/PostRequest.py
+-rw-r--r--   0        0        0     1128 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/SearxSearchWrapper.py
+-rw-r--r--   0        0        0     1004 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/SerpAPIWrapper.py
+-rw-r--r--   0        0        0     3118 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/UpdateRequest.py
+-rw-r--r--   0        0        0     1002 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/WikipediaAPIWrapper.py
+-rw-r--r--   0        0        0      700 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/utilities/WolframAlphaAPIWrapper.py
+-rw-r--r--   0        0        0     4701 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/Chroma.py
+-rw-r--r--   0        0        0      918 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/FAISS.py
+-rw-r--r--   0        0        0     1623 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/MongoDBAtlasVectorSearch.py
+-rw-r--r--   0        0        0     2527 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/Pinecone.py
+-rw-r--r--   0        0        0     4170 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/Qdrant.py
+-rw-r--r--   0        0        0     2866 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/Redis.py
+-rw-r--r--   0        0        0     1726 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/SupabaseVectorStore.py
+-rw-r--r--   0        0        0     2671 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/Vectara.py
+-rw-r--r--   0        0        0     3092 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/Weaviate.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/__init__.py
+-rw-r--r--   0        0        0     2648 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/components/vectorstores/pgvector.py
+-rw-r--r--   0        0        0    13860 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/config.yaml
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/core/__init__.py
+-rw-r--r--   0        0        0      351 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/core/celery_app.py
+-rw-r--r--   0        0        0      778 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/core/celeryconfig.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/custom/__init__.py
+-rw-r--r--   0        0        0     1661 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/custom/customs.py
+-rw-r--r--   0        0        0     1441 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/field_typing/__init__.py
+-rw-r--r--   0        0        0     1718 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/field_typing/constants.py
+-rw-r--r--   0        0        0      568 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/field_typing/range_spec.py
+-rw-r--r--   0        0        0  5559386 2024-02-29 18:32:25.873721 langflow-0.6.9/src/backend/langflow/frontend/assets/index-3732b41f.js
+-rw-r--r--   0        0        0   220191 2024-02-29 18:32:25.873721 langflow-0.6.9/src/backend/langflow/frontend/assets/index-e7ca4585.css
+-rw-r--r--   0        0        0    23161 2024-02-29 18:32:25.865722 langflow-0.6.9/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png
+-rw-r--r--   0        0        0    26806 2024-02-29 18:32:25.873721 langflow-0.6.9/src/backend/langflow/frontend/assets/robot-95e1b00d.png
+-rw-r--r--   0        0        0     4310 2024-02-29 18:32:25.873721 langflow-0.6.9/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
+-rw-r--r--   0        0        0   104187 2024-02-29 18:32:25.865722 langflow-0.6.9/src/backend/langflow/frontend/favicon.ico
+-rw-r--r--   0        0        0      724 2024-02-29 18:32:25.865722 langflow-0.6.9/src/backend/langflow/frontend/index.html
+-rw-r--r--   0        0        0      764 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/edge/__init__.py
+-rw-r--r--   0        0        0     4568 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/edge/base.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/graph/__init__.py
+-rw-r--r--   0        0        0     9691 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/graph/base.py
+-rw-r--r--   0        0        0     2725 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/graph/constants.py
+-rw-r--r--   0        0        0     8470 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/graph/utils.py
+-rw-r--r--   0        0        0      674 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/vertex/__init__.py
+-rw-r--r--   0        0        0    15149 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/vertex/base.py
+-rw-r--r--   0        0        0        1 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/vertex/constants.py
+-rw-r--r--   0        0        0    11785 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/vertex/types.py
+-rw-r--r--   0        0        0      125 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/graph/vertex/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.165871 langflow-0.6.9/src/backend/langflow/interface/__init__.py
+-rw-r--r--   0        0        0       84 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/agents/__init__.py
+-rw-r--r--   0        0        0     2442 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/agents/base.py
+-rw-r--r--   0        0        0     9147 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/agents/custom.py
+-rw-r--r--   0        0        0     1458 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/agents/prebuilt.py
+-rw-r--r--   0        0        0     4646 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/base.py
+-rw-r--r--   0        0        0       84 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/chains/__init__.py
+-rw-r--r--   0        0        0     2997 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/chains/base.py
+-rw-r--r--   0        0        0     4810 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/chains/custom.py
+-rw-r--r--   0        0        0      194 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/__init__.py
+-rw-r--r--   0        0        0     1579 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/base.py
+-rw-r--r--   0        0        0       62 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/code_parser/__init__.py
+-rw-r--r--   0        0        0    11288 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/code_parser/code_parser.py
+-rw-r--r--   0        0        0     1143 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/code_parser/utils.py
+-rw-r--r--   0        0        0       77 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/custom_component/__init__.py
+-rw-r--r--   0        0        0     3740 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/custom_component/component.py
+-rw-r--r--   0        0        0     9336 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/custom_component/custom_component.py
+-rw-r--r--   0        0        0       77 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/directory_reader/__init__.py
+-rw-r--r--   0        0        0    10510 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/directory_reader/directory_reader.py
+-rw-r--r--   0        0        0     5476 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/directory_reader/utils.py
+-rw-r--r--   0        0        0      583 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/schema.py
+-rw-r--r--   0        0        0    14434 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom/utils.py
+-rw-r--r--   0        0        0     2378 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/custom_lists.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/document_loaders/__init__.py
+-rw-r--r--   0        0        0     1566 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/document_loaders/base.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/embeddings/__init__.py
+-rw-r--r--   0        0        0     1532 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/embeddings/base.py
+-rw-r--r--   0        0        0      171 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/importing/__init__.py
+-rw-r--r--   0        0        0     6354 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/importing/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/initialize/__init__.py
+-rw-r--r--   0        0        0      363 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/initialize/llm.py
+-rw-r--r--   0        0        0    20463 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/initialize/loading.py
+-rw-r--r--   0        0        0     4142 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/initialize/utils.py
+-rw-r--r--   0        0        0     9557 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/initialize/vector_store.py
+-rw-r--r--   0        0        0      739 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/listing.py
+-rw-r--r--   0        0        0       78 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/llms/__init__.py
+-rw-r--r--   0        0        0     1442 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/llms/base.py
+-rw-r--r--   0        0        0       88 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/memories/__init__.py
+-rw-r--r--   0        0        0     2248 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/memories/base.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/output_parsers/__init__.py
+-rw-r--r--   0        0        0     2434 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/output_parsers/base.py
+-rw-r--r--   0        0        0       87 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/prompts/__init__.py
+-rw-r--r--   0        0        0     2546 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/prompts/base.py
+-rw-r--r--   0        0        0     2444 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/prompts/custom.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/retrievers/__init__.py
+-rw-r--r--   0        0        0     2202 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/retrievers/base.py
+-rw-r--r--   0        0        0     2359 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/run.py
+-rw-r--r--   0        0        0      106 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/text_splitters/__init__.py
+-rw-r--r--   0        0        0     1537 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/text_splitters/base.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/toolkits/__init__.py
+-rw-r--r--   0        0        0     2604 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/toolkits/base.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/toolkits/custom.py
+-rw-r--r--   0        0        0       81 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/tools/__init__.py
+-rw-r--r--   0        0        0     5835 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/tools/base.py
+-rw-r--r--   0        0        0      888 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/tools/constants.py
+-rw-r--r--   0        0        0     1272 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/tools/custom.py
+-rw-r--r--   0        0        0     4168 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/tools/util.py
+-rw-r--r--   0        0        0     2550 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/types.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/utilities/__init__.py
+-rw-r--r--   0        0        0     2527 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/utilities/base.py
+-rw-r--r--   0        0        0     2932 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/vector_store/__init__.py
+-rw-r--r--   0        0        0     1871 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/vector_store/base.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/wrappers/__init__.py
+-rw-r--r--   0        0        0     1515 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/interface/wrappers/base.py
+-rw-r--r--   0        0        0     3296 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/main.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/processing/__init__.py
+-rw-r--r--   0        0        0     3841 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/processing/base.py
+-rw-r--r--   0        0        0     1745 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/processing/load.py
+-rw-r--r--   0        0        0    11806 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/processing/process.py
+-rw-r--r--   0        0        0      605 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/server.py
+-rw-r--r--   0        0        0      115 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/services/auth/__init__.py
+-rw-r--r--   0        0        0      327 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/services/auth/factory.py
+-rw-r--r--   0        0        0      329 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/services/auth/service.py
+-rw-r--r--   0        0        0    11614 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/services/auth/utils.py
+-rw-r--r--   0        0        0      170 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/services/base.py
+-rw-r--r--   0        0        0      156 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/services/cache/__init__.py
+-rw-r--r--   0        0        0     2148 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/services/cache/base.py
+-rw-r--r--   0        0        0     1420 2024-02-29 18:31:26.169870 langflow-0.6.9/src/backend/langflow/services/cache/factory.py
+-rw-r--r--   0        0        0    10129 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/cache/service.py
+-rw-r--r--   0        0        0     4752 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/cache/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/chat/__init__.py
+-rw-r--r--   0        0        0     4561 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/chat/cache.py
+-rw-r--r--   0        0        0       45 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/chat/config.py
+-rw-r--r--   0        0        0      340 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/chat/factory.py
+-rw-r--r--   0        0        0    10565 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/chat/service.py
+-rw-r--r--   0        0        0     1793 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/chat/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/credentials/__init__.py
+-rw-r--r--   0        0        0      470 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/credentials/factory.py
+-rw-r--r--   0        0        0     1628 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/credentials/service.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/__init__.py
+-rw-r--r--   0        0        0      670 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/factory.py
+-rw-r--r--   0        0        0      161 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/__init__.py
+-rw-r--r--   0        0        0      146 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/api_key/__init__.py
+-rw-r--r--   0        0        0     2495 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/api_key/crud.py
+-rw-r--r--   0        0        0     1451 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/api_key/model.py
+-rw-r--r--   0        0        0      760 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/base.py
+-rw-r--r--   0        0        0       88 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/component/__init__.py
+-rw-r--r--   0        0        0     1046 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/component/model.py
+-rw-r--r--   0        0        0      166 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/credential/__init__.py
+-rw-r--r--   0        0        0     1851 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/credential/model.py
+-rw-r--r--   0        0        0      202 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/credential/schema.py
+-rw-r--r--   0        0        0      118 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/flow/__init__.py
+-rw-r--r--   0        0        0     2230 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/flow/model.py
+-rw-r--r--   0        0        0      137 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/user/__init__.py
+-rw-r--r--   0        0        0     2043 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/user/crud.py
+-rw-r--r--   0        0        0     2020 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/models/user/model.py
+-rw-r--r--   0        0        0    10785 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/service.py
+-rw-r--r--   0        0        0     2643 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/database/utils.py
+-rw-r--r--   0        0        0     2240 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/deps.py
+-rw-r--r--   0        0        0      292 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/factory.py
+-rw-r--r--   0        0        0     4682 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/manager.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/plugins/__init__.py
+-rw-r--r--   0        0        0      247 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/plugins/base.py
+-rw-r--r--   0        0        0      476 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/plugins/factory.py
+-rw-r--r--   0        0        0     2439 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/plugins/langfuse_plugin.py
+-rw-r--r--   0        0        0     2453 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/plugins/service.py
+-rw-r--r--   0        0        0      551 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/schema.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/session/__init__.py
+-rw-r--r--   0        0        0      446 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/session/factory.py
+-rw-r--r--   0        0        0     1760 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/session/service.py
+-rw-r--r--   0        0        0      516 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/session/utils.py
+-rw-r--r--   0        0        0       65 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/settings/__init__.py
+-rw-r--r--   0        0        0     4051 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/settings/auth.py
+-rw-r--r--   0        0        0     9270 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/settings/base.py
+-rw-r--r--   0        0        0       71 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/settings/constants.py
+-rw-r--r--   0        0        0      505 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/settings/factory.py
+-rw-r--r--   0        0        0     1501 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/settings/service.py
+-rw-r--r--   0        0        0     1381 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/settings/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/store/__init__.py
+-rw-r--r--   0        0        0      720 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/store/exceptions.py
+-rw-r--r--   0        0        0      443 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/store/factory.py
+-rw-r--r--   0        0        0     2013 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/store/schema.py
+-rw-r--r--   0        0        0    22729 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/store/service.py
+-rw-r--r--   0        0        0     2020 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/store/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/task/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/task/backends/__init__.py
+-rw-r--r--   0        0        0     2373 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/task/backends/anyio.py
+-rw-r--r--   0        0        0      292 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/task/backends/base.py
+-rw-r--r--   0        0        0      882 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/task/backends/celery.py
+-rw-r--r--   0        0        0      340 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/task/factory.py
+-rw-r--r--   0        0        0     2509 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/task/service.py
+-rw-r--r--   0        0        0      613 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/task/utils.py
+-rw-r--r--   0        0        0     8182 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/services/utils.py
+-rw-r--r--   0        0        0     6567 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/settings.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/field/__init__.py
+-rw-r--r--   0        0        0     3445 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/field/base.py
+-rw-r--r--   0        0        0      423 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/__init__.py
+-rw-r--r--   0        0        0     5289 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/agents.py
+-rw-r--r--   0        0        0    10322 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/base.py
+-rw-r--r--   0        0        0     7831 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/chains.py
+-rw-r--r--   0        0        0     1745 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/constants.py
+-rw-r--r--   0        0        0     1719 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/custom_components.py
+-rw-r--r--   0        0        0     9188 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/documentloaders.py
+-rw-r--r--   0        0        0     3702 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/embeddings.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/formatter/__init__.py
+-rw-r--r--   0        0        0      297 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/formatter/base.py
+-rw-r--r--   0        0        0     5719 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/formatter/field_formatters.py
+-rw-r--r--   0        0        0     5274 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/llms.py
+-rw-r--r--   0        0        0     6534 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/memories.py
+-rw-r--r--   0        0        0      364 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/output_parsers.py
+-rw-r--r--   0        0        0     3419 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/prompts.py
+-rw-r--r--   0        0        0      523 2024-02-29 18:31:26.173870 langflow-0.6.9/src/backend/langflow/template/frontend_node/retrievers.py
+-rw-r--r--   0        0        0     2355 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/template/frontend_node/textsplitters.py
+-rw-r--r--   0        0        0     3836 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/template/frontend_node/tools.py
+-rw-r--r--   0        0        0     1035 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/template/frontend_node/utilities.py
+-rw-r--r--   0        0        0    11972 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/template/frontend_node/vectorstores.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/template/template/__init__.py
+-rw-r--r--   0        0        0     2495 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/template/template/base.py
+-rw-r--r--   0        0        0        0 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/utils/__init__.py
+-rw-r--r--   0        0        0     5656 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/utils/constants.py
+-rw-r--r--   0        0        0      386 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/utils/lazy_load.py
+-rw-r--r--   0        0        0     1988 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/utils/logger.py
+-rw-r--r--   0        0        0     3154 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/utils/payload.py
+-rw-r--r--   0        0        0       23 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/utils/types.py
+-rw-r--r--   0        0        0    13908 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/utils/util.py
+-rw-r--r--   0        0        0    10201 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/utils/validate.py
+-rw-r--r--   0        0        0     2809 2024-02-29 18:31:26.177870 langflow-0.6.9/src/backend/langflow/worker.py
+-rw-r--r--   0        0        0    13644 1970-01-01 00:00:00.000000 langflow-0.6.9/PKG-INFO
```

### Comparing `langflow-0.6.8/LICENSE` & `langflow-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/README.md` & `langflow-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/pyproject.toml` & `langflow-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "0.6.8"
+version = "0.6.9"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Gustavo Schaedler <gustavopoa@gmail.com>",
```

### Comparing `langflow-0.6.8/src/backend/langflow/__init__.py` & `langflow-0.6.9/src/backend/langflow/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/__main__.py` & `langflow-0.6.9/src/backend/langflow/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,19 @@
         typer.echo(f"Langflow Version: {__version__}")
         raise typer.Exit()
 
 
 @app.callback()
 def main_entry_point(
     version: bool = typer.Option(
-        None, "--version", callback=version_callback, is_eager=True, help="Show the version and exit."
+        None,
+        "--version",
+        callback=version_callback,
+        is_eager=True,
+        help="Show the version and exit.",
     ),
 ):
     """
     Main entry point for the Langflow CLI.
     """
     pass
```

### Comparing `langflow-0.6.8/src/backend/langflow/alembic/env.py` & `langflow-0.6.9/src/backend/langflow/alembic/env.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import os
 from logging.config import fileConfig
 
-from sqlalchemy import engine_from_config
-from sqlalchemy import pool
-
 from alembic import context
+from loguru import logger
+from sqlalchemy import engine_from_config, pool
 
+from langflow.services.database.models import *  # noqa
 from langflow.services.database.service import SQLModel
 
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
 config = context.config
 
 # Interpret the config file for Python logging.
@@ -36,15 +37,16 @@
     here as well.  By skipping the Engine creation
     we don't even need a DBAPI to be available.
 
     Calls to context.execute() here emit the given string to the
     script output.
 
     """
-    url = config.get_main_option("sqlalchemy.url")
+    url = os.getenv("LANGFLOW_DATABASE_URL")
+    url = url or config.get_main_option("sqlalchemy.url")
     context.configure(
         url=url,
         target_metadata=target_metadata,
         literal_binds=True,
         dialect_opts={"paramstyle": "named"},
         render_as_batch=True,
     )
@@ -56,20 +58,25 @@
 def run_migrations_online() -> None:
     """Run migrations in 'online' mode.
 
     In this scenario we need to create an Engine
     and associate a connection with the context.
 
     """
-    connectable = engine_from_config(
-        config.get_section(config.config_ini_section, {}),
-        prefix="sqlalchemy.",
-        poolclass=pool.NullPool,
-    )
+    from langflow.services.deps import get_db_service
 
+    try:
+        connectable = get_db_service().engine
+    except Exception as e:
+        logger.error(f"Error getting database engine: {e}")
+        connectable = engine_from_config(
+            config.get_section(config.config_ini_section, {}),
+            prefix="sqlalchemy.",
+            poolclass=pool.NullPool,
+        )
     with connectable.connect() as connection:
         context.configure(
             connection=connection, target_metadata=target_metadata, render_as_batch=True
         )
 
         with context.begin_transaction():
             context.run_migrations()
```

### Comparing `langflow-0.6.8/src/backend/langflow/alembic/versions/006b3990db50_add_unique_constraints.py` & `langflow-0.6.9/src/backend/langflow/alembic/versions/006b3990db50_add_unique_constraints.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,75 @@
 """Add unique constraints
 
 Revision ID: 006b3990db50
 Revises: 1ef9c4f3765d
 Create Date: 2023-12-13 18:55:52.587360
 
 """
+
 from typing import Sequence, Union
 
 from alembic import op
+from sqlalchemy.engine.reflection import Inspector
 
 # revision identifiers, used by Alembic.
-revision: str = '006b3990db50'
-down_revision: Union[str, None] = '1ef9c4f3765d'
+revision: str = "006b3990db50"
+down_revision: Union[str, None] = "1ef9c4f3765d"
 branch_labels: Union[str, Sequence[str], None] = None
 depends_on: Union[str, Sequence[str], None] = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
+    conn = op.get_bind()
+    inspector = Inspector.from_engine(conn)  # type: ignore
+    api_key_constraints = inspector.get_unique_constraints("apikey")
+    flow_constraints = inspector.get_unique_constraints("flow")
+    user_constraints = inspector.get_unique_constraints("user")
     try:
-        with op.batch_alter_table('apikey', schema=None) as batch_op:
-            batch_op.create_unique_constraint('uq_apikey_id', ['id'])
-
-        with op.batch_alter_table('flow', schema=None) as batch_op:
-            batch_op.create_unique_constraint('uq_flow_id', ['id'])
-
-        with op.batch_alter_table('user', schema=None) as batch_op:
-            batch_op.create_unique_constraint('uq_user_id', ['id'])
+        if not any(
+            constraint["name"] == "uq_apikey_id" for constraint in api_key_constraints
+        ):
+            with op.batch_alter_table("apikey", schema=None) as batch_op:
+
+                batch_op.create_unique_constraint("uq_apikey_id", ["id"])
+        if not any(
+            constraint["name"] == "uq_flow_id" for constraint in flow_constraints
+        ):
+            with op.batch_alter_table("flow", schema=None) as batch_op:
+                batch_op.create_unique_constraint("uq_flow_id", ["id"])
+        if not any(
+            constraint["name"] == "uq_user_id" for constraint in user_constraints
+        ):
+            with op.batch_alter_table("user", schema=None) as batch_op:
+                batch_op.create_unique_constraint("uq_user_id", ["id"])
     except Exception as e:
         print(e)
         pass
 
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
+    conn = op.get_bind()
+    inspector = Inspector.from_engine(conn)  # type: ignore
+    api_key_constraints = inspector.get_unique_constraints("apikey")
+    flow_constraints = inspector.get_unique_constraints("flow")
+    user_constraints = inspector.get_unique_constraints("user")
     try:
-        with op.batch_alter_table('user', schema=None) as batch_op:
-            batch_op.drop_constraint('uq_user_id', type_='unique')
-
-        with op.batch_alter_table('flow', schema=None) as batch_op:
-            batch_op.drop_constraint('uq_flow_id', type_='unique')
+        if any(
+            constraint["name"] == "uq_apikey_id" for constraint in api_key_constraints
+        ):
+            with op.batch_alter_table("user", schema=None) as batch_op:
+                batch_op.drop_constraint("uq_user_id", type_="unique")
+        if any(constraint["name"] == "uq_flow_id" for constraint in flow_constraints):
+            with op.batch_alter_table("flow", schema=None) as batch_op:
+                batch_op.drop_constraint("uq_flow_id", type_="unique")
+        if any(constraint["name"] == "uq_user_id" for constraint in user_constraints):
 
-        with op.batch_alter_table('apikey', schema=None) as batch_op:
-            batch_op.drop_constraint('uq_apikey_id', type_='unique')
+            with op.batch_alter_table("apikey", schema=None) as batch_op:
+                batch_op.drop_constraint("uq_apikey_id", type_="unique")
     except Exception as e:
         print(e)
         pass
     # ### end Alembic commands ###
```

### Comparing `langflow-0.6.8/src/backend/langflow/alembic/versions/1ef9c4f3765d_.py` & `langflow-0.6.9/src/backend/langflow/alembic/versions/1ef9c4f3765d_.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,42 +2,41 @@
 
 
 Revision ID: 1ef9c4f3765d
 Revises: fd531f8868b1
 Create Date: 2023-12-04 15:00:27.968998
 
 """
+
 from typing import Sequence, Union
 
 import sqlalchemy as sa
 import sqlmodel
 from alembic import op
 
 # revision identifiers, used by Alembic.
-revision: str = '1ef9c4f3765d'
-down_revision: Union[str, None] = 'fd531f8868b1'
+revision: str = "1ef9c4f3765d"
+down_revision: Union[str, None] = "fd531f8868b1"
 branch_labels: Union[str, Sequence[str], None] = None
 depends_on: Union[str, Sequence[str], None] = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     try:
-        with op.batch_alter_table('apikey', schema=None) as batch_op:
-            batch_op.alter_column('name',
-                existing_type=sqlmodel.sql.sqltypes.AutoString(),
-                nullable=True)
+        with op.batch_alter_table("apikey", schema=None) as batch_op:
+            batch_op.alter_column(
+                "name", existing_type=sqlmodel.sql.sqltypes.AutoString(), nullable=True
+            )
     except Exception as e:
         pass
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     try:
-        with op.batch_alter_table('apikey', schema=None) as batch_op:
-            batch_op.alter_column('name',
-                existing_type=sa.VARCHAR(),
-                nullable=False)
+        with op.batch_alter_table("apikey", schema=None) as batch_op:
+            batch_op.alter_column("name", existing_type=sa.VARCHAR(), nullable=False)
     except Exception as e:
         pass
     # ### end Alembic commands ###
```

### Comparing `langflow-0.6.8/src/backend/langflow/alembic/versions/260dbcc8b680_adds_tables.py` & `langflow-0.6.9/src/backend/langflow/alembic/versions/260dbcc8b680_adds_tables.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Adds tables
 
 Revision ID: 260dbcc8b680
 Revises:
 Create Date: 2023-08-27 19:49:02.681355
 
 """
+
 from typing import Sequence, Union
 
 import sqlalchemy as sa
 import sqlmodel
 from alembic import op
 from sqlalchemy.engine.reflection import Inspector
 
@@ -29,15 +30,17 @@
     # Drop 'flowstyle' table if it exists
     # and other related indices
     if "flowstyle" in existing_tables:
         op.drop_table("flowstyle")
         if "ix_flowstyle_flow_id" in [
             index["name"] for index in inspector.get_indexes("flowstyle")
         ]:
-            op.drop_index("ix_flowstyle_flow_id", table_name="flowstyle")
+            op.drop_index(
+                "ix_flowstyle_flow_id", table_name="flowstyle", if_exists=True
+            )
 
     existing_indices_flow = []
     existing_fks_flow = []
     if "flow" in existing_tables:
         existing_indices_flow = [
             index["name"] for index in inspector.get_indexes("flow")
         ]
@@ -76,16 +79,15 @@
             sa.Column("last_used_at", sa.DateTime(), nullable=True),
             sa.Column("total_uses", sa.Integer(), nullable=False, default=0),
             sa.Column("is_active", sa.Boolean(), nullable=False, default=True),
             sa.Column("id", sqlmodel.sql.sqltypes.GUID(), nullable=False),
             sa.Column("api_key", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
             sa.Column("user_id", sqlmodel.sql.sqltypes.GUID(), nullable=False),
             sa.ForeignKeyConstraint(
-                ["user_id"],
-                ["user.id"],
+                ["user_id"], ["user.id"], name="fk_apikey_user_id_user"
             ),
             sa.PrimaryKeyConstraint("id", name="pk_apikey"),
             sa.UniqueConstraint("id", name="uq_apikey_id"),
         )
         with op.batch_alter_table("apikey", schema=None) as batch_op:
             batch_op.create_index(
                 batch_op.f("ix_apikey_api_key"), ["api_key"], unique=True
@@ -99,16 +101,15 @@
             "flow",
             sa.Column("data", sa.JSON(), nullable=True),
             sa.Column("name", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
             sa.Column("description", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
             sa.Column("id", sqlmodel.sql.sqltypes.GUID(), nullable=False),
             sa.Column("user_id", sqlmodel.sql.sqltypes.GUID(), nullable=False),
             sa.ForeignKeyConstraint(
-                ["user_id"],
-                ["user.id"],
+                ["user_id"], ["user.id"], name="fk_flow_user_id_user"
             ),
             sa.PrimaryKeyConstraint("id", name="pk_flow"),
             sa.UniqueConstraint("id", name="uq_flow_id"),
         )
     # Conditionally create indices for 'flow' table
     # if _alembic_tmp_flow exists, then we need to drop it first
     # This is to deal with SQLite not being able to ROLLBACK
@@ -147,29 +148,29 @@
 
     conn = op.get_bind()
     inspector = Inspector.from_engine(conn)  # type: ignore
     # List existing tables
     existing_tables = inspector.get_table_names()
     if "flow" in existing_tables:
         with op.batch_alter_table("flow", schema=None) as batch_op:
-            batch_op.drop_index(batch_op.f("ix_flow_user_id"))
-            batch_op.drop_index(batch_op.f("ix_flow_name"))
-            batch_op.drop_index(batch_op.f("ix_flow_description"))
+            batch_op.drop_index(batch_op.f("ix_flow_user_id"), if_exists=True)
+            batch_op.drop_index(batch_op.f("ix_flow_name"), if_exists=True)
+            batch_op.drop_index(batch_op.f("ix_flow_description"), if_exists=True)
 
         op.drop_table("flow")
     if "apikey" in existing_tables:
         with op.batch_alter_table("apikey", schema=None) as batch_op:
-            batch_op.drop_index(batch_op.f("ix_apikey_user_id"))
-            batch_op.drop_index(batch_op.f("ix_apikey_name"))
-            batch_op.drop_index(batch_op.f("ix_apikey_api_key"))
+            batch_op.drop_index(batch_op.f("ix_apikey_user_id"), if_exists=True)
+            batch_op.drop_index(batch_op.f("ix_apikey_name"), if_exists=True)
+            batch_op.drop_index(batch_op.f("ix_apikey_api_key"), if_exists=True)
 
         op.drop_table("apikey")
     if "user" in existing_tables:
         with op.batch_alter_table("user", schema=None) as batch_op:
-            batch_op.drop_index(batch_op.f("ix_user_username"))
+            batch_op.drop_index(batch_op.f("ix_user_username"), if_exists=True)
 
         op.drop_table("user")
 
     if "flowstyle" in existing_tables:
         op.drop_table("flowstyle")
 
     if "component" in existing_tables:
```

### Comparing `langflow-0.6.8/src/backend/langflow/alembic/versions/67cc006d50bf_add_profile_image_column.py` & `langflow-0.6.9/src/backend/langflow/alembic/versions/67cc006d50bf_add_profile_image_column.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add profile-image column
 
 Revision ID: 67cc006d50bf
 Revises: 260dbcc8b680
 Create Date: 2023-09-08 07:36:13.387318
 
 """
+
 from typing import Sequence, Union
 
 import sqlalchemy as sa
 import sqlmodel
 from alembic import op
 from sqlalchemy.engine.reflection import Inspector
 
@@ -17,33 +18,40 @@
 down_revision: Union[str, None] = "260dbcc8b680"
 branch_labels: Union[str, Sequence[str], None] = None
 depends_on: Union[str, Sequence[str], None] = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
-    conn = op.get_bind()
-    inspector = Inspector.from_engine(conn) # type: ignore
-    if "user" in inspector.get_table_names() and "profile_image" not in [
-        column["name"] for column in inspector.get_columns("user")
-    ]:
-        with op.batch_alter_table("user", schema=None) as batch_op:
-            batch_op.add_column(
-                sa.Column(
-                    "profile_image", sqlmodel.sql.sqltypes.AutoString(), nullable=True
+    try:
+        conn = op.get_bind()
+        inspector = Inspector.from_engine(conn)  # type: ignore
+        if "user" in inspector.get_table_names() and "profile_image" not in [
+            column["name"] for column in inspector.get_columns("user")
+        ]:
+            with op.batch_alter_table("user", schema=None) as batch_op:
+                batch_op.add_column(
+                    sa.Column(
+                        "profile_image",
+                        sqlmodel.sql.sqltypes.AutoString(),
+                        nullable=True,
+                    )
                 )
-            )
-
+    except Exception as e:
+        print(e)
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
-    conn = op.get_bind()
-    inspector = Inspector.from_engine(conn) # type: ignore
-    if "user" in inspector.get_table_names() and "profile_image" in [
-        column["name"] for column in inspector.get_columns("user")
-    ]:
-        with op.batch_alter_table("user", schema=None) as batch_op:
-            batch_op.drop_column("profile_image")
+    try:
+        conn = op.get_bind()
+        inspector = Inspector.from_engine(conn)  # type: ignore
+        if "user" in inspector.get_table_names() and "profile_image" in [
+            column["name"] for column in inspector.get_columns("user")
+        ]:
+            with op.batch_alter_table("user", schema=None) as batch_op:
+                batch_op.drop_column("profile_image")
+    except Exception as e:
+        print(e)
 
     # ### end Alembic commands ###
```

### Comparing `langflow-0.6.8/src/backend/langflow/alembic/versions/7843803a87b5_store_updates.py` & `langflow-0.6.9/src/backend/langflow/alembic/versions/7843803a87b5_store_updates.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 """Store updates
 
 Revision ID: 7843803a87b5
 Revises: eb5866d51fd2
 Create Date: 2023-10-18 23:08:57.744906
 
 """
+
 from typing import Sequence, Union
 
 import sqlalchemy as sa
 import sqlmodel
 from alembic import op
-from loguru import logger
+from sqlalchemy.engine.reflection import Inspector
 
 # revision identifiers, used by Alembic.
 revision: str = "7843803a87b5"
 down_revision: Union[str, None] = "eb5866d51fd2"
 branch_labels: Union[str, Sequence[str], None] = None
 depends_on: Union[str, Sequence[str], None] = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
+    conn = op.get_bind()
+    inspector = Inspector.from_engine(conn)  # type: ignore
+    flow_columns = [column["name"] for column in inspector.get_columns("flow")]
+    user_columns = [column["name"] for column in inspector.get_columns("user")]
     try:
-        with op.batch_alter_table("flow", schema=None) as batch_op:
-            batch_op.add_column(sa.Column("is_component", sa.Boolean(), nullable=True))
-
-        with op.batch_alter_table("user", schema=None) as batch_op:
-            batch_op.add_column(
-                sa.Column(
-                    "store_api_key", sqlmodel.AutoString(), nullable=True
+        if "is_component" not in flow_columns:
+            with op.batch_alter_table("flow", schema=None) as batch_op:
+                batch_op.add_column(
+                    sa.Column("is_component", sa.Boolean(), nullable=True)
                 )
-            )
     except Exception as e:
-        logger.exception(e)
-
+        pass
+    try:
+        if "store_api_key" not in user_columns:
+            with op.batch_alter_table("user", schema=None) as batch_op:
+                batch_op.add_column(
+                    sa.Column("store_api_key", sqlmodel.AutoString(), nullable=True)
+                )
+    except Exception as e:
+        pass
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     try:
         with op.batch_alter_table("user", schema=None) as batch_op:
```

### Comparing `langflow-0.6.8/src/backend/langflow/alembic/versions/f5ee9749d1a6_user_id_can_be_null_in_flow.py` & `langflow-0.6.9/src/backend/langflow/alembic/versions/f5ee9749d1a6_user_id_can_be_null_in_flow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """User id can be null in Flow
 
 Revision ID: f5ee9749d1a6
 Revises: 7843803a87b5
 Create Date: 2023-10-18 23:12:27.297016
 
 """
+
 from typing import Sequence, Union
 
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision: str = "f5ee9749d1a6"
```

### Comparing `langflow-0.6.8/src/backend/langflow/alembic.ini` & `langflow-0.6.9/src/backend/langflow/alembic.ini`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 # the output encoding used when revision files
 # are written from script.py.mako
 # output_encoding = utf-8
 
 # This is the path to the db in the root of the project.
 # When the user runs the Langflow the database url will
 # be set dinamically.
-sqlalchemy.url = sqlite:///../../../langflow.db
+sqlalchemy.url = sqlite:///./langflow.db
 
 
 [post_write_hooks]
 # post_write_hooks defines scripts or Python functions that are run
 # on newly generated revision scripts.  See the documentation for further
 # detail and examples
 
@@ -94,15 +94,15 @@
 
 [logger_sqlalchemy]
 level = WARN
 handlers =
 qualname = sqlalchemy.engine
 
 [logger_alembic]
-level = INFO
+level = DEBUG
 handlers =
 qualname = alembic
 
 [handler_console]
 class = StreamHandler
 args = (sys.stderr,)
 level = NOTSET
```

### Comparing `langflow-0.6.8/src/backend/langflow/api/router.py` & `langflow-0.6.9/src/backend/langflow/api/router.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/utils.py` & `langflow-0.6.9/src/backend/langflow/api/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/__init__.py` & `langflow-0.6.9/src/backend/langflow/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/api_key.py` & `langflow-0.6.9/src/backend/langflow/api/v1/api_key.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/base.py` & `langflow-0.6.9/src/backend/langflow/api/v1/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/callback.py` & `langflow-0.6.9/src/backend/langflow/api/v1/callback.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/chat.py` & `langflow-0.6.9/src/backend/langflow/api/v1/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 import time
 
-from fastapi import APIRouter, Depends, HTTPException, WebSocket, WebSocketException, status
+from fastapi import (
+    APIRouter,
+    Depends,
+    HTTPException,
+    WebSocket,
+    WebSocketException,
+    status,
+)
 from fastapi.responses import StreamingResponse
+from loguru import logger
+from sqlmodel import Session
+
 from langflow.api.utils import build_input_keys_response, format_elapsed_time
 from langflow.api.v1.schemas import BuildStatus, BuiltResponse, InitResponse, StreamData
 from langflow.graph.graph.base import Graph
-from langflow.services.auth.utils import get_current_active_user, get_current_user_for_websocket
+from langflow.services.auth.utils import (
+    get_current_active_user,
+    get_current_user_for_websocket,
+)
 from langflow.services.cache.service import BaseCacheService
 from langflow.services.cache.utils import update_build_status
 from langflow.services.chat.service import ChatService
 from langflow.services.deps import get_cache_service, get_chat_service, get_session
-from loguru import logger
-from sqlmodel import Session
 
 router = APIRouter(tags=["Chat"])
 
 
 @router.websocket("/chat/{client_id}")
 async def chat(
     client_id: str,
```

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/credential.py` & `langflow-0.6.9/src/backend/langflow/api/v1/credential.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/endpoints.py` & `langflow-0.6.9/src/backend/langflow/api/v1/endpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/flows.py` & `langflow-0.6.9/src/backend/langflow/api/v1/flows.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/login.py` & `langflow-0.6.9/src/backend/langflow/api/v1/login.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/schemas.py` & `langflow-0.6.9/src/backend/langflow/api/v1/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/store.py` & `langflow-0.6.9/src/backend/langflow/api/v1/store.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/users.py` & `langflow-0.6.9/src/backend/langflow/api/v1/users.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/api/v1/validate.py` & `langflow-0.6.9/src/backend/langflow/api/v1/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/agents/AgentInitializer.py` & `langflow-0.6.9/src/backend/langflow/components/agents/AgentInitializer.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/agents/CSVAgent.py` & `langflow-0.6.9/src/backend/langflow/components/agents/CSVAgent.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/agents/JsonAgent.py` & `langflow-0.6.9/src/backend/langflow/components/agents/JsonAgent.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/agents/OpenAIConversationalAgent.py` & `langflow-0.6.9/src/backend/langflow/components/agents/OpenAIConversationalAgent.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/agents/SQLAgent.py` & `langflow-0.6.9/src/backend/langflow/components/agents/SQLAgent.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/agents/VectorStoreAgent.py` & `langflow-0.6.9/src/backend/langflow/components/agents/VectorStoreAgent.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/agents/VectorStoreRouterAgent.py` & `langflow-0.6.9/src/backend/langflow/components/agents/VectorStoreRouterAgent.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/chains/ConversationChain.py` & `langflow-0.6.9/src/backend/langflow/components/chains/ConversationChain.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/chains/LLMChain.py` & `langflow-0.6.9/src/backend/langflow/components/chains/LLMChain.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/chains/LLMCheckerChain.py` & `langflow-0.6.9/src/backend/langflow/components/chains/LLMCheckerChain.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/chains/LLMMathChain.py` & `langflow-0.6.9/src/backend/langflow/components/chains/LLMMathChain.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/chains/PromptRunner.py` & `langflow-0.6.9/src/backend/langflow/components/chains/PromptRunner.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/chains/RetrievalQA.py` & `langflow-0.6.9/src/backend/langflow/components/chains/RetrievalQA.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/chains/RetrievalQAWithSourcesChain.py` & `langflow-0.6.9/src/backend/langflow/components/chains/RetrievalQAWithSourcesChain.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/chains/SQLDatabaseChain.py` & `langflow-0.6.9/src/backend/langflow/components/chains/SQLDatabaseChain.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/documentloaders/DirectoryLoader.py` & `langflow-0.6.9/src/backend/langflow/components/documentloaders/DirectoryLoader.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/documentloaders/FileLoader.py` & `langflow-0.6.9/src/backend/langflow/components/documentloaders/FileLoader.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/documentloaders/UrlLoader.py` & `langflow-0.6.9/src/backend/langflow/components/documentloaders/UrlLoader.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/embeddings/AmazonBedrockEmbeddings.py` & `langflow-0.6.9/src/backend/langflow/components/embeddings/AmazonBedrockEmbeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/embeddings/AzureOpenAIEmbeddings.py` & `langflow-0.6.9/src/backend/langflow/components/embeddings/AzureOpenAIEmbeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/embeddings/CohereEmbeddings.py` & `langflow-0.6.9/src/backend/langflow/components/embeddings/CohereEmbeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/embeddings/HuggingFaceEmbeddings.py` & `langflow-0.6.9/src/backend/langflow/components/embeddings/HuggingFaceEmbeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/embeddings/HuggingFaceInferenceAPIEmbeddings.py` & `langflow-0.6.9/src/backend/langflow/components/embeddings/HuggingFaceInferenceAPIEmbeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/embeddings/OllamaEmbeddings.py` & `langflow-0.6.9/src/backend/langflow/components/embeddings/OllamaEmbeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/embeddings/OpenAIEmbeddings.py` & `langflow-0.6.9/src/backend/langflow/components/embeddings/OpenAIEmbeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/embeddings/VertexAIEmbeddings.py` & `langflow-0.6.9/src/backend/langflow/components/embeddings/VertexAIEmbeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/AmazonBedrock.py` & `langflow-0.6.9/src/backend/langflow/components/llms/AmazonBedrock.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/Anthropic.py` & `langflow-0.6.9/src/backend/langflow/components/llms/Anthropic.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/AnthropicLLM.py` & `langflow-0.6.9/src/backend/langflow/components/llms/AnthropicLLM.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/AzureChatOpenAI.py` & `langflow-0.6.9/src/backend/langflow/components/llms/AzureChatOpenAI.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/BaiduQianfanChatEndpoints.py` & `langflow-0.6.9/src/backend/langflow/components/llms/BaiduQianfanChatEndpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/BaiduQianfanLLMEndpoints.py` & `langflow-0.6.9/src/backend/langflow/components/llms/BaiduQianfanLLMEndpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/CTransformers.py` & `langflow-0.6.9/src/backend/langflow/components/llms/CTransformers.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/ChatAnthropic.py` & `langflow-0.6.9/src/backend/langflow/components/llms/ChatAnthropic.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/ChatLiteLLM.py` & `langflow-0.6.9/src/backend/langflow/components/llms/ChatLiteLLM.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/ChatOllamaEndpoint.py` & `langflow-0.6.9/src/backend/langflow/components/llms/ChatOllamaEndpoint.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/ChatOpenAI.py` & `langflow-0.6.9/src/backend/langflow/components/llms/ChatOpenAI.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/ChatVertexAI.py` & `langflow-0.6.9/src/backend/langflow/components/llms/ChatVertexAI.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/Cohere.py` & `langflow-0.6.9/src/backend/langflow/components/llms/Cohere.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/GoogleGenerativeAI.py` & `langflow-0.6.9/src/backend/langflow/components/llms/GoogleGenerativeAI.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/HuggingFaceEndpoints.py` & `langflow-0.6.9/src/backend/langflow/components/llms/HuggingFaceEndpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/LlamaCpp.py` & `langflow-0.6.9/src/backend/langflow/components/llms/LlamaCpp.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/OllamaLLM.py` & `langflow-0.6.9/src/backend/langflow/components/llms/OllamaLLM.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/llms/VertexAI.py` & `langflow-0.6.9/src/backend/langflow/components/llms/VertexAI.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/retrievers/AmazonKendra.py` & `langflow-0.6.9/src/backend/langflow/components/retrievers/AmazonKendra.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/retrievers/MetalRetriever.py` & `langflow-0.6.9/src/backend/langflow/components/retrievers/MetalRetriever.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/retrievers/MultiQueryRetriever.py` & `langflow-0.6.9/src/backend/langflow/components/retrievers/MultiQueryRetriever.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/retrievers/VectaraSelfQueryRetriver.py` & `langflow-0.6.9/src/backend/langflow/components/retrievers/VectaraSelfQueryRetriver.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/textsplitters/CharacterTextSplitter.py` & `langflow-0.6.9/src/backend/langflow/components/textsplitters/CharacterTextSplitter.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/textsplitters/LanguageRecursiveTextSplitter.py` & `langflow-0.6.9/src/backend/langflow/components/textsplitters/LanguageRecursiveTextSplitter.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/textsplitters/RecursiveCharacterTextSplitter.py` & `langflow-0.6.9/src/backend/langflow/components/textsplitters/RecursiveCharacterTextSplitter.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/toolkits/JsonToolkit.py` & `langflow-0.6.9/src/backend/langflow/components/toolkits/JsonToolkit.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/toolkits/Metaphor.py` & `langflow-0.6.9/src/backend/langflow/components/toolkits/Metaphor.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/toolkits/OpenAPIToolkit.py` & `langflow-0.6.9/src/backend/langflow/components/toolkits/OpenAPIToolkit.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/toolkits/VectorStoreInfo.py` & `langflow-0.6.9/src/backend/langflow/components/toolkits/VectorStoreInfo.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/toolkits/VectorStoreRouterToolkit.py` & `langflow-0.6.9/src/backend/langflow/components/toolkits/VectorStoreRouterToolkit.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/toolkits/VectorStoreToolkit.py` & `langflow-0.6.9/src/backend/langflow/components/toolkits/VectorStoreToolkit.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/tools/SearchApi.py` & `langflow-0.6.9/src/backend/langflow/components/tools/SearchApi.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/BingSearchAPIWrapper.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/BingSearchAPIWrapper.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/GetRequest.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/GetRequest.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/GoogleSearchAPIWrapper.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/GoogleSearchAPIWrapper.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/GoogleSerperAPIWrapper.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/GoogleSerperAPIWrapper.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/JSONDocumentBuilder.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/JSONDocumentBuilder.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/PostRequest.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/PostRequest.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/SearxSearchWrapper.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/SearxSearchWrapper.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/SerpAPIWrapper.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/SerpAPIWrapper.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/UpdateRequest.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/UpdateRequest.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/WikipediaAPIWrapper.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/WikipediaAPIWrapper.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/utilities/WolframAlphaAPIWrapper.py` & `langflow-0.6.9/src/backend/langflow/components/utilities/WolframAlphaAPIWrapper.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/vectorstores/Chroma.py` & `langflow-0.6.9/src/backend/langflow/components/vectorstores/Chroma.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/vectorstores/FAISS.py` & `langflow-0.6.9/src/backend/langflow/components/vectorstores/FAISS.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/vectorstores/MongoDBAtlasVectorSearch.py` & `langflow-0.6.9/src/backend/langflow/components/vectorstores/MongoDBAtlasVectorSearch.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/vectorstores/Pinecone.py` & `langflow-0.6.9/src/backend/langflow/components/vectorstores/Pinecone.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/vectorstores/Qdrant.py` & `langflow-0.6.9/src/backend/langflow/components/vectorstores/Qdrant.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/vectorstores/Redis.py` & `langflow-0.6.9/src/backend/langflow/components/vectorstores/Redis.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/vectorstores/SupabaseVectorStore.py` & `langflow-0.6.9/src/backend/langflow/components/vectorstores/SupabaseVectorStore.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/vectorstores/Vectara.py` & `langflow-0.6.9/src/backend/langflow/components/vectorstores/Vectara.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/vectorstores/Weaviate.py` & `langflow-0.6.9/src/backend/langflow/components/vectorstores/Weaviate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/components/vectorstores/pgvector.py` & `langflow-0.6.9/src/backend/langflow/components/vectorstores/pgvector.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/config.yaml` & `langflow-0.6.9/src/backend/langflow/config.yaml`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/core/celeryconfig.py` & `langflow-0.6.9/src/backend/langflow/core/celeryconfig.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/custom/customs.py` & `langflow-0.6.9/src/backend/langflow/custom/customs.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/field_typing/__init__.py` & `langflow-0.6.9/src/backend/langflow/field_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/field_typing/constants.py` & `langflow-0.6.9/src/backend/langflow/field_typing/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/field_typing/range_spec.py` & `langflow-0.6.9/src/backend/langflow/field_typing/range_spec.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/frontend/assets/index-c6d7fba2.css` & `langflow-0.6.9/src/backend/langflow/frontend/assets/index-e7ca4585.css`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-.react-flow__container{position:absolute;width:100%;height:100%;top:0;left:0}.react-flow__pane{z-index:1;cursor:grab}.react-flow__pane.selection{cursor:pointer}.react-flow__pane.dragging{cursor:grabbing}.react-flow__viewport{transform-origin:0 0;z-index:2;pointer-events:none}.react-flow__renderer{z-index:4}.react-flow__selection{z-index:6}.react-flow__nodesselection-rect:focus,.react-flow__nodesselection-rect:focus-visible{outline:none}.react-flow .react-flow__edges{pointer-events:none;overflow:visible}.react-flow__edge-path,.react-flow__connection-path{stroke:#b1b1b7;stroke-width:1;fill:none}.react-flow__edge{pointer-events:visibleStroke;cursor:pointer}.react-flow__edge.animated path{stroke-dasharray:5;animation:dashdraw .5s linear infinite}.react-flow__edge.animated path.react-flow__edge-interaction{stroke-dasharray:none;animation:none}.react-flow__edge.inactive{pointer-events:none}.react-flow__edge.selected,.react-flow__edge:focus,.react-flow__edge:focus-visible{outline:none}.react-flow__edge.selected .react-flow__edge-path,.react-flow__edge:focus .react-flow__edge-path,.react-flow__edge:focus-visible .react-flow__edge-path{stroke:#555}.react-flow__edge-textwrapper{pointer-events:all}.react-flow__edge-textbg{fill:#fff}.react-flow__edge .react-flow__edge-text{pointer-events:none;-webkit-user-select:none;user-select:none}.react-flow__connection{pointer-events:none}.react-flow__connection .animated{stroke-dasharray:5;animation:dashdraw .5s linear infinite}.react-flow__connectionline{z-index:1001}.react-flow__nodes{pointer-events:none;transform-origin:0 0}.react-flow__node{position:absolute;-webkit-user-select:none;user-select:none;pointer-events:all;transform-origin:0 0;box-sizing:border-box;cursor:grab}.react-flow__node.dragging{cursor:grabbing}.react-flow__nodesselection{z-index:3;transform-origin:left top;pointer-events:none}.react-flow__nodesselection-rect{position:absolute;pointer-events:all;cursor:grab}.react-flow__handle{position:absolute;pointer-events:none;min-width:5px;min-height:5px;width:6px;height:6px;background:#1a192b;border:1px solid white;border-radius:100%}.react-flow__handle.connectionindicator{pointer-events:all;cursor:crosshair}.react-flow__handle-bottom{top:auto;left:50%;bottom:-4px;transform:translate(-50%)}.react-flow__handle-top{left:50%;top:-4px;transform:translate(-50%)}.react-flow__handle-left{top:50%;left:-4px;transform:translateY(-50%)}.react-flow__handle-right{right:-4px;top:50%;transform:translateY(-50%)}.react-flow__edgeupdater{cursor:move;pointer-events:all}.react-flow__panel{position:absolute;z-index:5;margin:15px}.react-flow__panel.top{top:0}.react-flow__panel.bottom{bottom:0}.react-flow__panel.left{left:0}.react-flow__panel.right{right:0}.react-flow__panel.center{left:50%;transform:translate(-50%)}.react-flow__attribution{font-size:10px;background:rgba(255,255,255,.5);padding:2px 3px;margin:0}.react-flow__attribution a{text-decoration:none;color:#999}@keyframes dashdraw{0%{stroke-dashoffset:10}}.react-flow__edgelabel-renderer{position:absolute;width:100%;height:100%;pointer-events:none;-webkit-user-select:none;user-select:none}.react-flow__edge.updating .react-flow__edge-path{stroke:#777}.react-flow__edge-text{font-size:10px}.react-flow__node.selectable:focus,.react-flow__node.selectable:focus-visible{outline:none}.react-flow__node-default,.react-flow__node-input,.react-flow__node-output,.react-flow__node-group{padding:10px;border-radius:3px;width:150px;font-size:12px;color:#222;text-align:center;border-width:1px;border-style:solid;border-color:#1a192b;background-color:#fff}.react-flow__node-default.selectable:hover,.react-flow__node-input.selectable:hover,.react-flow__node-output.selectable:hover,.react-flow__node-group.selectable:hover{box-shadow:0 1px 4px 1px #00000014}.react-flow__node-default.selectable.selected,.react-flow__node-default.selectable:focus,.react-flow__node-default.selectable:focus-visible,.react-flow__node-input.selectable.selected,.react-flow__node-input.selectable:focus,.react-flow__node-input.selectable:focus-visible,.react-flow__node-output.selectable.selected,.react-flow__node-output.selectable:focus,.react-flow__node-output.selectable:focus-visible,.react-flow__node-group.selectable.selected,.react-flow__node-group.selectable:focus,.react-flow__node-group.selectable:focus-visible{box-shadow:0 0 0 .5px #1a192b}.react-flow__node-group{background-color:#f0f0f040}.react-flow__nodesselection-rect,.react-flow__selection{background:rgba(0,89,220,.08);border:1px dotted rgba(0,89,220,.8)}.react-flow__nodesselection-rect:focus,.react-flow__nodesselection-rect:focus-visible,.react-flow__selection:focus,.react-flow__selection:focus-visible{outline:none}.react-flow__controls{box-shadow:0 0 2px 1px #00000014}.react-flow__controls-button{border:none;background:#fefefe;border-bottom:1px solid #eee;box-sizing:content-box;display:flex;justify-content:center;align-items:center;width:16px;height:16px;cursor:pointer;-webkit-user-select:none;user-select:none;padding:5px}.react-flow__controls-button:hover{background:#f4f4f4}.react-flow__controls-button svg{width:100%;max-width:12px;max-height:12px}.react-flow__controls-button:disabled{pointer-events:none}.react-flow__controls-button:disabled svg{fill-opacity:.4}.react-flow__minimap{background-color:#fff}.react-flow__resize-control{position:absolute}.react-flow__resize-control.left,.react-flow__resize-control.right{cursor:ew-resize}.react-flow__resize-control.top,.react-flow__resize-control.bottom{cursor:ns-resize}.react-flow__resize-control.top.left,.react-flow__resize-control.bottom.right{cursor:nwse-resize}.react-flow__resize-control.bottom.left,.react-flow__resize-control.top.right{cursor:nesw-resize}.react-flow__resize-control.handle{width:4px;height:4px;border:1px solid #fff;border-radius:1px;background-color:#3367d9;transform:translate(-50%,-50%)}.react-flow__resize-control.handle.left{left:0;top:50%}.react-flow__resize-control.handle.right{left:100%;top:50%}.react-flow__resize-control.handle.top{left:50%;top:0}.react-flow__resize-control.handle.bottom{left:50%;top:100%}.react-flow__resize-control.handle.top.left,.react-flow__resize-control.handle.bottom.left{left:0}.react-flow__resize-control.handle.top.right,.react-flow__resize-control.handle.bottom.right{left:100%}.react-flow__resize-control.line{border-color:#3367d9;border-width:0;border-style:solid}.react-flow__resize-control.line.left,.react-flow__resize-control.line.right{width:1px;transform:translate(-50%);top:0;height:100%}.react-flow__resize-control.line.left{left:0;border-left-width:1px}.react-flow__resize-control.line.right{left:100%;border-right-width:1px}.react-flow__resize-control.line.top,.react-flow__resize-control.line.bottom{height:1px;transform:translateY(-50%);left:0;width:100%}.react-flow__resize-control.line.top{top:0;border-top-width:1px}.react-flow__resize-control.line.bottom{border-bottom-width:1px;top:100%}.\!loading{pointer-events:none!important;display:inline-block!important;aspect-ratio:1 / 1!important;width:1.5rem!important;background-color:currentColor!important;-webkit-mask-size:100%!important;mask-size:100%!important;-webkit-mask-repeat:no-repeat!important;mask-repeat:no-repeat!important;-webkit-mask-position:center!important;mask-position:center!important;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important;mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important}.loading{pointer-events:none;display:inline-block;aspect-ratio:1 / 1;width:1.5rem;background-color:currentColor;-webkit-mask-size:100%;mask-size:100%;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-position:center;mask-position:center;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}.loading-spinner{-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}body{overflow:hidden}.App{text-align:center}.react-flow__node{width:auto;height:auto;border-radius:auto;min-width:inherit}.App-logo{height:40vmin;pointer-events:none}@media (prefers-reduced-motion: no-preference){.App-logo{animation:App-logo-spin infinite 20s linear}}.App-header{background-color:#282c34;min-height:100vh;display:flex;flex-direction:column;align-items:center;justify-content:center;font-size:calc(10px + 2vmin);color:#fff}.App-link{color:#61dafb}@keyframes App-logo-spin{0%{transform:rotate(0)}to{transform:rotate(360deg)}}@font-face{font-family:text-security-disc;src:url(data:font/woff;base64,d09GRgABAAAAAAusAAsAAAAAMGgAAQAAAAAAAAAAAAAAAAAAAAAAAAAAAABHU1VCAAABCAAAADsAAABUIIslek9TLzIAAAFEAAAAPgAAAFZjRmM5Y21hcAAAAYQAAAgCAAArYmjjYVVnbHlmAAAJiAAAAEEAAABQiOYj2mhlYWQAAAnMAAAALgAAADYR8XmmaGhlYQAACfwAAAAcAAAAJAqNAyNobXR4AAAKGAAAAAgAAAAIAyAAAGxvY2EAAAogAAAABgAAAAYAKAAAbWF4cAAACigAAAAeAAAAIAEOACJuYW1lAAAKSAAAAUIAAAKOcN63t3Bvc3QAAAuMAAAAHQAAAC5lhHRpeJxjYGRgYOBiMGCwY2BycfMJYeDLSSzJY5BiYGGAAJA8MpsxJzM9kYEDxgPKsYBpDiBmg4gCACY7BUgAeJxjYGScwDiBgZWBgSGVtYKBgVECQjMfYEhiYmFgYGJgZWbACgLSXFMYHIAq/rNfAHK3gEmgASACAIekCT4AAHic7dhl0zDVmUXh5+XFHYK7E0IguFtwt4QQgmtwd3d3d7cED+4SXIO7u7vbsNfaUzU1fyGcu66u1adOf+6uHhgYGGpgYGDwL37/iyEHBoZZcWDQLzUw9NK/7A5if/DA8OwPOfQknBky+0P8/PPPOcd1UJ785frr/Dq/zq/z6/w3zsCgoX/xX74GRsxbcYpRB1iDB/7PGvT/DFGDenBwe8hKD1XpoSs9TKWHrfRwlR6+0iNUesRKj1TpkSs9SqVHrfRolR690r+p9BiVHrPSY1V67EqPU+lxKz1epcev9ASVnrDSE1V64kpPUulJKz1ZpSev9BSVnrLSU1V66kr/ttLTVPp3lZ62/KJSerpKT1/pP1R6hkrPWOmZKj1zpWep9KyVnq3Ss1d6jkrPWem5Kj13peep9LyVnq/S81d6gUr/sdILVnqhSi9c6UUqvWilF6v04pVeotJLVnqpSi9d6WUqvWyll6v08pVeodIrVvpPlf5zpVeq9F8qvXKl/1rpVSr9t0qvWunVKr16pdeo9JqVXqvSa1d6nUqvW+n1Kr1+pTeo9N8rvWGlN6r0xpXepNKbVnqzSm9e6S0qvWWlt6r01pXeptLbVnq7Sm9f6R0qvWOld6r0zpXepdK7Vnq3Su9e6T0qvWel96r03pXep9L7Vnq/Su9f6QMqfWClD6r0wZU+pNKHVvqwSh9e6SMqfWSlj6r00ZU+ptLHVvq4Sh9f6RMqfWKlT6r0yZU+pdKnVvq0Sp9e6TMqfWalz6r02ZU+p9LnVvq8Sp9f6QsqfWGl/1Hpf1b6okpfXOlLKn1ppS+r9OWVvqLS/6r0lZW+qtJXV/qaSl9b6esqfX2lb6j0jZW+qdI3V/qWSt9a6dsqfXul76j0vyt9Z6XvqvTdlb6n0vdW+r5K31/pByr9YKUfqvTDlX6k0v+p9KOVfqzSj1f6iUo/WemnKv10pZ+p9LOVfq7Sz1f6hUq/WOmXKv1ypV+p9KuVfq3Sr1f6jUq/Wem3Kv12pd+p9LuVfq/S71f6g0p/WOmPKv1xpT+p9KeV/qzSn1f6i0p/WemvKv11pb+p9LeV/q7S31f6h0r/WOmfKv1zDfI26KKHED1Y9JCihxI9tOhhRA8rejjRw4seQfSIokcSPbLoUUSPKno00aOL/o3oMUSPKXos0WOLHkf0uKLHEz2+6AlETyh6ItETi55E9KSiJxM9uegpRE8peirRU4v+rehpRP9O9LSify96OtHTi/6D6BlEzyh6JtEzi55F9KyiZxM9u+g5RM8pei7Rc4ueR/S8oucTPb/oBUT/UfSCohcSvbDoRUQvKnox0YuLXkL0kqKXEr206GVELyt6OdHLi15B9Iqi/yT6z6JXEv0X0SuL/qvoVUT/TfSqolcTvbroNUSvKXot0WuLXkf0uqLXE72+6A1E/130hqI3Er2x6E1Ebyp6M9Gbi95C9JaitxK9tehtRG8rejvR24veQfSOoncSvbPoXUTvKno30buL3kP0nqL3Er236H1E7yt6P9H7iz5A9IGiDxJ9sOhDRB8q+jDRh4s+QvSRoo8SfbToY0QfK/o40ceLPkH0iaJPEn2y6FNEnyr6NNGniz5D9JmizxJ9tuhzRJ8r+jzR54u+QPSFov8h+p+iLxJ9sehLRF8q+jLRl4u+QvS/RF8p+irRV4u+RvS1oq8Tfb3oG0TfKPom0TeLvkX0raJvE3276DtE/1v0naLvEn236HtE3yv6PtH3i35A9IOiHxL9sOhHRP9H9KOiHxP9uOgnRD8p+inRT4t+RvSzop8T/bzoF0S/KPol0S+LfkX0q6JfE/266DdEvyn6LdFvi35H9Lui3xP9vugPRH8o+iPRH4v+RPSnoj8T/bnoL0R/Kfor0V+L/kb0t6K/E/296B9E/yj6J9E/K/2/v/npoocQPVj0kKKHEj206GFEDyt6ONHDix5B9IiiRxI9suhRRI8qejTRo4v+jegxRI8peizRY4seR/S4oscTPb7oCURPKHoi0ROLnkT0pKInEz256ClETyl6KtFTi/6t6GlE/070tKJ/L3o60dOL/oPoGUTPKHom0TOLnkX0rKJnEz276DlEzyl6LtFzi55H9Lyi5xM9v+gFRP9R9IKiFxK9sOhFRC8qejHRi4teQvSSopcSvbToZUQvK3o50cuLXkH0iqL/JPrPolcS/RfRK4v+q+hVRP9N9KqiVxO9uug1RK8pei3Ra4teR/S6otcTvb7oDUT/XfSGojcSvbHoTURvKnoz0ZuL3kL0lqK3Er216G1Ebyt6O9Hbi95B9I6idxK9s+hdRO8qejfRu4veQ/SeovcSvbfofUTvK3o/0fuLPkD0gaIPEn2w6ENEHyr6MNGHiz5C9JGijxJ9tOhjRB8r+jjRx4s+QfSJok8SfbLoU0SfKvo00aeLPkP0maLPEn226HNEnyv6PNHni75A9IWi/yH6n6IvEn2x6EtEXyr6MtGXi75C9L9EXyn6KtFXi75G9LWirxN9vegbRN8o+ibRN4u+RfStom8TfbvoO0T/W/Sdou8Sfbfoe0TfK/o+0feLfkD0g6IfEv2w6EdE/0f0o6IfE/246CdEPyn6KdFPi35G9LOinxP9vOgXRL8o+iXRL4t+RfSrol8T/broN0S/Kfot0W+Lfkf0u6LfE/2+6A9Efyj6I9Efi/5E9KeiPxP9uegvRH8p+ivRX4v+RvS3or8T/b3oH0T/KPon0T9rYND/AOaSEScAAHicY2BiAAKmPSy+QEqUgYFRUURcTFzMyNzM3MxEXU1dTYmdjZ2NccK/K5oaLm6L3Fw0NOEMZoVAFD6IAQD4PA9iAAAAeJxjYGRgYADilrme/fH8Nl8ZuNkvAEUYbnDPcEOmmfaw+AIpDgYmEA8AHMMJGAAAeJxjYGRgYL/AAATMCiCSaQ8DIwMqYAIAK/QBvQAAAAADIAAAAAAAAAAoAAB4nGNgZGBgYGIQA2IGMIuBgQsIGRj+g/kMAArUATEAAHicjY69TsMwFIWP+4doJYSKhMTmoUJIqOnPWIm1ZWDq0IEtTZw2VRpHjlu1D8A7MPMczAw8DM/AifFEl9qS9d1zzr3XAK7xBYHqCHTdW50aLlj9cZ1057lBfvTcRAdPnlvUnz23mXj13MEN3jhBNC6p9PDuuYYrfHquU//23CD/eG7iVnQ9t9ATD57bWIgXzx3ciw+rDrZfqmhnUnvsx2kZzdVql4Xm1DhVFsqUqc7lKBiemjOVKxNaFcvlUZb71djaRCZGb+VU51ZlmZaF0RsV2WBtbTEZDBKvB5HewkLhwLePkhRhB4OU9ZFKTCqpzems6GQI6Z7TcU5mQceQUmjkkBghwPCszhmd3HWHLh+ze8mEpLvnT8dULRLWCTMaW9LUbanSGa+mUjhv47ZY7l67rgITDHiTf/mAKU76BTuXfk8AAHicY2BigAARBuyAiZGJkZmBJSWzOJmBAQALQwHHAAAA) format("woff")}.json-view{height:370px!important;background-color:#2c2c2c!important;border-radius:10px!important;padding:10px!important}.jv-indent{overflow-y:auto!important;max-height:310px!important;border-radius:10px}.jv-indent::-webkit-scrollbar{width:8px!important;height:8px!important;border-radius:10px}.jv-indent::-webkit-scrollbar-track{background-color:#f1f1f1!important;border-radius:10px}.jv-indent::-webkit-scrollbar-thumb{background-color:#ccc!important;border-radius:999px!important}.jv-indent::-webkit-scrollbar-thumb:hover{background-color:#bbb!important}:is(.dark .json-view,.dark.json-view){color:#d1d1d1;--json-property: #009033;--json-index: #5d75f2;--json-number: #5d75f2;--json-string: #c57e29;--json-boolean: #e4407b;--json-null: #e4407b}:is(.dark .json-view_a11y,.dark.json-view_a11y){color:#d1d1d1;--json-property: #ffd700;--json-index: #00e0e0;--json-number: #00e0e0;--json-string: #abe338;--json-boolean: #ffa07a;--json-null: #ffa07a}:is(.dark .json-view_github,.dark.json-view_github){color:#79b8ff;--json-property: #79b8ff;--json-index: #79b8ff;--json-number: #79b8ff;--json-string: #9ecbff;--json-boolean: #79b8ff;--json-null: #79b8ff}:is(.dark .json-view_vscode,.dark.json-view_vscode){color:orchid;--json-property: #9cdcfe;--json-index: #b5cea8;--json-number: #b5cea8;--json-string: #ce9178;--json-boolean: #569cd6;--json-null: #569cd6}:is(.dark .json-view_atom,.dark.json-view_atom){color:#abb2bf;--json-property: #e06c75;--json-index: #d19a66;--json-number: #d19a66;--json-string: #98c379;--json-boolean: #56b6c2;--json-null: #56b6c2}:is(.dark .json-view_winter-is-coming,.dark.json-view_winter-is-coming){color:#a7dbf7;--json-property: #91dacd;--json-index: #8dec95;--json-number: #8dec95;--json-string: #e0aff5;--json-boolean: #f29fd8;--json-null: #f29fd8}.json-view{display:block;color:#4d4d4d;text-align:left;--json-property: #009033;--json-index: #676dff;--json-number: #676dff;--json-string: #b2762e;--json-boolean: #dc155e;--json-null: #dc155e}.json-view .json-view--property{color:var(--json-property)}.json-view .json-view--index{color:var(--json-index)}.json-view .json-view--number{color:var(--json-number)}.json-view .json-view--string{color:var(--json-string)}.json-view .json-view--boolean{color:var(--json-boolean)}.json-view .json-view--null{color:var(--json-null)}.json-view .jv-indent{padding-left:1em}.json-view .jv-chevron{display:inline-block;vertical-align:-20%;cursor:pointer;opacity:.4;width:1em;height:1em}:is(.json-view .jv-chevron:hover,.json-view .jv-size:hover+.jv-chevron){opacity:.8}.json-view .jv-size{cursor:pointer;opacity:.4;font-size:.875em;font-style:italic;margin-left:.5em;vertical-align:-5%;line-height:1}.json-view :is(.json-view--copy,.json-view--edit),.json-view .json-view--link svg{display:none;width:1em;height:1em;margin-left:.25em;cursor:pointer}.json-view .json-view--input{width:120px;margin-left:.25em;border-radius:4px;border:1px solid currentColor;padding:0 4px;font-size:87.5%;line-height:1.25;background:transparent}.json-view .json-view--deleting{outline:1px solid #da0000;background-color:#da000011;text-decoration-line:line-through}:is(.json-view:hover,.json-view--pair:hover)>:is(.json-view--copy,.json-view--edit),:is(.json-view:hover,.json-view--pair:hover)>.json-view--link svg{display:inline-block}.json-view .jv-button{background:transparent;outline:none;border:none;cursor:pointer}.json-view .cursor-pointer{cursor:pointer}.json-view svg{vertical-align:-10%}.jv-size-chevron~svg{vertical-align:-16%}.json-view_a11y{color:#545454;--json-property: #aa5d00;--json-index: #007299;--json-number: #007299;--json-string: #008000;--json-boolean: #d91e18;--json-null: #d91e18}.json-view_github{color:#005cc5;--json-property: #005cc5;--json-index: #005cc5;--json-number: #005cc5;--json-string: #032f62;--json-boolean: #005cc5;--json-null: #005cc5}.json-view_vscode{color:#005cc5;--json-property: #0451a5;--json-index: #0000ff;--json-number: #0000ff;--json-string: #a31515;--json-boolean: #0000ff;--json-null: #0000ff}.json-view_atom{color:#383a42;--json-property: #e45649;--json-index: #986801;--json-number: #986801;--json-string: #50a14f;--json-boolean: #0184bc;--json-null: #0184bc}.json-view_winter-is-coming{color:#0431fa;--json-property: #3a9685;--json-index: #ae408b;--json-number: #ae408b;--json-string: #8123a9;--json-boolean: #0184bc;--json-null: #0184bc}:root{--background: 0 0% 100%;--foreground: 222.2 47.4% 11.2%;--muted: 210 40% 98%;--muted-foreground: 215.4 16.3% 46.9%;--popover: 0 0% 100%;--popover-foreground: 222.2 47.4% 11.2%;--card: 0 0% 100%;--card-foreground: 222.2 47.4% 11.2%;--border: 214.3 21.8% 91.4%;--input: 214.3 21.8% 91.4%;--primary: 222.2 27% 11.2%;--primary-foreground: 210 40% 98%;--secondary: 210 40% 96.1%;--secondary-foreground: 222.2 47.4% 11.2%;--accent: 210 30% 96.1%;--accent-foreground: 222.2 47.4% 11.2%;--destructive: 0 100% 50%;--destructive-foreground: 210 40% 98%;--radius: .5rem;--ring: 215 20.2% 65.1%;--round-btn-shadow: #00000063;--error-background: #fef2f2;--error-foreground: #991b1b;--success-background: #f0fdf4;--success-foreground: #14532d;--info-background: #f0f4fd;--info-foreground: #141653;--high-indigo: #4338ca;--medium-indigo: #6366f1;--low-indigo: #e0e7ff;--beta-background: rgb(219 234 254);--beta-foreground: rgb(37 99 235);--chat-bot-icon: #afe6ef;--chat-user-icon: #aface9;--component-icon: #d8598a;--flow-icon: #2f67d0;--blur-shared: #151923de;--build-trigger: #dc735b;--chat-trigger: #5c8be1;--chat-trigger-disabled: #b4c3da;--status-red: #ef4444;--status-yellow: #eab308;--chat-send: #059669;--status-green: #4ade80;--status-blue: #2563eb;--connection: #555}.\!dark{--background: 224 35% 7.5% !important;--foreground: 213 31% 80% !important;--muted: 223 27% 11% !important;--muted-foreground: 215.4 16.3% 56.9% !important;--popover: 224 71% 4% !important;--popover-foreground: 215 20.2% 65.1% !important;--card: 224 25% 15.5% !important;--card-foreground: 213 31% 80% !important;--border: 216 24% 17% !important;--input: 216 24% 17% !important;--primary: 210 20% 80% !important;--primary-foreground: 222.2 27.4% 1.2% !important;--secondary: 222.2 37.4% 7.2% !important;--secondary-foreground: 210 40% 80% !important;--accent: 216 24% 20% !important;--accent-foreground: 210 30% 98% !important;--destructive: 0 63% 31% !important;--destructive-foreground: 210 40% 98% !important;--ring: 216 24% 30% !important;--radius: .5rem !important;--round-btn-shadow: #00000063 !important;--success-background: #022c22 !important;--success-foreground: #ecfdf5 !important;--error-foreground: #fef2f2 !important;--error-background: #450a0a !important;--info-foreground: #eff6ff !important;--info-background: #172554 !important;--high-indigo: #4338ca !important;--medium-indigo: #6366f1 !important;--low-indigo: #e0e7ff !important;--component-icon: #c35f85 !important;--flow-icon: #2467e4 !important;--blur-shared: #151923d2 !important;--build-trigger: #dc735b !important;--chat-trigger: #5c8be1 !important;--chat-trigger-disabled: #2d3b54 !important;--status-red: #ef4444 !important;--status-yellow: #eab308 !important;--chat-send: #059669 !important;--status-green: #4ade80 !important;--status-blue: #2563eb !important;--connection: #555 !important;--beta-background: rgb(37 99 235) !important;--beta-foreground: rgb(219 234 254) !important;--chat-bot-icon: #235d70 !important;--chat-user-icon: #4f3d6e !important}.dark{--background: 224 35% 7.5%;--foreground: 213 31% 80%;--muted: 223 27% 11%;--muted-foreground: 215.4 16.3% 56.9%;--popover: 224 71% 4%;--popover-foreground: 215 20.2% 65.1%;--card: 224 25% 15.5%;--card-foreground: 213 31% 80%;--border: 216 24% 17%;--input: 216 24% 17%;--primary: 210 20% 80%;--primary-foreground: 222.2 27.4% 1.2%;--secondary: 222.2 37.4% 7.2%;--secondary-foreground: 210 40% 80%;--accent: 216 24% 20%;--accent-foreground: 210 30% 98%;--destructive: 0 63% 31%;--destructive-foreground: 210 40% 98%;--ring: 216 24% 30%;--radius: .5rem;--round-btn-shadow: #00000063;--success-background: #022c22;--success-foreground: #ecfdf5;--error-foreground: #fef2f2;--error-background: #450a0a;--info-foreground: #eff6ff;--info-background: #172554;--high-indigo: #4338ca;--medium-indigo: #6366f1;--low-indigo: #e0e7ff;--component-icon: #c35f85;--flow-icon: #2467e4;--blur-shared: #151923d2;--build-trigger: #dc735b;--chat-trigger: #5c8be1;--chat-trigger-disabled: #2d3b54;--status-red: #ef4444;--status-yellow: #eab308;--chat-send: #059669;--status-green: #4ade80;--status-blue: #2563eb;--connection: #555;--beta-background: rgb(37 99 235);--beta-foreground: rgb(219 234 254);--chat-bot-icon: #235d70;--chat-user-icon: #4f3d6e}.\!loading{pointer-events:none!important;display:inline-block!important;aspect-ratio:1 / 1!important;width:1.5rem!important;background-color:currentColor!important;-webkit-mask-size:100%!important;mask-size:100%!important;-webkit-mask-repeat:no-repeat!important;mask-repeat:no-repeat!important;-webkit-mask-position:center!important;mask-position:center!important;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important;mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important}.loading{pointer-events:none;display:inline-block;aspect-ratio:1 / 1;width:1.5rem;background-color:currentColor;-webkit-mask-size:100%;mask-size:100%;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-position:center;mask-position:center;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}.loading-spinner{-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}*,:before,:after{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}:before,:after{--tw-content: ""}html,:host{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;tab-size:4;font-family:var(--font-sans),ui-sans-serif,system-ui,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,samp,pre{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,[type=button],[type=reset],[type=submit]{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dl,dd,h1,h2,h3,h4,h5,h6,hr,figure,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}ol,ul,menu{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}button,[role=button]{cursor:pointer}:disabled{cursor:default}img,svg,video,canvas,audio,iframe,embed,object{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}:root,[data-theme]{background-color:var(--fallback-b1,oklch(var(--b1)/1));color:var(--fallback-bc,oklch(var(--bc)/1))}@supports not (color: oklch(0 0 0)){:root{color-scheme:light;--fallback-p: #491eff;--fallback-pc: #d4dbff;--fallback-s: #ff41c7;--fallback-sc: #fff9fc;--fallback-a: #00cfbd;--fallback-ac: #00100d;--fallback-n: #2b3440;--fallback-nc: #d7dde4;--fallback-b1: #ffffff;--fallback-b2: #e5e6e6;--fallback-b3: #e5e6e6;--fallback-bc: #1f2937;--fallback-in: #00b3f0;--fallback-inc: #000000;--fallback-su: #00ca92;--fallback-suc: #000000;--fallback-wa: #ffc22d;--fallback-wac: #000000;--fallback-er: #ff6f70;--fallback-erc: #000000}@media (prefers-color-scheme: dark){:root{color-scheme:dark;--fallback-p: #7582ff;--fallback-pc: #050617;--fallback-s: #ff71cf;--fallback-sc: #190211;--fallback-a: #00c7b5;--fallback-ac: #000e0c;--fallback-n: #2a323c;--fallback-nc: #a6adbb;--fallback-b1: #1d232a;--fallback-b2: #191e24;--fallback-b3: #15191e;--fallback-bc: #a6adbb;--fallback-in: #00b3f0;--fallback-inc: #000000;--fallback-su: #00ca92;--fallback-suc: #000000;--fallback-wa: #ffc22d;--fallback-wac: #000000;--fallback-er: #ff6f70;--fallback-erc: #000000}}}html{-webkit-tap-highlight-color:transparent}:root{color-scheme:light;--in: .7206 .191 231.6;--su: 64.8% .15 160;--wa: .8471 .199 83.87;--er: .7176 .221 22.18;--pc: .89824 .06192 275.75;--ac: .15352 .0368 183.61;--inc: 0 0 0;--suc: 0 0 0;--wac: 0 0 0;--erc: 0 0 0;--rounded-box: 1rem;--rounded-btn: .5rem;--rounded-badge: 1.9rem;--animation-btn: .25s;--animation-input: .2s;--btn-focus-scale: .95;--border-btn: 1px;--tab-border: 1px;--tab-radius: .5rem;--p: .4912 .3096 275.75;--s: .6971 .329 342.55;--sc: .9871 .0106 342.55;--a: .7676 .184 183.61;--n: .321785 .02476 255.701624;--nc: .894994 .011585 252.096176;--b1: 1 0 0;--b2: .961151 0 0;--b3: .924169 .00108 197.137559;--bc: .278078 .029596 256.847952}@media (prefers-color-scheme: dark){:root{color-scheme:dark;--in: .7206 .191 231.6;--su: 64.8% .15 160;--wa: .8471 .199 83.87;--er: .7176 .221 22.18;--pc: .13138 .0392 275.75;--sc: .1496 .052 342.55;--ac: .14902 .0334 183.61;--inc: 0 0 0;--suc: 0 0 0;--wac: 0 0 0;--erc: 0 0 0;--rounded-box: 1rem;--rounded-btn: .5rem;--rounded-badge: 1.9rem;--animation-btn: .25s;--animation-input: .2s;--btn-focus-scale: .95;--border-btn: 1px;--tab-border: 1px;--tab-radius: .5rem;--p: .6569 .196 275.75;--s: .748 .26 342.55;--a: .7451 .167 183.61;--n: .313815 .021108 254.139175;--nc: .746477 .0216 264.435964;--b1: .253267 .015896 252.417568;--b2: .232607 .013807 253.100675;--b3: .211484 .01165 254.087939;--bc: .746477 .0216 264.435964}}[data-theme=light]{color-scheme:light;--in: .7206 .191 231.6;--su: 64.8% .15 160;--wa: .8471 .199 83.87;--er: .7176 .221 22.18;--pc: .89824 .06192 275.75;--ac: .15352 .0368 183.61;--inc: 0 0 0;--suc: 0 0 0;--wac: 0 0 0;--erc: 0 0 0;--rounded-box: 1rem;--rounded-btn: .5rem;--rounded-badge: 1.9rem;--animation-btn: .25s;--animation-input: .2s;--btn-focus-scale: .95;--border-btn: 1px;--tab-border: 1px;--tab-radius: .5rem;--p: .4912 .3096 275.75;--s: .6971 .329 342.55;--sc: .9871 .0106 342.55;--a: .7676 .184 183.61;--n: .321785 .02476 255.701624;--nc: .894994 .011585 252.096176;--b1: 1 0 0;--b2: .961151 0 0;--b3: .924169 .00108 197.137559;--bc: .278078 .029596 256.847952}[data-theme=dark]{color-scheme:dark;--in: .7206 .191 231.6;--su: 64.8% .15 160;--wa: .8471 .199 83.87;--er: .7176 .221 22.18;--pc: .13138 .0392 275.75;--sc: .1496 .052 342.55;--ac: .14902 .0334 183.61;--inc: 0 0 0;--suc: 0 0 0;--wac: 0 0 0;--erc: 0 0 0;--rounded-box: 1rem;--rounded-btn: .5rem;--rounded-badge: 1.9rem;--animation-btn: .25s;--animation-input: .2s;--btn-focus-scale: .95;--border-btn: 1px;--tab-border: 1px;--tab-radius: .5rem;--p: .6569 .196 275.75;--s: .748 .26 342.55;--a: .7451 .167 183.61;--n: .313815 .021108 254.139175;--nc: .746477 .0216 264.435964;--b1: .253267 .015896 252.417568;--b2: .232607 .013807 253.100675;--b3: .211484 .01165 254.087939;--bc: .746477 .0216 264.435964}*{border-color:hsl(var(--border))}body{background-color:hsl(var(--background));color:hsl(var(--foreground));font-feature-settings:"rlig" 1,"calt" 1}*,:before,:after{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.form-input,.form-textarea,.form-select,.form-multiselect{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.form-input:focus,.form-textarea:focus,.form-select:focus,.form-multiselect:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.form-input::placeholder,.form-textarea::placeholder{color:#6b7280;opacity:1}.form-input::-webkit-datetime-edit-fields-wrapper{padding:0}.form-input::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.form-input::-webkit-datetime-edit{display:inline-flex}.form-input::-webkit-datetime-edit,.form-input::-webkit-datetime-edit-year-field,.form-input::-webkit-datetime-edit-month-field,.form-input::-webkit-datetime-edit-day-field,.form-input::-webkit-datetime-edit-hour-field,.form-input::-webkit-datetime-edit-minute-field,.form-input::-webkit-datetime-edit-second-field,.form-input::-webkit-datetime-edit-millisecond-field,.form-input::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.prose{color:var(--tw-prose-body);max-width:65ch}.prose :where(p):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em;margin-bottom:1.25em}.prose :where([class~=lead]):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-lead);font-size:1.25em;line-height:1.6;margin-top:1.2em;margin-bottom:1.2em}.prose :where(a):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-links);text-decoration:underline;font-weight:500}.prose :where(strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-bold);font-weight:600}.prose :where(a strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(blockquote strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(thead th strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(ol):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:decimal;margin-top:1.25em;margin-bottom:1.25em;padding-left:1.625em}.prose :where(ol[type=A]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-alpha}.prose :where(ol[type=a]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-alpha}.prose :where(ol[type=A s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-alpha}.prose :where(ol[type=a s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-alpha}.prose :where(ol[type=I]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-roman}.prose :where(ol[type=i]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-roman}.prose :where(ol[type=I s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-roman}.prose :where(ol[type=i s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-roman}.prose :where(ol[type="1"]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:decimal}.prose :where(ul):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:disc;margin-top:1.25em;margin-bottom:1.25em;padding-left:1.625em}.prose :where(ol>li):not(:where([class~=not-prose],[class~=not-prose] *))::marker{font-weight:400;color:var(--tw-prose-counters)}.prose :where(ul>li):not(:where([class~=not-prose],[class~=not-prose] *))::marker{color:var(--tw-prose-bullets)}.prose :where(dt):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;margin-top:1.25em}.prose :where(hr):not(:where([class~=not-prose],[class~=not-prose] *)){border-color:var(--tw-prose-hr);border-top-width:1px;margin-top:3em;margin-bottom:3em}.prose :where(blockquote):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:500;font-style:italic;color:var(--tw-prose-quotes);border-left-width:.25rem;border-left-color:var(--tw-prose-quote-borders);quotes:"“""”""‘""’";margin-top:1.6em;margin-bottom:1.6em;padding-left:1em}.prose :where(blockquote p:first-of-type):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:open-quote}.prose :where(blockquote p:last-of-type):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:close-quote}.prose :where(h1):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:800;font-size:2.25em;margin-top:0;margin-bottom:.8888889em;line-height:1.1111111}.prose :where(h1 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:900;color:inherit}.prose :where(h2):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:700;font-size:1.5em;margin-top:2em;margin-bottom:1em;line-height:1.3333333}.prose :where(h2 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:800;color:inherit}.prose :where(h3):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;font-size:1.25em;margin-top:1.6em;margin-bottom:.6em;line-height:1.6}.prose :where(h3 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:700;color:inherit}.prose :where(h4):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;margin-top:1.5em;margin-bottom:.5em;line-height:1.5}.prose :where(h4 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:700;color:inherit}.prose :where(img):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(picture):not(:where([class~=not-prose],[class~=not-prose] *)){display:block;margin-top:2em;margin-bottom:2em}.prose :where(kbd):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:500;font-family:inherit;color:var(--tw-prose-kbd);box-shadow:0 0 0 1px rgb(var(--tw-prose-kbd-shadows) / 10%),0 3px 0 rgb(var(--tw-prose-kbd-shadows) / 10%);font-size:.875em;border-radius:.3125rem;padding:.1875em .375em}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-code);font-weight:600;font-size:.875em}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:"`"}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:"`"}.prose :where(a code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(h1 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(h2 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit;font-size:.875em}.prose :where(h3 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit;font-size:.9em}.prose :where(h4 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(blockquote code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(thead th code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(pre):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-pre-code);background-color:var(--tw-prose-pre-bg);overflow-x:auto;font-weight:400;font-size:.875em;line-height:1.7142857;margin-top:1.7142857em;margin-bottom:1.7142857em;border-radius:.375rem;padding:.8571429em 1.1428571em}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)){background-color:transparent;border-width:0;border-radius:0;padding:0;font-weight:inherit;color:inherit;font-size:inherit;font-family:inherit;line-height:inherit}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:none}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:none}.prose :where(table):not(:where([class~=not-prose],[class~=not-prose] *)){width:100%;table-layout:auto;text-align:left;margin-top:2em;margin-bottom:2em;font-size:.875em;line-height:1.7142857}.prose :where(thead):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:1px;border-bottom-color:var(--tw-prose-th-borders)}.prose :where(thead th):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;vertical-align:bottom;padding-right:.5714286em;padding-bottom:.5714286em;padding-left:.5714286em}.prose :where(tbody tr):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:1px;border-bottom-color:var(--tw-prose-td-borders)}.prose :where(tbody tr:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:0}.prose :where(tbody td):not(:where([class~=not-prose],[class~=not-prose] *)){vertical-align:baseline}.prose :where(tfoot):not(:where([class~=not-prose],[class~=not-prose] *)){border-top-width:1px;border-top-color:var(--tw-prose-th-borders)}.prose :where(tfoot td):not(:where([class~=not-prose],[class~=not-prose] *)){vertical-align:top}.prose :where(figure>*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0;margin-bottom:0}.prose :where(figcaption):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-captions);font-size:.875em;line-height:1.4285714;margin-top:.8571429em}.prose{--tw-prose-body: #374151;--tw-prose-headings: #111827;--tw-prose-lead: #4b5563;--tw-prose-links: #111827;--tw-prose-bold: #111827;--tw-prose-counters: #6b7280;--tw-prose-bullets: #d1d5db;--tw-prose-hr: #e5e7eb;--tw-prose-quotes: #111827;--tw-prose-quote-borders: #e5e7eb;--tw-prose-captions: #6b7280;--tw-prose-kbd: #111827;--tw-prose-kbd-shadows: 17 24 39;--tw-prose-code: #111827;--tw-prose-pre-code: #e5e7eb;--tw-prose-pre-bg: #1f2937;--tw-prose-th-borders: #d1d5db;--tw-prose-td-borders: #e5e7eb;--tw-prose-invert-body: #d1d5db;--tw-prose-invert-headings: #fff;--tw-prose-invert-lead: #9ca3af;--tw-prose-invert-links: #fff;--tw-prose-invert-bold: #fff;--tw-prose-invert-counters: #9ca3af;--tw-prose-invert-bullets: #4b5563;--tw-prose-invert-hr: #374151;--tw-prose-invert-quotes: #f3f4f6;--tw-prose-invert-quote-borders: #374151;--tw-prose-invert-captions: #9ca3af;--tw-prose-invert-kbd: #fff;--tw-prose-invert-kbd-shadows: 255 255 255;--tw-prose-invert-code: #fff;--tw-prose-invert-pre-code: #d1d5db;--tw-prose-invert-pre-bg: rgb(0 0 0 / 50%);--tw-prose-invert-th-borders: #4b5563;--tw-prose-invert-td-borders: #374151;font-size:1rem;line-height:1.75}.prose :where(picture>img):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0;margin-bottom:0}.prose :where(video):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(li):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.5em;margin-bottom:.5em}.prose :where(ol>li):not(:where([class~=not-prose],[class~=not-prose] *)){padding-left:.375em}.prose :where(ul>li):not(:where([class~=not-prose],[class~=not-prose] *)){padding-left:.375em}.prose :where(.prose>ul>li p):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.75em;margin-bottom:.75em}.prose :where(.prose>ul>li>*:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em}.prose :where(.prose>ul>li>*:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:1.25em}.prose :where(.prose>ol>li>*:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em}.prose :where(.prose>ol>li>*:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:1.25em}.prose :where(ul ul,ul ol,ol ul,ol ol):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.75em;margin-bottom:.75em}.prose :where(dl):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em;margin-bottom:1.25em}.prose :where(dd):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.5em;padding-left:1.625em}.prose :where(hr+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h2+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h3+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h4+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(thead th:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-left:0}.prose :where(thead th:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-right:0}.prose :where(tbody td,tfoot td):not(:where([class~=not-prose],[class~=not-prose] *)){padding:.5714286em}.prose :where(tbody td:first-child,tfoot td:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-left:0}.prose :where(tbody td:last-child,tfoot td:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-right:0}.prose :where(figure):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(.prose>:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(.prose>:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:0}.alert{display:grid;width:100%;grid-auto-flow:row;align-content:flex-start;align-items:center;justify-items:center;gap:1rem;text-align:center;border-radius:var(--rounded-box, 1rem);border-width:1px;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)));padding:1rem;--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--alert-bg: var(--fallback-b2,oklch(var(--b2)/1));--alert-bg-mix: var(--fallback-b1,oklch(var(--b1)/1));background-color:var(--alert-bg)}@media (min-width: 640px){.alert{grid-auto-flow:column;grid-template-columns:auto minmax(auto,1fr);justify-items:start;text-align:start}}.avatar.placeholder>div{display:flex;align-items:center;justify-content:center}.badge{display:inline-flex;align-items:center;justify-content:center;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);transition-duration:.2s;height:1.25rem;font-size:.875rem;line-height:1.25rem;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;padding-left:.563rem;padding-right:.563rem;border-radius:var(--rounded-badge, 1.9rem);border-width:1px;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))}@media (hover:hover){.label a:hover{--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))}.menu li>*:not(ul):not(.menu-title):not(details):active,.menu li>*:not(ul):not(.menu-title):not(details).active,.menu li>details>summary:active{--tw-bg-opacity: 1;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-nc,oklch(var(--nc)/var(--tw-text-opacity)))}.tab:hover{--tw-text-opacity: 1}.table tr.hover:hover,.table tr.hover:nth-child(2n):hover{--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)))}.table-zebra tr.hover:hover,.table-zebra tr.hover:nth-child(2n):hover{--tw-bg-opacity: 1;background-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-bg-opacity)))}}.btn{display:inline-flex;height:3rem;min-height:3rem;flex-shrink:0;cursor:pointer;-webkit-user-select:none;user-select:none;flex-wrap:wrap;align-items:center;justify-content:center;border-radius:var(--rounded-btn, .5rem);border-color:transparent;border-color:oklch(var(--btn-color, var(--b2)) / var(--tw-border-opacity));padding-left:1rem;padding-right:1rem;text-align:center;font-size:.875rem;line-height:1em;gap:.5rem;font-weight:600;text-decoration-line:none;transition-duration:.2s;transition-timing-function:cubic-bezier(0,0,.2,1);border-width:var(--border-btn, 1px);animation:button-pop var(--animation-btn, .25s) ease-out;transition-property:color,background-color,border-color,opacity,box-shadow,transform;--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);outline-color:var(--fallback-bc,oklch(var(--bc)/1));background-color:oklch(var(--btn-color, var(--b2)) / var(--tw-bg-opacity));--tw-bg-opacity: 1;--tw-border-opacity: 1}.btn-disabled,.btn[disabled],.btn:disabled{pointer-events:none}:where(.btn:is(input[type=checkbox])),:where(.btn:is(input[type=radio])){width:auto;-webkit-appearance:none;-moz-appearance:none;appearance:none}.btn:is(input[type=checkbox]):after,.btn:is(input[type=radio]):after{--tw-content: attr(aria-label);content:var(--tw-content)}.card{position:relative;display:flex;flex-direction:column;border-radius:var(--rounded-box, 1rem)}.card:focus{outline:2px solid transparent;outline-offset:2px}.card figure{display:flex;align-items:center;justify-content:center}.card.image-full{display:grid}.card.image-full:before{position:relative;content:"";z-index:10;border-radius:var(--rounded-box, 1rem);--tw-bg-opacity: 1;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));opacity:.75}.card.image-full:before,.card.image-full>*{grid-column-start:1;grid-row-start:1}.card.image-full>figure img{height:100%;object-fit:cover}.card.image-full>.card-body{position:relative;z-index:20;--tw-text-opacity: 1;color:var(--fallback-nc,oklch(var(--nc)/var(--tw-text-opacity)))}.\!chat{display:grid!important;grid-template-columns:repeat(2,minmax(0,1fr))!important;column-gap:.75rem!important;padding-top:.25rem!important;padding-bottom:.25rem!important}.chat{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));column-gap:.75rem;padding-top:.25rem;padding-bottom:.25rem}.checkbox{flex-shrink:0;--chkbg: var(--fallback-bc,oklch(var(--bc)/1));--chkfg: var(--fallback-b1,oklch(var(--b1)/1));height:1.5rem;width:1.5rem;cursor:pointer;-webkit-appearance:none;-moz-appearance:none;appearance:none;border-radius:var(--rounded-btn, .5rem);border-width:1px;border-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-border-opacity)));--tw-border-opacity: .2}@media (hover: hover){.btm-nav>*.\!disabled:hover{pointer-events:none!important;--tw-border-opacity: 0 !important;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)))!important;--tw-bg-opacity: .1 !important;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))!important;--tw-text-opacity: .2 !important}.btm-nav>*.disabled:hover,.btm-nav>*[disabled]:hover{pointer-events:none;--tw-border-opacity: 0;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-bg-opacity: .1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}.btn:hover{--tw-border-opacity: 1;border-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-bg-opacity)))}@supports (color: color-mix(in oklab,black,black)){.btn:hover{background-color:color-mix(in oklab,oklch(var(--btn-color, var(--b2)) / var(--tw-bg-opacity, 1)) 90%,black);border-color:color-mix(in oklab,oklch(var(--btn-color, var(--b2)) / var(--tw-border-opacity, 1)) 90%,black)}}@supports not (color: oklch(0 0 0)){.btn:hover{background-color:var(--btn-color, var(--fallback-b2));border-color:var(--btn-color, var(--fallback-b2))}}.btn.glass:hover{--glass-opacity: 25%;--glass-border-opacity: 15%}.btn-disabled:hover,.btn[disabled]:hover,.btn:disabled:hover{--tw-border-opacity: 0;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-bg-opacity: .2;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}@supports (color: color-mix(in oklab,black,black)){.btn:is(input[type=checkbox]:checked):hover,.btn:is(input[type=radio]:checked):hover{background-color:color-mix(in oklab,var(--fallback-p,oklch(var(--p)/1)) 90%,black);border-color:color-mix(in oklab,var(--fallback-p,oklch(var(--p)/1)) 90%,black)}}:where(.menu li:not(.menu-title):not(.disabled)>*:not(ul):not(details):not(.menu-title)):not(.active):hover,:where(.menu li:not(.menu-title):not(.disabled)>details>summary:not(.menu-title)):not(.active):hover{cursor:pointer;outline:2px solid transparent;outline-offset:2px}@supports (color: oklch(0 0 0)){:where(.menu li:not(.menu-title):not(.disabled)>*:not(ul):not(details):not(.menu-title)):not(.active):hover,:where(.menu li:not(.menu-title):not(.disabled)>details>summary:not(.menu-title)):not(.active):hover{background-color:var(--fallback-bc,oklch(var(--bc)/.1))}}.tab[disabled],.tab[disabled]:hover{cursor:not-allowed;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}}.label{display:flex;-webkit-user-select:none;user-select:none;align-items:center;justify-content:space-between;padding:.5rem .25rem}.input{flex-shrink:1;-webkit-appearance:none;-moz-appearance:none;appearance:none;height:3rem;padding-left:1rem;padding-right:1rem;font-size:1rem;line-height:2;line-height:1.5rem;border-radius:var(--rounded-btn, .5rem);border-width:1px;border-color:transparent;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.join{display:inline-flex;align-items:stretch;border-radius:var(--rounded-btn, .5rem)}.join :where(.join-item){border-start-end-radius:0;border-end-end-radius:0;border-end-start-radius:0;border-start-start-radius:0}.join .join-item:not(:first-child):not(:last-child),.join *:not(:first-child):not(:last-child) .join-item{border-start-end-radius:0;border-end-end-radius:0;border-end-start-radius:0;border-start-start-radius:0}.join .join-item:first-child:not(:last-child),.join *:first-child:not(:last-child) .join-item{border-start-end-radius:0;border-end-end-radius:0}.join .dropdown .join-item:first-child:not(:last-child),.join *:first-child:not(:last-child) .dropdown .join-item{border-start-end-radius:inherit;border-end-end-radius:inherit}.join :where(.join-item:first-child:not(:last-child)),.join :where(*:first-child:not(:last-child) .join-item){border-end-start-radius:inherit;border-start-start-radius:inherit}.join .join-item:last-child:not(:first-child),.join *:last-child:not(:first-child) .join-item{border-end-start-radius:0;border-start-start-radius:0}.join :where(.join-item:last-child:not(:first-child)),.join :where(*:last-child:not(:first-child) .join-item){border-start-end-radius:inherit;border-end-end-radius:inherit}@supports not selector(:has(*)){:where(.join *){border-radius:inherit}}@supports selector(:has(*)){:where(.join *:has(.join-item)){border-radius:inherit}}.link{cursor:pointer;text-decoration-line:underline}.mask{-webkit-mask-size:contain;mask-size:contain;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-position:center;mask-position:center}.menu{display:flex;flex-direction:column;flex-wrap:wrap;font-size:.875rem;line-height:1.25rem;padding:.5rem}.menu :where(li ul){position:relative;white-space:nowrap;margin-inline-start:1rem;padding-inline-start:.5rem}.menu :where(li:not(.menu-title)>*:not(ul):not(details):not(.menu-title)),.menu :where(li:not(.menu-title)>details>summary:not(.menu-title)){display:grid;grid-auto-flow:column;align-content:flex-start;align-items:center;gap:.5rem;grid-auto-columns:minmax(auto,-webkit-max-content) auto -webkit-max-content;grid-auto-columns:minmax(auto,max-content) auto max-content;-webkit-user-select:none;user-select:none}.menu li.disabled{cursor:not-allowed;-webkit-user-select:none;user-select:none;color:var(--fallback-bc,oklch(var(--bc)/.3))}.menu li.\!disabled{cursor:not-allowed!important;-webkit-user-select:none!important;user-select:none!important;color:var(--fallback-bc,oklch(var(--bc)/.3))!important}.menu :where(li>.menu-dropdown:not(.menu-dropdown-show)){display:none}:where(.menu li){position:relative;display:flex;flex-shrink:0;flex-direction:column;flex-wrap:wrap;align-items:stretch}:where(.menu li) .badge{justify-self:end}.modal{pointer-events:none;position:fixed;top:0;right:0;bottom:0;left:0;margin:0;display:grid;height:100%;max-height:none;width:100%;max-width:none;justify-items:center;padding:0;opacity:0;overscroll-behavior:contain;z-index:999;background-color:transparent;color:inherit;transition-duration:.2s;transition-timing-function:cubic-bezier(0,0,.2,1);transition-property:transform,opacity,visibility;overflow-y:hidden}:where(.modal){align-items:center}.modal-open,.modal:target,.modal-toggle:checked+.modal,.modal[open]{pointer-events:auto;visibility:visible;opacity:1}:root:has(:is(.modal-open,.modal:target,.modal-toggle:checked+.modal,.modal[open])){overflow:hidden}.progress{position:relative;width:100%;-webkit-appearance:none;-moz-appearance:none;appearance:none;overflow:hidden;height:.5rem;border-radius:var(--rounded-box, 1rem);background-color:var(--fallback-bc,oklch(var(--bc)/.2))}.radial-progress{position:relative;display:inline-grid;height:var(--size);width:var(--size);place-content:center;border-radius:9999px;background-color:transparent;vertical-align:middle;box-sizing:content-box;--value: 0;--size: 5rem;--thickness: calc(var(--size) / 10)}.radial-progress::-moz-progress-bar{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:transparent}.radial-progress::-webkit-progress-value{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:transparent}.radial-progress::-webkit-progress-bar{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:transparent}.radial-progress:before,.radial-progress:after{position:absolute;border-radius:9999px;content:""}.radial-progress:before{top:0;right:0;bottom:0;left:0;background:radial-gradient(farthest-side,currentColor 98%,#0000) top/var(--thickness) var(--thickness) no-repeat,conic-gradient(currentColor calc(var(--value) * 1%),#0000 0);-webkit-mask:radial-gradient(farthest-side,#0000 calc(99% - var(--thickness)),#000 calc(100% - var(--thickness)));mask:radial-gradient(farthest-side,#0000 calc(99% - var(--thickness)),#000 calc(100% - var(--thickness)))}.radial-progress:after{inset:calc(50% - var(--thickness) / 2);transform:rotate(calc(var(--value) * 3.6deg - 90deg)) translate(calc(var(--size) / 2 - 50%));background-color:currentColor}.select{display:inline-flex;cursor:pointer;-webkit-user-select:none;user-select:none;-webkit-appearance:none;-moz-appearance:none;appearance:none;height:3rem;min-height:3rem;padding-left:1rem;padding-right:2.5rem;font-size:.875rem;line-height:1.25rem;line-height:2;border-radius:var(--rounded-btn, .5rem);border-width:1px;border-color:transparent;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)));background-image:linear-gradient(45deg,transparent 50%,currentColor 50%),linear-gradient(135deg,currentColor 50%,transparent 50%);background-position:calc(100% - 20px) calc(1px + 50%),calc(100% - 16.1px) calc(1px + 50%);background-size:4px 4px,4px 4px;background-repeat:no-repeat}.select[multiple]{height:auto}.stack{display:inline-grid;place-items:center;align-items:flex-end}.stack>*{grid-column-start:1;grid-row-start:1;transform:translateY(10%) scale(.9);z-index:1;width:100%;opacity:.6}.stack>*:nth-child(2){transform:translateY(5%) scale(.95);z-index:2;opacity:.8}.stack>*:nth-child(1){transform:translateY(0) scale(1);z-index:3;opacity:1}.steps .step{display:grid;grid-template-columns:repeat(1,minmax(0,1fr));grid-template-columns:auto;grid-template-rows:repeat(2,minmax(0,1fr));grid-template-rows:40px 1fr;place-items:center;text-align:center;min-width:4rem}.tabs{display:grid;align-items:flex-end}.tabs-lifted:has(.tab-content[class^=rounded-]) .tab:first-child:not(.tab-active),.tabs-lifted:has(.tab-content[class*=" rounded-"]) .tab:first-child:not(.tab-active){border-bottom-color:transparent}.tab{position:relative;grid-row-start:1;display:inline-flex;height:2rem;cursor:pointer;-webkit-user-select:none;user-select:none;-webkit-appearance:none;-moz-appearance:none;appearance:none;flex-wrap:wrap;align-items:center;justify-content:center;text-align:center;font-size:.875rem;line-height:1.25rem;line-height:2;--tab-padding: 1rem;--tw-text-opacity: .5;--tab-color: var(--fallback-bc,oklch(var(--bc)/1));--tab-bg: var(--fallback-b1,oklch(var(--b1)/1));--tab-border-color: var(--fallback-b3,oklch(var(--b3)/1));color:var(--tab-color);padding-inline-start:var(--tab-padding, 1rem);padding-inline-end:var(--tab-padding, 1rem)}.tab:is(input[type=radio]){width:auto;border-bottom-right-radius:0;border-bottom-left-radius:0}.tab:is(input[type=radio]):after{--tw-content: attr(aria-label);content:var(--tw-content)}.tab:not(input):empty{cursor:default;grid-column-start:span 9999}input.tab:checked+.tab-content,.tab-active+.tab-content{display:block}.table{position:relative;width:100%;border-radius:var(--rounded-box, 1rem);text-align:left;font-size:.875rem;line-height:1.25rem}.table :where(.table-pin-rows thead tr){position:-webkit-sticky;position:sticky;top:0;z-index:1;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.table :where(.table-pin-rows tfoot tr){position:-webkit-sticky;position:sticky;bottom:0;z-index:1;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.table :where(.table-pin-cols tr th){position:-webkit-sticky;position:sticky;left:0;right:0;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.textarea{min-height:3rem;flex-shrink:1;padding:.5rem 1rem;font-size:.875rem;line-height:1.25rem;line-height:2;border-radius:var(--rounded-btn, .5rem);border-width:1px;border-color:transparent;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.toggle{flex-shrink:0;--tglbg: var(--fallback-b1,oklch(var(--b1)/1));--handleoffset: 1.5rem;--handleoffsetcalculator: calc(var(--handleoffset) * -1);--togglehandleborder: 0 0;height:1.5rem;width:3rem;cursor:pointer;-webkit-appearance:none;-moz-appearance:none;appearance:none;border-radius:var(--rounded-badge, 1.9rem);border-width:1px;border-color:currentColor;background-color:currentColor;color:var(--fallback-bc,oklch(var(--bc)/.5));transition:background,box-shadow var(--animation-input, .2s) ease-out;box-shadow:var(--handleoffsetcalculator) 0 0 2px var(--tglbg) inset,0 0 0 2px var(--tglbg) inset,var(--togglehandleborder)}.btm-nav>*:where(.active){border-top-width:2px;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.btm-nav>*.\!disabled{pointer-events:none!important;--tw-border-opacity: 0 !important;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)))!important;--tw-bg-opacity: .1 !important;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))!important;--tw-text-opacity: .2 !important}.btm-nav>*.disabled,.btm-nav>*[disabled]{pointer-events:none;--tw-border-opacity: 0;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-bg-opacity: .1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}.btm-nav>* .label{font-size:1rem;line-height:1.5rem}.btn:active:hover,.btn:active:focus{animation:button-pop 0s ease-out;transform:scale(var(--btn-focus-scale, .97))}@supports not (color: oklch(0 0 0)){.btn{background-color:var(--btn-color, var(--fallback-b2));border-color:var(--btn-color, var(--fallback-b2))}.prose :where(code):not(:where([class~=not-prose] *,pre *)){background-color:var(--fallback-b3,oklch(var(--b3)/1))}}.btn:focus-visible{outline-style:solid;outline-width:2px;outline-offset:2px}.btn.glass{--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);outline-color:currentColor}.btn.glass.btn-active{--glass-opacity: 25%;--glass-border-opacity: 15%}.btn.btn-disabled,.btn[disabled],.btn:disabled{--tw-border-opacity: 0;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-bg-opacity: .2;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}.btn:is(input[type=checkbox]:checked),.btn:is(input[type=radio]:checked){--tw-border-opacity: 1;border-color:var(--fallback-p,oklch(var(--p)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-p,oklch(var(--p)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-pc,oklch(var(--pc)/var(--tw-text-opacity)))}.btn:is(input[type=checkbox]:checked):focus-visible,.btn:is(input[type=radio]:checked):focus-visible{outline-color:var(--fallback-p,oklch(var(--p)/1))}@keyframes button-pop{0%{transform:scale(var(--btn-focus-scale, .98))}40%{transform:scale(1.02)}to{transform:scale(1)}}.card :where(figure:first-child){overflow:hidden;border-start-start-radius:inherit;border-start-end-radius:inherit;border-end-start-radius:unset;border-end-end-radius:unset}.card :where(figure:last-child){overflow:hidden;border-start-start-radius:unset;border-start-end-radius:unset;border-end-start-radius:inherit;border-end-end-radius:inherit}.card:focus-visible{outline:2px solid currentColor;outline-offset:2px}.card.bordered{border-width:1px;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)))}.card.compact .card-body{padding:1rem;font-size:.875rem;line-height:1.25rem}.card.image-full :where(figure){overflow:hidden;border-radius:inherit}.checkbox:focus{box-shadow:none}.checkbox:focus-visible{outline-style:solid;outline-width:2px;outline-offset:2px;outline-color:var(--fallback-bc,oklch(var(--bc)/1))}.checkbox:checked,.checkbox[checked=true],.checkbox[aria-checked=true]{background-repeat:no-repeat;animation:checkmark var(--animation-input, .2s) ease-out;background-color:var(--chkbg);background-image:linear-gradient(-45deg,transparent 65%,var(--chkbg) 65.99%),linear-gradient(45deg,transparent 75%,var(--chkbg) 75.99%),linear-gradient(-45deg,var(--chkbg) 40%,transparent 40.99%),linear-gradient(45deg,var(--chkbg) 30%,var(--chkfg) 30.99%,var(--chkfg) 40%,transparent 40.99%),linear-gradient(-45deg,var(--chkfg) 50%,var(--chkbg) 50.99%)}.checkbox:indeterminate{--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)));background-repeat:no-repeat;animation:checkmark var(--animation-input, .2s) ease-out;background-image:linear-gradient(90deg,transparent 80%,var(--chkbg) 80%),linear-gradient(-90deg,transparent 80%,var(--chkbg) 80%),linear-gradient(0deg,var(--chkbg) 43%,var(--chkfg) 43%,var(--chkfg) 57%,var(--chkbg) 57%)}.checkbox:disabled{cursor:not-allowed;border-color:transparent;--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)));opacity:.2}@keyframes checkmark{0%{background-position-y:5px}50%{background-position-y:-2px}to{background-position-y:0}}.input input:focus{outline:2px solid transparent;outline-offset:2px}.input[list]::-webkit-calendar-picker-indicator{line-height:1em}.input:focus,.input:focus-within{box-shadow:none;border-color:var(--fallback-bc,oklch(var(--bc)/.2));outline-style:solid;outline-width:2px;outline-offset:2px;outline-color:var(--fallback-bc,oklch(var(--bc)/.2))}.input-disabled,.input:disabled,.input[disabled]{cursor:not-allowed;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)));color:var(--fallback-bc,oklch(var(--bc)/.4))}.input-disabled::placeholder,.input:disabled::placeholder,.input[disabled]::placeholder{color:var(--fallback-bc,oklch(var(--bc)/var(--tw-placeholder-opacity)));--tw-placeholder-opacity: .2}.input::-webkit-date-and-time-value{text-align:inherit}.join>:where(*:not(:first-child)){margin-top:0;margin-bottom:0;margin-inline-start:-1px}.link:focus{outline:2px solid transparent;outline-offset:2px}.link:focus-visible{outline:2px solid currentColor;outline-offset:2px}.\!loading{pointer-events:none!important;display:inline-block!important;aspect-ratio:1 / 1!important;width:1.5rem!important;background-color:currentColor!important;-webkit-mask-size:100%!important;mask-size:100%!important;-webkit-mask-repeat:no-repeat!important;mask-repeat:no-repeat!important;-webkit-mask-position:center!important;mask-position:center!important;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important;mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important}.loading{pointer-events:none;display:inline-block;aspect-ratio:1 / 1;width:1.5rem;background-color:currentColor;-webkit-mask-size:100%;mask-size:100%;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-position:center;mask-position:center;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}.loading-spinner{-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}.loading-sm{width:1.25rem}:where(.menu li:empty){--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)));opacity:.1;margin:.5rem 1rem;height:1px}.menu :where(li ul):before{position:absolute;bottom:.75rem;inset-inline-start:0px;top:.75rem;width:1px;--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)));opacity:.1;content:""}.menu :where(li:not(.menu-title)>*:not(ul):not(details):not(.menu-title)),.menu :where(li:not(.menu-title)>details>summary:not(.menu-title)){border-radius:var(--rounded-btn, .5rem);padding:.5rem 1rem;text-align:start;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);transition-duration:.2s;text-wrap:balance}:where(.menu li:not(.menu-title):not(.disabled)>*:not(ul):not(details):not(.menu-title)):not(summary):not(.active).focus,:where(.menu li:not(.menu-title):not(.disabled)>*:not(ul):not(details):not(.menu-title)):not(summary):not(.active):focus,:where(.menu li:not(.menu-title):not(.disabled)>*:not(ul):not(details):not(.menu-title)):is(summary):not(.active):focus-visible,:where(.menu li:not(.menu-title):not(.disabled)>details>summary:not(.menu-title)):not(summary):not(.active).focus,:where(.menu li:not(.menu-title):not(.disabled)>details>summary:not(.menu-title)):not(summary):not(.active):focus,:where(.menu li:not(.menu-title):not(.disabled)>details>summary:not(.menu-title)):is(summary):not(.active):focus-visible{cursor:pointer;background-color:var(--fallback-bc,oklch(var(--bc)/.1));--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));outline:2px solid transparent;outline-offset:2px}.menu li>*:not(ul):not(.menu-title):not(details):active,.menu li>*:not(ul):not(.menu-title):not(details).active,.menu li>details>summary:active{--tw-bg-opacity: 1;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-nc,oklch(var(--nc)/var(--tw-text-opacity)))}.menu :where(li>details>summary)::-webkit-details-marker{display:none}.menu :where(li>details>summary):after,.menu :where(li>.menu-dropdown-toggle):after{justify-self:end;display:block;margin-top:-.5rem;height:.5rem;width:.5rem;transform:rotate(45deg);transition-property:transform,margin-top;transition-duration:.3s;transition-timing-function:cubic-bezier(.4,0,.2,1);content:"";transform-origin:75% 75%;box-shadow:2px 2px;pointer-events:none}.menu :where(li>details[open]>summary):after,.menu :where(li>.menu-dropdown-toggle.menu-dropdown-show):after{transform:rotate(225deg);margin-top:0}.mockup-phone .display{overflow:hidden;border-radius:40px;margin-top:-25px}.mockup-browser .mockup-browser-toolbar .input{position:relative;margin-left:auto;margin-right:auto;display:block;height:1.75rem;width:24rem;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)));padding-left:2rem;direction:ltr}.mockup-browser .mockup-browser-toolbar .input:before{content:"";position:absolute;left:.5rem;top:50%;aspect-ratio:1 / 1;height:.75rem;--tw-translate-y: -50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));border-radius:9999px;border-width:2px;border-color:currentColor;opacity:.6}.mockup-browser .mockup-browser-toolbar .input:after{content:"";position:absolute;left:1.25rem;top:50%;height:.5rem;--tw-translate-y: 25%;--tw-rotate: -45deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));border-radius:9999px;border-width:1px;border-color:currentColor;opacity:.6}.modal:not(dialog:not(.modal-open)),.modal::backdrop{background-color:#0006;animation:modal-pop .2s ease-out}.modal-open .modal-box,.modal-toggle:checked+.modal .modal-box,.modal:target .modal-box,.modal[open] .modal-box{--tw-translate-y: 0px;--tw-scale-x: 1;--tw-scale-y: 1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@keyframes modal-pop{0%{opacity:0}}.progress::-moz-progress-bar{border-radius:var(--rounded-box, 1rem);--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)))}.progress:indeterminate{--progress-color: var(--fallback-bc,oklch(var(--bc)/1));background-image:repeating-linear-gradient(90deg,var(--progress-color) -1%,var(--progress-color) 10%,transparent 10%,transparent 90%);background-size:200%;background-position-x:15%;animation:progress-loading 5s ease-in-out infinite}.progress::-webkit-progress-bar{border-radius:var(--rounded-box, 1rem);background-color:transparent}.progress::-webkit-progress-value{border-radius:var(--rounded-box, 1rem);--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)))}.progress:indeterminate::-moz-progress-bar{background-color:transparent;background-image:repeating-linear-gradient(90deg,var(--progress-color) -1%,var(--progress-color) 10%,transparent 10%,transparent 90%);background-size:200%;background-position-x:15%;animation:progress-loading 5s ease-in-out infinite}@keyframes progress-loading{50%{background-position-x:-115%}}@keyframes radiomark{0%{box-shadow:0 0 0 12px var(--fallback-b1,oklch(var(--b1)/1)) inset,0 0 0 12px var(--fallback-b1,oklch(var(--b1)/1)) inset}50%{box-shadow:0 0 0 3px var(--fallback-b1,oklch(var(--b1)/1)) inset,0 0 0 3px var(--fallback-b1,oklch(var(--b1)/1)) inset}to{box-shadow:0 0 0 4px var(--fallback-b1,oklch(var(--b1)/1)) inset,0 0 0 4px var(--fallback-b1,oklch(var(--b1)/1)) inset}}@keyframes rating-pop{0%{transform:translateY(-.125em)}40%{transform:translateY(-.125em)}to{transform:translateY(0)}}.select:focus{box-shadow:none;border-color:var(--fallback-bc,oklch(var(--bc)/.2));outline-style:solid;outline-width:2px;outline-offset:2px;outline-color:var(--fallback-bc,oklch(var(--bc)/.2))}.select-disabled,.select:disabled,.select[disabled]{cursor:not-allowed;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)));color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}.select-disabled::placeholder,.select:disabled::placeholder,.select[disabled]::placeholder{color:var(--fallback-bc,oklch(var(--bc)/var(--tw-placeholder-opacity)));--tw-placeholder-opacity: .2}.select-multiple,.select[multiple],.select[size].select:not([size="1"]){background-image:none;padding-right:1rem}[dir=rtl] .select{background-position:calc(0% + 12px) calc(1px + 50%),calc(0% + 16px) calc(1px + 50%)}@keyframes skeleton{0%{background-position:150%}to{background-position:-50%}}.steps .step:before{top:0;grid-column-start:1;grid-row-start:1;height:.5rem;width:100%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));--tw-bg-opacity: 1;background-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));content:"";margin-inline-start:-100%}.steps .step:after{content:counter(step);counter-increment:step;z-index:1;position:relative;grid-column-start:1;grid-row-start:1;display:grid;height:2rem;width:2rem;place-items:center;place-self:center;border-radius:9999px;--tw-bg-opacity: 1;background-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))}.steps .step:first-child:before{content:none}.steps .step[data-content]:after{content:attr(data-content)}.tabs-lifted>.tab:focus-visible{border-end-end-radius:0;border-end-start-radius:0}.tab.tab-active:not(.tab-disabled):not([disabled]),.tab:is(input:checked){border-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-border-opacity)));--tw-border-opacity: 1;--tw-text-opacity: 1}.tab:focus{outline:2px solid transparent;outline-offset:2px}.tab:focus-visible{outline:2px solid currentColor;outline-offset:-5px}.tab-disabled,.tab[disabled]{cursor:not-allowed;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}.tabs-bordered>.tab{border-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-border-opacity)));--tw-border-opacity: .2;border-style:solid;border-bottom-width:calc(var(--tab-border, 1px) + 1px)}.tabs-lifted>.tab{border:var(--tab-border, 1px) solid transparent;border-width:0 0 var(--tab-border, 1px) 0;border-start-start-radius:var(--tab-radius, .5rem);border-start-end-radius:var(--tab-radius, .5rem);border-bottom-color:var(--tab-border-color);padding-inline-start:var(--tab-padding, 1rem);padding-inline-end:var(--tab-padding, 1rem);padding-top:var(--tab-border, 1px)}.tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]),.tabs-lifted>.tab:is(input:checked){background-color:var(--tab-bg);border-width:var(--tab-border, 1px) var(--tab-border, 1px) 0 var(--tab-border, 1px);border-inline-start-color:var(--tab-border-color);border-inline-end-color:var(--tab-border-color);border-top-color:var(--tab-border-color);padding-inline-start:calc(var(--tab-padding, 1rem) - var(--tab-border, 1px));padding-inline-end:calc(var(--tab-padding, 1rem) - var(--tab-border, 1px));padding-bottom:var(--tab-border, 1px);padding-top:0}.tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]):before,.tabs-lifted>.tab:is(input:checked):before{z-index:1;content:"";display:block;position:absolute;width:calc(100% + var(--tab-radius, .5rem) * 2);height:var(--tab-radius, .5rem);bottom:0;background-size:var(--tab-radius, .5rem);background-position:top left,top right;background-repeat:no-repeat;--tab-grad: calc(69% - var(--tab-border, 1px));--radius-start: radial-gradient( circle at top left, transparent var(--tab-grad), var(--tab-border-color) calc(var(--tab-grad) + .25px), var(--tab-border-color) calc(var(--tab-grad) + var(--tab-border, 1px)), var(--tab-bg) calc(var(--tab-grad) + var(--tab-border, 1px) + .25px) );--radius-end: radial-gradient( circle at top right, transparent var(--tab-grad), var(--tab-border-color) calc(var(--tab-grad) + .25px), var(--tab-border-color) calc(var(--tab-grad) + var(--tab-border, 1px)), var(--tab-bg) calc(var(--tab-grad) + var(--tab-border, 1px) + .25px) );background-image:var(--radius-start),var(--radius-end)}.tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]):first-child:before,.tabs-lifted>.tab:is(input:checked):first-child:before{background-image:var(--radius-end);background-position:top right}[dir=rtl] .tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]):first-child:before,[dir=rtl] .tabs-lifted>.tab:is(input:checked):first-child:before{background-image:var(--radius-start);background-position:top left}.tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]):last-child:before,.tabs-lifted>.tab:is(input:checked):last-child:before{background-image:var(--radius-start);background-position:top left}[dir=rtl] .tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]):last-child:before,[dir=rtl] .tabs-lifted>.tab:is(input:checked):last-child:before{background-image:var(--radius-end);background-position:top right}.tabs-lifted>.tab-active:not(.tab-disabled):not([disabled])+.tabs-lifted .tab-active:not(.tab-disabled):not([disabled]):before,.tabs-lifted>.tab:is(input:checked)+.tabs-lifted .tab:is(input:checked):before{background-image:var(--radius-end);background-position:top right}.tabs-boxed .tab{border-radius:var(--rounded-btn, .5rem)}:is([dir=rtl] .table){text-align:right}.table :where(th,td){padding:.75rem 1rem;vertical-align:middle}.table tr.active,.table tr.active:nth-child(2n),.table-zebra tbody tr:nth-child(2n){--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)))}.table-zebra tr.active,.table-zebra tr.active:nth-child(2n),.table-zebra-zebra tbody tr:nth-child(2n){--tw-bg-opacity: 1;background-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-bg-opacity)))}.table :where(thead,tbody) :where(tr:not(:last-child)),.table :where(thead,tbody) :where(tr:first-child:last-child){border-bottom-width:1px;--tw-border-opacity: 1;border-bottom-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)))}.table :where(thead,tfoot){white-space:nowrap;font-size:.75rem;line-height:1rem;font-weight:700;color:var(--fallback-bc,oklch(var(--bc)/.6))}.textarea:focus{box-shadow:none;border-color:var(--fallback-bc,oklch(var(--bc)/.2));outline-style:solid;outline-width:2px;outline-offset:2px;outline-color:var(--fallback-bc,oklch(var(--bc)/.2))}.textarea-primary{--tw-border-opacity: 1;border-color:var(--fallback-p,oklch(var(--p)/var(--tw-border-opacity)))}.textarea-primary:focus{--tw-border-opacity: 1;border-color:var(--fallback-p,oklch(var(--p)/var(--tw-border-opacity)));outline-color:var(--fallback-p,oklch(var(--p)/1))}.textarea-disabled,.textarea:disabled,.textarea[disabled]{cursor:not-allowed;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)));--tw-text-opacity: .2}.textarea-disabled::placeholder,.textarea:disabled::placeholder,.textarea[disabled]::placeholder{color:var(--fallback-bc,oklch(var(--bc)/var(--tw-placeholder-opacity)));--tw-placeholder-opacity: .2}@keyframes toast-pop{0%{transform:scale(.9);opacity:0}to{transform:scale(1);opacity:1}}[dir=rtl] .toggle{--handleoffsetcalculator: calc(var(--handleoffset) * 1)}.toggle:focus-visible{outline-style:solid;outline-width:2px;outline-offset:2px;outline-color:var(--fallback-bc,oklch(var(--bc)/.2))}.toggle:hover{background-color:currentColor}.toggle:checked,.toggle[checked=true],.toggle[aria-checked=true]{background-image:none;--handleoffsetcalculator: var(--handleoffset);--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))}[dir=rtl] .toggle:checked,[dir=rtl] .toggle[checked=true],[dir=rtl] .toggle[aria-checked=true]{--handleoffsetcalculator: calc(var(--handleoffset) * -1)}.toggle:indeterminate{--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));box-shadow:calc(var(--handleoffset) / 2) 0 0 2px var(--tglbg) inset,calc(var(--handleoffset) / -2) 0 0 2px var(--tglbg) inset,0 0 0 2px var(--tglbg) inset}[dir=rtl] .toggle:indeterminate{box-shadow:calc(var(--handleoffset) / 2) 0 0 2px var(--tglbg) inset,calc(var(--handleoffset) / -2) 0 0 2px var(--tglbg) inset,0 0 0 2px var(--tglbg) inset}.toggle:disabled{cursor:not-allowed;--tw-border-opacity: 1;border-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-border-opacity)));background-color:transparent;opacity:.3;--togglehandleborder: 0 0 0 3px var(--fallback-bc,oklch(var(--bc)/1)) inset, var(--handleoffsetcalculator) 0 0 3px var(--fallback-bc,oklch(var(--bc)/1)) inset}:root .prose{--tw-prose-body: var(--fallback-bc,oklch(var(--bc)/.8));--tw-prose-headings: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-lead: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-links: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-bold: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-counters: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-bullets: var(--fallback-bc,oklch(var(--bc)/.5));--tw-prose-hr: var(--fallback-bc,oklch(var(--bc)/.2));--tw-prose-quotes: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-quote-borders: var(--fallback-bc,oklch(var(--bc)/.2));--tw-prose-captions: var(--fallback-bc,oklch(var(--bc)/.5));--tw-prose-code: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-pre-code: var(--fallback-nc,oklch(var(--nc)/1));--tw-prose-pre-bg: var(--fallback-n,oklch(var(--n)/1));--tw-prose-th-borders: var(--fallback-bc,oklch(var(--bc)/.5));--tw-prose-td-borders: var(--fallback-bc,oklch(var(--bc)/.2))}.prose :where(code):not(:where([class~=not-prose] *,pre *)){padding:1px 8px;border-radius:var(--rounded-badge);font-weight:initial;background-color:var(--fallback-bc,oklch(var(--bc)/.1))}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):before,.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):after{display:none}.prose pre code{border-radius:0;padding:0}.prose :where(tbody tr,thead):not(:where([class~=not-prose] *)){border-bottom-color:var(--fallback-bc,oklch(var(--bc)/.2))}.artboard.phone-1.horizontal,.artboard.phone-1.artboard-horizontal{width:568px;height:320px}.artboard.phone-2.horizontal,.artboard.phone-2.artboard-horizontal{width:667px;height:375px}.artboard.phone-3.horizontal,.artboard.phone-3.artboard-horizontal{width:736px;height:414px}.artboard.phone-4.horizontal,.artboard.phone-4.artboard-horizontal{width:812px;height:375px}.artboard.phone-5.horizontal,.artboard.phone-5.artboard-horizontal{width:896px;height:414px}.artboard.phone-6.horizontal,.artboard.phone-6.artboard-horizontal{width:1024px;height:320px}.btm-nav-xs>*:where(.active){border-top-width:1px}.btm-nav-sm>*:where(.active){border-top-width:2px}.btm-nav-md>*:where(.active){border-top-width:2px}.btm-nav-lg>*:where(.active){border-top-width:4px}.join.join-vertical{flex-direction:column}.join.join-vertical .join-item:first-child:not(:last-child),.join.join-vertical *:first-child:not(:last-child) .join-item{border-end-start-radius:0;border-end-end-radius:0;border-start-start-radius:inherit;border-start-end-radius:inherit}.join.join-vertical .join-item:last-child:not(:first-child),.join.join-vertical *:last-child:not(:first-child) .join-item{border-start-start-radius:0;border-start-end-radius:0;border-end-start-radius:inherit;border-end-end-radius:inherit}.join.join-horizontal{flex-direction:row}.join.join-horizontal .join-item:first-child:not(:last-child),.join.join-horizontal *:first-child:not(:last-child) .join-item{border-end-end-radius:0;border-start-end-radius:0;border-end-start-radius:inherit;border-start-start-radius:inherit}.join.join-horizontal .join-item:last-child:not(:first-child),.join.join-horizontal *:last-child:not(:first-child) .join-item{border-end-start-radius:0;border-start-start-radius:0;border-end-end-radius:inherit;border-start-end-radius:inherit}.steps-horizontal .step{display:grid;grid-template-columns:repeat(1,minmax(0,1fr));grid-template-rows:repeat(2,minmax(0,1fr));place-items:center;text-align:center}.steps-vertical .step{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));grid-template-rows:repeat(1,minmax(0,1fr))}.tabs-md :where(.tab){height:2rem;font-size:.875rem;line-height:1.25rem;line-height:2;--tab-padding: 1rem}.tabs-lg :where(.tab){height:3rem;font-size:1.125rem;line-height:1.75rem;line-height:2;--tab-padding: 1.25rem}.tabs-sm :where(.tab){height:1.5rem;font-size:.875rem;line-height:.75rem;--tab-padding: .75rem}.tabs-xs :where(.tab){height:1.25rem;font-size:.75rem;line-height:.75rem;--tab-padding: .5rem}.tooltip{position:relative;display:inline-block;--tooltip-offset: calc(100% + 1px + var(--tooltip-tail, 0px))}.tooltip:before{position:absolute;pointer-events:none;z-index:1;content:var(--tw-content);--tw-content: attr(data-tip)}.tooltip:before,.tooltip-top:before{transform:translate(-50%);top:auto;left:50%;right:auto;bottom:var(--tooltip-offset)}.join.join-vertical>:where(*:not(:first-child)){margin-left:0;margin-right:0;margin-top:-1px}.join.join-horizontal>:where(*:not(:first-child)){margin-top:0;margin-bottom:0;margin-inline-start:-1px}.steps-horizontal .step{grid-template-rows:40px 1fr;grid-template-columns:auto;min-width:4rem}.steps-horizontal .step:before{height:.5rem;width:100%;--tw-translate-x: 0px;--tw-translate-y: 0px;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));content:"";margin-inline-start:-100%}:is([dir=rtl] .steps-horizontal .step):before{--tw-translate-x: 0px;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.steps-vertical .step{gap:.5rem;grid-template-columns:40px 1fr;grid-template-rows:auto;min-height:4rem;justify-items:start}.steps-vertical .step:before{height:100%;width:.5rem;--tw-translate-x: -50%;--tw-translate-y: -50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));margin-inline-start:50%}:is([dir=rtl] .steps-vertical .step):before{--tw-translate-x: 50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.tooltip{position:relative;display:inline-block;text-align:center;--tooltip-tail: .1875rem;--tooltip-color: var(--fallback-n,oklch(var(--n)/1));--tooltip-text-color: var(--fallback-nc,oklch(var(--nc)/1));--tooltip-tail-offset: calc(100% + .0625rem - var(--tooltip-tail))}.tooltip:before,.tooltip:after{opacity:0;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-delay:.1s;transition-duration:.2s;transition-timing-function:cubic-bezier(.4,0,.2,1)}.tooltip:after{position:absolute;content:"";border-style:solid;border-width:var(--tooltip-tail, 0);width:0;height:0;display:block}.tooltip:before{max-width:20rem;border-radius:.25rem;padding:.25rem .5rem;font-size:.875rem;line-height:1.25rem;background-color:var(--tooltip-color);color:var(--tooltip-text-color);width:-webkit-max-content;width:max-content}.tooltip.tooltip-open:before{opacity:1;transition-delay:75ms}.tooltip.tooltip-open:after{opacity:1;transition-delay:75ms}.tooltip:hover:before{opacity:1;transition-delay:75ms}.tooltip:hover:after{opacity:1;transition-delay:75ms}.tooltip:has(:focus-visible):after,.tooltip:has(:focus-visible):before{opacity:1;transition-delay:75ms}.tooltip:not([data-tip]):hover:before,.tooltip:not([data-tip]):hover:after{visibility:hidden;opacity:0}.tooltip:after,.tooltip-top:after{transform:translate(-50%);border-color:var(--tooltip-color) transparent transparent transparent;top:auto;left:50%;right:auto;bottom:var(--tooltip-tail-offset)}.side-bar-arrangement{display:flex;height:100%;width:14.5rem;flex-direction:column;overflow:hidden;border-right-width:1px;-ms-overflow-style:none;scrollbar-width:none}.side-bar-arrangement::-webkit-scrollbar{display:none}.side-bar-search-div-placement{position:relative;margin-left:auto;margin-right:auto;margin-bottom:.5rem;margin-top:.5rem;display:flex;align-items:center}.side-bar-components-icon{height:1.5rem;width:1rem;color:hsl(var(--ring))}.side-bar-components-text{width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;padding-right:.25rem;font-size:.75rem;line-height:1rem;color:hsl(var(--foreground))}.side-bar-components-div-form{display:flex;width:100%;align-items:center;justify-content:space-between;border-radius:calc(var(--radius) - 2px);border-top-left-radius:0;border-bottom-left-radius:0;border-width:1px;border-left-width:0px;border-style:dashed;border-color:hsl(var(--ring));background-color:var(--white);padding:.25rem .75rem;font-size:.875rem;line-height:1.25rem}.side-bar-components-border{cursor:grab;border-top-left-radius:calc(var(--radius) - 2px);border-bottom-left-radius:calc(var(--radius) - 2px);border-left-width:8px}.side-bar-components-gap{display:flex;flex-direction:column;gap:.5rem;padding:.5rem}.side-bar-components-div-arrangement{width:100%;overflow:auto;padding-bottom:2.5rem;-ms-overflow-style:none;scrollbar-width:none}.side-bar-components-div-arrangement::-webkit-scrollbar{display:none}.search-icon{position:absolute;top:0;bottom:0;right:0;display:flex;align-items:center;padding-top:.375rem;padding-bottom:.375rem;padding-right:1.25rem}.extra-side-bar-save-disable{color:hsl(var(--muted-foreground))}.extra-side-bar-save-disable:hover:hover{color:hsl(var(--accent-foreground))}.side-bar-button-size{height:1.25rem;width:1.25rem}.side-bar-button-size:hover:hover{color:hsl(var(--accent-foreground))}.side-bar-buttons-arrangement{margin-bottom:.5rem;margin-top:.5rem;display:flex;width:100%;align-items:center;justify-content:space-between;gap:.5rem;padding-left:.5rem;padding-right:.5rem}.side-bar-button{display:flex;width:100%}.button-disable{pointer-events:none}.extra-side-bar-buttons{position:relative;display:inline-flex;width:100%;align-items:center;justify-content:center;border-radius:calc(var(--radius) - 2px);background-color:hsl(var(--background));padding:.5rem;color:hsl(var(--foreground));--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);--tw-ring-inset: inset;--tw-ring-color: hsl(var(--input));transition-property:all;transition-duration:.5s;transition-timing-function:cubic-bezier(.4,0,.2,1);animation-duration:.5s;animation-timing-function:cubic-bezier(.4,0,.2,1)}.extra-side-bar-buttons:hover:hover{background-color:hsl(var(--muted))}.primary-input{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.primary-input:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.primary-input::placeholder{color:#6b7280;opacity:1}.primary-input::-webkit-datetime-edit-fields-wrapper{padding:0}.primary-input::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.primary-input::-webkit-datetime-edit{display:inline-flex}.primary-input::-webkit-datetime-edit,.primary-input::-webkit-datetime-edit-year-field,.primary-input::-webkit-datetime-edit-month-field,.primary-input::-webkit-datetime-edit-day-field,.primary-input::-webkit-datetime-edit-hour-field,.primary-input::-webkit-datetime-edit-minute-field,.primary-input::-webkit-datetime-edit-second-field,.primary-input::-webkit-datetime-edit-millisecond-field,.primary-input::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.primary-input{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;font-size:.875rem;line-height:1.25rem;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.primary-input::placeholder{color:hsl(var(--muted-foreground))}.primary-input:focus{border-color:hsl(var(--ring))}.primary-input:focus::placeholder{color:transparent}.primary-input:focus{--tw-ring-color: hsl(var(--ring))}.primary-input:disabled{cursor:not-allowed;opacity:.5}.skeleton-card{display:flex;height:12rem;flex-direction:column;gap:1.5rem;border-radius:var(--radius);border-width:1px;background-color:hsl(var(--background));padding:1rem}.skeleton-card-wrapper{display:flex;align-items:center}.skeleton-card-wrapper>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(1rem * var(--tw-space-x-reverse));margin-left:calc(1rem * calc(1 - var(--tw-space-x-reverse)))}.skeleton-card-text{display:flex;flex-direction:column;gap:.75rem}.textarea-primary{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.textarea-primary:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.textarea-primary::placeholder{color:#6b7280;opacity:1}.textarea-primary::-webkit-datetime-edit-fields-wrapper{padding:0}.textarea-primary::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.textarea-primary::-webkit-datetime-edit{display:inline-flex}.textarea-primary::-webkit-datetime-edit,.textarea-primary::-webkit-datetime-edit-year-field,.textarea-primary::-webkit-datetime-edit-month-field,.textarea-primary::-webkit-datetime-edit-day-field,.textarea-primary::-webkit-datetime-edit-hour-field,.textarea-primary::-webkit-datetime-edit-minute-field,.textarea-primary::-webkit-datetime-edit-second-field,.textarea-primary::-webkit-datetime-edit-millisecond-field,.textarea-primary::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.textarea-primary{display:block;width:100%;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.textarea-primary::placeholder{color:hsl(var(--muted-foreground))}.textarea-primary:focus{border-color:hsl(var(--ring))}.textarea-primary:focus::placeholder{color:transparent}.textarea-primary:focus{--tw-ring-color: hsl(var(--ring))}.textarea-primary:disabled{cursor:not-allowed;opacity:.5}@media (min-width: 640px){.textarea-primary{font-size:.875rem;line-height:1.25rem}}.input-edit-node{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.input-edit-node:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.input-edit-node::placeholder{color:#6b7280;opacity:1}.input-edit-node::-webkit-datetime-edit-fields-wrapper{padding:0}.input-edit-node::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.input-edit-node::-webkit-datetime-edit{display:inline-flex}.input-edit-node::-webkit-datetime-edit,.input-edit-node::-webkit-datetime-edit-year-field,.input-edit-node::-webkit-datetime-edit-month-field,.input-edit-node::-webkit-datetime-edit-day-field,.input-edit-node::-webkit-datetime-edit-hour-field,.input-edit-node::-webkit-datetime-edit-minute-field,.input-edit-node::-webkit-datetime-edit-second-field,.input-edit-node::-webkit-datetime-edit-millisecond-field,.input-edit-node::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.input-edit-node{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;font-size:.875rem;line-height:1.25rem;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.input-edit-node::placeholder{color:hsl(var(--muted-foreground))}.input-edit-node:focus{border-color:hsl(var(--ring))}.input-edit-node:focus::placeholder{color:transparent}.input-edit-node:focus{--tw-ring-color: hsl(var(--ring))}.input-edit-node:disabled{cursor:not-allowed;opacity:.5}.input-edit-node{width:100%;padding-bottom:.125rem;padding-top:.125rem;text-align:left}.input-search{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.input-search:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.input-search::placeholder{color:#6b7280;opacity:1}.input-search::-webkit-datetime-edit-fields-wrapper{padding:0}.input-search::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.input-search::-webkit-datetime-edit{display:inline-flex}.input-search::-webkit-datetime-edit,.input-search::-webkit-datetime-edit-year-field,.input-search::-webkit-datetime-edit-month-field,.input-search::-webkit-datetime-edit-day-field,.input-search::-webkit-datetime-edit-hour-field,.input-search::-webkit-datetime-edit-minute-field,.input-search::-webkit-datetime-edit-second-field,.input-search::-webkit-datetime-edit-millisecond-field,.input-search::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.input-search{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;font-size:.875rem;line-height:1.25rem;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.input-search::placeholder{color:hsl(var(--muted-foreground))}.input-search:focus{border-color:hsl(var(--ring))}.input-search:focus::placeholder{color:transparent}.input-search:focus{--tw-ring-color: hsl(var(--ring))}.input-search:disabled{cursor:not-allowed;opacity:.5}.input-search{margin-left:.5rem;margin-right:.5rem;padding-right:1.75rem}.input-disable{border-color:transparent;background-color:hsl(var(--border))}.input-disable::placeholder{color:hsl(var(--ring))}.input-dialog{cursor:pointer;background-color:transparent;color:hsl(var(--ring))}.message-button{position:fixed;bottom:1rem;right:1rem;display:flex;height:3rem;width:3rem;align-items:center;justify-content:center;border-radius:9999px;background-color:hsl(var(--border));padding:.25rem .75rem;--tw-shadow: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.round-button-form{display:flex;height:3rem;width:3rem;cursor:pointer;justify-content:center;border-radius:9999px;background-color:hsl(var(--border));padding:.25rem .75rem;--tw-shadow: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.round-button-div{display:flex;align-items:center;gap:.75rem}.build-trigger-loading-icon{stroke:var(--build-trigger)}.message-button-icon{fill:var(--chat-trigger);stroke:var(--chat-trigger);stroke-width:1}.disabled-message-button-icon{fill:var(--chat-trigger-disabled);stroke:var(--chat-trigger-disabled);stroke-width:1}.components-disclosure-arrangement{margin-top:-1px;display:flex;width:100%;-webkit-user-select:none;user-select:none;align-items:center;justify-content:space-between;border-top-width:1px;border-bottom-width:1px;border-top-color:hsl(var(--input));border-bottom-color:hsl(var(--input));background-color:hsl(var(--muted));padding:.5rem .75rem}.components-disclosure-title{display:flex;align-items:center;font-size:.875rem;line-height:1.25rem;color:hsl(var(--primary))}.components-disclosure-div{display:flex;gap:.5rem}.flow-page-positioning{height:100%;width:100%;overflow:hidden}.logspace-page-icon{position:absolute;bottom:.5rem;left:1.75rem;display:flex;height:1.5rem;cursor:pointer;flex-direction:column;align-items:center;justify-content:flex-start;overflow:hidden;border-radius:var(--radius);background-color:hsl(var(--foreground));padding-left:.5rem;padding-right:.5rem;text-align:center;font-family:var(--font-sans),ui-sans-serif,system-ui,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";font-size:.75rem;line-height:1rem;letter-spacing:.025em;color:hsl(var(--secondary));transition-property:all;transition-duration:.5s;transition-timing-function:cubic-bezier(.4,0,.2,1);animation-duration:.5s;animation-timing-function:cubic-bezier(.4,0,.2,1)}.logspace-page-icon:hover:hover{height:3rem}.flex-max-width{display:flex;width:100%}.loading-page-panel{display:flex;height:100%;width:100%;align-items:center;justify-content:center;background-color:hsl(var(--background))}.main-page-panel,.admin-page-panel{display:flex;width:100%;height:100%;flex-direction:column;overflow:auto;background-color:hsl(var(--background));padding-left:4rem;padding-right:4rem}.main-page-nav-arrangement{display:flex;width:100%;justify-content:space-between;padding-top:2rem;padding-bottom:.5rem}.main-page-nav-title{display:flex;align-items:center;justify-content:center;gap:.5rem;font-size:1.5rem;line-height:2rem;font-weight:600}.main-page-nav-button{margin-right:.5rem;width:1rem}.admin-page-description-text{display:flex;width:80%;padding-bottom:2rem;color:hsl(var(--muted-foreground))}.community-page-arrangement{display:flex;width:100%;height:100%;flex-direction:column;justify-content:space-between;overflow:auto;background-color:hsl(var(--background));padding-left:4rem;padding-right:4rem}.community-page-nav-arrangement{display:flex;width:100%;justify-content:space-between;padding-top:2rem;padding-bottom:.5rem}.community-page-nav-title{display:flex;align-items:center;justify-content:center;gap:.5rem;font-size:1.5rem;line-height:2rem;font-weight:600}.community-page-description-text{display:flex;width:70%;padding-bottom:2rem;color:hsl(var(--muted-foreground))}.generic-node-div{position:relative;display:flex;flex-direction:column;justify-content:center;background-color:hsl(var(--background))}.generic-node-div-title{display:flex;width:100%;align-items:center;gap:2rem;border-bottom-width:1px;background-color:hsl(var(--muted));padding:1rem}.generic-node-title-arrangement{display:flex;width:100%;align-items:center;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.generic-node-icon{height:2.5rem;width:2.5rem;border-radius:.25rem;padding:.25rem}.generic-node-tooltip-div{margin-left:.5rem;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.generic-node-status-position{position:relative;top:3px;height:1.25rem;width:1.25rem}.green-status{height:1rem;width:1rem;border-radius:9999px;opacity:1;background-color:var(--status-green)}.red-status{height:1rem;width:1rem;border-radius:9999px;opacity:1;background-color:var(--status-red)}.yellow-status{height:1rem;width:1rem;border-radius:9999px;opacity:1;background-color:var(--status-yellow)}.status-build-animation{display:none;height:1rem;width:1rem}.status-build-animation{animation:spin 1s linear infinite;border-radius:9999px;background-color:hsl(var(--ring));opacity:0}.status-div{position:absolute;width:1rem;transition-duration:.2s;transition-timing-function:cubic-bezier(.4,0,.2,1);animation-duration:.2s;animation-timing-function:cubic-bezier(.4,0,.2,1)}.status-div:hover:hover{color:hsl(var(--accent-foreground));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.generic-node-desc{margin-bottom:1rem;height:100%;width:100%;padding-left:1.25rem;padding-right:1.25rem;color:hsl(var(--foreground))}.generic-node-desc-text{width:100%;font-size:.875rem;line-height:1.25rem;color:hsl(var(--muted-foreground))}.error-build-message{margin-top:1.5rem;width:24rem;cursor:pointer;border-radius:calc(var(--radius) - 2px);background-color:var(--error-background);padding:1rem;--tw-shadow: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--tw-shadow-colored: 0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.error-build-message-circle{height:1.25rem;width:1.25rem;color:var(--status-red)}.error-build-foreground{font-size:.875rem;line-height:1.25rem;font-weight:500;color:var(--error-foreground);word-break:break-word}.error-build-message-div{color:var(--error-foreground);word-break:break-word;margin-top:.5rem;font-size:.875rem;line-height:1.25rem}.error-build-message-list{list-style-type:disc}.error-build-message-list>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0;margin-top:calc(.25rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(.25rem * var(--tw-space-y-reverse))}.error-build-message-list{padding-left:1.25rem}.success-alert{margin-top:1.5rem;width:24rem;border-radius:calc(var(--radius) - 2px);background-color:var(--success-background);padding:1rem;--tw-shadow: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--tw-shadow-colored: 0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.success-alert-icon{height:1.25rem;width:1.25rem;color:var(--status-green)}.success-alert-message{font-size:.875rem;line-height:1.25rem;font-weight:500;color:var(--success-foreground);word-break:break-word}.dropdown-component-outline{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.dropdown-component-outline:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.dropdown-component-outline::placeholder{color:#6b7280;opacity:1}.dropdown-component-outline::-webkit-datetime-edit-fields-wrapper{padding:0}.dropdown-component-outline::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.dropdown-component-outline::-webkit-datetime-edit{display:inline-flex}.dropdown-component-outline::-webkit-datetime-edit,.dropdown-component-outline::-webkit-datetime-edit-year-field,.dropdown-component-outline::-webkit-datetime-edit-month-field,.dropdown-component-outline::-webkit-datetime-edit-day-field,.dropdown-component-outline::-webkit-datetime-edit-hour-field,.dropdown-component-outline::-webkit-datetime-edit-minute-field,.dropdown-component-outline::-webkit-datetime-edit-second-field,.dropdown-component-outline::-webkit-datetime-edit-millisecond-field,.dropdown-component-outline::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.dropdown-component-outline{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;font-size:.875rem;line-height:1.25rem;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.dropdown-component-outline::placeholder{color:hsl(var(--muted-foreground))}.dropdown-component-outline:focus{border-color:hsl(var(--ring))}.dropdown-component-outline:focus::placeholder{color:transparent}.dropdown-component-outline:focus{--tw-ring-color: hsl(var(--ring))}.dropdown-component-outline:disabled{cursor:not-allowed;opacity:.5}.dropdown-component-outline{width:100%;padding-bottom:.125rem;padding-top:.125rem;text-align:left;position:relative;padding-right:2rem}.dropdown-component-false-outline{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.dropdown-component-false-outline:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.dropdown-component-false-outline::placeholder{color:#6b7280;opacity:1}.dropdown-component-false-outline::-webkit-datetime-edit-fields-wrapper{padding:0}.dropdown-component-false-outline::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.dropdown-component-false-outline::-webkit-datetime-edit{display:inline-flex}.dropdown-component-false-outline::-webkit-datetime-edit,.dropdown-component-false-outline::-webkit-datetime-edit-year-field,.dropdown-component-false-outline::-webkit-datetime-edit-month-field,.dropdown-component-false-outline::-webkit-datetime-edit-day-field,.dropdown-component-false-outline::-webkit-datetime-edit-hour-field,.dropdown-component-false-outline::-webkit-datetime-edit-minute-field,.dropdown-component-false-outline::-webkit-datetime-edit-second-field,.dropdown-component-false-outline::-webkit-datetime-edit-millisecond-field,.dropdown-component-false-outline::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.dropdown-component-false-outline{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;font-size:.875rem;line-height:1.25rem;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.dropdown-component-false-outline::placeholder{color:hsl(var(--muted-foreground))}.dropdown-component-false-outline:focus{border-color:hsl(var(--ring))}.dropdown-component-false-outline:focus::placeholder{color:transparent}.dropdown-component-false-outline:focus{--tw-ring-color: hsl(var(--ring))}.dropdown-component-false-outline:disabled{cursor:not-allowed;opacity:.5}.dropdown-component-false-outline{padding:.5rem 2.5rem .5rem .75rem;text-align:left}.dropdown-component-display{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;background-color:hsl(var(--background))}.dropdown-component-arrow{pointer-events:none;position:absolute;top:0;bottom:0;right:0;display:flex;align-items:center;padding-right:.5rem}.dropdown-component-arrow-color{color:hsl(var(--muted-foreground))}.dropdown-component-arrow-color:hover:hover{color:hsl(var(--accent-foreground))}.dropdown-component-arrow-color{height:1.25rem;width:1.25rem}.dropdown-component-true-options{z-index:10;margin-top:.25rem;max-height:15rem;overflow:auto;border-radius:calc(var(--radius) - 2px);background-color:hsl(var(--background));padding-top:.25rem;padding-bottom:.25rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);--tw-ring-color: rgb(0 0 0 / var(--tw-ring-opacity));--tw-ring-opacity: .05}.dropdown-component-true-options:focus{outline:2px solid transparent;outline-offset:2px}@media (min-width: 640px){.dropdown-component-true-options{font-size:.875rem;line-height:1.25rem}}@media (min-width: 1024px){.dropdown-component-true-options{width:32%}}.dropdown-component-false-options{z-index:10;margin-top:.25rem;max-height:15rem;overflow:auto;border-radius:calc(var(--radius) - 2px);background-color:hsl(var(--background));padding-top:.25rem;padding-bottom:.25rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);--tw-ring-color: rgb(0 0 0 / var(--tw-ring-opacity));--tw-ring-opacity: .05}.dropdown-component-false-options:focus{outline:2px solid transparent;outline-offset:2px}@media (min-width: 640px){.dropdown-component-false-options{font-size:.875rem;line-height:1.25rem}}.dropdown-component-false-options{width:100%}.dropdown-component-false-option{position:relative;cursor:default;-webkit-user-select:none;user-select:none;padding:.125rem 3rem .125rem .75rem}.dropdown-component-true-option{position:relative;cursor:default;-webkit-user-select:none;user-select:none;padding:.5rem 2.25rem .5rem .75rem}.dropdown-component-choosal{position:absolute;top:0;bottom:0;right:0;display:flex;align-items:center;padding-right:1rem}.dropdown-component-check-icon{height:1.25rem;width:1.25rem;--tw-text-opacity: 1;color:rgb(0 0 0 / var(--tw-text-opacity))}.edit-flow-arrangement{display:flex;justify-content:space-between}.edit-flow-span{margin-left:2.5rem}.edit-flow-span{animation:pulse 2s cubic-bezier(.4,0,.6,1) infinite;color:var(--status-red)}.header-menu-bar{display:flex;align-items:center;gap:.125rem;border-radius:calc(var(--radius) - 2px);padding:.25rem .375rem;font-size:.875rem;line-height:1.25rem;font-weight:500}.header-menu-bar-display{display:flex;max-width:120px;cursor:pointer;align-items:center;gap:.5rem}@media (min-width: 1024px){.header-menu-bar-display{max-width:200px}}.header-menu-flow-name{flex:1 1 0%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.header-menu-options{margin-right:.5rem;height:1rem;width:1rem}.header-arrangement{display:flex;width:100%;height:3rem;align-items:center;justify-content:space-between;border-bottom-width:1px;border-color:hsl(var(--border));background-color:hsl(var(--muted))}.header-start-display{display:flex;align-items:center;justify-content:flex-start;gap:.5rem}.header-end-division{display:flex;justify-content:flex-end;padding-left:.5rem;padding-right:.5rem}.header-end-display{margin-left:auto;margin-right:.5rem;display:flex;align-items:center;gap:1.25rem}.header-github-link{display:inline-flex;height:2.25rem;align-items:center;justify-content:center;border-radius:calc(var(--radius) - 2px);border-width:1px;border-color:hsl(var(--input));padding-left:.75rem;padding-right:.75rem;padding-right:0;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);font-size:.875rem;line-height:1.25rem;font-weight:500;color:hsl(var(--muted-foreground));--tw-ring-offset-color: hsl(var(--background))}.header-github-link:disabled{pointer-events:none;opacity:.5}.header-github-link:focus-visible:focus-visible{outline:2px solid transparent;outline-offset:2px;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);--tw-ring-color: hsl(var(--ring));--tw-ring-offset-width: 2px}.header-github-link:hover:hover{background-color:hsl(var(--accent));color:hsl(var(--accent-foreground))}.header-github-display{margin-right:-1px;margin-left:.25rem;display:flex;height:2.25rem;align-items:center;justify-content:center;border-radius:calc(var(--radius) - 2px);border-top-left-radius:0;border-bottom-left-radius:0;border-width:1px;background-color:hsl(var(--background));padding-left:.5rem;padding-right:.5rem;font-size:.875rem;line-height:1.25rem}.header-notifications{position:absolute;right:3px;height:.375rem;width:.375rem;border-radius:9999px;background-color:hsl(var(--destructive))}.input-component-div{pointer-events:none;position:relative;cursor:not-allowed}.input-component-true-button{position:absolute;top:0;bottom:0;right:0;align-items:center;color:hsl(var(--muted-foreground));padding-right:.5rem}.input-component-false-button{position:absolute;top:0;bottom:0;right:0;align-items:center;color:hsl(var(--muted-foreground));padding-left:1rem;padding-right:1rem}.input-component-true-svg{height:1.25rem;width:1.25rem}.input-component-true-svg:hover:hover{color:hsl(var(--accent-foreground))}.input-component-true-svg{position:absolute;bottom:.125rem;right:.5rem}.input-component-false-svg{height:1.25rem;width:1.25rem}.input-component-false-svg:hover:hover{color:hsl(var(--accent-foreground))}.input-component-false-svg{position:absolute;bottom:.5rem;right:.75rem}.input-file-component{display:flex;width:100%;align-items:center}.toggle-component-switch{position:relative;display:inline-flex;height:1.5rem;width:2.75rem;flex-shrink:0;cursor:pointer;border-radius:9999px;border-width:2px;border-color:transparent;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-duration:.2s;transition-timing-function:cubic-bezier(.4,0,.2,1);animation-duration:.2s;animation-timing-function:cubic-bezier(.4,0,.2,1)}.toggle-component-switch:focus:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);--tw-ring-color: hsl(var(--primary));--tw-ring-offset-width: 1px}.toggle-component-span{pointer-events:none;position:relative;height:1.25rem;width:1.25rem;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));border-radius:9999px;--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(0px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-duration:.2s;transition-timing-function:cubic-bezier(.4,0,.2,1);animation-duration:.2s;animation-timing-function:cubic-bezier(.4,0,.2,1)}.toggle-component-second-span{position:absolute;top:0;right:0;bottom:0;left:0;display:flex;height:100%;width:100%;align-items:center;justify-content:center;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.app-div{position:fixed;bottom:1.25rem;left:1.25rem;display:flex;flex-direction:column-reverse}.code-block-modal{display:flex;align-items:center;justify-content:space-between;padding:.375rem 1rem}.code-block-modal-span{font-size:.75rem;line-height:1rem;text-transform:lowercase;color:hsl(var(--muted-foreground))}.code-block-modal-button{display:flex;align-items:center;gap:.375rem;border-radius:.25rem;background-image:none;padding:.25rem;font-size:.75rem;line-height:1rem;color:hsl(var(--muted-foreground))}.file-card-modal-image-div{position:absolute;right:0;top:0;border-bottom-left-radius:var(--radius);background-color:hsl(var(--muted));padding-left:.25rem;padding-right:.25rem;font-size:.875rem;line-height:1.25rem;font-weight:700;color:hsl(var(--foreground))}.file-card-modal-image-button{padding:.25rem .5rem;color:hsl(var(--ring))}.file-card-modal-button{display:flex;width:50%;align-items:center;justify-content:space-between;border-radius:.25rem;border-width:1px;border-color:hsl(var(--ring));background-color:hsl(var(--muted));padding:.5rem;color:hsl(var(--foreground));--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.file-card-modal-button:hover{--tw-drop-shadow: drop-shadow(0 10px 8px rgb(0 0 0 / .04)) drop-shadow(0 4px 3px rgb(0 0 0 / .1));filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.file-card-modal-div{display:flex;width:100%;margin-right:.5rem;align-items:center;gap:.5rem;color:currentColor}.file-card-modal-footer{display:flex;flex-direction:column;align-items:flex-start}.file-card-modal-name{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;font-size:.875rem;line-height:1.25rem;color:currentColor}.file-card-modal-type{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;font-size:.75rem;line-height:1rem;color:hsl(var(--ring))}.edit-node-modal-variable{height:1.25rem;width:1.25rem;stroke-width:2;padding-inline-end:.25rem;color:hsl(var(--muted-foreground))}.edit-node-modal-span{font-size:.875rem;line-height:1.25rem;font-weight:600;color:hsl(var(--primary))}.edit-node-modal-arrangement{display:flex;width:100%;height:-webkit-fit-content;height:-moz-fit-content;height:fit-content;max-height:400px}.edit-node-modal-box{width:100%;border-radius:var(--radius);border-width:1px;border-color:hsl(var(--input));background-color:hsl(var(--background))}.edit-node-modal-table{display:flex;height:-webkit-fit-content;height:-moz-fit-content;height:fit-content;flex-direction:column;gap:1.25rem}.edit-node-modal-table-header{height:2.5rem;border-color:hsl(var(--input));font-size:.75rem;line-height:1rem;font-weight:500;color:hsl(var(--ring))}.link-color{font-weight:600;color:hsl(var(--foreground))}.api-modal-tabs{display:flex;height:100%;max-width:100%;flex-direction:column;overflow:hidden;border-radius:calc(var(--radius) - 2px);border-width:1px;background-color:hsl(var(--muted));text-align:center}@media (min-width: 640px){.api-modal-tabs{width:75vw}}@media (min-width: 768px){.api-modal-tabs{width:75vw}}@media (min-width: 1024px){.api-modal-tabs{width:75vw}}@media (min-width: 1280px){.api-modal-tabs{width:76vw}}@media (min-width: 1536px){.api-modal-tabs{width:100%}}.api-modal-tablist-div{display:flex;align-items:center;justify-content:space-between;padding-left:.5rem;padding-right:.5rem}.api-modal-tabs-content{margin-top:-.25rem;height:100%;width:100%;overflow:hidden;padding-left:1rem;padding-right:1rem;padding-bottom:1rem}.api-modal-table-arrangement{display:flex;height:-webkit-fit-content;height:-moz-fit-content;height:fit-content;flex-direction:column;gap:1.25rem}.icons-parameters-comp{margin-left:.75rem;height:1.5rem;width:1.5rem}.form-modal-lock-true{background-color:hsl(var(--input));color:hsl(var(--primary))}.form-modal-no-input{background-color:hsl(var(--input));text-align:center;color:hsl(var(--primary))}:is(.dark .form-modal-no-input){--tw-bg-opacity: 1;background-color:rgb(55 65 81 / var(--tw-bg-opacity));--tw-text-opacity: 1;color:rgb(209 213 219 / var(--tw-text-opacity))}.form-modal-lock-false{background-color:var(--white);color:hsl(var(--primary))}.code-highlight{display:block;max-height:64vh;width:100%;overflow-y:hidden;border-width:0px;padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;outline-width:0px;word-break:break-word}.code-nohighlight{display:block;max-height:70vh;width:100%;overflow-y:hidden;border-width:0px;padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;outline-width:0px;word-break:break-word}.form-modal-lockchat{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.form-modal-lockchat:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.form-modal-lockchat::placeholder{color:#6b7280;opacity:1}.form-modal-lockchat::-webkit-datetime-edit-fields-wrapper{padding:0}.form-modal-lockchat::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.form-modal-lockchat::-webkit-datetime-edit{display:inline-flex}.form-modal-lockchat::-webkit-datetime-edit,.form-modal-lockchat::-webkit-datetime-edit-year-field,.form-modal-lockchat::-webkit-datetime-edit-month-field,.form-modal-lockchat::-webkit-datetime-edit-day-field,.form-modal-lockchat::-webkit-datetime-edit-hour-field,.form-modal-lockchat::-webkit-datetime-edit-minute-field,.form-modal-lockchat::-webkit-datetime-edit-second-field,.form-modal-lockchat::-webkit-datetime-edit-millisecond-field,.form-modal-lockchat::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.form-modal-lockchat{display:block;width:100%;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));padding:1rem 4rem 1rem 1rem}.form-modal-lockchat::-webkit-scrollbar{width:8px;height:8px}.form-modal-lockchat::-webkit-scrollbar-track{background-color:#f1f1f1}.form-modal-lockchat::-webkit-scrollbar-thumb{background-color:#ccc;border-radius:999px}.form-modal-lockchat::-webkit-scrollbar-thumb:hover{background-color:#bbb}.form-modal-lockchat{cursor:auto}.form-modal-lockchat:focus{border-color:hsl(var(--ring));--tw-ring-color: hsl(var(--ring))}@media (min-width: 640px){.form-modal-lockchat{font-size:.875rem;line-height:1.25rem}}.form-modal-send-icon-position{position:absolute;bottom:.5rem;right:1rem}.form-modal-send-button{border-radius:calc(var(--radius) - 2px);padding:.5rem .25rem;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.3s;animation-duration:.3s}.form-modal-lock-icon{margin-left:.25rem;margin-right:.25rem;height:1.25rem;width:1.25rem}.form-modal-lock-icon{animation:pulse 2s cubic-bezier(.4,0,.6,1) infinite}.form-modal-send-icon{margin-right:.5rem;height:1.25rem;width:1.25rem;--tw-rotate: 44deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.form-modal-play-icon{margin-left:.25rem;margin-right:.25rem;height:1.25rem;width:1.25rem}.form-modal-chat-position{display:flex;width:100%;padding:1.5rem 2.25rem 1.5rem 1rem}.form-modal-chatbot-icon{margin:.25rem 1.5rem .75rem .75rem}.form-modal-chat-image{display:flex;flex-direction:column;align-items:center;gap:.25rem}.form-modal-chat-bot-icon{position:relative;display:flex;height:2rem;width:2rem;align-items:center;justify-content:center;overflow:hidden;border-radius:calc(var(--radius) - 2px);padding:1.25rem;font-size:1.5rem;line-height:2rem;background-color:var(--chat-bot-icon)}.form-modal-chat-user-icon{position:relative;display:flex;height:2rem;width:2rem;align-items:center;justify-content:center;overflow:hidden;border-radius:calc(var(--radius) - 2px);padding:1.25rem;font-size:1.5rem;line-height:2rem;background-color:var(--chat-user-icon)}.form-modal-chat-icon-img{position:absolute;--tw-scale-x: 60%;--tw-scale-y: 60%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.form-modal-chat-text-position{display:flex;width:100%;flex:1 1 0%;text-align:start}.form-modal-chat-text{position:relative;display:flex;width:100%;flex-direction:column;text-align:start;font-size:.875rem;line-height:1.25rem;font-weight:400;color:hsl(var(--muted-foreground))}.form-modal-chat-icon-div{position:absolute;left:-1.5rem;top:-.75rem;cursor:pointer}.form-modal-chat-icon{height:1rem;width:1rem}.form-modal-chat-icon{animation:bounce 1s infinite}.form-modal-chat-thought{border-radius:calc(var(--radius) - 2px);border-width:1px;border-color:hsl(var(--ring) / .6);height:100%;width:95%;cursor:pointer;overflow:scroll;background-color:hsl(var(--background));padding:.5rem;text-align:start;color:hsl(var(--primary));-ms-overflow-style:none;scrollbar-width:none}.form-modal-chat-thought::-webkit-scrollbar{display:none}.form-modal-markdown-span{margin-top:.25rem}.form-modal-markdown-span{animation:pulse 2s cubic-bezier(.4,0,.6,1) infinite;cursor:default}.form-modal-initial-prompt-btn{margin-bottom:.5rem;display:flex;align-items:center;gap:.5rem;border-radius:calc(var(--radius) - 2px);border-width:1px;border-color:hsl(var(--border));background-color:hsl(var(--background));padding:.5rem 1rem;font-size:.875rem;line-height:1.25rem;font-weight:600;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.form-modal-iv-box{display:flex;width:100%;margin-top:.5rem;height:80vh}.form-modal-iv-size{margin-right:1.5rem;display:flex;height:100%;width:33.333333%;flex-direction:column;justify-content:flex-start;overflow:auto;-ms-overflow-style:none;scrollbar-width:none}.form-modal-iv-size::-webkit-scrollbar{display:none}.file-component-arrangement{display:flex;align-items:center;padding-top:.5rem;padding-bottom:.5rem}.file-component-variable{margin-left:-1px;margin-right:.25rem;height:1rem;width:1rem;color:hsl(var(--primary))}.file-component-variables-span{font-weight:600;color:hsl(var(--primary))}.file-component-variables-title{display:flex;align-items:center;justify-content:space-between;padding-top:.5rem}.file-component-variables-div{margin-right:.625rem;display:flex;align-items:center}.file-component-accordion-div{display:flex;align-items:flex-start;gap:.75rem}.file-component-badge-div{display:flex;width:100%;align-items:center;justify-content:space-between}.file-component-tab-column{display:flex;flex-direction:column;gap:.5rem;padding:.25rem}.eraser-column-arrangement{display:flex;width:100%;flex:1 1 0%;flex-direction:column}.eraser-size{position:relative;display:flex;height:100%;width:100%;flex-direction:column;border-radius:calc(var(--radius) - 2px);border-width:1px;background-color:hsl(var(--muted))}.eraser-position{position:absolute;right:.75rem;top:.75rem;z-index:50}.chat-message-div{display:flex;width:100%;height:100%;flex-direction:column;align-items:center;overflow:scroll;-ms-overflow-style:none;scrollbar-width:none}.chat-message-div::-webkit-scrollbar{display:none}.chat-alert-box{display:flex;width:100%;height:100%;flex-direction:column;align-items:center;justify-content:center;text-align:center;vertical-align:middle}.langflow-chat-span{font-size:1.125rem;line-height:1.75rem;color:hsl(var(--foreground))}.langflow-chat-desc{width:50%;border-radius:calc(var(--radius) - 2px);border-width:1px;border-color:hsl(var(--border));background-color:hsl(var(--muted));padding:2rem 1.5rem}.langflow-chat-desc-span{font-size:1rem;line-height:1.5rem;color:hsl(var(--muted-foreground))}.langflow-chat-input-div{display:flex;width:100%;flex-direction:column;align-items:center;justify-content:space-between;padding-left:2rem;padding-right:2rem;padding-bottom:1.5rem}.langflow-chat-input{position:relative;width:100%;border-radius:calc(var(--radius) - 2px);--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.tooltip-fixed-width{max-height:25vh;max-width:30vw;overflow:auto}.export-modal-save-api{font-weight:500;line-height:1}.peer:disabled~.export-modal-save-api{cursor:not-allowed;opacity:.7}.beta-badge-wrapper{position:absolute;right:0;top:0;height:4rem;width:4rem;overflow:hidden;border-top-right-radius:var(--radius)}.beta-badge-content{margin-top:.5rem;width:6rem;--tw-rotate: 45deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));background-color:var(--beta-background);text-align:center;font-size:.75rem;line-height:1rem;font-weight:600;color:var(--beta-foreground)}.chat-message-highlight{border-radius:calc(var(--radius) - 2px);--tw-bg-opacity: 1;background-color:rgb(224 231 255 / var(--tw-bg-opacity));padding-left:.125rem;padding-right:.125rem}:is(.dark .chat-message-highlight){--tw-bg-opacity: 1;background-color:rgb(49 46 129 / var(--tw-bg-opacity))}.field-invalid{position:absolute;font-size:.8rem;font-weight:500;color:hsl(var(--destructive))}.input-invalid{border-color:hsl(var(--destructive))}.input-invalid:focus{border-color:hsl(var(--destructive));--tw-ring-color: hsl(var(--destructive))}.fade-container{position:relative;overflow:hidden}.fade-container:before,.fade-container:after{pointer-events:none;position:absolute;bottom:0;top:0;background-image:linear-gradient(to right,var(--tw-gradient-stops));--tw-gradient-from: hsl(var(--background)) var(--tw-gradient-from-position);--tw-gradient-to: hsl(var(--background) / 0) var(--tw-gradient-to-position);--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);--tw-gradient-to: transparent var(--tw-gradient-to-position);content:"";width:50px;opacity:0;transition:opacity .3s}.fade-container:after{right:0;transform:rotate(180deg)}.fade-container.fade-left:before,.fade-container.fade-right:after{opacity:1}.fade-container-dark.fade-left:before,.fade-container-dark.fade-right:after{opacity:1}.scroll-container{display:flex;overflow-x:scroll;-ms-overflow-style:none;scrollbar-width:none}.scroll-container::-webkit-scrollbar{display:none}.store-beta-icon{position:relative;bottom:.75rem;left:.25rem;margin-left:.5rem;border-radius:9999px;background-color:var(--beta-background);padding:.25rem .5rem;text-align:center;font-size:.75rem;line-height:1rem;font-weight:600;color:var(--beta-foreground)}.sr-only{position:absolute!important;width:1px!important;height:1px!important;padding:0!important;margin:-1px!important;overflow:hidden!important;clip:rect(0,0,0,0)!important;white-space:nowrap!important;border-width:0!important}.pointer-events-none{pointer-events:none!important}.visible{visibility:visible!important}.fixed{position:fixed!important}.absolute{position:absolute!important}.relative{position:relative!important}.sticky{position:-webkit-sticky!important;position:sticky!important}.inset-0{top:0!important;right:0!important;bottom:0!important;left:0!important}.inset-x-6{left:1.5rem!important;right:1.5rem!important}.bottom-0{bottom:0!important}.bottom-0\.5{bottom:.125rem!important}.bottom-20{bottom:5rem!important}.bottom-\[1px\]{bottom:1px!important}.left-0{left:0!important}.left-1{left:.25rem!important}.left-2{left:.5rem!important}.left-\[50\%\]{left:50%!important}.left-\[500\%\]{left:500%!important}.right-0{right:0!important}.right-2{right:.5rem!important}.right-4{right:1rem!important}.top-0{top:0!important}.top-0\.5{top:.125rem!important}.top-4{top:1rem!important}.top-\[50\%\]{top:50%!important}.top-\[500\%\]{top:500%!important}.isolate{isolation:isolate!important}.z-50{z-index:50!important}.z-\[9999\]{z-index:9999!important}.float-right{float:right!important}.-m-0{margin:-0px!important}.-m-0\.5{margin:-.125rem!important}.-m-1{margin:-.25rem!important}.m-1{margin:.25rem!important}.m-4{margin:1rem!important}.m-auto{margin:auto!important}.-mx-1{margin-left:-.25rem!important;margin-right:-.25rem!important}.-mx-1\.5{margin-left:-.375rem!important;margin-right:-.375rem!important}.-my-1{margin-top:-.25rem!important;margin-bottom:-.25rem!important}.-my-1\.5{margin-top:-.375rem!important;margin-bottom:-.375rem!important}.mx-0{margin-left:0!important;margin-right:0!important}.mx-0\.5{margin-left:.125rem!important;margin-right:.125rem!important}.mx-1{margin-left:.25rem!important;margin-right:.25rem!important}.mx-2{margin-left:.5rem!important;margin-right:.5rem!important}.mx-\[0\.08rem\]{margin-left:.08rem!important;margin-right:.08rem!important}.mx-auto{margin-left:auto!important;margin-right:auto!important}.my-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-12{margin-top:3rem!important;margin-bottom:3rem!important}.my-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-3{margin-top:.75rem!important;margin-bottom:.75rem!important}.my-6{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-auto{margin-top:auto!important;margin-bottom:auto!important}.-mb-1{margin-bottom:-.25rem!important}.-ml-0{margin-left:-0px!important}.-ml-0\.5{margin-left:-.125rem!important}.-ml-1{margin-left:-.25rem!important}.-ml-px{margin-left:-1px!important}.-mr-0{margin-right:-0px!important}.-mr-0\.5{margin-right:-.125rem!important}.mb-1{margin-bottom:.25rem!important}.mb-2{margin-bottom:.5rem!important}.mb-24{margin-bottom:6rem!important}.mb-3{margin-bottom:.75rem!important}.mb-4{margin-bottom:1rem!important}.mb-6{margin-bottom:1.5rem!important}.mb-auto{margin-bottom:auto!important}.ml-1{margin-left:.25rem!important}.ml-2{margin-left:.5rem!important}.ml-3{margin-left:.75rem!important}.ml-4{margin-left:1rem!important}.ml-auto{margin-left:auto!important}.mr-1{margin-right:.25rem!important}.mr-2{margin-right:.5rem!important}.mr-3{margin-right:.75rem!important}.mr-4{margin-right:1rem!important}.mt-0{margin-top:0!important}.mt-1{margin-top:.25rem!important}.mt-2{margin-top:.5rem!important}.mt-3{margin-top:.75rem!important}.mt-4{margin-top:1rem!important}.mt-5{margin-top:1.25rem!important}.mt-6{margin-top:1.5rem!important}.mt-8{margin-top:2rem!important}.block{display:block!important}.\!inline,.inline{display:inline!important}.flex{display:flex!important}.inline-flex{display:inline-flex!important}.table{display:table!important}.grid{display:grid!important}.contents{display:contents!important}.\!hidden,.hidden{display:none!important}.h-0{height:0px!important}.h-1\/3{height:33.333333%!important}.h-1\/4{height:25%!important}.h-10{height:2.5rem!important}.h-11{height:2.75rem!important}.h-12{height:3rem!important}.h-16{height:4rem!important}.h-2{height:.5rem!important}.h-2\/6{height:33.333333%!important}.h-24{height:6rem!important}.h-3{height:.75rem!important}.h-3\.5{height:.875rem!important}.h-4{height:1rem!important}.h-5{height:1.25rem!important}.h-6{height:1.5rem!important}.h-7{height:1.75rem!important}.h-8{height:2rem!important}.h-9{height:2.25rem!important}.h-\[1\.1rem\]{height:1.1rem!important}.h-\[11rem\]{height:11rem!important}.h-\[1px\]{height:1px!important}.h-\[24px\]{height:24px!important}.h-\[40vh\]{height:40vh!important}.h-\[500px\]{height:500px!important}.h-\[60vh\]{height:60vh!important}.h-\[70vh\]{height:70vh!important}.h-\[80vh\]{height:80vh!important}.h-\[var\(--radix-select-trigger-height\)\]{height:var(--radix-select-trigger-height)!important}.h-fit{height:-webkit-fit-content!important;height:-moz-fit-content!important;height:fit-content!important}.h-full{height:100%!important}.h-px{height:1px!important}.h-screen{height:100vh!important}.max-h-20{max-height:5rem!important}.max-h-48{max-height:12rem!important}.max-h-96{max-height:24rem!important}.max-h-\[100px\]{max-height:100px!important}.max-h-\[10rem\]{max-height:10rem!important}.max-h-\[15rem\]{max-height:15rem!important}.max-h-\[300px\]{max-height:300px!important}.min-h-fit{min-height:-webkit-fit-content!important;min-height:-moz-fit-content!important;min-height:fit-content!important}.w-1\/4{width:25%!important}.w-1\/6{width:16.666667%!important}.w-12{width:3rem!important}.w-16{width:4rem!important}.w-2{width:.5rem!important}.w-24{width:6rem!important}.w-28{width:7rem!important}.w-3{width:.75rem!important}.w-3\.5{width:.875rem!important}.w-32{width:8rem!important}.w-4{width:1rem!important}.w-40{width:10rem!important}.w-44{width:11rem!important}.w-5{width:1.25rem!important}.w-5\/6{width:83.333333%!important}.w-6{width:1.5rem!important}.w-7{width:1.75rem!important}.w-72{width:18rem!important}.w-8{width:2rem!important}.w-96{width:24rem!important}.w-\[1\.1rem\]{width:1.1rem!important}.w-\[100px\]{width:100px!important}.w-\[1010px\]{width:1010px!important}.w-\[160px\]{width:160px!important}.w-\[1px\]{width:1px!important}.w-\[200px\]{width:200px!important}.w-\[250px\]{width:250px!important}.w-\[300px\]{width:300px!important}.w-\[31px\]{width:31px!important}.w-\[40\%\]{width:40%!important}.w-\[44px\]{width:44px!important}.w-\[500px\]{width:500px!important}.w-\[80\%\]{width:80%!important}.w-\[90\%\]{width:90%!important}.w-fit{width:-webkit-fit-content!important;width:-moz-fit-content!important;width:fit-content!important}.w-full{width:100%!important}.min-w-\[12rem\]{min-width:12rem!important}.min-w-\[20vw\]{min-width:20vw!important}.min-w-\[40vw\]{min-width:40vw!important}.min-w-\[60vw\]{min-width:60vw!important}.min-w-\[80vw\]{min-width:80vw!important}.min-w-\[8rem\]{min-width:8rem!important}.min-w-\[var\(--radix-select-trigger-width\)\]{min-width:var(--radix-select-trigger-width)!important}.min-w-full{min-width:100%!important}.min-w-min{min-width:-webkit-min-content!important;min-width:min-content!important}.max-w-4xl{max-width:56rem!important}.max-w-\[40vw\]{max-width:40vw!important}.max-w-lg{max-width:32rem!important}.flex-1{flex:1 1 0%!important}.flex-shrink-0,.shrink-0{flex-shrink:0!important}.flex-grow{flex-grow:1!important}.basis-1\/2{flex-basis:50%!important}.basis-5\/6{flex-basis:83.333333%!important}.table-fixed{table-layout:fixed!important}.caption-bottom{caption-side:bottom!important}.translate-x-0{--tw-translate-x: 0px !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-x-5{--tw-translate-x: 1.25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-x-\[-100\%\]{--tw-translate-x: -100% !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-x-\[-50\%\]{--tw-translate-x: -50% !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-y-0{--tw-translate-y: 0px !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-y-96{--tw-translate-y: 24rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-y-\[-50\%\]{--tw-translate-y: -50% !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.rotate-180{--tw-rotate: 180deg !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.rotate-90{--tw-rotate: 90deg !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}@keyframes bounce{0%,to{transform:translateY(-25%);animation-timing-function:cubic-bezier(.8,0,1,1)}50%{transform:none;animation-timing-function:cubic-bezier(0,0,.2,1)}}.animate-bounce{animation:bounce 1s infinite!important}@keyframes pulse{50%{opacity:.5}}.animate-pulse{animation:pulse 2s cubic-bezier(.4,0,.6,1) infinite!important}@keyframes spin{to{transform:rotate(360deg)}}.animate-spin{animation:spin 1s linear infinite!important}.cursor-default{cursor:default!important}.cursor-grabbing{cursor:grabbing!important}.cursor-not-allowed{cursor:not-allowed!important}.cursor-pointer{cursor:pointer!important}.select-none{-webkit-user-select:none!important;user-select:none!important}.resize{resize:both!important}.list-disc{list-style-type:disc!important}.grid-cols-1{grid-template-columns:repeat(1,minmax(0,1fr))!important}.flex-row{flex-direction:row!important}.flex-row-reverse{flex-direction:row-reverse!important}.flex-col{flex-direction:column!important}.flex-col-reverse{flex-direction:column-reverse!important}.flex-wrap{flex-wrap:wrap!important}.items-start{align-items:flex-start!important}.items-end{align-items:flex-end!important}.items-center{align-items:center!important}.justify-start{justify-content:flex-start!important}.justify-end{justify-content:flex-end!important}.justify-center{justify-content:center!important}.justify-between{justify-content:space-between!important}.justify-evenly{justify-content:space-evenly!important}.gap-0{gap:0px!important}.gap-0\.5{gap:.125rem!important}.gap-1{gap:.25rem!important}.gap-1\.5{gap:.375rem!important}.gap-2{gap:.5rem!important}.gap-3{gap:.75rem!important}.gap-4{gap:1rem!important}.gap-5{gap:1.25rem!important}.gap-8{gap:2rem!important}.gap-\[4px\]{gap:4px!important}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(.25rem * var(--tw-space-x-reverse))!important;margin-left:calc(.25rem * calc(1 - var(--tw-space-x-reverse)))!important}.space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(.5rem * var(--tw-space-x-reverse))!important;margin-left:calc(.5rem * calc(1 - var(--tw-space-x-reverse)))!important}.space-x-6>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(1.5rem * var(--tw-space-x-reverse))!important;margin-left:calc(1.5rem * calc(1 - var(--tw-space-x-reverse)))!important}.space-y-0>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(0px * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(0px * var(--tw-space-y-reverse))!important}.space-y-0\.5>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(.125rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(.125rem * var(--tw-space-y-reverse))!important}.space-y-1>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(.25rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(.25rem * var(--tw-space-y-reverse))!important}.space-y-1\.5>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(.375rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(.375rem * var(--tw-space-y-reverse))!important}.space-y-2>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(.5rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(.5rem * var(--tw-space-y-reverse))!important}.space-y-6>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(1.5rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(1.5rem * var(--tw-space-y-reverse))!important}.space-y-8>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(2rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(2rem * var(--tw-space-y-reverse))!important}.overflow-auto{overflow:auto!important}.overflow-hidden{overflow:hidden!important}.overflow-scroll{overflow:scroll!important}.overflow-y-auto{overflow-y:auto!important}.overflow-x-hidden{overflow-x:hidden!important}.overflow-x-clip{overflow-x:clip!important}.overflow-y-scroll{overflow-y:scroll!important}.truncate{overflow:hidden!important;text-overflow:ellipsis!important;white-space:nowrap!important}.text-clip{text-overflow:clip!important}.whitespace-nowrap{white-space:nowrap!important}.whitespace-break-spaces{white-space:break-spaces!important}.break-words{overflow-wrap:break-word!important}.rounded{border-radius:.25rem!important}.rounded-full{border-radius:9999px!important}.rounded-lg{border-radius:var(--radius)!important}.rounded-md{border-radius:calc(var(--radius) - 2px)!important}.rounded-sm{border-radius:calc(var(--radius) - 4px)!important}.rounded-l-md{border-top-left-radius:calc(var(--radius) - 2px)!important;border-bottom-left-radius:calc(var(--radius) - 2px)!important}.rounded-r-md{border-top-right-radius:calc(var(--radius) - 2px)!important;border-bottom-right-radius:calc(var(--radius) - 2px)!important}.rounded-t-lg{border-top-left-radius:var(--radius)!important;border-top-right-radius:var(--radius)!important}.border{border-width:1px!important}.border-0{border-width:0px!important}.border-2{border-width:2px!important}.border-\[1px\]{border-width:1px!important}.border-b{border-bottom-width:1px!important}.border-b-2{border-bottom-width:2px!important}.border-border{border-color:hsl(var(--border))!important}.border-error{--tw-border-opacity: 1 !important;border-color:var(--fallback-er,oklch(var(--er)/var(--tw-border-opacity)))!important}.border-gray-300{--tw-border-opacity: 1 !important;border-color:rgb(209 213 219 / var(--tw-border-opacity))!important}.border-indigo-300{--tw-border-opacity: 1 !important;border-color:rgb(165 180 252 / var(--tw-border-opacity))!important}.border-input{border-color:hsl(var(--input))!important}.border-muted{border-color:hsl(var(--muted))!important}.border-primary{border-color:hsl(var(--primary))!important}.border-ring{border-color:hsl(var(--ring))!important}.border-ring\/60{border-color:hsl(var(--ring) / .6)!important}.border-transparent{border-color:transparent!important}.\!bg-white{background-color:var(--white)!important}.bg-accent{background-color:hsl(var(--accent))!important}.bg-background{background-color:hsl(var(--background))!important}.bg-beta-foreground{background-color:var(--beta-foreground)!important}.bg-blur-shared{background-color:var(--blur-shared)!important}.bg-border{background-color:hsl(var(--border))!important}.bg-chat-send{background-color:var(--chat-send)!important}.bg-destructive{background-color:hsl(var(--destructive))!important}.bg-error-background{background-color:var(--error-background)!important}.bg-foreground{background-color:hsl(var(--foreground))!important}.bg-high-indigo{background-color:var(--high-indigo)!important}.bg-info-background{background-color:var(--info-background)!important}.bg-input{background-color:hsl(var(--input))!important}.bg-muted{background-color:hsl(var(--muted))!important}.bg-popover{background-color:hsl(var(--popover))!important}.bg-primary{background-color:hsl(var(--primary))!important}.bg-ring\/40{background-color:hsl(var(--ring) / .4)!important}.bg-secondary{background-color:hsl(var(--secondary))!important}.bg-status-blue{background-color:var(--status-blue)!important}.bg-status-green{background-color:var(--status-green)!important}.bg-status-red{background-color:var(--status-red)!important}.bg-status-yellow{background-color:var(--status-yellow)!important}.bg-success-background{background-color:var(--success-background)!important}.bg-transparent{background-color:transparent!important}.bg-opacity-50{--tw-bg-opacity: .5 !important}.bg-gradient-to-br{background-image:linear-gradient(to bottom right,var(--tw-gradient-stops))!important}.bg-gradient-to-r{background-image:linear-gradient(to right,var(--tw-gradient-stops))!important}.bg-gradient-to-tr{background-image:linear-gradient(to top right,var(--tw-gradient-stops))!important}.bg-none{background-image:none!important}.from-amber-200{--tw-gradient-from: #fde68a var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(253 230 138 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-amber-700{--tw-gradient-from: #b45309 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(180 83 9 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-blue-100{--tw-gradient-from: #dbeafe var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(219 234 254 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-blue-300{--tw-gradient-from: #93c5fd var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(147 197 253 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-blue-700{--tw-gradient-from: #1d4ed8 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(29 78 216 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-emerald-500{--tw-gradient-from: #10b981 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(16 185 129 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-fuchsia-500{--tw-gradient-from: #d946ef var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(217 70 239 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-fuchsia-600{--tw-gradient-from: #c026d3 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(192 38 211 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-gray-300{--tw-gradient-from: #d1d5db var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(209 213 219 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-gray-800{--tw-gradient-from: #1f2937 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(31 41 55 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-gray-900{--tw-gradient-from: #111827 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(17 24 39 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-green-200{--tw-gradient-from: #bbf7d0 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(187 247 208 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-green-300{--tw-gradient-from: #86efac var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(134 239 172 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-green-500{--tw-gradient-from: #22c55e var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(34 197 94 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-lime-600{--tw-gradient-from: #65a30d var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(101 163 13 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-purple-400{--tw-gradient-from: #c084fc var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(192 132 252 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-red-400{--tw-gradient-from: #f87171 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(248 113 113 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-red-800{--tw-gradient-from: #991b1b var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(153 27 27 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-rose-400{--tw-gradient-from: #fb7185 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(251 113 133 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-rose-500{--tw-gradient-from: #f43f5e var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(244 63 94 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-sky-400{--tw-gradient-from: #38bdf8 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(56 189 248 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-violet-500{--tw-gradient-from: #8b5cf6 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(139 92 246 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-yellow-200{--tw-gradient-from: #fef08a var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(254 240 138 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.via-blue-300{--tw-gradient-to: rgb(147 197 253 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #93c5fd var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-blue-800{--tw-gradient-to: rgb(30 64 175 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #1e40af var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-fuchsia-500{--tw-gradient-to: rgb(217 70 239 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #d946ef var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-fuchsia-600{--tw-gradient-to: rgb(192 38 211 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #c026d3 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-gray-300{--tw-gradient-to: rgb(209 213 219 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #d1d5db var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-green-200{--tw-gradient-to: rgb(187 247 208 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #bbf7d0 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-green-300{--tw-gradient-to: rgb(134 239 172 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #86efac var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-green-400{--tw-gradient-to: rgb(74 222 128 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #4ade80 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-orange-300{--tw-gradient-to: rgb(253 186 116 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #fdba74 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-pink-200{--tw-gradient-to: rgb(251 207 232 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #fbcfe8 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-purple-900{--tw-gradient-to: rgb(88 28 135 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #581c87 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-red-400{--tw-gradient-to: rgb(248 113 113 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #f87171 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-red-500{--tw-gradient-to: rgb(239 68 68 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #ef4444 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-red-600{--tw-gradient-to: rgb(220 38 38 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #dc2626 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-rose-400{--tw-gradient-to: rgb(251 113 133 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #fb7185 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-rose-700{--tw-gradient-to: rgb(190 18 60 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #be123c var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-violet-600{--tw-gradient-to: rgb(124 58 237 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #7c3aed var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-yellow-300{--tw-gradient-to: rgb(253 224 71 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #fde047 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-yellow-400{--tw-gradient-to: rgb(250 204 21 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #facc15 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-yellow-600{--tw-gradient-to: rgb(202 138 4 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #ca8a04 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.to-blue-500{--tw-gradient-to: #3b82f6 var(--tw-gradient-to-position) !important}.to-fuchsia-500{--tw-gradient-to: #d946ef var(--tw-gradient-to-position) !important}.to-gray-600{--tw-gradient-to: #4b5563 var(--tw-gradient-to-position) !important}.to-gray-900{--tw-gradient-to: #111827 var(--tw-gradient-to-position) !important}.to-green-500{--tw-gradient-to: #22c55e var(--tw-gradient-to-position) !important}.to-green-700{--tw-gradient-to: #15803d var(--tw-gradient-to-position) !important}.to-indigo-500{--tw-gradient-to: #6366f1 var(--tw-gradient-to-position) !important}.to-indigo-700{--tw-gradient-to: #4338ca var(--tw-gradient-to-position) !important}.to-indigo-900{--tw-gradient-to: #312e81 var(--tw-gradient-to-position) !important}.to-lime-400{--tw-gradient-to: #a3e635 var(--tw-gradient-to-position) !important}.to-lime-600{--tw-gradient-to: #65a30d var(--tw-gradient-to-position) !important}.to-orange-300{--tw-gradient-to: #fdba74 var(--tw-gradient-to-position) !important}.to-orange-400{--tw-gradient-to: #fb923c var(--tw-gradient-to-position) !important}.to-orange-600{--tw-gradient-to: #ea580c var(--tw-gradient-to-position) !important}.to-pink-400{--tw-gradient-to: #f472b6 var(--tw-gradient-to-position) !important}.to-pink-600{--tw-gradient-to: #db2777 var(--tw-gradient-to-position) !important}.to-purple-400{--tw-gradient-to: #c084fc var(--tw-gradient-to-position) !important}.to-purple-700{--tw-gradient-to: #7e22ce var(--tw-gradient-to-position) !important}.to-red-500{--tw-gradient-to: #ef4444 var(--tw-gradient-to-position) !important}.to-red-600{--tw-gradient-to: #dc2626 var(--tw-gradient-to-position) !important}.to-rose-800{--tw-gradient-to: #9f1239 var(--tw-gradient-to-position) !important}.to-sky-900{--tw-gradient-to: #0c4a6e var(--tw-gradient-to-position) !important}.to-violet-600{--tw-gradient-to: #7c3aed var(--tw-gradient-to-position) !important}.to-violet-900{--tw-gradient-to: #4c1d95 var(--tw-gradient-to-position) !important}.to-yellow-300{--tw-gradient-to: #fde047 var(--tw-gradient-to-position) !important}.to-yellow-400{--tw-gradient-to: #facc15 var(--tw-gradient-to-position) !important}.to-yellow-500{--tw-gradient-to: #eab308 var(--tw-gradient-to-position) !important}.to-yellow-700{--tw-gradient-to: #a16207 var(--tw-gradient-to-position) !important}.fill-almost-medium-blue{fill:var(--almost-medium-blue)!important}.fill-build-trigger{fill:var(--build-trigger)!important}.fill-current{fill:currentColor!important}.fill-destructive{fill:hsl(var(--destructive))!important}.fill-foreground{fill:hsl(var(--foreground))!important}.stroke-build-trigger{stroke:var(--build-trigger)!important}.stroke-connection{stroke:var(--connection)!important}.stroke-destructive{stroke:hsl(var(--destructive))!important}.stroke-foreground{stroke:hsl(var(--foreground))!important}.stroke-gray-800{stroke:#1f2937!important}.stroke-gray-900{stroke:#111827!important}.stroke-1{stroke-width:1!important}.stroke-\[1\.5\]{stroke-width:1.5!important}.p-0{padding:0!important}.p-0\.5{padding:.125rem!important}.p-1{padding:.25rem!important}.p-1\.5{padding:.375rem!important}.p-2{padding:.5rem!important}.p-2\.5{padding:.625rem!important}.p-3{padding:.75rem!important}.p-4{padding:1rem!important}.p-6{padding:1.5rem!important}.p-8{padding:2rem!important}.px-0{padding-left:0!important;padding-right:0!important}.px-0\.5{padding-left:.125rem!important;padding-right:.125rem!important}.px-1{padding-left:.25rem!important;padding-right:.25rem!important}.px-16{padding-left:4rem!important;padding-right:4rem!important}.px-2{padding-left:.5rem!important;padding-right:.5rem!important}.px-2\.5{padding-left:.625rem!important;padding-right:.625rem!important}.px-3{padding-left:.75rem!important;padding-right:.75rem!important}.px-4{padding-left:1rem!important;padding-right:1rem!important}.px-5{padding-left:1.25rem!important;padding-right:1.25rem!important}.px-6{padding-left:1.5rem!important;padding-right:1.5rem!important}.px-8{padding-left:2rem!important;padding-right:2rem!important}.py-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-1\.5{padding-top:.375rem!important;padding-bottom:.375rem!important}.py-12{padding-top:3rem!important;padding-bottom:3rem!important}.py-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-3{padding-top:.75rem!important;padding-bottom:.75rem!important}.py-4{padding-top:1rem!important;padding-bottom:1rem!important}.py-5{padding-top:1.25rem!important;padding-bottom:1.25rem!important}.py-6{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-8{padding-top:2rem!important;padding-bottom:2rem!important}.pb-16{padding-bottom:4rem!important}.pb-2{padding-bottom:.5rem!important}.pb-4{padding-bottom:1rem!important}.pb-5{padding-bottom:1.25rem!important}.pb-8{padding-bottom:2rem!important}.pl-1{padding-left:.25rem!important}.pl-2{padding-left:.5rem!important}.pl-3{padding-left:.75rem!important}.pl-5{padding-left:1.25rem!important}.pl-8{padding-left:2rem!important}.pr-1{padding-right:.25rem!important}.pr-10{padding-right:2.5rem!important}.pr-12{padding-right:3rem!important}.pr-2{padding-right:.5rem!important}.pr-3{padding-right:.75rem!important}.pr-8{padding-right:2rem!important}.ps-2{padding-inline-start:.5rem!important}.pt-0{padding-top:0!important}.pt-2{padding-top:.5rem!important}.pt-3{padding-top:.75rem!important}.text-left{text-align:left!important}.text-center{text-align:center!important}.text-right{text-align:right!important}.text-start{text-align:start!important}.text-end{text-align:end!important}.align-middle{vertical-align:middle!important}.font-sans{font-family:var(--font-sans),ui-sans-serif,system-ui,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji"!important}.\!text-xs{font-size:.75rem!important;line-height:1rem!important}.text-2xl{font-size:1.5rem!important;line-height:2rem!important}.text-3xl{font-size:1.875rem!important;line-height:2.25rem!important}.text-5xl{font-size:3rem!important;line-height:1!important}.text-\[16px\]{font-size:16px!important}.text-\[8px\]{font-size:8px!important}.text-base{font-size:1rem!important;line-height:1.5rem!important}.text-lg{font-size:1.125rem!important;line-height:1.75rem!important}.text-sm{font-size:.875rem!important;line-height:1.25rem!important}.text-xl{font-size:1.25rem!important;line-height:1.75rem!important}.text-xs{font-size:.75rem!important;line-height:1rem!important}.\!font-normal{font-weight:400!important}.font-bold{font-weight:700!important}.font-light{font-weight:300!important}.font-medium{font-weight:500!important}.font-normal{font-weight:400!important}.font-semibold{font-weight:600!important}.italic{font-style:italic!important}.leading-none{line-height:1!important}.leading-tight{line-height:1.25!important}.tracking-tight{letter-spacing:-.025em!important}.tracking-widest{letter-spacing:.1em!important}.\!text-foreground{color:hsl(var(--foreground))!important}.text-almost-medium-blue{color:var(--almost-medium-blue)!important}.text-background{color:hsl(var(--background))!important}.text-black{--tw-text-opacity: 1 !important;color:rgb(0 0 0 / var(--tw-text-opacity))!important}.text-build-trigger{color:var(--build-trigger)!important}.text-card-foreground{color:hsl(var(--card-foreground))!important}.text-component-icon{color:var(--component-icon)!important}.text-current{color:currentColor!important}.text-destructive{color:hsl(var(--destructive))!important}.text-destructive-foreground{color:hsl(var(--destructive-foreground))!important}.text-error-foreground{color:var(--error-foreground)!important}.text-flow-icon{color:var(--flow-icon)!important}.text-foreground{color:hsl(var(--foreground))!important}.text-gray-500{--tw-text-opacity: 1 !important;color:rgb(107 114 128 / var(--tw-text-opacity))!important}.text-gray-800{--tw-text-opacity: 1 !important;color:rgb(31 41 55 / var(--tw-text-opacity))!important}.text-high-indigo{color:var(--high-indigo)!important}.text-info-foreground{color:var(--info-foreground)!important}.text-muted{color:hsl(var(--muted))!important}.text-muted-foreground{color:hsl(var(--muted-foreground))!important}.text-popover-foreground{color:hsl(var(--popover-foreground))!important}.text-primary{color:hsl(var(--primary))!important}.text-primary-foreground{color:hsl(var(--primary-foreground))!important}.text-primary\/80{color:hsl(var(--primary) / .8)!important}.text-ring{color:hsl(var(--ring))!important}.text-secondary-foreground{color:hsl(var(--secondary-foreground))!important}.text-status-blue{color:var(--status-blue)!important}.text-status-green{color:var(--status-green)!important}.text-status-red{color:var(--status-red)!important}.text-success-foreground{color:var(--success-foreground)!important}.underline{text-decoration-line:underline!important}.underline-offset-4{text-underline-offset:4px!important}.\!opacity-100{opacity:1!important}.opacity-0{opacity:0!important}.opacity-100{opacity:1!important}.opacity-50{opacity:.5!important}.opacity-60{opacity:.6!important}.opacity-70{opacity:.7!important}.\!shadow-md{--tw-shadow: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow-inner{--tw-shadow: inset 0 2px 4px 0 rgb(0 0 0 / .05) !important;--tw-shadow-colored: inset 0 2px 4px 0 var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow-lg{--tw-shadow: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow-md{--tw-shadow: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow-sm{--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05) !important;--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow-xl{--tw-shadow: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.outline-none{outline:2px solid transparent!important;outline-offset:2px!important}.outline{outline-style:solid!important}.outline-1{outline-width:1px!important}.outline-ring{outline-color:hsl(var(--ring))!important}.ring-0{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(0px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.ring-1{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.ring-2{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.ring-inset{--tw-ring-inset: inset !important}.ring-primary{--tw-ring-color: hsl(var(--primary)) !important}.ring-ring{--tw-ring-color: hsl(var(--ring)) !important}.ring-offset-background{--tw-ring-offset-color: hsl(var(--background)) !important}.blur{--tw-blur: blur(8px) !important;filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)!important}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)!important}.backdrop-blur-sm{--tw-backdrop-blur: blur(4px) !important;-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)!important;backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)!important}.transition{transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter!important;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter!important;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter!important;transition-timing-function:cubic-bezier(.4,0,.2,1)!important;transition-duration:.15s!important}.transition-all{transition-property:all!important;transition-timing-function:cubic-bezier(.4,0,.2,1)!important;transition-duration:.15s!important}.transition-colors{transition-property:color,background-color,border-color,text-decoration-color,fill,stroke!important;transition-timing-function:cubic-bezier(.4,0,.2,1)!important;transition-duration:.15s!important}.transition-opacity{transition-property:opacity!important;transition-timing-function:cubic-bezier(.4,0,.2,1)!important;transition-duration:.15s!important}.transition-transform{transition-property:transform!important;transition-timing-function:cubic-bezier(.4,0,.2,1)!important;transition-duration:.15s!important}.delay-500{transition-delay:.5s!important}.duration-100{transition-duration:.1s!important}.duration-200{transition-duration:.2s!important}.duration-300{transition-duration:.3s!important}.duration-500{transition-duration:.5s!important}.ease-in{transition-timing-function:cubic-bezier(.4,0,1,1)!important}.ease-in-out{transition-timing-function:cubic-bezier(.4,0,.2,1)!important}.ease-out{transition-timing-function:cubic-bezier(0,0,.2,1)!important}@keyframes enter{0%{opacity:var(--tw-enter-opacity, 1);transform:translate3d(var(--tw-enter-translate-x, 0),var(--tw-enter-translate-y, 0),0) scale3d(var(--tw-enter-scale, 1),var(--tw-enter-scale, 1),var(--tw-enter-scale, 1)) rotate(var(--tw-enter-rotate, 0))}}@keyframes exit{to{opacity:var(--tw-exit-opacity, 1);transform:translate3d(var(--tw-exit-translate-x, 0),var(--tw-exit-translate-y, 0),0) scale3d(var(--tw-exit-scale, 1),var(--tw-exit-scale, 1),var(--tw-exit-scale, 1)) rotate(var(--tw-exit-rotate, 0))}}.animate-in{animation-name:enter!important;animation-duration:.15s!important;--tw-enter-opacity: initial !important;--tw-enter-scale: initial !important;--tw-enter-rotate: initial !important;--tw-enter-translate-x: initial !important;--tw-enter-translate-y: initial !important}.fade-in-50{--tw-enter-opacity: .5 !important}.slide-in-from-top-1{--tw-enter-translate-y: -.25rem !important}.duration-100{animation-duration:.1s!important}.duration-200{animation-duration:.2s!important}.duration-300{animation-duration:.3s!important}.duration-500{animation-duration:.5s!important}.delay-500{animation-delay:.5s!important}.ease-in{animation-timing-function:cubic-bezier(.4,0,1,1)!important}.ease-in-out{animation-timing-function:cubic-bezier(.4,0,.2,1)!important}.ease-out{animation-timing-function:cubic-bezier(0,0,.2,1)!important}.scrollbar-hide{-ms-overflow-style:none!important;scrollbar-width:none!important}.scrollbar-hide::-webkit-scrollbar{display:none!important}.truncate-multiline{display:-webkit-box!important;-webkit-line-clamp:3!important;-webkit-box-orient:vertical!important;overflow:hidden!important;text-overflow:ellipsis!important}.truncate-doubleline{display:-webkit-box!important;-webkit-line-clamp:2!important;-webkit-box-orient:vertical!important;overflow:hidden!important;text-overflow:ellipsis!important}.word-break-break-word{word-break:break-word!important}.password{-webkit-text-security:disc!important;font-family:text-security-disc!important}.stop{animation-play-state:paused!important}.custom-scroll::-webkit-scrollbar{width:8px!important;height:8px!important}.custom-scroll::-webkit-scrollbar-track{background-color:#f1f1f1!important}.custom-scroll::-webkit-scrollbar-thumb{background-color:#ccc!important;border-radius:999px!important}.custom-scroll::-webkit-scrollbar-thumb:hover{background-color:#bbb!important}.custom-scroll{cursor:auto!important}.\!dark .theme-attribution .react-flow__attribution,.dark .theme-attribution .react-flow__attribution{background-color:#fff3!important;padding:0 5px!important}.\!dark .theme-attribution .react-flow__attribution a,.dark .theme-attribution .react-flow__attribution a{color:#000!important}.text-align-last-left{text-align-last:left!important}@keyframes slideDown{0%{height:0}to{height:var(--radix-accordion-content-height)}}@keyframes slideUp{0%{height:var(--radix-accordion-content-height)}to{height:0}}@keyframes gradient-motion-start{0%{stop-color:#9c8aec}50%{stop-color:#ff82b8}80%{stop-color:#ffa564}to{stop-color:#9c8aec}}@keyframes gradient-motion-end{0%{stop-color:#9c8aec}50%{stop-color:#ffa564}80%{stop-color:#ff82b8}to{stop-color:#9c8aec}}.data-\[invalid\]\:label-invalid[data-invalid]{color:hsl(var(--destructive))}:is(.dark .dark\:prose-invert){--tw-prose-body: var(--tw-prose-invert-body);--tw-prose-headings: var(--tw-prose-invert-headings);--tw-prose-lead: var(--tw-prose-invert-lead);--tw-prose-links: var(--tw-prose-invert-links);--tw-prose-bold: var(--tw-prose-invert-bold);--tw-prose-counters: var(--tw-prose-invert-counters);--tw-prose-bullets: var(--tw-prose-invert-bullets);--tw-prose-hr: var(--tw-prose-invert-hr);--tw-prose-quotes: var(--tw-prose-invert-quotes);--tw-prose-quote-borders: var(--tw-prose-invert-quote-borders);--tw-prose-captions: var(--tw-prose-invert-captions);--tw-prose-kbd: var(--tw-prose-invert-kbd);--tw-prose-kbd-shadows: var(--tw-prose-invert-kbd-shadows);--tw-prose-code: var(--tw-prose-invert-code);--tw-prose-pre-code: var(--tw-prose-invert-pre-code);--tw-prose-pre-bg: var(--tw-prose-invert-pre-bg);--tw-prose-th-borders: var(--tw-prose-invert-th-borders);--tw-prose-td-borders: var(--tw-prose-invert-td-borders)}.placeholder\:text-muted-foreground::placeholder{color:hsl(var(--muted-foreground))!important}.hover\:scale-110:hover{--tw-scale-x: 1.1 !important;--tw-scale-y: 1.1 !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.hover\:border-border:hover{border-color:hsl(var(--border))!important}.hover\:bg-accent:hover{background-color:hsl(var(--accent))!important}.hover\:bg-beta-foreground:hover{background-color:var(--beta-foreground)!important}.hover\:bg-border\/80:hover{background-color:hsl(var(--border) / .8)!important}.hover\:bg-destructive\/80:hover{background-color:hsl(var(--destructive) / .8)!important}.hover\:bg-destructive\/90:hover{background-color:hsl(var(--destructive) / .9)!important}.hover\:bg-error-foreground:hover{background-color:var(--error-foreground)!important}.hover\:bg-muted:hover{background-color:hsl(var(--muted))!important}.hover\:bg-muted\/50:hover{background-color:hsl(var(--muted) / .5)!important}.hover\:bg-primary\/80:hover{background-color:hsl(var(--primary) / .8)!important}.hover\:bg-primary\/90:hover{background-color:hsl(var(--primary) / .9)!important}.hover\:bg-ring:hover{background-color:hsl(var(--ring))!important}.hover\:bg-secondary-foreground\/5:hover{background-color:hsl(var(--secondary-foreground) / .05)!important}.hover\:bg-secondary\/80:hover{background-color:hsl(var(--secondary) / .8)!important}.hover\:bg-status-red:hover{background-color:var(--status-red)!important}.hover\:bg-transparent:hover{background-color:transparent!important}.hover\:text-accent-foreground:hover{color:hsl(var(--accent-foreground))!important}.hover\:text-destructive:hover{color:hsl(var(--destructive))!important}.hover\:text-gray-600:hover{--tw-text-opacity: 1 !important;color:rgb(75 85 99 / var(--tw-text-opacity))!important}.hover\:text-indigo-500:hover{--tw-text-opacity: 1 !important;color:rgb(99 102 241 / var(--tw-text-opacity))!important}.hover\:text-muted-foreground:hover{color:hsl(var(--muted-foreground))!important}.hover\:text-primary:hover{color:hsl(var(--primary))!important}.hover\:text-status-red:hover{color:var(--status-red)!important}.hover\:underline:hover{text-decoration-line:underline!important}.hover\:opacity-100:hover{opacity:1!important}.hover\:shadow-lg:hover{--tw-shadow: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.hover\:shadow-md:hover{--tw-shadow: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.hover\:shadow-sm:hover{--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05) !important;--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.hover\:outline:hover{outline-style:solid!important}.focus\:z-10:focus{z-index:10!important}.focus\:border-none:focus{border-style:none!important}.focus\:bg-accent:focus{background-color:hsl(var(--accent))!important}.focus\:text-accent-foreground:focus{color:hsl(var(--accent-foreground))!important}.focus\:outline-none:focus{outline:2px solid transparent!important;outline-offset:2px!important}.focus\:outline:focus{outline-style:solid!important}.focus\:ring-1:focus{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.focus\:ring-2:focus{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.focus\:ring-ring:focus{--tw-ring-color: hsl(var(--ring)) !important}.focus\:ring-offset-1:focus{--tw-ring-offset-width: 1px !important}.focus\:ring-offset-2:focus{--tw-ring-offset-width: 2px !important}.focus-visible\:outline-none:focus-visible{outline:2px solid transparent!important;outline-offset:2px!important}.focus-visible\:outline-0:focus-visible{outline-width:0px!important}.focus-visible\:ring-1:focus-visible{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.focus-visible\:ring-2:focus-visible{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.focus-visible\:ring-ring:focus-visible{--tw-ring-color: hsl(var(--ring)) !important}.focus-visible\:ring-offset-2:focus-visible{--tw-ring-offset-width: 2px !important}.focus-visible\:ring-offset-background:focus-visible{--tw-ring-offset-color: hsl(var(--background)) !important}.active\:outline:active{outline-style:solid!important}.disabled\:pointer-events-none:disabled{pointer-events:none!important}.disabled\:cursor-not-allowed:disabled{cursor:not-allowed!important}.disabled\:opacity-50:disabled{opacity:.5!important}.group:hover .group-hover\:opacity-100{opacity:1!important}.peer:disabled~.peer-disabled\:cursor-not-allowed{cursor:not-allowed!important}.peer:disabled~.peer-disabled\:opacity-70{opacity:.7!important}.aria-disabled\:bg-muted\/70[aria-disabled=true]{background-color:hsl(var(--muted) / .7)!important}.aria-selected\:bg-accent[aria-selected=true]{background-color:hsl(var(--accent))!important}.aria-selected\:text-accent-foreground[aria-selected=true]{color:hsl(var(--accent-foreground))!important}.data-\[disabled\]\:pointer-events-none[data-disabled]{pointer-events:none!important}.data-\[side\=bottom\]\:translate-y-1[data-side=bottom]{--tw-translate-y: .25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[side\=left\]\:-translate-x-1[data-side=left]{--tw-translate-x: -.25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[side\=right\]\:translate-x-1[data-side=right]{--tw-translate-x: .25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[side\=top\]\:-translate-y-1[data-side=top]{--tw-translate-y: -.25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[state\=checked\]\:translate-x-5[data-state=checked]{--tw-translate-x: 1.25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[state\=unchecked\]\:translate-x-0[data-state=unchecked]{--tw-translate-x: 0px !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[state\=active\]\:border[data-state=active],.data-\[state\=inactive\]\:border[data-state=inactive]{border-width:1px!important}.data-\[state\=inactive\]\:border-muted[data-state=inactive]{border-color:hsl(var(--muted))!important}.data-\[state\=active\]\:bg-background[data-state=active]{background-color:hsl(var(--background))!important}.data-\[state\=active\]\:bg-primary-foreground[data-state=active]{background-color:hsl(var(--primary-foreground))!important}.data-\[state\=checked\]\:bg-primary[data-state=checked]{background-color:hsl(var(--primary))!important}.data-\[state\=open\]\:bg-accent[data-state=open]{background-color:hsl(var(--accent))!important}.data-\[state\=selected\]\:bg-muted[data-state=selected]{background-color:hsl(var(--muted))!important}.data-\[state\=unchecked\]\:bg-ring[data-state=unchecked]{background-color:hsl(var(--ring))!important}.data-\[state\=active\]\:text-foreground[data-state=active]{color:hsl(var(--foreground))!important}.data-\[state\=checked\]\:text-primary-foreground[data-state=checked]{color:hsl(var(--primary-foreground))!important}.data-\[state\=open\]\:text-accent-foreground[data-state=open]{color:hsl(var(--accent-foreground))!important}.data-\[state\=open\]\:text-muted-foreground[data-state=open]{color:hsl(var(--muted-foreground))!important}.data-\[disabled\]\:opacity-50[data-disabled]{opacity:.5!important}.data-\[state\=active\]\:shadow-sm[data-state=active]{--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05) !important;--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.data-\[state\=open\]\:animate-in[data-state=open]{animation-name:enter!important;animation-duration:.15s!important;--tw-enter-opacity: initial !important;--tw-enter-scale: initial !important;--tw-enter-rotate: initial !important;--tw-enter-translate-x: initial !important;--tw-enter-translate-y: initial !important}.data-\[state\=closed\]\:animate-out[data-state=closed]{animation-name:exit!important;animation-duration:.15s!important;--tw-exit-opacity: initial !important;--tw-exit-scale: initial !important;--tw-exit-rotate: initial !important;--tw-exit-translate-x: initial !important;--tw-exit-translate-y: initial !important}.data-\[state\=closed\]\:fade-out-0[data-state=closed]{--tw-exit-opacity: 0 !important}.data-\[state\=open\]\:fade-in-0[data-state=open]{--tw-enter-opacity: 0 !important}.data-\[state\=closed\]\:zoom-out-95[data-state=closed]{--tw-exit-scale: .95 !important}.data-\[state\=open\]\:zoom-in-95[data-state=open]{--tw-enter-scale: .95 !important}.data-\[side\=bottom\]\:slide-in-from-top-1[data-side=bottom]{--tw-enter-translate-y: -.25rem !important}.data-\[side\=bottom\]\:slide-in-from-top-2[data-side=bottom]{--tw-enter-translate-y: -.5rem !important}.data-\[side\=left\]\:slide-in-from-right-1[data-side=left]{--tw-enter-translate-x: .25rem !important}.data-\[side\=left\]\:slide-in-from-right-2[data-side=left]{--tw-enter-translate-x: .5rem !important}.data-\[side\=right\]\:slide-in-from-left-1[data-side=right]{--tw-enter-translate-x: -.25rem !important}.data-\[side\=right\]\:slide-in-from-left-2[data-side=right]{--tw-enter-translate-x: -.5rem !important}.data-\[side\=top\]\:slide-in-from-bottom-1[data-side=top]{--tw-enter-translate-y: .25rem !important}.data-\[side\=top\]\:slide-in-from-bottom-2[data-side=top]{--tw-enter-translate-y: .5rem !important}.data-\[state\=closed\]\:slide-out-to-left-1\/2[data-state=closed]{--tw-exit-translate-x: -50% !important}.data-\[state\=closed\]\:slide-out-to-top-\[48\%\][data-state=closed]{--tw-exit-translate-y: -48% !important}.data-\[state\=open\]\:slide-in-from-left-1\/2[data-state=open]{--tw-enter-translate-x: -50% !important}.data-\[state\=open\]\:slide-in-from-top-\[48\%\][data-state=open]{--tw-enter-translate-y: -48% !important}.data-\[state\=inactive\]\:hover\:bg-secondary\/80:hover[data-state=inactive]{background-color:hsl(var(--secondary) / .8)!important}:is(.dark .dark\:border-gray-600){--tw-border-opacity: 1 !important;border-color:rgb(75 85 99 / var(--tw-border-opacity))!important}:is(.dark .dark\:border-b-muted){border-bottom-color:hsl(var(--muted))!important}:is(.dark .dark\:text-gray-300){--tw-text-opacity: 1 !important;color:rgb(209 213 219 / var(--tw-text-opacity))!important}:is(.dark .dark\:text-white){color:var(--white)!important}:is(.dark .dark\:hover\:bg-background\/10:hover){background-color:hsl(var(--background) / .1)!important}@media (min-width: 640px){.sm\:flex-row{flex-direction:row!important}.sm\:items-center{align-items:center!important}.sm\:justify-end{justify-content:flex-end!important}.sm\:space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(.5rem * var(--tw-space-x-reverse))!important;margin-left:calc(.5rem * calc(1 - var(--tw-space-x-reverse)))!important}.sm\:rounded-lg{border-radius:var(--radius)!important}.sm\:px-3{padding-left:.75rem!important;padding-right:.75rem!important}.sm\:text-left{text-align:left!important}}@media (min-width: 768px){.md\:ml-6{margin-left:1.5rem!important}.md\:mt-0{margin-top:0!important}.md\:block{display:block!important}.md\:flex{display:flex!important}.md\:w-full{width:100%!important}.md\:grid-cols-2{grid-template-columns:repeat(2,minmax(0,1fr))!important}.md\:justify-between{justify-content:space-between!important}}@media (min-width: 1024px){.lg\:block{display:block!important}.lg\:flex{display:flex!important}.lg\:w-1\/5{width:20%!important}.lg\:w-\[30\%\]{width:30%!important}.lg\:grid-cols-2{grid-template-columns:repeat(2,minmax(0,1fr))!important}.lg\:grid-cols-3{grid-template-columns:repeat(3,minmax(0,1fr))!important}.lg\:flex-row{flex-direction:row!important}.lg\:flex-col{flex-direction:column!important}.lg\:space-x-0>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(0px * var(--tw-space-x-reverse))!important;margin-left:calc(0px * calc(1 - var(--tw-space-x-reverse)))!important}.lg\:space-x-8>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(2rem * var(--tw-space-x-reverse))!important;margin-left:calc(2rem * calc(1 - var(--tw-space-x-reverse)))!important}.lg\:space-y-0>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(0px * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(0px * var(--tw-space-y-reverse))!important}.lg\:space-y-1>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(.25rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(.25rem * var(--tw-space-y-reverse))!important}}.\[\&\:has\(\[role\=checkbox\]\)\]\:pr-0:has([role=checkbox]){padding-right:0!important}.\[\&\>button\]\:border-b-border>button{border-bottom-color:hsl(var(--border))!important}.hover\:\[\&\>button\]\:bg-border>button:hover{background-color:hsl(var(--border))!important}.\[\&\[data-state\=open\]\>svg\]\:rotate-180[data-state=open]>svg{--tw-rotate: 180deg !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.\[\&_\[cmdk-group-heading\]\]\:px-2 [cmdk-group-heading]{padding-left:.5rem!important;padding-right:.5rem!important}.\[\&_\[cmdk-group-heading\]\]\:py-1\.5 [cmdk-group-heading]{padding-top:.375rem!important;padding-bottom:.375rem!important}.\[\&_\[cmdk-group-heading\]\]\:text-xs [cmdk-group-heading]{font-size:.75rem!important;line-height:1rem!important}.\[\&_\[cmdk-group-heading\]\]\:font-medium [cmdk-group-heading]{font-weight:500!important}.\[\&_\[cmdk-group-heading\]\]\:text-muted-foreground [cmdk-group-heading]{color:hsl(var(--muted-foreground))!important}.\[\&_\[cmdk-group\]\:not\(\[hidden\]\)_\~\[cmdk-group\]\]\:pt-0 [cmdk-group]:not([hidden])~[cmdk-group]{padding-top:0!important}.\[\&_\[cmdk-group\]\]\:px-2 [cmdk-group]{padding-left:.5rem!important;padding-right:.5rem!important}.\[\&_\[cmdk-input-wrapper\]_svg\]\:h-5 [cmdk-input-wrapper] svg{height:1.25rem!important}.\[\&_\[cmdk-input-wrapper\]_svg\]\:w-5 [cmdk-input-wrapper] svg{width:1.25rem!important}.\[\&_\[cmdk-input\]\]\:h-12 [cmdk-input]{height:3rem!important}.\[\&_\[cmdk-item\]\]\:px-2 [cmdk-item]{padding-left:.5rem!important;padding-right:.5rem!important}.\[\&_\[cmdk-item\]\]\:py-3 [cmdk-item]{padding-top:.75rem!important;padding-bottom:.75rem!important}.\[\&_\[cmdk-item\]_svg\]\:h-5 [cmdk-item] svg{height:1.25rem!important}.\[\&_\[cmdk-item\]_svg\]\:w-5 [cmdk-item] svg{width:1.25rem!important}.\[\&_tr\:last-child\]\:border-0 tr:last-child{border-width:0px!important}.\[\&_tr\]\:border-b tr{border-bottom-width:1px!important}body{margin:0;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}code{font-family:source-code-pro,Menlo,Monaco,Consolas,Courier New,monospace}pre{font-family:inherit}.react-flow__pane{cursor:default}.AccordionContent{overflow:hidden}.AccordionContent[data-state=open]{animation:slideDown .3s ease-out}.AccordionContent[data-state=closed]{animation:slideUp .3s ease-out}.gradient-end{animation:gradient-motion-end 3s infinite forwards}.gradient-start{animation:gradient-motion-start 4s infinite forwards}input:-webkit-autofill,input:-webkit-autofill:hover,input:-webkit-autofill:focus,textarea:-webkit-autofill,textarea:-webkit-autofill:hover,textarea:-webkit-autofill:focus,select:-webkit-autofill,select:-webkit-autofill:hover,select:-webkit-autofill:focus{-webkit-text-fill-color:black;box-shadow:0 0 0 1000px #fff6d0 inset;color:#000}.ace_scrollbar::-webkit-scrollbar{height:8px;width:8px}.ace_scrollbar::-webkit-scrollbar-track{background-color:#f1f1f1}.ace_scrollbar::-webkit-scrollbar-thumb{background-color:#ccc;border-radius:999px}.ace_scrollbar::-webkit-scrollbar-thumb:hover{background-color:#bbb;border-radius:999px}
+.react-flow__container{position:absolute;width:100%;height:100%;top:0;left:0}.react-flow__pane{z-index:1;cursor:grab}.react-flow__pane.selection{cursor:pointer}.react-flow__pane.dragging{cursor:grabbing}.react-flow__viewport{transform-origin:0 0;z-index:2;pointer-events:none}.react-flow__renderer{z-index:4}.react-flow__selection{z-index:6}.react-flow__nodesselection-rect:focus,.react-flow__nodesselection-rect:focus-visible{outline:none}.react-flow .react-flow__edges{pointer-events:none;overflow:visible}.react-flow__edge-path,.react-flow__connection-path{stroke:#b1b1b7;stroke-width:1;fill:none}.react-flow__edge{pointer-events:visibleStroke;cursor:pointer}.react-flow__edge.animated path{stroke-dasharray:5;animation:dashdraw .5s linear infinite}.react-flow__edge.animated path.react-flow__edge-interaction{stroke-dasharray:none;animation:none}.react-flow__edge.inactive{pointer-events:none}.react-flow__edge.selected,.react-flow__edge:focus,.react-flow__edge:focus-visible{outline:none}.react-flow__edge.selected .react-flow__edge-path,.react-flow__edge:focus .react-flow__edge-path,.react-flow__edge:focus-visible .react-flow__edge-path{stroke:#555}.react-flow__edge-textwrapper{pointer-events:all}.react-flow__edge-textbg{fill:#fff}.react-flow__edge .react-flow__edge-text{pointer-events:none;-webkit-user-select:none;user-select:none}.react-flow__connection{pointer-events:none}.react-flow__connection .animated{stroke-dasharray:5;animation:dashdraw .5s linear infinite}.react-flow__connectionline{z-index:1001}.react-flow__nodes{pointer-events:none;transform-origin:0 0}.react-flow__node{position:absolute;-webkit-user-select:none;user-select:none;pointer-events:all;transform-origin:0 0;box-sizing:border-box;cursor:grab}.react-flow__node.dragging{cursor:grabbing}.react-flow__nodesselection{z-index:3;transform-origin:left top;pointer-events:none}.react-flow__nodesselection-rect{position:absolute;pointer-events:all;cursor:grab}.react-flow__handle{position:absolute;pointer-events:none;min-width:5px;min-height:5px;width:6px;height:6px;background:#1a192b;border:1px solid white;border-radius:100%}.react-flow__handle.connectionindicator{pointer-events:all;cursor:crosshair}.react-flow__handle-bottom{top:auto;left:50%;bottom:-4px;transform:translate(-50%)}.react-flow__handle-top{left:50%;top:-4px;transform:translate(-50%)}.react-flow__handle-left{top:50%;left:-4px;transform:translateY(-50%)}.react-flow__handle-right{right:-4px;top:50%;transform:translateY(-50%)}.react-flow__edgeupdater{cursor:move;pointer-events:all}.react-flow__panel{position:absolute;z-index:5;margin:15px}.react-flow__panel.top{top:0}.react-flow__panel.bottom{bottom:0}.react-flow__panel.left{left:0}.react-flow__panel.right{right:0}.react-flow__panel.center{left:50%;transform:translate(-50%)}.react-flow__attribution{font-size:10px;background:rgba(255,255,255,.5);padding:2px 3px;margin:0}.react-flow__attribution a{text-decoration:none;color:#999}@keyframes dashdraw{0%{stroke-dashoffset:10}}.react-flow__edgelabel-renderer{position:absolute;width:100%;height:100%;pointer-events:none;-webkit-user-select:none;user-select:none}.react-flow__edge.updating .react-flow__edge-path{stroke:#777}.react-flow__edge-text{font-size:10px}.react-flow__node.selectable:focus,.react-flow__node.selectable:focus-visible{outline:none}.react-flow__node-default,.react-flow__node-input,.react-flow__node-output,.react-flow__node-group{padding:10px;border-radius:3px;width:150px;font-size:12px;color:#222;text-align:center;border-width:1px;border-style:solid;border-color:#1a192b;background-color:#fff}.react-flow__node-default.selectable:hover,.react-flow__node-input.selectable:hover,.react-flow__node-output.selectable:hover,.react-flow__node-group.selectable:hover{box-shadow:0 1px 4px 1px #00000014}.react-flow__node-default.selectable.selected,.react-flow__node-default.selectable:focus,.react-flow__node-default.selectable:focus-visible,.react-flow__node-input.selectable.selected,.react-flow__node-input.selectable:focus,.react-flow__node-input.selectable:focus-visible,.react-flow__node-output.selectable.selected,.react-flow__node-output.selectable:focus,.react-flow__node-output.selectable:focus-visible,.react-flow__node-group.selectable.selected,.react-flow__node-group.selectable:focus,.react-flow__node-group.selectable:focus-visible{box-shadow:0 0 0 .5px #1a192b}.react-flow__node-group{background-color:#f0f0f040}.react-flow__nodesselection-rect,.react-flow__selection{background:rgba(0,89,220,.08);border:1px dotted rgba(0,89,220,.8)}.react-flow__nodesselection-rect:focus,.react-flow__nodesselection-rect:focus-visible,.react-flow__selection:focus,.react-flow__selection:focus-visible{outline:none}.react-flow__controls{box-shadow:0 0 2px 1px #00000014}.react-flow__controls-button{border:none;background:#fefefe;border-bottom:1px solid #eee;box-sizing:content-box;display:flex;justify-content:center;align-items:center;width:16px;height:16px;cursor:pointer;-webkit-user-select:none;user-select:none;padding:5px}.react-flow__controls-button:hover{background:#f4f4f4}.react-flow__controls-button svg{width:100%;max-width:12px;max-height:12px}.react-flow__controls-button:disabled{pointer-events:none}.react-flow__controls-button:disabled svg{fill-opacity:.4}.react-flow__minimap{background-color:#fff}.react-flow__resize-control{position:absolute}.react-flow__resize-control.left,.react-flow__resize-control.right{cursor:ew-resize}.react-flow__resize-control.top,.react-flow__resize-control.bottom{cursor:ns-resize}.react-flow__resize-control.top.left,.react-flow__resize-control.bottom.right{cursor:nwse-resize}.react-flow__resize-control.bottom.left,.react-flow__resize-control.top.right{cursor:nesw-resize}.react-flow__resize-control.handle{width:4px;height:4px;border:1px solid #fff;border-radius:1px;background-color:#3367d9;transform:translate(-50%,-50%)}.react-flow__resize-control.handle.left{left:0;top:50%}.react-flow__resize-control.handle.right{left:100%;top:50%}.react-flow__resize-control.handle.top{left:50%;top:0}.react-flow__resize-control.handle.bottom{left:50%;top:100%}.react-flow__resize-control.handle.top.left,.react-flow__resize-control.handle.bottom.left{left:0}.react-flow__resize-control.handle.top.right,.react-flow__resize-control.handle.bottom.right{left:100%}.react-flow__resize-control.line{border-color:#3367d9;border-width:0;border-style:solid}.react-flow__resize-control.line.left,.react-flow__resize-control.line.right{width:1px;transform:translate(-50%);top:0;height:100%}.react-flow__resize-control.line.left{left:0;border-left-width:1px}.react-flow__resize-control.line.right{left:100%;border-right-width:1px}.react-flow__resize-control.line.top,.react-flow__resize-control.line.bottom{height:1px;transform:translateY(-50%);left:0;width:100%}.react-flow__resize-control.line.top{top:0;border-top-width:1px}.react-flow__resize-control.line.bottom{border-bottom-width:1px;top:100%}.\!loading{pointer-events:none!important;display:inline-block!important;aspect-ratio:1 / 1!important;width:1.5rem!important;background-color:currentColor!important;-webkit-mask-size:100%!important;mask-size:100%!important;-webkit-mask-repeat:no-repeat!important;mask-repeat:no-repeat!important;-webkit-mask-position:center!important;mask-position:center!important;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important;mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important}.loading{pointer-events:none;display:inline-block;aspect-ratio:1 / 1;width:1.5rem;background-color:currentColor;-webkit-mask-size:100%;mask-size:100%;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-position:center;mask-position:center;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}.loading-spinner{-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}body{overflow:hidden}.App{text-align:center}.react-flow__node{width:auto;height:auto;border-radius:auto;min-width:inherit}.App-logo{height:40vmin;pointer-events:none}@media (prefers-reduced-motion: no-preference){.App-logo{animation:App-logo-spin infinite 20s linear}}.App-header{background-color:#282c34;min-height:100vh;display:flex;flex-direction:column;align-items:center;justify-content:center;font-size:calc(10px + 2vmin);color:#fff}.App-link{color:#61dafb}@keyframes App-logo-spin{0%{transform:rotate(0)}to{transform:rotate(360deg)}}@font-face{font-family:text-security-disc;src:url(data:font/woff;base64,d09GRgABAAAAAAusAAsAAAAAMGgAAQAAAAAAAAAAAAAAAAAAAAAAAAAAAABHU1VCAAABCAAAADsAAABUIIslek9TLzIAAAFEAAAAPgAAAFZjRmM5Y21hcAAAAYQAAAgCAAArYmjjYVVnbHlmAAAJiAAAAEEAAABQiOYj2mhlYWQAAAnMAAAALgAAADYR8XmmaGhlYQAACfwAAAAcAAAAJAqNAyNobXR4AAAKGAAAAAgAAAAIAyAAAGxvY2EAAAogAAAABgAAAAYAKAAAbWF4cAAACigAAAAeAAAAIAEOACJuYW1lAAAKSAAAAUIAAAKOcN63t3Bvc3QAAAuMAAAAHQAAAC5lhHRpeJxjYGRgYOBiMGCwY2BycfMJYeDLSSzJY5BiYGGAAJA8MpsxJzM9kYEDxgPKsYBpDiBmg4gCACY7BUgAeJxjYGScwDiBgZWBgSGVtYKBgVECQjMfYEhiYmFgYGJgZWbACgLSXFMYHIAq/rNfAHK3gEmgASACAIekCT4AAHic7dhl0zDVmUXh5+XFHYK7E0IguFtwt4QQgmtwd3d3d7cED+4SXIO7u7vbsNfaUzU1fyGcu66u1adOf+6uHhgYGGpgYGDwL37/iyEHBoZZcWDQLzUw9NK/7A5if/DA8OwPOfQknBky+0P8/PPPOcd1UJ785frr/Dq/zq/z6/w3zsCgoX/xX74GRsxbcYpRB1iDB/7PGvT/DFGDenBwe8hKD1XpoSs9TKWHrfRwlR6+0iNUesRKj1TpkSs9SqVHrfRolR690r+p9BiVHrPSY1V67EqPU+lxKz1epcev9ASVnrDSE1V64kpPUulJKz1ZpSev9BSVnrLSU1V66kr/ttLTVPp3lZ62/KJSerpKT1/pP1R6hkrPWOmZKj1zpWep9KyVnq3Ss1d6jkrPWem5Kj13peep9LyVnq/S81d6gUr/sdILVnqhSi9c6UUqvWilF6v04pVeotJLVnqpSi9d6WUqvWyll6v08pVeodIrVvpPlf5zpVeq9F8qvXKl/1rpVSr9t0qvWunVKr16pdeo9JqVXqvSa1d6nUqvW+n1Kr1+pTeo9N8rvWGlN6r0xpXepNKbVnqzSm9e6S0qvWWlt6r01pXeptLbVnq7Sm9f6R0qvWOld6r0zpXepdK7Vnq3Su9e6T0qvWel96r03pXep9L7Vnq/Su9f6QMqfWClD6r0wZU+pNKHVvqwSh9e6SMqfWSlj6r00ZU+ptLHVvq4Sh9f6RMqfWKlT6r0yZU+pdKnVvq0Sp9e6TMqfWalz6r02ZU+p9LnVvq8Sp9f6QsqfWGl/1Hpf1b6okpfXOlLKn1ppS+r9OWVvqLS/6r0lZW+qtJXV/qaSl9b6esqfX2lb6j0jZW+qdI3V/qWSt9a6dsqfXul76j0vyt9Z6XvqvTdlb6n0vdW+r5K31/pByr9YKUfqvTDlX6k0v+p9KOVfqzSj1f6iUo/WemnKv10pZ+p9LOVfq7Sz1f6hUq/WOmXKv1ypV+p9KuVfq3Sr1f6jUq/Wem3Kv12pd+p9LuVfq/S71f6g0p/WOmPKv1xpT+p9KeV/qzSn1f6i0p/WemvKv11pb+p9LeV/q7S31f6h0r/WOmfKv1zDfI26KKHED1Y9JCihxI9tOhhRA8rejjRw4seQfSIokcSPbLoUUSPKno00aOL/o3oMUSPKXos0WOLHkf0uKLHEz2+6AlETyh6ItETi55E9KSiJxM9uegpRE8peirRU4v+rehpRP9O9LSify96OtHTi/6D6BlEzyh6JtEzi55F9KyiZxM9u+g5RM8pei7Rc4ueR/S8oucTPb/oBUT/UfSCohcSvbDoRUQvKnox0YuLXkL0kqKXEr206GVELyt6OdHLi15B9Iqi/yT6z6JXEv0X0SuL/qvoVUT/TfSqolcTvbroNUSvKXot0WuLXkf0uqLXE72+6A1E/130hqI3Er2x6E1Ebyp6M9Gbi95C9JaitxK9tehtRG8rejvR24veQfSOoncSvbPoXUTvKno30buL3kP0nqL3Er236H1E7yt6P9H7iz5A9IGiDxJ9sOhDRB8q+jDRh4s+QvSRoo8SfbToY0QfK/o40ceLPkH0iaJPEn2y6FNEnyr6NNGniz5D9JmizxJ9tuhzRJ8r+jzR54u+QPSFov8h+p+iLxJ9sehLRF8q+jLRl4u+QvS/RF8p+irRV4u+RvS1oq8Tfb3oG0TfKPom0TeLvkX0raJvE3276DtE/1v0naLvEn236HtE3yv6PtH3i35A9IOiHxL9sOhHRP9H9KOiHxP9uOgnRD8p+inRT4t+RvSzop8T/bzoF0S/KPol0S+LfkX0q6JfE/266DdEvyn6LdFvi35H9Lui3xP9vugPRH8o+iPRH4v+RPSnoj8T/bnoL0R/Kfor0V+L/kb0t6K/E/296B9E/yj6J9E/K/2/v/npoocQPVj0kKKHEj206GFEDyt6ONHDix5B9IiiRxI9suhRRI8qejTRo4v+jegxRI8peizRY4seR/S4oscTPb7oCURPKHoi0ROLnkT0pKInEz256ClETyl6KtFTi/6t6GlE/070tKJ/L3o60dOL/oPoGUTPKHom0TOLnkX0rKJnEz276DlEzyl6LtFzi55H9Lyi5xM9v+gFRP9R9IKiFxK9sOhFRC8qejHRi4teQvSSopcSvbToZUQvK3o50cuLXkH0iqL/JPrPolcS/RfRK4v+q+hVRP9N9KqiVxO9uug1RK8pei3Ra4teR/S6otcTvb7oDUT/XfSGojcSvbHoTURvKnoz0ZuL3kL0lqK3Er216G1Ebyt6O9Hbi95B9I6idxK9s+hdRO8qejfRu4veQ/SeovcSvbfofUTvK3o/0fuLPkD0gaIPEn2w6ENEHyr6MNGHiz5C9JGijxJ9tOhjRB8r+jjRx4s+QfSJok8SfbLoU0SfKvo00aeLPkP0maLPEn226HNEnyv6PNHni75A9IWi/yH6n6IvEn2x6EtEXyr6MtGXi75C9L9EXyn6KtFXi75G9LWirxN9vegbRN8o+ibRN4u+RfStom8TfbvoO0T/W/Sdou8Sfbfoe0TfK/o+0feLfkD0g6IfEv2w6EdE/0f0o6IfE/246CdEPyn6KdFPi35G9LOinxP9vOgXRL8o+iXRL4t+RfSrol8T/broN0S/Kfot0W+Lfkf0u6LfE/2+6A9Efyj6I9Efi/5E9KeiPxP9uegvRH8p+ivRX4v+RvS3or8T/b3oH0T/KPon0T9rYND/AOaSEScAAHicY2BiAAKmPSy+QEqUgYFRUURcTFzMyNzM3MxEXU1dTYmdjZ2NccK/K5oaLm6L3Fw0NOEMZoVAFD6IAQD4PA9iAAAAeJxjYGRgYADilrme/fH8Nl8ZuNkvAEUYbnDPcEOmmfaw+AIpDgYmEA8AHMMJGAAAeJxjYGRgYL/AAATMCiCSaQ8DIwMqYAIAK/QBvQAAAAADIAAAAAAAAAAoAAB4nGNgZGBgYGIQA2IGMIuBgQsIGRj+g/kMAArUATEAAHicjY69TsMwFIWP+4doJYSKhMTmoUJIqOnPWIm1ZWDq0IEtTZw2VRpHjlu1D8A7MPMczAw8DM/AifFEl9qS9d1zzr3XAK7xBYHqCHTdW50aLlj9cZ1057lBfvTcRAdPnlvUnz23mXj13MEN3jhBNC6p9PDuuYYrfHquU//23CD/eG7iVnQ9t9ATD57bWIgXzx3ciw+rDrZfqmhnUnvsx2kZzdVql4Xm1DhVFsqUqc7lKBiemjOVKxNaFcvlUZb71djaRCZGb+VU51ZlmZaF0RsV2WBtbTEZDBKvB5HewkLhwLePkhRhB4OU9ZFKTCqpzems6GQI6Z7TcU5mQceQUmjkkBghwPCszhmd3HWHLh+ze8mEpLvnT8dULRLWCTMaW9LUbanSGa+mUjhv47ZY7l67rgITDHiTf/mAKU76BTuXfk8AAHicY2BigAARBuyAiZGJkZmBJSWzOJmBAQALQwHHAAAA) format("woff")}.json-view{height:370px!important;background-color:#2c2c2c!important;border-radius:10px!important;padding:10px!important}.jv-indent{overflow-y:auto!important;max-height:310px!important;border-radius:10px}.jv-indent::-webkit-scrollbar{width:8px!important;height:8px!important;border-radius:10px}.jv-indent::-webkit-scrollbar-track{background-color:#f1f1f1!important;border-radius:10px}.jv-indent::-webkit-scrollbar-thumb{background-color:#ccc!important;border-radius:999px!important}.jv-indent::-webkit-scrollbar-thumb:hover{background-color:#bbb!important}:is(.dark .json-view,.dark.json-view){color:#d1d1d1;--json-property: #009033;--json-index: #5d75f2;--json-number: #5d75f2;--json-string: #c57e29;--json-boolean: #e4407b;--json-null: #e4407b}:is(.dark .json-view_a11y,.dark.json-view_a11y){color:#d1d1d1;--json-property: #ffd700;--json-index: #00e0e0;--json-number: #00e0e0;--json-string: #abe338;--json-boolean: #ffa07a;--json-null: #ffa07a}:is(.dark .json-view_github,.dark.json-view_github){color:#79b8ff;--json-property: #79b8ff;--json-index: #79b8ff;--json-number: #79b8ff;--json-string: #9ecbff;--json-boolean: #79b8ff;--json-null: #79b8ff}:is(.dark .json-view_vscode,.dark.json-view_vscode){color:orchid;--json-property: #9cdcfe;--json-index: #b5cea8;--json-number: #b5cea8;--json-string: #ce9178;--json-boolean: #569cd6;--json-null: #569cd6}:is(.dark .json-view_atom,.dark.json-view_atom){color:#abb2bf;--json-property: #e06c75;--json-index: #d19a66;--json-number: #d19a66;--json-string: #98c379;--json-boolean: #56b6c2;--json-null: #56b6c2}:is(.dark .json-view_winter-is-coming,.dark.json-view_winter-is-coming){color:#a7dbf7;--json-property: #91dacd;--json-index: #8dec95;--json-number: #8dec95;--json-string: #e0aff5;--json-boolean: #f29fd8;--json-null: #f29fd8}.json-view{display:block;color:#4d4d4d;text-align:left;--json-property: #009033;--json-index: #676dff;--json-number: #676dff;--json-string: #b2762e;--json-boolean: #dc155e;--json-null: #dc155e}.json-view .json-view--property{color:var(--json-property)}.json-view .json-view--index{color:var(--json-index)}.json-view .json-view--number{color:var(--json-number)}.json-view .json-view--string{color:var(--json-string)}.json-view .json-view--boolean{color:var(--json-boolean)}.json-view .json-view--null{color:var(--json-null)}.json-view .jv-indent{padding-left:1em}.json-view .jv-chevron{display:inline-block;vertical-align:-20%;cursor:pointer;opacity:.4;width:1em;height:1em}:is(.json-view .jv-chevron:hover,.json-view .jv-size:hover+.jv-chevron){opacity:.8}.json-view .jv-size{cursor:pointer;opacity:.4;font-size:.875em;font-style:italic;margin-left:.5em;vertical-align:-5%;line-height:1}.json-view :is(.json-view--copy,.json-view--edit),.json-view .json-view--link svg{display:none;width:1em;height:1em;margin-left:.25em;cursor:pointer}.json-view .json-view--input{width:120px;margin-left:.25em;border-radius:4px;border:1px solid currentColor;padding:0 4px;font-size:87.5%;line-height:1.25;background:transparent}.json-view .json-view--deleting{outline:1px solid #da0000;background-color:#da000011;text-decoration-line:line-through}:is(.json-view:hover,.json-view--pair:hover)>:is(.json-view--copy,.json-view--edit),:is(.json-view:hover,.json-view--pair:hover)>.json-view--link svg{display:inline-block}.json-view .jv-button{background:transparent;outline:none;border:none;cursor:pointer}.json-view .cursor-pointer{cursor:pointer}.json-view svg{vertical-align:-10%}.jv-size-chevron~svg{vertical-align:-16%}.json-view_a11y{color:#545454;--json-property: #aa5d00;--json-index: #007299;--json-number: #007299;--json-string: #008000;--json-boolean: #d91e18;--json-null: #d91e18}.json-view_github{color:#005cc5;--json-property: #005cc5;--json-index: #005cc5;--json-number: #005cc5;--json-string: #032f62;--json-boolean: #005cc5;--json-null: #005cc5}.json-view_vscode{color:#005cc5;--json-property: #0451a5;--json-index: #0000ff;--json-number: #0000ff;--json-string: #a31515;--json-boolean: #0000ff;--json-null: #0000ff}.json-view_atom{color:#383a42;--json-property: #e45649;--json-index: #986801;--json-number: #986801;--json-string: #50a14f;--json-boolean: #0184bc;--json-null: #0184bc}.json-view_winter-is-coming{color:#0431fa;--json-property: #3a9685;--json-index: #ae408b;--json-number: #ae408b;--json-string: #8123a9;--json-boolean: #0184bc;--json-null: #0184bc}:root{--background: 0 0% 100%;--foreground: 222.2 47.4% 11.2%;--muted: 210 40% 98%;--muted-foreground: 215.4 16.3% 46.9%;--popover: 0 0% 100%;--popover-foreground: 222.2 47.4% 11.2%;--card: 0 0% 100%;--card-foreground: 222.2 47.4% 11.2%;--border: 214.3 21.8% 91.4%;--input: 214.3 21.8% 91.4%;--primary: 222.2 27% 11.2%;--primary-foreground: 210 40% 98%;--secondary: 210 40% 96.1%;--secondary-foreground: 222.2 47.4% 11.2%;--accent: 210 30% 96.1%;--accent-foreground: 222.2 47.4% 11.2%;--destructive: 0 100% 50%;--destructive-foreground: 210 40% 98%;--radius: .5rem;--ring: 215 20.2% 65.1%;--round-btn-shadow: #00000063;--error-background: #fef2f2;--error-foreground: #991b1b;--success-background: #f0fdf4;--success-foreground: #14532d;--info-background: #f0f4fd;--info-foreground: #141653;--high-indigo: #4338ca;--medium-indigo: #6366f1;--low-indigo: #e0e7ff;--beta-background: rgb(219 234 254);--beta-foreground: rgb(37 99 235);--chat-bot-icon: #afe6ef;--chat-user-icon: #aface9;--component-icon: #d8598a;--flow-icon: #2f67d0;--blur-shared: #151923de;--build-trigger: #dc735b;--chat-trigger: #5c8be1;--chat-trigger-disabled: #b4c3da;--status-red: #ef4444;--status-yellow: #eab308;--chat-send: #059669;--status-green: #4ade80;--status-blue: #2563eb;--connection: #555}.\!dark{--background: 224 35% 7.5% !important;--foreground: 213 31% 80% !important;--muted: 223 27% 11% !important;--muted-foreground: 215.4 16.3% 56.9% !important;--popover: 224 71% 4% !important;--popover-foreground: 215 20.2% 65.1% !important;--card: 224 25% 15.5% !important;--card-foreground: 213 31% 80% !important;--border: 216 24% 17% !important;--input: 216 24% 17% !important;--primary: 210 20% 80% !important;--primary-foreground: 222.2 27.4% 1.2% !important;--secondary: 222.2 37.4% 7.2% !important;--secondary-foreground: 210 40% 80% !important;--accent: 216 24% 20% !important;--accent-foreground: 210 30% 98% !important;--destructive: 0 63% 31% !important;--destructive-foreground: 210 40% 98% !important;--ring: 216 24% 30% !important;--radius: .5rem !important;--round-btn-shadow: #00000063 !important;--success-background: #022c22 !important;--success-foreground: #ecfdf5 !important;--error-foreground: #fef2f2 !important;--error-background: #450a0a !important;--info-foreground: #eff6ff !important;--info-background: #172554 !important;--high-indigo: #4338ca !important;--medium-indigo: #6366f1 !important;--low-indigo: #e0e7ff !important;--component-icon: #c35f85 !important;--flow-icon: #2467e4 !important;--blur-shared: #151923d2 !important;--build-trigger: #dc735b !important;--chat-trigger: #5c8be1 !important;--chat-trigger-disabled: #2d3b54 !important;--status-red: #ef4444 !important;--status-yellow: #eab308 !important;--chat-send: #059669 !important;--status-green: #4ade80 !important;--status-blue: #2563eb !important;--connection: #555 !important;--beta-background: rgb(37 99 235) !important;--beta-foreground: rgb(219 234 254) !important;--chat-bot-icon: #235d70 !important;--chat-user-icon: #4f3d6e !important}.dark{--background: 224 35% 7.5%;--foreground: 213 31% 80%;--muted: 223 27% 11%;--muted-foreground: 215.4 16.3% 56.9%;--popover: 224 71% 4%;--popover-foreground: 215 20.2% 65.1%;--card: 224 25% 15.5%;--card-foreground: 213 31% 80%;--border: 216 24% 17%;--input: 216 24% 17%;--primary: 210 20% 80%;--primary-foreground: 222.2 27.4% 1.2%;--secondary: 222.2 37.4% 7.2%;--secondary-foreground: 210 40% 80%;--accent: 216 24% 20%;--accent-foreground: 210 30% 98%;--destructive: 0 63% 31%;--destructive-foreground: 210 40% 98%;--ring: 216 24% 30%;--radius: .5rem;--round-btn-shadow: #00000063;--success-background: #022c22;--success-foreground: #ecfdf5;--error-foreground: #fef2f2;--error-background: #450a0a;--info-foreground: #eff6ff;--info-background: #172554;--high-indigo: #4338ca;--medium-indigo: #6366f1;--low-indigo: #e0e7ff;--component-icon: #c35f85;--flow-icon: #2467e4;--blur-shared: #151923d2;--build-trigger: #dc735b;--chat-trigger: #5c8be1;--chat-trigger-disabled: #2d3b54;--status-red: #ef4444;--status-yellow: #eab308;--chat-send: #059669;--status-green: #4ade80;--status-blue: #2563eb;--connection: #555;--beta-background: rgb(37 99 235);--beta-foreground: rgb(219 234 254);--chat-bot-icon: #235d70;--chat-user-icon: #4f3d6e}.\!loading{pointer-events:none!important;display:inline-block!important;aspect-ratio:1 / 1!important;width:1.5rem!important;background-color:currentColor!important;-webkit-mask-size:100%!important;mask-size:100%!important;-webkit-mask-repeat:no-repeat!important;mask-repeat:no-repeat!important;-webkit-mask-position:center!important;mask-position:center!important;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important;mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important}.loading{pointer-events:none;display:inline-block;aspect-ratio:1 / 1;width:1.5rem;background-color:currentColor;-webkit-mask-size:100%;mask-size:100%;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-position:center;mask-position:center;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}.loading-spinner{-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}*,:before,:after{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}:before,:after{--tw-content: ""}html,:host{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;tab-size:4;font-family:var(--font-sans),ui-sans-serif,system-ui,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,samp,pre{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,[type=button],[type=reset],[type=submit]{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dl,dd,h1,h2,h3,h4,h5,h6,hr,figure,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}ol,ul,menu{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}button,[role=button]{cursor:pointer}:disabled{cursor:default}img,svg,video,canvas,audio,iframe,embed,object{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}:root,[data-theme]{background-color:var(--fallback-b1,oklch(var(--b1)/1));color:var(--fallback-bc,oklch(var(--bc)/1))}@supports not (color: oklch(0 0 0)){:root{color-scheme:light;--fallback-p: #491eff;--fallback-pc: #d4dbff;--fallback-s: #ff41c7;--fallback-sc: #fff9fc;--fallback-a: #00cfbd;--fallback-ac: #00100d;--fallback-n: #2b3440;--fallback-nc: #d7dde4;--fallback-b1: #ffffff;--fallback-b2: #e5e6e6;--fallback-b3: #e5e6e6;--fallback-bc: #1f2937;--fallback-in: #00b3f0;--fallback-inc: #000000;--fallback-su: #00ca92;--fallback-suc: #000000;--fallback-wa: #ffc22d;--fallback-wac: #000000;--fallback-er: #ff6f70;--fallback-erc: #000000}@media (prefers-color-scheme: dark){:root{color-scheme:dark;--fallback-p: #7582ff;--fallback-pc: #050617;--fallback-s: #ff71cf;--fallback-sc: #190211;--fallback-a: #00c7b5;--fallback-ac: #000e0c;--fallback-n: #2a323c;--fallback-nc: #a6adbb;--fallback-b1: #1d232a;--fallback-b2: #191e24;--fallback-b3: #15191e;--fallback-bc: #a6adbb;--fallback-in: #00b3f0;--fallback-inc: #000000;--fallback-su: #00ca92;--fallback-suc: #000000;--fallback-wa: #ffc22d;--fallback-wac: #000000;--fallback-er: #ff6f70;--fallback-erc: #000000}}}html{-webkit-tap-highlight-color:transparent}:root{color-scheme:light;--in: .7206 .191 231.6;--su: 64.8% .15 160;--wa: .8471 .199 83.87;--er: .7176 .221 22.18;--pc: .89824 .06192 275.75;--ac: .15352 .0368 183.61;--inc: 0 0 0;--suc: 0 0 0;--wac: 0 0 0;--erc: 0 0 0;--rounded-box: 1rem;--rounded-btn: .5rem;--rounded-badge: 1.9rem;--animation-btn: .25s;--animation-input: .2s;--btn-focus-scale: .95;--border-btn: 1px;--tab-border: 1px;--tab-radius: .5rem;--p: .4912 .3096 275.75;--s: .6971 .329 342.55;--sc: .9871 .0106 342.55;--a: .7676 .184 183.61;--n: .321785 .02476 255.701624;--nc: .894994 .011585 252.096176;--b1: 1 0 0;--b2: .961151 0 0;--b3: .924169 .00108 197.137559;--bc: .278078 .029596 256.847952}@media (prefers-color-scheme: dark){:root{color-scheme:dark;--in: .7206 .191 231.6;--su: 64.8% .15 160;--wa: .8471 .199 83.87;--er: .7176 .221 22.18;--pc: .13138 .0392 275.75;--sc: .1496 .052 342.55;--ac: .14902 .0334 183.61;--inc: 0 0 0;--suc: 0 0 0;--wac: 0 0 0;--erc: 0 0 0;--rounded-box: 1rem;--rounded-btn: .5rem;--rounded-badge: 1.9rem;--animation-btn: .25s;--animation-input: .2s;--btn-focus-scale: .95;--border-btn: 1px;--tab-border: 1px;--tab-radius: .5rem;--p: .6569 .196 275.75;--s: .748 .26 342.55;--a: .7451 .167 183.61;--n: .313815 .021108 254.139175;--nc: .746477 .0216 264.435964;--b1: .253267 .015896 252.417568;--b2: .232607 .013807 253.100675;--b3: .211484 .01165 254.087939;--bc: .746477 .0216 264.435964}}[data-theme=light]{color-scheme:light;--in: .7206 .191 231.6;--su: 64.8% .15 160;--wa: .8471 .199 83.87;--er: .7176 .221 22.18;--pc: .89824 .06192 275.75;--ac: .15352 .0368 183.61;--inc: 0 0 0;--suc: 0 0 0;--wac: 0 0 0;--erc: 0 0 0;--rounded-box: 1rem;--rounded-btn: .5rem;--rounded-badge: 1.9rem;--animation-btn: .25s;--animation-input: .2s;--btn-focus-scale: .95;--border-btn: 1px;--tab-border: 1px;--tab-radius: .5rem;--p: .4912 .3096 275.75;--s: .6971 .329 342.55;--sc: .9871 .0106 342.55;--a: .7676 .184 183.61;--n: .321785 .02476 255.701624;--nc: .894994 .011585 252.096176;--b1: 1 0 0;--b2: .961151 0 0;--b3: .924169 .00108 197.137559;--bc: .278078 .029596 256.847952}[data-theme=dark]{color-scheme:dark;--in: .7206 .191 231.6;--su: 64.8% .15 160;--wa: .8471 .199 83.87;--er: .7176 .221 22.18;--pc: .13138 .0392 275.75;--sc: .1496 .052 342.55;--ac: .14902 .0334 183.61;--inc: 0 0 0;--suc: 0 0 0;--wac: 0 0 0;--erc: 0 0 0;--rounded-box: 1rem;--rounded-btn: .5rem;--rounded-badge: 1.9rem;--animation-btn: .25s;--animation-input: .2s;--btn-focus-scale: .95;--border-btn: 1px;--tab-border: 1px;--tab-radius: .5rem;--p: .6569 .196 275.75;--s: .748 .26 342.55;--a: .7451 .167 183.61;--n: .313815 .021108 254.139175;--nc: .746477 .0216 264.435964;--b1: .253267 .015896 252.417568;--b2: .232607 .013807 253.100675;--b3: .211484 .01165 254.087939;--bc: .746477 .0216 264.435964}*{border-color:hsl(var(--border))}body{background-color:hsl(var(--background));color:hsl(var(--foreground));font-feature-settings:"rlig" 1,"calt" 1}*,:before,:after{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.form-input,.form-textarea,.form-select,.form-multiselect{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.form-input:focus,.form-textarea:focus,.form-select:focus,.form-multiselect:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.form-input::placeholder,.form-textarea::placeholder{color:#6b7280;opacity:1}.form-input::-webkit-datetime-edit-fields-wrapper{padding:0}.form-input::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.form-input::-webkit-datetime-edit{display:inline-flex}.form-input::-webkit-datetime-edit,.form-input::-webkit-datetime-edit-year-field,.form-input::-webkit-datetime-edit-month-field,.form-input::-webkit-datetime-edit-day-field,.form-input::-webkit-datetime-edit-hour-field,.form-input::-webkit-datetime-edit-minute-field,.form-input::-webkit-datetime-edit-second-field,.form-input::-webkit-datetime-edit-millisecond-field,.form-input::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.prose{color:var(--tw-prose-body);max-width:65ch}.prose :where(p):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em;margin-bottom:1.25em}.prose :where([class~=lead]):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-lead);font-size:1.25em;line-height:1.6;margin-top:1.2em;margin-bottom:1.2em}.prose :where(a):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-links);text-decoration:underline;font-weight:500}.prose :where(strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-bold);font-weight:600}.prose :where(a strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(blockquote strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(thead th strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(ol):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:decimal;margin-top:1.25em;margin-bottom:1.25em;padding-left:1.625em}.prose :where(ol[type=A]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-alpha}.prose :where(ol[type=a]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-alpha}.prose :where(ol[type=A s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-alpha}.prose :where(ol[type=a s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-alpha}.prose :where(ol[type=I]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-roman}.prose :where(ol[type=i]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-roman}.prose :where(ol[type=I s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-roman}.prose :where(ol[type=i s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-roman}.prose :where(ol[type="1"]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:decimal}.prose :where(ul):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:disc;margin-top:1.25em;margin-bottom:1.25em;padding-left:1.625em}.prose :where(ol>li):not(:where([class~=not-prose],[class~=not-prose] *))::marker{font-weight:400;color:var(--tw-prose-counters)}.prose :where(ul>li):not(:where([class~=not-prose],[class~=not-prose] *))::marker{color:var(--tw-prose-bullets)}.prose :where(dt):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;margin-top:1.25em}.prose :where(hr):not(:where([class~=not-prose],[class~=not-prose] *)){border-color:var(--tw-prose-hr);border-top-width:1px;margin-top:3em;margin-bottom:3em}.prose :where(blockquote):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:500;font-style:italic;color:var(--tw-prose-quotes);border-left-width:.25rem;border-left-color:var(--tw-prose-quote-borders);quotes:"“""”""‘""’";margin-top:1.6em;margin-bottom:1.6em;padding-left:1em}.prose :where(blockquote p:first-of-type):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:open-quote}.prose :where(blockquote p:last-of-type):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:close-quote}.prose :where(h1):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:800;font-size:2.25em;margin-top:0;margin-bottom:.8888889em;line-height:1.1111111}.prose :where(h1 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:900;color:inherit}.prose :where(h2):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:700;font-size:1.5em;margin-top:2em;margin-bottom:1em;line-height:1.3333333}.prose :where(h2 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:800;color:inherit}.prose :where(h3):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;font-size:1.25em;margin-top:1.6em;margin-bottom:.6em;line-height:1.6}.prose :where(h3 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:700;color:inherit}.prose :where(h4):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;margin-top:1.5em;margin-bottom:.5em;line-height:1.5}.prose :where(h4 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:700;color:inherit}.prose :where(img):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(picture):not(:where([class~=not-prose],[class~=not-prose] *)){display:block;margin-top:2em;margin-bottom:2em}.prose :where(kbd):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:500;font-family:inherit;color:var(--tw-prose-kbd);box-shadow:0 0 0 1px rgb(var(--tw-prose-kbd-shadows) / 10%),0 3px 0 rgb(var(--tw-prose-kbd-shadows) / 10%);font-size:.875em;border-radius:.3125rem;padding:.1875em .375em}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-code);font-weight:600;font-size:.875em}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:"`"}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:"`"}.prose :where(a code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(h1 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(h2 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit;font-size:.875em}.prose :where(h3 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit;font-size:.9em}.prose :where(h4 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(blockquote code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(thead th code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(pre):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-pre-code);background-color:var(--tw-prose-pre-bg);overflow-x:auto;font-weight:400;font-size:.875em;line-height:1.7142857;margin-top:1.7142857em;margin-bottom:1.7142857em;border-radius:.375rem;padding:.8571429em 1.1428571em}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)){background-color:transparent;border-width:0;border-radius:0;padding:0;font-weight:inherit;color:inherit;font-size:inherit;font-family:inherit;line-height:inherit}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:none}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:none}.prose :where(table):not(:where([class~=not-prose],[class~=not-prose] *)){width:100%;table-layout:auto;text-align:left;margin-top:2em;margin-bottom:2em;font-size:.875em;line-height:1.7142857}.prose :where(thead):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:1px;border-bottom-color:var(--tw-prose-th-borders)}.prose :where(thead th):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;vertical-align:bottom;padding-right:.5714286em;padding-bottom:.5714286em;padding-left:.5714286em}.prose :where(tbody tr):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:1px;border-bottom-color:var(--tw-prose-td-borders)}.prose :where(tbody tr:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:0}.prose :where(tbody td):not(:where([class~=not-prose],[class~=not-prose] *)){vertical-align:baseline}.prose :where(tfoot):not(:where([class~=not-prose],[class~=not-prose] *)){border-top-width:1px;border-top-color:var(--tw-prose-th-borders)}.prose :where(tfoot td):not(:where([class~=not-prose],[class~=not-prose] *)){vertical-align:top}.prose :where(figure>*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0;margin-bottom:0}.prose :where(figcaption):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-captions);font-size:.875em;line-height:1.4285714;margin-top:.8571429em}.prose{--tw-prose-body: #374151;--tw-prose-headings: #111827;--tw-prose-lead: #4b5563;--tw-prose-links: #111827;--tw-prose-bold: #111827;--tw-prose-counters: #6b7280;--tw-prose-bullets: #d1d5db;--tw-prose-hr: #e5e7eb;--tw-prose-quotes: #111827;--tw-prose-quote-borders: #e5e7eb;--tw-prose-captions: #6b7280;--tw-prose-kbd: #111827;--tw-prose-kbd-shadows: 17 24 39;--tw-prose-code: #111827;--tw-prose-pre-code: #e5e7eb;--tw-prose-pre-bg: #1f2937;--tw-prose-th-borders: #d1d5db;--tw-prose-td-borders: #e5e7eb;--tw-prose-invert-body: #d1d5db;--tw-prose-invert-headings: #fff;--tw-prose-invert-lead: #9ca3af;--tw-prose-invert-links: #fff;--tw-prose-invert-bold: #fff;--tw-prose-invert-counters: #9ca3af;--tw-prose-invert-bullets: #4b5563;--tw-prose-invert-hr: #374151;--tw-prose-invert-quotes: #f3f4f6;--tw-prose-invert-quote-borders: #374151;--tw-prose-invert-captions: #9ca3af;--tw-prose-invert-kbd: #fff;--tw-prose-invert-kbd-shadows: 255 255 255;--tw-prose-invert-code: #fff;--tw-prose-invert-pre-code: #d1d5db;--tw-prose-invert-pre-bg: rgb(0 0 0 / 50%);--tw-prose-invert-th-borders: #4b5563;--tw-prose-invert-td-borders: #374151;font-size:1rem;line-height:1.75}.prose :where(picture>img):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0;margin-bottom:0}.prose :where(video):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(li):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.5em;margin-bottom:.5em}.prose :where(ol>li):not(:where([class~=not-prose],[class~=not-prose] *)){padding-left:.375em}.prose :where(ul>li):not(:where([class~=not-prose],[class~=not-prose] *)){padding-left:.375em}.prose :where(.prose>ul>li p):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.75em;margin-bottom:.75em}.prose :where(.prose>ul>li>*:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em}.prose :where(.prose>ul>li>*:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:1.25em}.prose :where(.prose>ol>li>*:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em}.prose :where(.prose>ol>li>*:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:1.25em}.prose :where(ul ul,ul ol,ol ul,ol ol):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.75em;margin-bottom:.75em}.prose :where(dl):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em;margin-bottom:1.25em}.prose :where(dd):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.5em;padding-left:1.625em}.prose :where(hr+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h2+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h3+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h4+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(thead th:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-left:0}.prose :where(thead th:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-right:0}.prose :where(tbody td,tfoot td):not(:where([class~=not-prose],[class~=not-prose] *)){padding:.5714286em}.prose :where(tbody td:first-child,tfoot td:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-left:0}.prose :where(tbody td:last-child,tfoot td:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-right:0}.prose :where(figure):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(.prose>:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(.prose>:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:0}.alert{display:grid;width:100%;grid-auto-flow:row;align-content:flex-start;align-items:center;justify-items:center;gap:1rem;text-align:center;border-radius:var(--rounded-box, 1rem);border-width:1px;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)));padding:1rem;--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--alert-bg: var(--fallback-b2,oklch(var(--b2)/1));--alert-bg-mix: var(--fallback-b1,oklch(var(--b1)/1));background-color:var(--alert-bg)}@media (min-width: 640px){.alert{grid-auto-flow:column;grid-template-columns:auto minmax(auto,1fr);justify-items:start;text-align:start}}.avatar.placeholder>div{display:flex;align-items:center;justify-content:center}.badge{display:inline-flex;align-items:center;justify-content:center;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);transition-duration:.2s;height:1.25rem;font-size:.875rem;line-height:1.25rem;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;padding-left:.563rem;padding-right:.563rem;border-radius:var(--rounded-badge, 1.9rem);border-width:1px;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))}@media (hover:hover){.label a:hover{--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))}.menu li>*:not(ul):not(.menu-title):not(details):active,.menu li>*:not(ul):not(.menu-title):not(details).active,.menu li>details>summary:active{--tw-bg-opacity: 1;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-nc,oklch(var(--nc)/var(--tw-text-opacity)))}.tab:hover{--tw-text-opacity: 1}.table tr.hover:hover,.table tr.hover:nth-child(2n):hover{--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)))}.table-zebra tr.hover:hover,.table-zebra tr.hover:nth-child(2n):hover{--tw-bg-opacity: 1;background-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-bg-opacity)))}}.btn{display:inline-flex;height:3rem;min-height:3rem;flex-shrink:0;cursor:pointer;-webkit-user-select:none;user-select:none;flex-wrap:wrap;align-items:center;justify-content:center;border-radius:var(--rounded-btn, .5rem);border-color:transparent;border-color:oklch(var(--btn-color, var(--b2)) / var(--tw-border-opacity));padding-left:1rem;padding-right:1rem;text-align:center;font-size:.875rem;line-height:1em;gap:.5rem;font-weight:600;text-decoration-line:none;transition-duration:.2s;transition-timing-function:cubic-bezier(0,0,.2,1);border-width:var(--border-btn, 1px);animation:button-pop var(--animation-btn, .25s) ease-out;transition-property:color,background-color,border-color,opacity,box-shadow,transform;--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);outline-color:var(--fallback-bc,oklch(var(--bc)/1));background-color:oklch(var(--btn-color, var(--b2)) / var(--tw-bg-opacity));--tw-bg-opacity: 1;--tw-border-opacity: 1}.btn-disabled,.btn[disabled],.btn:disabled{pointer-events:none}:where(.btn:is(input[type=checkbox])),:where(.btn:is(input[type=radio])){width:auto;-webkit-appearance:none;-moz-appearance:none;appearance:none}.btn:is(input[type=checkbox]):after,.btn:is(input[type=radio]):after{--tw-content: attr(aria-label);content:var(--tw-content)}.card{position:relative;display:flex;flex-direction:column;border-radius:var(--rounded-box, 1rem)}.card:focus{outline:2px solid transparent;outline-offset:2px}.card figure{display:flex;align-items:center;justify-content:center}.card.image-full{display:grid}.card.image-full:before{position:relative;content:"";z-index:10;border-radius:var(--rounded-box, 1rem);--tw-bg-opacity: 1;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));opacity:.75}.card.image-full:before,.card.image-full>*{grid-column-start:1;grid-row-start:1}.card.image-full>figure img{height:100%;object-fit:cover}.card.image-full>.card-body{position:relative;z-index:20;--tw-text-opacity: 1;color:var(--fallback-nc,oklch(var(--nc)/var(--tw-text-opacity)))}.\!chat{display:grid!important;grid-template-columns:repeat(2,minmax(0,1fr))!important;column-gap:.75rem!important;padding-top:.25rem!important;padding-bottom:.25rem!important}.chat{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));column-gap:.75rem;padding-top:.25rem;padding-bottom:.25rem}.checkbox{flex-shrink:0;--chkbg: var(--fallback-bc,oklch(var(--bc)/1));--chkfg: var(--fallback-b1,oklch(var(--b1)/1));height:1.5rem;width:1.5rem;cursor:pointer;-webkit-appearance:none;-moz-appearance:none;appearance:none;border-radius:var(--rounded-btn, .5rem);border-width:1px;border-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-border-opacity)));--tw-border-opacity: .2}@media (hover: hover){.btm-nav>*.\!disabled:hover{pointer-events:none!important;--tw-border-opacity: 0 !important;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)))!important;--tw-bg-opacity: .1 !important;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))!important;--tw-text-opacity: .2 !important}.btm-nav>*.disabled:hover,.btm-nav>*[disabled]:hover{pointer-events:none;--tw-border-opacity: 0;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-bg-opacity: .1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}.btn:hover{--tw-border-opacity: 1;border-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-bg-opacity)))}@supports (color: color-mix(in oklab,black,black)){.btn:hover{background-color:color-mix(in oklab,oklch(var(--btn-color, var(--b2)) / var(--tw-bg-opacity, 1)) 90%,black);border-color:color-mix(in oklab,oklch(var(--btn-color, var(--b2)) / var(--tw-border-opacity, 1)) 90%,black)}}@supports not (color: oklch(0 0 0)){.btn:hover{background-color:var(--btn-color, var(--fallback-b2));border-color:var(--btn-color, var(--fallback-b2))}}.btn.glass:hover{--glass-opacity: 25%;--glass-border-opacity: 15%}.btn-disabled:hover,.btn[disabled]:hover,.btn:disabled:hover{--tw-border-opacity: 0;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-bg-opacity: .2;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}@supports (color: color-mix(in oklab,black,black)){.btn:is(input[type=checkbox]:checked):hover,.btn:is(input[type=radio]:checked):hover{background-color:color-mix(in oklab,var(--fallback-p,oklch(var(--p)/1)) 90%,black);border-color:color-mix(in oklab,var(--fallback-p,oklch(var(--p)/1)) 90%,black)}}:where(.menu li:not(.menu-title):not(.disabled)>*:not(ul):not(details):not(.menu-title)):not(.active):hover,:where(.menu li:not(.menu-title):not(.disabled)>details>summary:not(.menu-title)):not(.active):hover{cursor:pointer;outline:2px solid transparent;outline-offset:2px}@supports (color: oklch(0 0 0)){:where(.menu li:not(.menu-title):not(.disabled)>*:not(ul):not(details):not(.menu-title)):not(.active):hover,:where(.menu li:not(.menu-title):not(.disabled)>details>summary:not(.menu-title)):not(.active):hover{background-color:var(--fallback-bc,oklch(var(--bc)/.1))}}.tab[disabled],.tab[disabled]:hover{cursor:not-allowed;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}}.label{display:flex;-webkit-user-select:none;user-select:none;align-items:center;justify-content:space-between;padding:.5rem .25rem}.input{flex-shrink:1;-webkit-appearance:none;-moz-appearance:none;appearance:none;height:3rem;padding-left:1rem;padding-right:1rem;font-size:1rem;line-height:2;line-height:1.5rem;border-radius:var(--rounded-btn, .5rem);border-width:1px;border-color:transparent;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.join{display:inline-flex;align-items:stretch;border-radius:var(--rounded-btn, .5rem)}.join :where(.join-item){border-start-end-radius:0;border-end-end-radius:0;border-end-start-radius:0;border-start-start-radius:0}.join .join-item:not(:first-child):not(:last-child),.join *:not(:first-child):not(:last-child) .join-item{border-start-end-radius:0;border-end-end-radius:0;border-end-start-radius:0;border-start-start-radius:0}.join .join-item:first-child:not(:last-child),.join *:first-child:not(:last-child) .join-item{border-start-end-radius:0;border-end-end-radius:0}.join .dropdown .join-item:first-child:not(:last-child),.join *:first-child:not(:last-child) .dropdown .join-item{border-start-end-radius:inherit;border-end-end-radius:inherit}.join :where(.join-item:first-child:not(:last-child)),.join :where(*:first-child:not(:last-child) .join-item){border-end-start-radius:inherit;border-start-start-radius:inherit}.join .join-item:last-child:not(:first-child),.join *:last-child:not(:first-child) .join-item{border-end-start-radius:0;border-start-start-radius:0}.join :where(.join-item:last-child:not(:first-child)),.join :where(*:last-child:not(:first-child) .join-item){border-start-end-radius:inherit;border-end-end-radius:inherit}@supports not selector(:has(*)){:where(.join *){border-radius:inherit}}@supports selector(:has(*)){:where(.join *:has(.join-item)){border-radius:inherit}}.link{cursor:pointer;text-decoration-line:underline}.mask{-webkit-mask-size:contain;mask-size:contain;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-position:center;mask-position:center}.menu{display:flex;flex-direction:column;flex-wrap:wrap;font-size:.875rem;line-height:1.25rem;padding:.5rem}.menu :where(li ul){position:relative;white-space:nowrap;margin-inline-start:1rem;padding-inline-start:.5rem}.menu :where(li:not(.menu-title)>*:not(ul):not(details):not(.menu-title)),.menu :where(li:not(.menu-title)>details>summary:not(.menu-title)){display:grid;grid-auto-flow:column;align-content:flex-start;align-items:center;gap:.5rem;grid-auto-columns:minmax(auto,-webkit-max-content) auto -webkit-max-content;grid-auto-columns:minmax(auto,max-content) auto max-content;-webkit-user-select:none;user-select:none}.menu li.disabled{cursor:not-allowed;-webkit-user-select:none;user-select:none;color:var(--fallback-bc,oklch(var(--bc)/.3))}.menu li.\!disabled{cursor:not-allowed!important;-webkit-user-select:none!important;user-select:none!important;color:var(--fallback-bc,oklch(var(--bc)/.3))!important}.menu :where(li>.menu-dropdown:not(.menu-dropdown-show)){display:none}:where(.menu li){position:relative;display:flex;flex-shrink:0;flex-direction:column;flex-wrap:wrap;align-items:stretch}:where(.menu li) .badge{justify-self:end}.modal{pointer-events:none;position:fixed;top:0;right:0;bottom:0;left:0;margin:0;display:grid;height:100%;max-height:none;width:100%;max-width:none;justify-items:center;padding:0;opacity:0;overscroll-behavior:contain;z-index:999;background-color:transparent;color:inherit;transition-duration:.2s;transition-timing-function:cubic-bezier(0,0,.2,1);transition-property:transform,opacity,visibility;overflow-y:hidden}:where(.modal){align-items:center}.modal-open,.modal:target,.modal-toggle:checked+.modal,.modal[open]{pointer-events:auto;visibility:visible;opacity:1}:root:has(:is(.modal-open,.modal:target,.modal-toggle:checked+.modal,.modal[open])){overflow:hidden}.progress{position:relative;width:100%;-webkit-appearance:none;-moz-appearance:none;appearance:none;overflow:hidden;height:.5rem;border-radius:var(--rounded-box, 1rem);background-color:var(--fallback-bc,oklch(var(--bc)/.2))}.radial-progress{position:relative;display:inline-grid;height:var(--size);width:var(--size);place-content:center;border-radius:9999px;background-color:transparent;vertical-align:middle;box-sizing:content-box;--value: 0;--size: 5rem;--thickness: calc(var(--size) / 10)}.radial-progress::-moz-progress-bar{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:transparent}.radial-progress::-webkit-progress-value{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:transparent}.radial-progress::-webkit-progress-bar{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:transparent}.radial-progress:before,.radial-progress:after{position:absolute;border-radius:9999px;content:""}.radial-progress:before{top:0;right:0;bottom:0;left:0;background:radial-gradient(farthest-side,currentColor 98%,#0000) top/var(--thickness) var(--thickness) no-repeat,conic-gradient(currentColor calc(var(--value) * 1%),#0000 0);-webkit-mask:radial-gradient(farthest-side,#0000 calc(99% - var(--thickness)),#000 calc(100% - var(--thickness)));mask:radial-gradient(farthest-side,#0000 calc(99% - var(--thickness)),#000 calc(100% - var(--thickness)))}.radial-progress:after{inset:calc(50% - var(--thickness) / 2);transform:rotate(calc(var(--value) * 3.6deg - 90deg)) translate(calc(var(--size) / 2 - 50%));background-color:currentColor}.select{display:inline-flex;cursor:pointer;-webkit-user-select:none;user-select:none;-webkit-appearance:none;-moz-appearance:none;appearance:none;height:3rem;min-height:3rem;padding-left:1rem;padding-right:2.5rem;font-size:.875rem;line-height:1.25rem;line-height:2;border-radius:var(--rounded-btn, .5rem);border-width:1px;border-color:transparent;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)));background-image:linear-gradient(45deg,transparent 50%,currentColor 50%),linear-gradient(135deg,currentColor 50%,transparent 50%);background-position:calc(100% - 20px) calc(1px + 50%),calc(100% - 16.1px) calc(1px + 50%);background-size:4px 4px,4px 4px;background-repeat:no-repeat}.select[multiple]{height:auto}.stack{display:inline-grid;place-items:center;align-items:flex-end}.stack>*{grid-column-start:1;grid-row-start:1;transform:translateY(10%) scale(.9);z-index:1;width:100%;opacity:.6}.stack>*:nth-child(2){transform:translateY(5%) scale(.95);z-index:2;opacity:.8}.stack>*:nth-child(1){transform:translateY(0) scale(1);z-index:3;opacity:1}.steps .step{display:grid;grid-template-columns:repeat(1,minmax(0,1fr));grid-template-columns:auto;grid-template-rows:repeat(2,minmax(0,1fr));grid-template-rows:40px 1fr;place-items:center;text-align:center;min-width:4rem}.tabs{display:grid;align-items:flex-end}.tabs-lifted:has(.tab-content[class^=rounded-]) .tab:first-child:not(.tab-active),.tabs-lifted:has(.tab-content[class*=" rounded-"]) .tab:first-child:not(.tab-active){border-bottom-color:transparent}.tab{position:relative;grid-row-start:1;display:inline-flex;height:2rem;cursor:pointer;-webkit-user-select:none;user-select:none;-webkit-appearance:none;-moz-appearance:none;appearance:none;flex-wrap:wrap;align-items:center;justify-content:center;text-align:center;font-size:.875rem;line-height:1.25rem;line-height:2;--tab-padding: 1rem;--tw-text-opacity: .5;--tab-color: var(--fallback-bc,oklch(var(--bc)/1));--tab-bg: var(--fallback-b1,oklch(var(--b1)/1));--tab-border-color: var(--fallback-b3,oklch(var(--b3)/1));color:var(--tab-color);padding-inline-start:var(--tab-padding, 1rem);padding-inline-end:var(--tab-padding, 1rem)}.tab:is(input[type=radio]){width:auto;border-bottom-right-radius:0;border-bottom-left-radius:0}.tab:is(input[type=radio]):after{--tw-content: attr(aria-label);content:var(--tw-content)}.tab:not(input):empty{cursor:default;grid-column-start:span 9999}input.tab:checked+.tab-content,.tab-active+.tab-content{display:block}.table{position:relative;width:100%;border-radius:var(--rounded-box, 1rem);text-align:left;font-size:.875rem;line-height:1.25rem}.table :where(.table-pin-rows thead tr){position:-webkit-sticky;position:sticky;top:0;z-index:1;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.table :where(.table-pin-rows tfoot tr){position:-webkit-sticky;position:sticky;bottom:0;z-index:1;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.table :where(.table-pin-cols tr th){position:-webkit-sticky;position:sticky;left:0;right:0;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.textarea{min-height:3rem;flex-shrink:1;padding:.5rem 1rem;font-size:.875rem;line-height:1.25rem;line-height:2;border-radius:var(--rounded-btn, .5rem);border-width:1px;border-color:transparent;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.toggle{flex-shrink:0;--tglbg: var(--fallback-b1,oklch(var(--b1)/1));--handleoffset: 1.5rem;--handleoffsetcalculator: calc(var(--handleoffset) * -1);--togglehandleborder: 0 0;height:1.5rem;width:3rem;cursor:pointer;-webkit-appearance:none;-moz-appearance:none;appearance:none;border-radius:var(--rounded-badge, 1.9rem);border-width:1px;border-color:currentColor;background-color:currentColor;color:var(--fallback-bc,oklch(var(--bc)/.5));transition:background,box-shadow var(--animation-input, .2s) ease-out;box-shadow:var(--handleoffsetcalculator) 0 0 2px var(--tglbg) inset,0 0 0 2px var(--tglbg) inset,var(--togglehandleborder)}.btm-nav>*:where(.active){border-top-width:2px;--tw-bg-opacity: 1;background-color:var(--fallback-b1,oklch(var(--b1)/var(--tw-bg-opacity)))}.btm-nav>*.\!disabled{pointer-events:none!important;--tw-border-opacity: 0 !important;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)))!important;--tw-bg-opacity: .1 !important;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))!important;--tw-text-opacity: .2 !important}.btm-nav>*.disabled,.btm-nav>*[disabled]{pointer-events:none;--tw-border-opacity: 0;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-bg-opacity: .1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}.btm-nav>* .label{font-size:1rem;line-height:1.5rem}.btn:active:hover,.btn:active:focus{animation:button-pop 0s ease-out;transform:scale(var(--btn-focus-scale, .97))}@supports not (color: oklch(0 0 0)){.btn{background-color:var(--btn-color, var(--fallback-b2));border-color:var(--btn-color, var(--fallback-b2))}.prose :where(code):not(:where([class~=not-prose] *,pre *)){background-color:var(--fallback-b3,oklch(var(--b3)/1))}}.btn:focus-visible{outline-style:solid;outline-width:2px;outline-offset:2px}.btn.glass{--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);outline-color:currentColor}.btn.glass.btn-active{--glass-opacity: 25%;--glass-border-opacity: 15%}.btn.btn-disabled,.btn[disabled],.btn:disabled{--tw-border-opacity: 0;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-bg-opacity: .2;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}.btn:is(input[type=checkbox]:checked),.btn:is(input[type=radio]:checked){--tw-border-opacity: 1;border-color:var(--fallback-p,oklch(var(--p)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-p,oklch(var(--p)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-pc,oklch(var(--pc)/var(--tw-text-opacity)))}.btn:is(input[type=checkbox]:checked):focus-visible,.btn:is(input[type=radio]:checked):focus-visible{outline-color:var(--fallback-p,oklch(var(--p)/1))}@keyframes button-pop{0%{transform:scale(var(--btn-focus-scale, .98))}40%{transform:scale(1.02)}to{transform:scale(1)}}.card :where(figure:first-child){overflow:hidden;border-start-start-radius:inherit;border-start-end-radius:inherit;border-end-start-radius:unset;border-end-end-radius:unset}.card :where(figure:last-child){overflow:hidden;border-start-start-radius:unset;border-start-end-radius:unset;border-end-start-radius:inherit;border-end-end-radius:inherit}.card:focus-visible{outline:2px solid currentColor;outline-offset:2px}.card.bordered{border-width:1px;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)))}.card.compact .card-body{padding:1rem;font-size:.875rem;line-height:1.25rem}.card.image-full :where(figure){overflow:hidden;border-radius:inherit}.checkbox:focus{box-shadow:none}.checkbox:focus-visible{outline-style:solid;outline-width:2px;outline-offset:2px;outline-color:var(--fallback-bc,oklch(var(--bc)/1))}.checkbox:checked,.checkbox[checked=true],.checkbox[aria-checked=true]{background-repeat:no-repeat;animation:checkmark var(--animation-input, .2s) ease-out;background-color:var(--chkbg);background-image:linear-gradient(-45deg,transparent 65%,var(--chkbg) 65.99%),linear-gradient(45deg,transparent 75%,var(--chkbg) 75.99%),linear-gradient(-45deg,var(--chkbg) 40%,transparent 40.99%),linear-gradient(45deg,var(--chkbg) 30%,var(--chkfg) 30.99%,var(--chkfg) 40%,transparent 40.99%),linear-gradient(-45deg,var(--chkfg) 50%,var(--chkbg) 50.99%)}.checkbox:indeterminate{--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)));background-repeat:no-repeat;animation:checkmark var(--animation-input, .2s) ease-out;background-image:linear-gradient(90deg,transparent 80%,var(--chkbg) 80%),linear-gradient(-90deg,transparent 80%,var(--chkbg) 80%),linear-gradient(0deg,var(--chkbg) 43%,var(--chkfg) 43%,var(--chkfg) 57%,var(--chkbg) 57%)}.checkbox:disabled{cursor:not-allowed;border-color:transparent;--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)));opacity:.2}@keyframes checkmark{0%{background-position-y:5px}50%{background-position-y:-2px}to{background-position-y:0}}.input input:focus{outline:2px solid transparent;outline-offset:2px}.input[list]::-webkit-calendar-picker-indicator{line-height:1em}.input:focus,.input:focus-within{box-shadow:none;border-color:var(--fallback-bc,oklch(var(--bc)/.2));outline-style:solid;outline-width:2px;outline-offset:2px;outline-color:var(--fallback-bc,oklch(var(--bc)/.2))}.input-disabled,.input:disabled,.input[disabled]{cursor:not-allowed;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)));color:var(--fallback-bc,oklch(var(--bc)/.4))}.input-disabled::placeholder,.input:disabled::placeholder,.input[disabled]::placeholder{color:var(--fallback-bc,oklch(var(--bc)/var(--tw-placeholder-opacity)));--tw-placeholder-opacity: .2}.input::-webkit-date-and-time-value{text-align:inherit}.join>:where(*:not(:first-child)){margin-top:0;margin-bottom:0;margin-inline-start:-1px}.link:focus{outline:2px solid transparent;outline-offset:2px}.link:focus-visible{outline:2px solid currentColor;outline-offset:2px}.\!loading{pointer-events:none!important;display:inline-block!important;aspect-ratio:1 / 1!important;width:1.5rem!important;background-color:currentColor!important;-webkit-mask-size:100%!important;mask-size:100%!important;-webkit-mask-repeat:no-repeat!important;mask-repeat:no-repeat!important;-webkit-mask-position:center!important;mask-position:center!important;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important;mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")!important}.loading{pointer-events:none;display:inline-block;aspect-ratio:1 / 1;width:1.5rem;background-color:currentColor;-webkit-mask-size:100%;mask-size:100%;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-position:center;mask-position:center;-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}.loading-spinner{-webkit-mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E");mask-image:url("data:image/svg+xml,%3Csvg width='24' height='24' stroke='%23000' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cstyle%3E.spinner_V8m1%7Btransform-origin:center;animation:spinner_zKoa 2s linear infinite%7D.spinner_V8m1 circle%7Bstroke-linecap:round;animation:spinner_YpZS 1.5s ease-out infinite%7D%40keyframes spinner_zKoa%7B100%25%7Btransform:rotate(360deg)%7D%7D%40keyframes spinner_YpZS%7B0%25%7Bstroke-dasharray:0 150;stroke-dashoffset:0%7D47.5%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-16%7D95%25%2C100%25%7Bstroke-dasharray:42 150;stroke-dashoffset:-59%7D%7D%3C%2Fstyle%3E%3Cg class='spinner_V8m1'%3E%3Ccircle cx='12' cy='12' r='9.5' fill='none' stroke-width='3'%3E%3C%2Fcircle%3E%3C%2Fg%3E%3C%2Fsvg%3E")}.loading-sm{width:1.25rem}:where(.menu li:empty){--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)));opacity:.1;margin:.5rem 1rem;height:1px}.menu :where(li ul):before{position:absolute;bottom:.75rem;inset-inline-start:0px;top:.75rem;width:1px;--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)));opacity:.1;content:""}.menu :where(li:not(.menu-title)>*:not(ul):not(details):not(.menu-title)),.menu :where(li:not(.menu-title)>details>summary:not(.menu-title)){border-radius:var(--rounded-btn, .5rem);padding:.5rem 1rem;text-align:start;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);transition-duration:.2s;text-wrap:balance}:where(.menu li:not(.menu-title):not(.disabled)>*:not(ul):not(details):not(.menu-title)):not(summary):not(.active).focus,:where(.menu li:not(.menu-title):not(.disabled)>*:not(ul):not(details):not(.menu-title)):not(summary):not(.active):focus,:where(.menu li:not(.menu-title):not(.disabled)>*:not(ul):not(details):not(.menu-title)):is(summary):not(.active):focus-visible,:where(.menu li:not(.menu-title):not(.disabled)>details>summary:not(.menu-title)):not(summary):not(.active).focus,:where(.menu li:not(.menu-title):not(.disabled)>details>summary:not(.menu-title)):not(summary):not(.active):focus,:where(.menu li:not(.menu-title):not(.disabled)>details>summary:not(.menu-title)):is(summary):not(.active):focus-visible{cursor:pointer;background-color:var(--fallback-bc,oklch(var(--bc)/.1));--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));outline:2px solid transparent;outline-offset:2px}.menu li>*:not(ul):not(.menu-title):not(details):active,.menu li>*:not(ul):not(.menu-title):not(details).active,.menu li>details>summary:active{--tw-bg-opacity: 1;background-color:var(--fallback-n,oklch(var(--n)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-nc,oklch(var(--nc)/var(--tw-text-opacity)))}.menu :where(li>details>summary)::-webkit-details-marker{display:none}.menu :where(li>details>summary):after,.menu :where(li>.menu-dropdown-toggle):after{justify-self:end;display:block;margin-top:-.5rem;height:.5rem;width:.5rem;transform:rotate(45deg);transition-property:transform,margin-top;transition-duration:.3s;transition-timing-function:cubic-bezier(.4,0,.2,1);content:"";transform-origin:75% 75%;box-shadow:2px 2px;pointer-events:none}.menu :where(li>details[open]>summary):after,.menu :where(li>.menu-dropdown-toggle.menu-dropdown-show):after{transform:rotate(225deg);margin-top:0}.mockup-phone .display{overflow:hidden;border-radius:40px;margin-top:-25px}.mockup-browser .mockup-browser-toolbar .input{position:relative;margin-left:auto;margin-right:auto;display:block;height:1.75rem;width:24rem;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)));padding-left:2rem;direction:ltr}.mockup-browser .mockup-browser-toolbar .input:before{content:"";position:absolute;left:.5rem;top:50%;aspect-ratio:1 / 1;height:.75rem;--tw-translate-y: -50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));border-radius:9999px;border-width:2px;border-color:currentColor;opacity:.6}.mockup-browser .mockup-browser-toolbar .input:after{content:"";position:absolute;left:1.25rem;top:50%;height:.5rem;--tw-translate-y: 25%;--tw-rotate: -45deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));border-radius:9999px;border-width:1px;border-color:currentColor;opacity:.6}.modal:not(dialog:not(.modal-open)),.modal::backdrop{background-color:#0006;animation:modal-pop .2s ease-out}.modal-open .modal-box,.modal-toggle:checked+.modal .modal-box,.modal:target .modal-box,.modal[open] .modal-box{--tw-translate-y: 0px;--tw-scale-x: 1;--tw-scale-y: 1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@keyframes modal-pop{0%{opacity:0}}.progress::-moz-progress-bar{border-radius:var(--rounded-box, 1rem);--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)))}.progress:indeterminate{--progress-color: var(--fallback-bc,oklch(var(--bc)/1));background-image:repeating-linear-gradient(90deg,var(--progress-color) -1%,var(--progress-color) 10%,transparent 10%,transparent 90%);background-size:200%;background-position-x:15%;animation:progress-loading 5s ease-in-out infinite}.progress::-webkit-progress-bar{border-radius:var(--rounded-box, 1rem);background-color:transparent}.progress::-webkit-progress-value{border-radius:var(--rounded-box, 1rem);--tw-bg-opacity: 1;background-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-bg-opacity)))}.progress:indeterminate::-moz-progress-bar{background-color:transparent;background-image:repeating-linear-gradient(90deg,var(--progress-color) -1%,var(--progress-color) 10%,transparent 10%,transparent 90%);background-size:200%;background-position-x:15%;animation:progress-loading 5s ease-in-out infinite}@keyframes progress-loading{50%{background-position-x:-115%}}@keyframes radiomark{0%{box-shadow:0 0 0 12px var(--fallback-b1,oklch(var(--b1)/1)) inset,0 0 0 12px var(--fallback-b1,oklch(var(--b1)/1)) inset}50%{box-shadow:0 0 0 3px var(--fallback-b1,oklch(var(--b1)/1)) inset,0 0 0 3px var(--fallback-b1,oklch(var(--b1)/1)) inset}to{box-shadow:0 0 0 4px var(--fallback-b1,oklch(var(--b1)/1)) inset,0 0 0 4px var(--fallback-b1,oklch(var(--b1)/1)) inset}}@keyframes rating-pop{0%{transform:translateY(-.125em)}40%{transform:translateY(-.125em)}to{transform:translateY(0)}}.select:focus{box-shadow:none;border-color:var(--fallback-bc,oklch(var(--bc)/.2));outline-style:solid;outline-width:2px;outline-offset:2px;outline-color:var(--fallback-bc,oklch(var(--bc)/.2))}.select-disabled,.select:disabled,.select[disabled]{cursor:not-allowed;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)));color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}.select-disabled::placeholder,.select:disabled::placeholder,.select[disabled]::placeholder{color:var(--fallback-bc,oklch(var(--bc)/var(--tw-placeholder-opacity)));--tw-placeholder-opacity: .2}.select-multiple,.select[multiple],.select[size].select:not([size="1"]){background-image:none;padding-right:1rem}[dir=rtl] .select{background-position:calc(0% + 12px) calc(1px + 50%),calc(0% + 16px) calc(1px + 50%)}@keyframes skeleton{0%{background-position:150%}to{background-position:-50%}}.steps .step:before{top:0;grid-column-start:1;grid-row-start:1;height:.5rem;width:100%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));--tw-bg-opacity: 1;background-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));content:"";margin-inline-start:-100%}.steps .step:after{content:counter(step);counter-increment:step;z-index:1;position:relative;grid-column-start:1;grid-row-start:1;display:grid;height:2rem;width:2rem;place-items:center;place-self:center;border-radius:9999px;--tw-bg-opacity: 1;background-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-bg-opacity)));--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))}.steps .step:first-child:before{content:none}.steps .step[data-content]:after{content:attr(data-content)}.tabs-lifted>.tab:focus-visible{border-end-end-radius:0;border-end-start-radius:0}.tab.tab-active:not(.tab-disabled):not([disabled]),.tab:is(input:checked){border-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-border-opacity)));--tw-border-opacity: 1;--tw-text-opacity: 1}.tab:focus{outline:2px solid transparent;outline-offset:2px}.tab:focus-visible{outline:2px solid currentColor;outline-offset:-5px}.tab-disabled,.tab[disabled]{cursor:not-allowed;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));--tw-text-opacity: .2}.tabs-bordered>.tab{border-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-border-opacity)));--tw-border-opacity: .2;border-style:solid;border-bottom-width:calc(var(--tab-border, 1px) + 1px)}.tabs-lifted>.tab{border:var(--tab-border, 1px) solid transparent;border-width:0 0 var(--tab-border, 1px) 0;border-start-start-radius:var(--tab-radius, .5rem);border-start-end-radius:var(--tab-radius, .5rem);border-bottom-color:var(--tab-border-color);padding-inline-start:var(--tab-padding, 1rem);padding-inline-end:var(--tab-padding, 1rem);padding-top:var(--tab-border, 1px)}.tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]),.tabs-lifted>.tab:is(input:checked){background-color:var(--tab-bg);border-width:var(--tab-border, 1px) var(--tab-border, 1px) 0 var(--tab-border, 1px);border-inline-start-color:var(--tab-border-color);border-inline-end-color:var(--tab-border-color);border-top-color:var(--tab-border-color);padding-inline-start:calc(var(--tab-padding, 1rem) - var(--tab-border, 1px));padding-inline-end:calc(var(--tab-padding, 1rem) - var(--tab-border, 1px));padding-bottom:var(--tab-border, 1px);padding-top:0}.tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]):before,.tabs-lifted>.tab:is(input:checked):before{z-index:1;content:"";display:block;position:absolute;width:calc(100% + var(--tab-radius, .5rem) * 2);height:var(--tab-radius, .5rem);bottom:0;background-size:var(--tab-radius, .5rem);background-position:top left,top right;background-repeat:no-repeat;--tab-grad: calc(69% - var(--tab-border, 1px));--radius-start: radial-gradient( circle at top left, transparent var(--tab-grad), var(--tab-border-color) calc(var(--tab-grad) + .25px), var(--tab-border-color) calc(var(--tab-grad) + var(--tab-border, 1px)), var(--tab-bg) calc(var(--tab-grad) + var(--tab-border, 1px) + .25px) );--radius-end: radial-gradient( circle at top right, transparent var(--tab-grad), var(--tab-border-color) calc(var(--tab-grad) + .25px), var(--tab-border-color) calc(var(--tab-grad) + var(--tab-border, 1px)), var(--tab-bg) calc(var(--tab-grad) + var(--tab-border, 1px) + .25px) );background-image:var(--radius-start),var(--radius-end)}.tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]):first-child:before,.tabs-lifted>.tab:is(input:checked):first-child:before{background-image:var(--radius-end);background-position:top right}[dir=rtl] .tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]):first-child:before,[dir=rtl] .tabs-lifted>.tab:is(input:checked):first-child:before{background-image:var(--radius-start);background-position:top left}.tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]):last-child:before,.tabs-lifted>.tab:is(input:checked):last-child:before{background-image:var(--radius-start);background-position:top left}[dir=rtl] .tabs-lifted>.tab.tab-active:not(.tab-disabled):not([disabled]):last-child:before,[dir=rtl] .tabs-lifted>.tab:is(input:checked):last-child:before{background-image:var(--radius-end);background-position:top right}.tabs-lifted>.tab-active:not(.tab-disabled):not([disabled])+.tabs-lifted .tab-active:not(.tab-disabled):not([disabled]):before,.tabs-lifted>.tab:is(input:checked)+.tabs-lifted .tab:is(input:checked):before{background-image:var(--radius-end);background-position:top right}.tabs-boxed .tab{border-radius:var(--rounded-btn, .5rem)}:is([dir=rtl] .table){text-align:right}.table :where(th,td){padding:.75rem 1rem;vertical-align:middle}.table tr.active,.table tr.active:nth-child(2n),.table-zebra tbody tr:nth-child(2n){--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)))}.table-zebra tr.active,.table-zebra tr.active:nth-child(2n),.table-zebra-zebra tbody tr:nth-child(2n){--tw-bg-opacity: 1;background-color:var(--fallback-b3,oklch(var(--b3)/var(--tw-bg-opacity)))}.table :where(thead,tbody) :where(tr:not(:last-child)),.table :where(thead,tbody) :where(tr:first-child:last-child){border-bottom-width:1px;--tw-border-opacity: 1;border-bottom-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)))}.table :where(thead,tfoot){white-space:nowrap;font-size:.75rem;line-height:1rem;font-weight:700;color:var(--fallback-bc,oklch(var(--bc)/.6))}.textarea:focus{box-shadow:none;border-color:var(--fallback-bc,oklch(var(--bc)/.2));outline-style:solid;outline-width:2px;outline-offset:2px;outline-color:var(--fallback-bc,oklch(var(--bc)/.2))}.textarea-primary{--tw-border-opacity: 1;border-color:var(--fallback-p,oklch(var(--p)/var(--tw-border-opacity)))}.textarea-primary:focus{--tw-border-opacity: 1;border-color:var(--fallback-p,oklch(var(--p)/var(--tw-border-opacity)));outline-color:var(--fallback-p,oklch(var(--p)/1))}.textarea-disabled,.textarea:disabled,.textarea[disabled]{cursor:not-allowed;--tw-border-opacity: 1;border-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-border-opacity)));--tw-bg-opacity: 1;background-color:var(--fallback-b2,oklch(var(--b2)/var(--tw-bg-opacity)));--tw-text-opacity: .2}.textarea-disabled::placeholder,.textarea:disabled::placeholder,.textarea[disabled]::placeholder{color:var(--fallback-bc,oklch(var(--bc)/var(--tw-placeholder-opacity)));--tw-placeholder-opacity: .2}@keyframes toast-pop{0%{transform:scale(.9);opacity:0}to{transform:scale(1);opacity:1}}[dir=rtl] .toggle{--handleoffsetcalculator: calc(var(--handleoffset) * 1)}.toggle:focus-visible{outline-style:solid;outline-width:2px;outline-offset:2px;outline-color:var(--fallback-bc,oklch(var(--bc)/.2))}.toggle:hover{background-color:currentColor}.toggle:checked,.toggle[checked=true],.toggle[aria-checked=true]{background-image:none;--handleoffsetcalculator: var(--handleoffset);--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)))}[dir=rtl] .toggle:checked,[dir=rtl] .toggle[checked=true],[dir=rtl] .toggle[aria-checked=true]{--handleoffsetcalculator: calc(var(--handleoffset) * -1)}.toggle:indeterminate{--tw-text-opacity: 1;color:var(--fallback-bc,oklch(var(--bc)/var(--tw-text-opacity)));box-shadow:calc(var(--handleoffset) / 2) 0 0 2px var(--tglbg) inset,calc(var(--handleoffset) / -2) 0 0 2px var(--tglbg) inset,0 0 0 2px var(--tglbg) inset}[dir=rtl] .toggle:indeterminate{box-shadow:calc(var(--handleoffset) / 2) 0 0 2px var(--tglbg) inset,calc(var(--handleoffset) / -2) 0 0 2px var(--tglbg) inset,0 0 0 2px var(--tglbg) inset}.toggle:disabled{cursor:not-allowed;--tw-border-opacity: 1;border-color:var(--fallback-bc,oklch(var(--bc)/var(--tw-border-opacity)));background-color:transparent;opacity:.3;--togglehandleborder: 0 0 0 3px var(--fallback-bc,oklch(var(--bc)/1)) inset, var(--handleoffsetcalculator) 0 0 3px var(--fallback-bc,oklch(var(--bc)/1)) inset}:root .prose{--tw-prose-body: var(--fallback-bc,oklch(var(--bc)/.8));--tw-prose-headings: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-lead: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-links: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-bold: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-counters: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-bullets: var(--fallback-bc,oklch(var(--bc)/.5));--tw-prose-hr: var(--fallback-bc,oklch(var(--bc)/.2));--tw-prose-quotes: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-quote-borders: var(--fallback-bc,oklch(var(--bc)/.2));--tw-prose-captions: var(--fallback-bc,oklch(var(--bc)/.5));--tw-prose-code: var(--fallback-bc,oklch(var(--bc)/1));--tw-prose-pre-code: var(--fallback-nc,oklch(var(--nc)/1));--tw-prose-pre-bg: var(--fallback-n,oklch(var(--n)/1));--tw-prose-th-borders: var(--fallback-bc,oklch(var(--bc)/.5));--tw-prose-td-borders: var(--fallback-bc,oklch(var(--bc)/.2))}.prose :where(code):not(:where([class~=not-prose] *,pre *)){padding:1px 8px;border-radius:var(--rounded-badge);font-weight:initial;background-color:var(--fallback-bc,oklch(var(--bc)/.1))}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):before,.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):after{display:none}.prose pre code{border-radius:0;padding:0}.prose :where(tbody tr,thead):not(:where([class~=not-prose] *)){border-bottom-color:var(--fallback-bc,oklch(var(--bc)/.2))}.artboard.phone-1.horizontal,.artboard.phone-1.artboard-horizontal{width:568px;height:320px}.artboard.phone-2.horizontal,.artboard.phone-2.artboard-horizontal{width:667px;height:375px}.artboard.phone-3.horizontal,.artboard.phone-3.artboard-horizontal{width:736px;height:414px}.artboard.phone-4.horizontal,.artboard.phone-4.artboard-horizontal{width:812px;height:375px}.artboard.phone-5.horizontal,.artboard.phone-5.artboard-horizontal{width:896px;height:414px}.artboard.phone-6.horizontal,.artboard.phone-6.artboard-horizontal{width:1024px;height:320px}.btm-nav-xs>*:where(.active){border-top-width:1px}.btm-nav-sm>*:where(.active){border-top-width:2px}.btm-nav-md>*:where(.active){border-top-width:2px}.btm-nav-lg>*:where(.active){border-top-width:4px}.join.join-vertical{flex-direction:column}.join.join-vertical .join-item:first-child:not(:last-child),.join.join-vertical *:first-child:not(:last-child) .join-item{border-end-start-radius:0;border-end-end-radius:0;border-start-start-radius:inherit;border-start-end-radius:inherit}.join.join-vertical .join-item:last-child:not(:first-child),.join.join-vertical *:last-child:not(:first-child) .join-item{border-start-start-radius:0;border-start-end-radius:0;border-end-start-radius:inherit;border-end-end-radius:inherit}.join.join-horizontal{flex-direction:row}.join.join-horizontal .join-item:first-child:not(:last-child),.join.join-horizontal *:first-child:not(:last-child) .join-item{border-end-end-radius:0;border-start-end-radius:0;border-end-start-radius:inherit;border-start-start-radius:inherit}.join.join-horizontal .join-item:last-child:not(:first-child),.join.join-horizontal *:last-child:not(:first-child) .join-item{border-end-start-radius:0;border-start-start-radius:0;border-end-end-radius:inherit;border-start-end-radius:inherit}.steps-horizontal .step{display:grid;grid-template-columns:repeat(1,minmax(0,1fr));grid-template-rows:repeat(2,minmax(0,1fr));place-items:center;text-align:center}.steps-vertical .step{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));grid-template-rows:repeat(1,minmax(0,1fr))}.tabs-md :where(.tab){height:2rem;font-size:.875rem;line-height:1.25rem;line-height:2;--tab-padding: 1rem}.tabs-lg :where(.tab){height:3rem;font-size:1.125rem;line-height:1.75rem;line-height:2;--tab-padding: 1.25rem}.tabs-sm :where(.tab){height:1.5rem;font-size:.875rem;line-height:.75rem;--tab-padding: .75rem}.tabs-xs :where(.tab){height:1.25rem;font-size:.75rem;line-height:.75rem;--tab-padding: .5rem}.tooltip{position:relative;display:inline-block;--tooltip-offset: calc(100% + 1px + var(--tooltip-tail, 0px))}.tooltip:before{position:absolute;pointer-events:none;z-index:1;content:var(--tw-content);--tw-content: attr(data-tip)}.tooltip:before,.tooltip-top:before{transform:translate(-50%);top:auto;left:50%;right:auto;bottom:var(--tooltip-offset)}.join.join-vertical>:where(*:not(:first-child)){margin-left:0;margin-right:0;margin-top:-1px}.join.join-horizontal>:where(*:not(:first-child)){margin-top:0;margin-bottom:0;margin-inline-start:-1px}.steps-horizontal .step{grid-template-rows:40px 1fr;grid-template-columns:auto;min-width:4rem}.steps-horizontal .step:before{height:.5rem;width:100%;--tw-translate-x: 0px;--tw-translate-y: 0px;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));content:"";margin-inline-start:-100%}:is([dir=rtl] .steps-horizontal .step):before{--tw-translate-x: 0px;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.steps-vertical .step{gap:.5rem;grid-template-columns:40px 1fr;grid-template-rows:auto;min-height:4rem;justify-items:start}.steps-vertical .step:before{height:100%;width:.5rem;--tw-translate-x: -50%;--tw-translate-y: -50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));margin-inline-start:50%}:is([dir=rtl] .steps-vertical .step):before{--tw-translate-x: 50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.tooltip{position:relative;display:inline-block;text-align:center;--tooltip-tail: .1875rem;--tooltip-color: var(--fallback-n,oklch(var(--n)/1));--tooltip-text-color: var(--fallback-nc,oklch(var(--nc)/1));--tooltip-tail-offset: calc(100% + .0625rem - var(--tooltip-tail))}.tooltip:before,.tooltip:after{opacity:0;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-delay:.1s;transition-duration:.2s;transition-timing-function:cubic-bezier(.4,0,.2,1)}.tooltip:after{position:absolute;content:"";border-style:solid;border-width:var(--tooltip-tail, 0);width:0;height:0;display:block}.tooltip:before{max-width:20rem;border-radius:.25rem;padding:.25rem .5rem;font-size:.875rem;line-height:1.25rem;background-color:var(--tooltip-color);color:var(--tooltip-text-color);width:-webkit-max-content;width:max-content}.tooltip.tooltip-open:before{opacity:1;transition-delay:75ms}.tooltip.tooltip-open:after{opacity:1;transition-delay:75ms}.tooltip:hover:before{opacity:1;transition-delay:75ms}.tooltip:hover:after{opacity:1;transition-delay:75ms}.tooltip:has(:focus-visible):after,.tooltip:has(:focus-visible):before{opacity:1;transition-delay:75ms}.tooltip:not([data-tip]):hover:before,.tooltip:not([data-tip]):hover:after{visibility:hidden;opacity:0}.tooltip:after,.tooltip-top:after{transform:translate(-50%);border-color:var(--tooltip-color) transparent transparent transparent;top:auto;left:50%;right:auto;bottom:var(--tooltip-tail-offset)}.side-bar-arrangement{display:flex;height:100%;width:14.5rem;flex-direction:column;overflow:hidden;border-right-width:1px;-ms-overflow-style:none;scrollbar-width:none}.side-bar-arrangement::-webkit-scrollbar{display:none}.side-bar-search-div-placement{position:relative;margin-left:auto;margin-right:auto;margin-bottom:.5rem;margin-top:.5rem;display:flex;align-items:center}.side-bar-components-icon{height:1.5rem;width:1rem;color:hsl(var(--ring))}.side-bar-components-text{width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;padding-right:.25rem;font-size:.75rem;line-height:1rem;color:hsl(var(--foreground))}.side-bar-components-div-form{display:flex;width:100%;align-items:center;justify-content:space-between;border-radius:calc(var(--radius) - 2px);border-top-left-radius:0;border-bottom-left-radius:0;border-width:1px;border-left-width:0px;border-style:dashed;border-color:hsl(var(--ring));background-color:var(--white);padding:.25rem .75rem;font-size:.875rem;line-height:1.25rem}.side-bar-components-border{cursor:grab;border-top-left-radius:calc(var(--radius) - 2px);border-bottom-left-radius:calc(var(--radius) - 2px);border-left-width:8px}.side-bar-components-gap{display:flex;flex-direction:column;gap:.5rem;padding:.5rem}.side-bar-components-div-arrangement{width:100%;overflow:auto;padding-bottom:2.5rem;-ms-overflow-style:none;scrollbar-width:none}.side-bar-components-div-arrangement::-webkit-scrollbar{display:none}.search-icon{position:absolute;top:0;bottom:0;right:0;display:flex;align-items:center;padding-top:.375rem;padding-bottom:.375rem;padding-right:1.25rem}.extra-side-bar-save-disable{color:hsl(var(--muted-foreground))}.extra-side-bar-save-disable:hover:hover{color:hsl(var(--accent-foreground))}.side-bar-button-size{height:1.25rem;width:1.25rem}.side-bar-button-size:hover:hover{color:hsl(var(--accent-foreground))}.side-bar-buttons-arrangement{margin-bottom:.5rem;margin-top:.5rem;display:flex;width:100%;align-items:center;justify-content:space-between;gap:.5rem;padding-left:.5rem;padding-right:.5rem}.side-bar-button{display:flex;width:100%}.button-disable{pointer-events:none}.extra-side-bar-buttons{position:relative;display:inline-flex;width:100%;align-items:center;justify-content:center;border-radius:calc(var(--radius) - 2px);background-color:hsl(var(--background));padding:.5rem;color:hsl(var(--foreground));--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);--tw-ring-inset: inset;--tw-ring-color: hsl(var(--input));transition-property:all;transition-duration:.5s;transition-timing-function:cubic-bezier(.4,0,.2,1);animation-duration:.5s;animation-timing-function:cubic-bezier(.4,0,.2,1)}.extra-side-bar-buttons:hover:hover{background-color:hsl(var(--muted))}.primary-input{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.primary-input:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.primary-input::placeholder{color:#6b7280;opacity:1}.primary-input::-webkit-datetime-edit-fields-wrapper{padding:0}.primary-input::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.primary-input::-webkit-datetime-edit{display:inline-flex}.primary-input::-webkit-datetime-edit,.primary-input::-webkit-datetime-edit-year-field,.primary-input::-webkit-datetime-edit-month-field,.primary-input::-webkit-datetime-edit-day-field,.primary-input::-webkit-datetime-edit-hour-field,.primary-input::-webkit-datetime-edit-minute-field,.primary-input::-webkit-datetime-edit-second-field,.primary-input::-webkit-datetime-edit-millisecond-field,.primary-input::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.primary-input{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;font-size:.875rem;line-height:1.25rem;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.primary-input::placeholder{color:hsl(var(--muted-foreground))}.primary-input:focus{border-color:hsl(var(--ring))}.primary-input:focus::placeholder{color:transparent}.primary-input:focus{--tw-ring-color: hsl(var(--ring))}.primary-input:disabled{cursor:not-allowed;opacity:.5}.skeleton-card{display:flex;height:12rem;flex-direction:column;gap:1.5rem;border-radius:var(--radius);border-width:1px;background-color:hsl(var(--background));padding:1rem}.skeleton-card-wrapper{display:flex;align-items:center}.skeleton-card-wrapper>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(1rem * var(--tw-space-x-reverse));margin-left:calc(1rem * calc(1 - var(--tw-space-x-reverse)))}.skeleton-card-text{display:flex;flex-direction:column;gap:.75rem}.textarea-primary{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.textarea-primary:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.textarea-primary::placeholder{color:#6b7280;opacity:1}.textarea-primary::-webkit-datetime-edit-fields-wrapper{padding:0}.textarea-primary::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.textarea-primary::-webkit-datetime-edit{display:inline-flex}.textarea-primary::-webkit-datetime-edit,.textarea-primary::-webkit-datetime-edit-year-field,.textarea-primary::-webkit-datetime-edit-month-field,.textarea-primary::-webkit-datetime-edit-day-field,.textarea-primary::-webkit-datetime-edit-hour-field,.textarea-primary::-webkit-datetime-edit-minute-field,.textarea-primary::-webkit-datetime-edit-second-field,.textarea-primary::-webkit-datetime-edit-millisecond-field,.textarea-primary::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.textarea-primary{display:block;width:100%;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.textarea-primary::placeholder{color:hsl(var(--muted-foreground))}.textarea-primary:focus{border-color:hsl(var(--ring))}.textarea-primary:focus::placeholder{color:transparent}.textarea-primary:focus{--tw-ring-color: hsl(var(--ring))}.textarea-primary:disabled{cursor:not-allowed;opacity:.5}@media (min-width: 640px){.textarea-primary{font-size:.875rem;line-height:1.25rem}}.input-edit-node{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.input-edit-node:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.input-edit-node::placeholder{color:#6b7280;opacity:1}.input-edit-node::-webkit-datetime-edit-fields-wrapper{padding:0}.input-edit-node::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.input-edit-node::-webkit-datetime-edit{display:inline-flex}.input-edit-node::-webkit-datetime-edit,.input-edit-node::-webkit-datetime-edit-year-field,.input-edit-node::-webkit-datetime-edit-month-field,.input-edit-node::-webkit-datetime-edit-day-field,.input-edit-node::-webkit-datetime-edit-hour-field,.input-edit-node::-webkit-datetime-edit-minute-field,.input-edit-node::-webkit-datetime-edit-second-field,.input-edit-node::-webkit-datetime-edit-millisecond-field,.input-edit-node::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.input-edit-node{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;font-size:.875rem;line-height:1.25rem;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.input-edit-node::placeholder{color:hsl(var(--muted-foreground))}.input-edit-node:focus{border-color:hsl(var(--ring))}.input-edit-node:focus::placeholder{color:transparent}.input-edit-node:focus{--tw-ring-color: hsl(var(--ring))}.input-edit-node:disabled{cursor:not-allowed;opacity:.5}.input-edit-node{width:100%;padding-bottom:.125rem;padding-top:.125rem;text-align:left}.input-search{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.input-search:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.input-search::placeholder{color:#6b7280;opacity:1}.input-search::-webkit-datetime-edit-fields-wrapper{padding:0}.input-search::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.input-search::-webkit-datetime-edit{display:inline-flex}.input-search::-webkit-datetime-edit,.input-search::-webkit-datetime-edit-year-field,.input-search::-webkit-datetime-edit-month-field,.input-search::-webkit-datetime-edit-day-field,.input-search::-webkit-datetime-edit-hour-field,.input-search::-webkit-datetime-edit-minute-field,.input-search::-webkit-datetime-edit-second-field,.input-search::-webkit-datetime-edit-millisecond-field,.input-search::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.input-search{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;font-size:.875rem;line-height:1.25rem;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.input-search::placeholder{color:hsl(var(--muted-foreground))}.input-search:focus{border-color:hsl(var(--ring))}.input-search:focus::placeholder{color:transparent}.input-search:focus{--tw-ring-color: hsl(var(--ring))}.input-search:disabled{cursor:not-allowed;opacity:.5}.input-search{margin-left:.5rem;margin-right:.5rem;padding-right:1.75rem}.input-disable{border-color:transparent;background-color:hsl(var(--border))}.input-disable::placeholder{color:hsl(var(--ring))}.input-dialog{cursor:pointer;background-color:transparent;color:hsl(var(--ring))}.message-button{position:fixed;bottom:1rem;right:1rem;display:flex;height:3rem;width:3rem;align-items:center;justify-content:center;border-radius:9999px;background-color:hsl(var(--border));padding:.25rem .75rem;--tw-shadow: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.round-button-form{display:flex;height:3rem;width:3rem;cursor:pointer;justify-content:center;border-radius:9999px;background-color:hsl(var(--border));padding:.25rem .75rem;--tw-shadow: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.round-button-div{display:flex;align-items:center;gap:.75rem}.build-trigger-loading-icon{stroke:var(--build-trigger)}.message-button-icon{fill:var(--chat-trigger);stroke:var(--chat-trigger);stroke-width:1}.disabled-message-button-icon{fill:var(--chat-trigger-disabled);stroke:var(--chat-trigger-disabled);stroke-width:1}.components-disclosure-arrangement{margin-top:-1px;display:flex;width:100%;-webkit-user-select:none;user-select:none;align-items:center;justify-content:space-between;border-top-width:1px;border-bottom-width:1px;border-top-color:hsl(var(--input));border-bottom-color:hsl(var(--input));background-color:hsl(var(--muted));padding:.5rem .75rem}.components-disclosure-title{display:flex;align-items:center;font-size:.875rem;line-height:1.25rem;color:hsl(var(--primary))}.components-disclosure-div{display:flex;gap:.5rem}.flow-page-positioning{height:100%;width:100%;overflow:hidden}.logspace-page-icon{position:absolute;bottom:.5rem;left:1.75rem;display:flex;height:1.5rem;cursor:pointer;flex-direction:column;align-items:center;justify-content:flex-start;overflow:hidden;border-radius:var(--radius);background-color:hsl(var(--foreground));padding-left:.5rem;padding-right:.5rem;text-align:center;font-family:var(--font-sans),ui-sans-serif,system-ui,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";font-size:.75rem;line-height:1rem;letter-spacing:.025em;color:hsl(var(--secondary));transition-property:all;transition-duration:.5s;transition-timing-function:cubic-bezier(.4,0,.2,1);animation-duration:.5s;animation-timing-function:cubic-bezier(.4,0,.2,1)}.logspace-page-icon:hover:hover{height:3rem}.flex-max-width{display:flex;width:100%}.loading-page-panel{display:flex;height:100%;width:100%;align-items:center;justify-content:center;background-color:hsl(var(--background))}.main-page-panel,.admin-page-panel{display:flex;width:100%;height:100%;flex-direction:column;overflow:auto;background-color:hsl(var(--background));padding-left:4rem;padding-right:4rem}.main-page-nav-arrangement{display:flex;width:100%;justify-content:space-between;padding-top:2rem;padding-bottom:.5rem}.main-page-nav-title{display:flex;align-items:center;justify-content:center;gap:.5rem;font-size:1.5rem;line-height:2rem;font-weight:600}.main-page-nav-button{margin-right:.5rem;width:1rem}.admin-page-description-text{display:flex;width:80%;padding-bottom:2rem;color:hsl(var(--muted-foreground))}.community-page-arrangement{display:flex;width:100%;height:100%;flex-direction:column;justify-content:space-between;overflow:auto;background-color:hsl(var(--background));padding-left:4rem;padding-right:4rem}.community-page-nav-arrangement{display:flex;width:100%;justify-content:space-between;padding-top:2rem;padding-bottom:.5rem}.community-page-nav-title{display:flex;align-items:center;justify-content:center;gap:.5rem;font-size:1.5rem;line-height:2rem;font-weight:600}.community-page-description-text{display:flex;width:70%;padding-bottom:2rem;color:hsl(var(--muted-foreground))}.generic-node-div{position:relative;display:flex;flex-direction:column;justify-content:center;background-color:hsl(var(--background))}.generic-node-div-title{display:flex;width:100%;align-items:center;gap:2rem;border-bottom-width:1px;background-color:hsl(var(--muted));padding:1rem}.generic-node-title-arrangement{display:flex;width:100%;align-items:center;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.generic-node-icon{height:2.5rem;width:2.5rem;border-radius:.25rem;padding:.25rem}.generic-node-tooltip-div{margin-left:.5rem;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.generic-node-status-position{position:relative;top:3px;height:1.25rem;width:1.25rem}.green-status{height:1rem;width:1rem;border-radius:9999px;opacity:1;background-color:var(--status-green)}.red-status{height:1rem;width:1rem;border-radius:9999px;opacity:1;background-color:var(--status-red)}.yellow-status{height:1rem;width:1rem;border-radius:9999px;opacity:1;background-color:var(--status-yellow)}.status-build-animation{display:none;height:1rem;width:1rem}.status-build-animation{animation:spin 1s linear infinite;border-radius:9999px;background-color:hsl(var(--ring));opacity:0}.status-div{position:absolute;width:1rem;transition-duration:.2s;transition-timing-function:cubic-bezier(.4,0,.2,1);animation-duration:.2s;animation-timing-function:cubic-bezier(.4,0,.2,1)}.status-div:hover:hover{color:hsl(var(--accent-foreground));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.generic-node-desc{margin-bottom:1rem;height:100%;width:100%;padding-left:1.25rem;padding-right:1.25rem;color:hsl(var(--foreground))}.generic-node-desc-text{width:100%;font-size:.875rem;line-height:1.25rem;color:hsl(var(--muted-foreground))}.error-build-message{margin-top:1.5rem;width:24rem;cursor:pointer;border-radius:calc(var(--radius) - 2px);background-color:var(--error-background);padding:1rem;--tw-shadow: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--tw-shadow-colored: 0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.error-build-message-circle{height:1.25rem;width:1.25rem;color:var(--status-red)}.error-build-foreground{font-size:.875rem;line-height:1.25rem;font-weight:500;color:var(--error-foreground);word-break:break-word}.error-build-message-div{color:var(--error-foreground);word-break:break-word;margin-top:.5rem;font-size:.875rem;line-height:1.25rem}.error-build-message-list{list-style-type:disc}.error-build-message-list>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0;margin-top:calc(.25rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(.25rem * var(--tw-space-y-reverse))}.error-build-message-list{padding-left:1.25rem}.success-alert{margin-top:1.5rem;width:24rem;border-radius:calc(var(--radius) - 2px);background-color:var(--success-background);padding:1rem;--tw-shadow: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--tw-shadow-colored: 0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.success-alert-icon{height:1.25rem;width:1.25rem;color:var(--status-green)}.success-alert-message{font-size:.875rem;line-height:1.25rem;font-weight:500;color:var(--success-foreground);word-break:break-word}.dropdown-component-outline{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.dropdown-component-outline:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.dropdown-component-outline::placeholder{color:#6b7280;opacity:1}.dropdown-component-outline::-webkit-datetime-edit-fields-wrapper{padding:0}.dropdown-component-outline::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.dropdown-component-outline::-webkit-datetime-edit{display:inline-flex}.dropdown-component-outline::-webkit-datetime-edit,.dropdown-component-outline::-webkit-datetime-edit-year-field,.dropdown-component-outline::-webkit-datetime-edit-month-field,.dropdown-component-outline::-webkit-datetime-edit-day-field,.dropdown-component-outline::-webkit-datetime-edit-hour-field,.dropdown-component-outline::-webkit-datetime-edit-minute-field,.dropdown-component-outline::-webkit-datetime-edit-second-field,.dropdown-component-outline::-webkit-datetime-edit-millisecond-field,.dropdown-component-outline::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.dropdown-component-outline{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;font-size:.875rem;line-height:1.25rem;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.dropdown-component-outline::placeholder{color:hsl(var(--muted-foreground))}.dropdown-component-outline:focus{border-color:hsl(var(--ring))}.dropdown-component-outline:focus::placeholder{color:transparent}.dropdown-component-outline:focus{--tw-ring-color: hsl(var(--ring))}.dropdown-component-outline:disabled{cursor:not-allowed;opacity:.5}.dropdown-component-outline{width:100%;padding-bottom:.125rem;padding-top:.125rem;text-align:left;position:relative;padding-right:2rem}.dropdown-component-false-outline{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.dropdown-component-false-outline:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.dropdown-component-false-outline::placeholder{color:#6b7280;opacity:1}.dropdown-component-false-outline::-webkit-datetime-edit-fields-wrapper{padding:0}.dropdown-component-false-outline::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.dropdown-component-false-outline::-webkit-datetime-edit{display:inline-flex}.dropdown-component-false-outline::-webkit-datetime-edit,.dropdown-component-false-outline::-webkit-datetime-edit-year-field,.dropdown-component-false-outline::-webkit-datetime-edit-month-field,.dropdown-component-false-outline::-webkit-datetime-edit-day-field,.dropdown-component-false-outline::-webkit-datetime-edit-hour-field,.dropdown-component-false-outline::-webkit-datetime-edit-minute-field,.dropdown-component-false-outline::-webkit-datetime-edit-second-field,.dropdown-component-false-outline::-webkit-datetime-edit-millisecond-field,.dropdown-component-false-outline::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.dropdown-component-false-outline{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));background-color:hsl(var(--background));padding-left:.75rem;padding-right:.75rem;text-align:left;font-size:.875rem;line-height:1.25rem;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.dropdown-component-false-outline::placeholder{color:hsl(var(--muted-foreground))}.dropdown-component-false-outline:focus{border-color:hsl(var(--ring))}.dropdown-component-false-outline:focus::placeholder{color:transparent}.dropdown-component-false-outline:focus{--tw-ring-color: hsl(var(--ring))}.dropdown-component-false-outline:disabled{cursor:not-allowed;opacity:.5}.dropdown-component-false-outline{padding:.5rem 2.5rem .5rem .75rem;text-align:left}.dropdown-component-display{display:block;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;background-color:hsl(var(--background))}.dropdown-component-arrow{pointer-events:none;position:absolute;top:0;bottom:0;right:0;display:flex;align-items:center;padding-right:.5rem}.dropdown-component-arrow-color{color:hsl(var(--muted-foreground))}.dropdown-component-arrow-color:hover:hover{color:hsl(var(--accent-foreground))}.dropdown-component-arrow-color{height:1.25rem;width:1.25rem}.dropdown-component-true-options{z-index:10;margin-top:.25rem;max-height:15rem;overflow:auto;border-radius:calc(var(--radius) - 2px);background-color:hsl(var(--background));padding-top:.25rem;padding-bottom:.25rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);--tw-ring-color: rgb(0 0 0 / var(--tw-ring-opacity));--tw-ring-opacity: .05}.dropdown-component-true-options:focus{outline:2px solid transparent;outline-offset:2px}@media (min-width: 640px){.dropdown-component-true-options{font-size:.875rem;line-height:1.25rem}}@media (min-width: 1024px){.dropdown-component-true-options{width:32%}}.dropdown-component-false-options{z-index:10;margin-top:.25rem;max-height:15rem;overflow:auto;border-radius:calc(var(--radius) - 2px);background-color:hsl(var(--background));padding-top:.25rem;padding-bottom:.25rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);--tw-ring-color: rgb(0 0 0 / var(--tw-ring-opacity));--tw-ring-opacity: .05}.dropdown-component-false-options:focus{outline:2px solid transparent;outline-offset:2px}@media (min-width: 640px){.dropdown-component-false-options{font-size:.875rem;line-height:1.25rem}}.dropdown-component-false-options{width:100%}.dropdown-component-false-option{position:relative;cursor:default;-webkit-user-select:none;user-select:none;padding:.125rem 3rem .125rem .75rem}.dropdown-component-true-option{position:relative;cursor:default;-webkit-user-select:none;user-select:none;padding:.5rem 2.25rem .5rem .75rem}.dropdown-component-choosal{position:absolute;top:0;bottom:0;right:0;display:flex;align-items:center;padding-right:1rem}.dropdown-component-check-icon{height:1.25rem;width:1.25rem;--tw-text-opacity: 1;color:rgb(0 0 0 / var(--tw-text-opacity))}.edit-flow-arrangement{display:flex;justify-content:space-between}.edit-flow-span{margin-left:2.5rem}.edit-flow-span{animation:pulse 2s cubic-bezier(.4,0,.6,1) infinite;color:var(--status-red)}.header-menu-bar{display:flex;align-items:center;gap:.125rem;border-radius:calc(var(--radius) - 2px);padding:.25rem .375rem;font-size:.875rem;line-height:1.25rem;font-weight:500}.header-menu-bar-display{display:flex;max-width:120px;cursor:pointer;align-items:center;gap:.5rem}@media (min-width: 1024px){.header-menu-bar-display{max-width:200px}}.header-menu-flow-name{flex:1 1 0%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.header-menu-options{margin-right:.5rem;height:1rem;width:1rem}.header-arrangement{display:flex;width:100%;height:3rem;align-items:center;justify-content:space-between;border-bottom-width:1px;border-color:hsl(var(--border));background-color:hsl(var(--muted))}.header-start-display{display:flex;align-items:center;justify-content:flex-start;gap:.5rem}.header-end-division{display:flex;justify-content:flex-end;padding-left:.5rem;padding-right:.5rem}.header-end-display{margin-left:auto;margin-right:.5rem;display:flex;align-items:center;gap:1.25rem}.header-github-link{display:inline-flex;height:2.25rem;align-items:center;justify-content:center;border-radius:calc(var(--radius) - 2px);border-width:1px;border-color:hsl(var(--input));padding-left:.75rem;padding-right:.75rem;padding-right:0;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);font-size:.875rem;line-height:1.25rem;font-weight:500;color:hsl(var(--muted-foreground));--tw-ring-offset-color: hsl(var(--background))}.header-github-link:disabled{pointer-events:none;opacity:.5}.header-github-link:focus-visible:focus-visible{outline:2px solid transparent;outline-offset:2px;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);--tw-ring-color: hsl(var(--ring));--tw-ring-offset-width: 2px}.header-github-link:hover:hover{background-color:hsl(var(--accent));color:hsl(var(--accent-foreground))}.header-github-display{margin-right:-1px;margin-left:.25rem;display:flex;height:2.25rem;align-items:center;justify-content:center;border-radius:calc(var(--radius) - 2px);border-top-left-radius:0;border-bottom-left-radius:0;border-width:1px;background-color:hsl(var(--background));padding-left:.5rem;padding-right:.5rem;font-size:.875rem;line-height:1.25rem}.header-notifications{position:absolute;right:3px;height:.375rem;width:.375rem;border-radius:9999px;background-color:hsl(var(--destructive))}.input-component-div{pointer-events:none;position:relative;cursor:not-allowed}.input-component-true-button{position:absolute;top:0;bottom:0;right:0;align-items:center;color:hsl(var(--muted-foreground));padding-right:.5rem}.input-component-false-button{position:absolute;top:0;bottom:0;right:0;align-items:center;color:hsl(var(--muted-foreground));padding-left:1rem;padding-right:1rem}.input-component-true-svg{height:1.25rem;width:1.25rem}.input-component-true-svg:hover:hover{color:hsl(var(--accent-foreground))}.input-component-true-svg{position:absolute;bottom:.125rem;right:.5rem}.input-component-false-svg{height:1.25rem;width:1.25rem}.input-component-false-svg:hover:hover{color:hsl(var(--accent-foreground))}.input-component-false-svg{position:absolute;bottom:.5rem;right:.75rem}.input-file-component{display:flex;width:100%;align-items:center}.toggle-component-switch{position:relative;display:inline-flex;height:1.5rem;width:2.75rem;flex-shrink:0;cursor:pointer;border-radius:9999px;border-width:2px;border-color:transparent;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-duration:.2s;transition-timing-function:cubic-bezier(.4,0,.2,1);animation-duration:.2s;animation-timing-function:cubic-bezier(.4,0,.2,1)}.toggle-component-switch:focus:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);--tw-ring-color: hsl(var(--primary));--tw-ring-offset-width: 1px}.toggle-component-span{pointer-events:none;position:relative;height:1.25rem;width:1.25rem;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));border-radius:9999px;--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(0px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000);transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-duration:.2s;transition-timing-function:cubic-bezier(.4,0,.2,1);animation-duration:.2s;animation-timing-function:cubic-bezier(.4,0,.2,1)}.toggle-component-second-span{position:absolute;top:0;right:0;bottom:0;left:0;display:flex;height:100%;width:100%;align-items:center;justify-content:center;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.app-div{position:fixed;bottom:1.25rem;left:1.25rem;display:flex;flex-direction:column-reverse}.code-block-modal{display:flex;align-items:center;justify-content:space-between;padding:.375rem 1rem}.code-block-modal-span{font-size:.75rem;line-height:1rem;text-transform:lowercase;color:hsl(var(--muted-foreground))}.code-block-modal-button{display:flex;align-items:center;gap:.375rem;border-radius:.25rem;background-image:none;padding:.25rem;font-size:.75rem;line-height:1rem;color:hsl(var(--muted-foreground))}.file-card-modal-image-div{position:absolute;right:0;top:0;border-bottom-left-radius:var(--radius);background-color:hsl(var(--muted));padding-left:.25rem;padding-right:.25rem;font-size:.875rem;line-height:1.25rem;font-weight:700;color:hsl(var(--foreground))}.file-card-modal-image-button{padding:.25rem .5rem;color:hsl(var(--ring))}.file-card-modal-button{display:flex;width:50%;align-items:center;justify-content:space-between;border-radius:.25rem;border-width:1px;border-color:hsl(var(--ring));background-color:hsl(var(--muted));padding:.5rem;color:hsl(var(--foreground));--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.file-card-modal-button:hover{--tw-drop-shadow: drop-shadow(0 10px 8px rgb(0 0 0 / .04)) drop-shadow(0 4px 3px rgb(0 0 0 / .1));filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.file-card-modal-div{display:flex;width:100%;margin-right:.5rem;align-items:center;gap:.5rem;color:currentColor}.file-card-modal-footer{display:flex;flex-direction:column;align-items:flex-start}.file-card-modal-name{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;font-size:.875rem;line-height:1.25rem;color:currentColor}.file-card-modal-type{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;font-size:.75rem;line-height:1rem;color:hsl(var(--ring))}.edit-node-modal-variable{height:1.25rem;width:1.25rem;stroke-width:2;padding-inline-end:.25rem;color:hsl(var(--muted-foreground))}.edit-node-modal-span{font-size:.875rem;line-height:1.25rem;font-weight:600;color:hsl(var(--primary))}.edit-node-modal-arrangement{display:flex;width:100%;height:-webkit-fit-content;height:-moz-fit-content;height:fit-content;max-height:400px}.edit-node-modal-box{width:100%;border-radius:var(--radius);border-width:1px;border-color:hsl(var(--input));background-color:hsl(var(--background))}.edit-node-modal-table{display:flex;height:-webkit-fit-content;height:-moz-fit-content;height:fit-content;flex-direction:column;gap:1.25rem}.edit-node-modal-table-header{height:2.5rem;border-color:hsl(var(--input));font-size:.75rem;line-height:1rem;font-weight:500;color:hsl(var(--ring))}.link-color{font-weight:600;color:hsl(var(--foreground))}.api-modal-tabs{display:flex;height:100%;max-width:100%;flex-direction:column;overflow:hidden;border-radius:calc(var(--radius) - 2px);border-width:1px;background-color:hsl(var(--muted));text-align:center}@media (min-width: 640px){.api-modal-tabs{width:75vw}}@media (min-width: 768px){.api-modal-tabs{width:75vw}}@media (min-width: 1024px){.api-modal-tabs{width:75vw}}@media (min-width: 1280px){.api-modal-tabs{width:76vw}}@media (min-width: 1536px){.api-modal-tabs{width:100%}}.api-modal-tablist-div{display:flex;align-items:center;justify-content:space-between;padding-left:.5rem;padding-right:.5rem}.api-modal-tabs-content{margin-top:-.25rem;height:100%;width:100%;overflow:hidden;padding-left:1rem;padding-right:1rem;padding-bottom:1rem}.api-modal-table-arrangement{display:flex;height:-webkit-fit-content;height:-moz-fit-content;height:fit-content;flex-direction:column;gap:1.25rem}.icons-parameters-comp{margin-left:.75rem;height:1.5rem;width:1.5rem}.form-modal-lock-true{background-color:hsl(var(--input));color:hsl(var(--primary))}.form-modal-no-input{background-color:hsl(var(--input));text-align:center;color:hsl(var(--primary))}:is(.dark .form-modal-no-input){--tw-bg-opacity: 1;background-color:rgb(55 65 81 / var(--tw-bg-opacity));--tw-text-opacity: 1;color:rgb(209 213 219 / var(--tw-text-opacity))}.form-modal-lock-false{background-color:var(--white);color:hsl(var(--primary))}.code-highlight{display:block;max-height:64vh;width:100%;overflow-y:hidden;border-width:0px;padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;outline-width:0px;word-break:break-word}.code-nohighlight{display:block;max-height:70vh;width:100%;overflow-y:hidden;border-width:0px;padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;outline-width:0px;word-break:break-word}.form-modal-lockchat{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}.form-modal-lockchat:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}.form-modal-lockchat::placeholder{color:#6b7280;opacity:1}.form-modal-lockchat::-webkit-datetime-edit-fields-wrapper{padding:0}.form-modal-lockchat::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}.form-modal-lockchat::-webkit-datetime-edit{display:inline-flex}.form-modal-lockchat::-webkit-datetime-edit,.form-modal-lockchat::-webkit-datetime-edit-year-field,.form-modal-lockchat::-webkit-datetime-edit-month-field,.form-modal-lockchat::-webkit-datetime-edit-day-field,.form-modal-lockchat::-webkit-datetime-edit-hour-field,.form-modal-lockchat::-webkit-datetime-edit-minute-field,.form-modal-lockchat::-webkit-datetime-edit-second-field,.form-modal-lockchat::-webkit-datetime-edit-millisecond-field,.form-modal-lockchat::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}.form-modal-lockchat{display:block;width:100%;border-radius:calc(var(--radius) - 2px);border-color:hsl(var(--border));padding:1rem 4rem 1rem 1rem}.form-modal-lockchat::-webkit-scrollbar{width:8px;height:8px}.form-modal-lockchat::-webkit-scrollbar-track{background-color:#f1f1f1}.form-modal-lockchat::-webkit-scrollbar-thumb{background-color:#ccc;border-radius:999px}.form-modal-lockchat::-webkit-scrollbar-thumb:hover{background-color:#bbb}.form-modal-lockchat{cursor:auto}.form-modal-lockchat:focus{border-color:hsl(var(--ring));--tw-ring-color: hsl(var(--ring))}@media (min-width: 640px){.form-modal-lockchat{font-size:.875rem;line-height:1.25rem}}.form-modal-send-icon-position{position:absolute;bottom:.5rem;right:1rem}.form-modal-send-button{border-radius:calc(var(--radius) - 2px);padding:.5rem .25rem;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.3s;animation-duration:.3s}.form-modal-lock-icon{margin-left:.25rem;margin-right:.25rem;height:1.25rem;width:1.25rem}.form-modal-lock-icon{animation:pulse 2s cubic-bezier(.4,0,.6,1) infinite}.form-modal-send-icon{margin-right:.5rem;height:1.25rem;width:1.25rem;--tw-rotate: 44deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.form-modal-play-icon{margin-left:.25rem;margin-right:.25rem;height:1.25rem;width:1.25rem}.form-modal-chat-position{display:flex;width:100%;padding:1.5rem 2.25rem 1.5rem 1rem}.form-modal-chatbot-icon{margin:.25rem 1.5rem .75rem .75rem}.form-modal-chat-image{display:flex;flex-direction:column;align-items:center;gap:.25rem}.form-modal-chat-bot-icon{position:relative;display:flex;height:2rem;width:2rem;align-items:center;justify-content:center;overflow:hidden;border-radius:calc(var(--radius) - 2px);padding:1.25rem;font-size:1.5rem;line-height:2rem;background-color:var(--chat-bot-icon)}.form-modal-chat-user-icon{position:relative;display:flex;height:2rem;width:2rem;align-items:center;justify-content:center;overflow:hidden;border-radius:calc(var(--radius) - 2px);padding:1.25rem;font-size:1.5rem;line-height:2rem;background-color:var(--chat-user-icon)}.form-modal-chat-icon-img{position:absolute;--tw-scale-x: 60%;--tw-scale-y: 60%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.form-modal-chat-text-position{display:flex;width:100%;flex:1 1 0%;text-align:start}.form-modal-chat-text{position:relative;display:flex;width:100%;flex-direction:column;text-align:start;font-size:.875rem;line-height:1.25rem;font-weight:400;color:hsl(var(--muted-foreground))}.form-modal-chat-icon-div{position:absolute;left:-1.5rem;top:-.75rem;cursor:pointer}.form-modal-chat-icon{height:1rem;width:1rem}.form-modal-chat-icon{animation:bounce 1s infinite}.form-modal-chat-thought{border-radius:calc(var(--radius) - 2px);border-width:1px;border-color:hsl(var(--ring) / .6);height:100%;width:95%;cursor:pointer;overflow:scroll;background-color:hsl(var(--background));padding:.5rem;text-align:start;color:hsl(var(--primary));-ms-overflow-style:none;scrollbar-width:none}.form-modal-chat-thought::-webkit-scrollbar{display:none}.form-modal-markdown-span{margin-top:.25rem}.form-modal-markdown-span{animation:pulse 2s cubic-bezier(.4,0,.6,1) infinite;cursor:default}.form-modal-initial-prompt-btn{margin-bottom:.5rem;display:flex;align-items:center;gap:.5rem;border-radius:calc(var(--radius) - 2px);border-width:1px;border-color:hsl(var(--border));background-color:hsl(var(--background));padding:.5rem 1rem;font-size:.875rem;line-height:1.25rem;font-weight:600;--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.form-modal-iv-box{display:flex;width:100%;margin-top:.5rem;height:80vh}.form-modal-iv-size{margin-right:1.5rem;display:flex;height:100%;width:33.333333%;flex-direction:column;justify-content:flex-start;overflow:auto;-ms-overflow-style:none;scrollbar-width:none}.form-modal-iv-size::-webkit-scrollbar{display:none}.file-component-arrangement{display:flex;align-items:center;padding-top:.5rem;padding-bottom:.5rem}.file-component-variable{margin-left:-1px;margin-right:.25rem;height:1rem;width:1rem;color:hsl(var(--primary))}.file-component-variables-span{font-weight:600;color:hsl(var(--primary))}.file-component-variables-title{display:flex;align-items:center;justify-content:space-between;padding-top:.5rem}.file-component-variables-div{margin-right:.625rem;display:flex;align-items:center}.file-component-accordion-div{display:flex;align-items:flex-start;gap:.75rem}.file-component-badge-div{display:flex;width:100%;align-items:center;justify-content:space-between}.file-component-tab-column{display:flex;flex-direction:column;gap:.5rem;padding:.25rem}.eraser-column-arrangement{display:flex;width:100%;flex:1 1 0%;flex-direction:column}.eraser-size{position:relative;display:flex;height:100%;width:100%;flex-direction:column;border-radius:calc(var(--radius) - 2px);border-width:1px;background-color:hsl(var(--muted))}.eraser-position{position:absolute;right:.75rem;top:.75rem;z-index:50}.chat-message-div{display:flex;width:100%;height:100%;flex-direction:column;align-items:center;overflow:scroll;-ms-overflow-style:none;scrollbar-width:none}.chat-message-div::-webkit-scrollbar{display:none}.chat-alert-box{display:flex;width:100%;height:100%;flex-direction:column;align-items:center;justify-content:center;text-align:center;vertical-align:middle}.langflow-chat-span{font-size:1.125rem;line-height:1.75rem;color:hsl(var(--foreground))}.langflow-chat-desc{width:50%;border-radius:calc(var(--radius) - 2px);border-width:1px;border-color:hsl(var(--border));background-color:hsl(var(--muted));padding:2rem 1.5rem}.langflow-chat-desc-span{font-size:1rem;line-height:1.5rem;color:hsl(var(--muted-foreground))}.langflow-chat-input-div{display:flex;width:100%;flex-direction:column;align-items:center;justify-content:space-between;padding-left:2rem;padding-right:2rem;padding-bottom:1.5rem}.langflow-chat-input{position:relative;width:100%;border-radius:calc(var(--radius) - 2px);--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.tooltip-fixed-width{max-height:25vh;max-width:30vw;overflow:auto}.export-modal-save-api{font-weight:500;line-height:1}.peer:disabled~.export-modal-save-api{cursor:not-allowed;opacity:.7}.beta-badge-wrapper{position:absolute;right:0;top:0;height:4rem;width:4rem;overflow:hidden;border-top-right-radius:var(--radius)}.beta-badge-content{margin-top:.5rem;width:6rem;--tw-rotate: 45deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));background-color:var(--beta-background);text-align:center;font-size:.75rem;line-height:1rem;font-weight:600;color:var(--beta-foreground)}.chat-message-highlight{border-radius:calc(var(--radius) - 2px);--tw-bg-opacity: 1;background-color:rgb(224 231 255 / var(--tw-bg-opacity));padding-left:.125rem;padding-right:.125rem}:is(.dark .chat-message-highlight){--tw-bg-opacity: 1;background-color:rgb(49 46 129 / var(--tw-bg-opacity))}.field-invalid{position:absolute;font-size:.8rem;font-weight:500;color:hsl(var(--destructive))}.input-invalid{border-color:hsl(var(--destructive))}.input-invalid:focus{border-color:hsl(var(--destructive));--tw-ring-color: hsl(var(--destructive))}.fade-container{position:relative;overflow:hidden}.fade-container:before,.fade-container:after{pointer-events:none;position:absolute;bottom:0;top:0;background-image:linear-gradient(to right,var(--tw-gradient-stops));--tw-gradient-from: hsl(var(--background)) var(--tw-gradient-from-position);--tw-gradient-to: hsl(var(--background) / 0) var(--tw-gradient-to-position);--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);--tw-gradient-to: transparent var(--tw-gradient-to-position);content:"";width:50px;opacity:0;transition:opacity .3s}.fade-container:after{right:0;transform:rotate(180deg)}.fade-container.fade-left:before,.fade-container.fade-right:after{opacity:1}.fade-container-dark.fade-left:before,.fade-container-dark.fade-right:after{opacity:1}.scroll-container{display:flex;overflow-x:scroll;-ms-overflow-style:none;scrollbar-width:none}.scroll-container::-webkit-scrollbar{display:none}.store-beta-icon{position:relative;bottom:.75rem;left:.25rem;margin-left:.5rem;border-radius:9999px;background-color:var(--beta-background);padding:.25rem .5rem;text-align:center;font-size:.75rem;line-height:1rem;font-weight:600;color:var(--beta-foreground)}.sr-only{position:absolute!important;width:1px!important;height:1px!important;padding:0!important;margin:-1px!important;overflow:hidden!important;clip:rect(0,0,0,0)!important;white-space:nowrap!important;border-width:0!important}.pointer-events-none{pointer-events:none!important}.visible{visibility:visible!important}.fixed{position:fixed!important}.absolute{position:absolute!important}.relative{position:relative!important}.sticky{position:-webkit-sticky!important;position:sticky!important}.inset-0{top:0!important;right:0!important;bottom:0!important;left:0!important}.inset-x-6{left:1.5rem!important;right:1.5rem!important}.bottom-0{bottom:0!important}.bottom-0\.5{bottom:.125rem!important}.bottom-20{bottom:5rem!important}.bottom-\[1px\]{bottom:1px!important}.left-0{left:0!important}.left-1{left:.25rem!important}.left-2{left:.5rem!important}.left-\[50\%\]{left:50%!important}.left-\[500\%\]{left:500%!important}.right-0{right:0!important}.right-2{right:.5rem!important}.right-4{right:1rem!important}.top-0{top:0!important}.top-0\.5{top:.125rem!important}.top-4{top:1rem!important}.top-\[50\%\]{top:50%!important}.top-\[500\%\]{top:500%!important}.isolate{isolation:isolate!important}.z-50{z-index:50!important}.z-\[9999\]{z-index:9999!important}.float-right{float:right!important}.-m-0{margin:-0px!important}.-m-0\.5{margin:-.125rem!important}.-m-1{margin:-.25rem!important}.m-1{margin:.25rem!important}.m-4{margin:1rem!important}.m-auto{margin:auto!important}.-mx-1{margin-left:-.25rem!important;margin-right:-.25rem!important}.-mx-1\.5{margin-left:-.375rem!important;margin-right:-.375rem!important}.-my-1{margin-top:-.25rem!important;margin-bottom:-.25rem!important}.-my-1\.5{margin-top:-.375rem!important;margin-bottom:-.375rem!important}.mx-0{margin-left:0!important;margin-right:0!important}.mx-0\.5{margin-left:.125rem!important;margin-right:.125rem!important}.mx-1{margin-left:.25rem!important;margin-right:.25rem!important}.mx-2{margin-left:.5rem!important;margin-right:.5rem!important}.mx-\[0\.08rem\]{margin-left:.08rem!important;margin-right:.08rem!important}.mx-auto{margin-left:auto!important;margin-right:auto!important}.my-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-12{margin-top:3rem!important;margin-bottom:3rem!important}.my-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-3{margin-top:.75rem!important;margin-bottom:.75rem!important}.my-6{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-auto{margin-top:auto!important;margin-bottom:auto!important}.-mb-1{margin-bottom:-.25rem!important}.-ml-0{margin-left:-0px!important}.-ml-0\.5{margin-left:-.125rem!important}.-ml-1{margin-left:-.25rem!important}.-ml-px{margin-left:-1px!important}.-mr-0{margin-right:-0px!important}.-mr-0\.5{margin-right:-.125rem!important}.mb-1{margin-bottom:.25rem!important}.mb-2{margin-bottom:.5rem!important}.mb-24{margin-bottom:6rem!important}.mb-3{margin-bottom:.75rem!important}.mb-4{margin-bottom:1rem!important}.mb-6{margin-bottom:1.5rem!important}.mb-auto{margin-bottom:auto!important}.ml-1{margin-left:.25rem!important}.ml-2{margin-left:.5rem!important}.ml-3{margin-left:.75rem!important}.ml-4{margin-left:1rem!important}.ml-auto{margin-left:auto!important}.mr-1{margin-right:.25rem!important}.mr-2{margin-right:.5rem!important}.mr-3{margin-right:.75rem!important}.mr-4{margin-right:1rem!important}.mt-0{margin-top:0!important}.mt-1{margin-top:.25rem!important}.mt-2{margin-top:.5rem!important}.mt-3{margin-top:.75rem!important}.mt-4{margin-top:1rem!important}.mt-5{margin-top:1.25rem!important}.mt-6{margin-top:1.5rem!important}.mt-8{margin-top:2rem!important}.block{display:block!important}.\!inline,.inline{display:inline!important}.flex{display:flex!important}.inline-flex{display:inline-flex!important}.table{display:table!important}.grid{display:grid!important}.contents{display:contents!important}.\!hidden,.hidden{display:none!important}.h-0{height:0px!important}.h-1\/4{height:25%!important}.h-10{height:2.5rem!important}.h-11{height:2.75rem!important}.h-12{height:3rem!important}.h-16{height:4rem!important}.h-2{height:.5rem!important}.h-2\/6{height:33.333333%!important}.h-24{height:6rem!important}.h-3{height:.75rem!important}.h-3\.5{height:.875rem!important}.h-4{height:1rem!important}.h-5{height:1.25rem!important}.h-6{height:1.5rem!important}.h-7{height:1.75rem!important}.h-8{height:2rem!important}.h-9{height:2.25rem!important}.h-\[1\.1rem\]{height:1.1rem!important}.h-\[11rem\]{height:11rem!important}.h-\[1px\]{height:1px!important}.h-\[24px\]{height:24px!important}.h-\[40vh\]{height:40vh!important}.h-\[500px\]{height:500px!important}.h-\[60vh\]{height:60vh!important}.h-\[70vh\]{height:70vh!important}.h-\[80vh\]{height:80vh!important}.h-\[var\(--radix-select-trigger-height\)\]{height:var(--radix-select-trigger-height)!important}.h-fit{height:-webkit-fit-content!important;height:-moz-fit-content!important;height:fit-content!important}.h-full{height:100%!important}.h-px{height:1px!important}.h-screen{height:100vh!important}.max-h-20{max-height:5rem!important}.max-h-48{max-height:12rem!important}.max-h-96{max-height:24rem!important}.max-h-\[100px\]{max-height:100px!important}.max-h-\[10rem\]{max-height:10rem!important}.max-h-\[15rem\]{max-height:15rem!important}.max-h-\[300px\]{max-height:300px!important}.w-1\/2{width:50%!important}.w-1\/4{width:25%!important}.w-1\/6{width:16.666667%!important}.w-12{width:3rem!important}.w-16{width:4rem!important}.w-2{width:.5rem!important}.w-24{width:6rem!important}.w-28{width:7rem!important}.w-3{width:.75rem!important}.w-3\.5{width:.875rem!important}.w-32{width:8rem!important}.w-4{width:1rem!important}.w-40{width:10rem!important}.w-44{width:11rem!important}.w-5{width:1.25rem!important}.w-5\/6{width:83.333333%!important}.w-6{width:1.5rem!important}.w-7{width:1.75rem!important}.w-72{width:18rem!important}.w-8{width:2rem!important}.w-96{width:24rem!important}.w-\[1\.1rem\]{width:1.1rem!important}.w-\[100px\]{width:100px!important}.w-\[1010px\]{width:1010px!important}.w-\[160px\]{width:160px!important}.w-\[1px\]{width:1px!important}.w-\[200px\]{width:200px!important}.w-\[250px\]{width:250px!important}.w-\[300px\]{width:300px!important}.w-\[31px\]{width:31px!important}.w-\[40\%\]{width:40%!important}.w-\[44px\]{width:44px!important}.w-\[500px\]{width:500px!important}.w-\[80\%\]{width:80%!important}.w-\[90\%\]{width:90%!important}.w-fit{width:-webkit-fit-content!important;width:-moz-fit-content!important;width:fit-content!important}.w-full{width:100%!important}.w-screen{width:100vw!important}.min-w-\[12rem\]{min-width:12rem!important}.min-w-\[20vw\]{min-width:20vw!important}.min-w-\[40vw\]{min-width:40vw!important}.min-w-\[60vw\]{min-width:60vw!important}.min-w-\[80vw\]{min-width:80vw!important}.min-w-\[8rem\]{min-width:8rem!important}.min-w-\[var\(--radix-select-trigger-width\)\]{min-width:var(--radix-select-trigger-width)!important}.min-w-full{min-width:100%!important}.min-w-min{min-width:-webkit-min-content!important;min-width:min-content!important}.max-w-\[40vw\]{max-width:40vw!important}.max-w-lg{max-width:32rem!important}.flex-1{flex:1 1 0%!important}.flex-shrink-0,.shrink-0{flex-shrink:0!important}.flex-grow{flex-grow:1!important}.basis-1\/2{flex-basis:50%!important}.basis-5\/6{flex-basis:83.333333%!important}.table-fixed{table-layout:fixed!important}.caption-bottom{caption-side:bottom!important}.translate-x-0{--tw-translate-x: 0px !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-x-5{--tw-translate-x: 1.25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-x-\[-100\%\]{--tw-translate-x: -100% !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-x-\[-50\%\]{--tw-translate-x: -50% !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-y-0{--tw-translate-y: 0px !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-y-96{--tw-translate-y: 24rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.translate-y-\[-50\%\]{--tw-translate-y: -50% !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.rotate-180{--tw-rotate: 180deg !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.rotate-90{--tw-rotate: 90deg !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}@keyframes bounce{0%,to{transform:translateY(-25%);animation-timing-function:cubic-bezier(.8,0,1,1)}50%{transform:none;animation-timing-function:cubic-bezier(0,0,.2,1)}}.animate-bounce{animation:bounce 1s infinite!important}@keyframes pulse{50%{opacity:.5}}.animate-pulse{animation:pulse 2s cubic-bezier(.4,0,.6,1) infinite!important}@keyframes spin{to{transform:rotate(360deg)}}.animate-spin{animation:spin 1s linear infinite!important}.cursor-default{cursor:default!important}.cursor-grabbing{cursor:grabbing!important}.cursor-not-allowed{cursor:not-allowed!important}.cursor-pointer{cursor:pointer!important}.select-none{-webkit-user-select:none!important;user-select:none!important}.resize{resize:both!important}.list-disc{list-style-type:disc!important}.grid-cols-1{grid-template-columns:repeat(1,minmax(0,1fr))!important}.flex-row{flex-direction:row!important}.flex-row-reverse{flex-direction:row-reverse!important}.flex-col{flex-direction:column!important}.flex-col-reverse{flex-direction:column-reverse!important}.flex-wrap{flex-wrap:wrap!important}.items-start{align-items:flex-start!important}.items-end{align-items:flex-end!important}.items-center{align-items:center!important}.justify-start{justify-content:flex-start!important}.justify-end{justify-content:flex-end!important}.justify-center{justify-content:center!important}.justify-between{justify-content:space-between!important}.gap-0{gap:0px!important}.gap-0\.5{gap:.125rem!important}.gap-1{gap:.25rem!important}.gap-1\.5{gap:.375rem!important}.gap-2{gap:.5rem!important}.gap-3{gap:.75rem!important}.gap-4{gap:1rem!important}.gap-5{gap:1.25rem!important}.gap-8{gap:2rem!important}.gap-\[4px\]{gap:4px!important}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(.25rem * var(--tw-space-x-reverse))!important;margin-left:calc(.25rem * calc(1 - var(--tw-space-x-reverse)))!important}.space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(.5rem * var(--tw-space-x-reverse))!important;margin-left:calc(.5rem * calc(1 - var(--tw-space-x-reverse)))!important}.space-x-6>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(1.5rem * var(--tw-space-x-reverse))!important;margin-left:calc(1.5rem * calc(1 - var(--tw-space-x-reverse)))!important}.space-y-0>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(0px * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(0px * var(--tw-space-y-reverse))!important}.space-y-0\.5>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(.125rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(.125rem * var(--tw-space-y-reverse))!important}.space-y-1>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(.25rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(.25rem * var(--tw-space-y-reverse))!important}.space-y-1\.5>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(.375rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(.375rem * var(--tw-space-y-reverse))!important}.space-y-2>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(.5rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(.5rem * var(--tw-space-y-reverse))!important}.space-y-6>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(1.5rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(1.5rem * var(--tw-space-y-reverse))!important}.space-y-8>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(2rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(2rem * var(--tw-space-y-reverse))!important}.overflow-auto{overflow:auto!important}.overflow-hidden{overflow:hidden!important}.overflow-scroll{overflow:scroll!important}.overflow-y-auto{overflow-y:auto!important}.overflow-x-hidden{overflow-x:hidden!important}.overflow-x-clip{overflow-x:clip!important}.overflow-y-scroll{overflow-y:scroll!important}.truncate{overflow:hidden!important;text-overflow:ellipsis!important;white-space:nowrap!important}.text-clip{text-overflow:clip!important}.whitespace-nowrap{white-space:nowrap!important}.whitespace-break-spaces{white-space:break-spaces!important}.break-words{overflow-wrap:break-word!important}.rounded{border-radius:.25rem!important}.rounded-full{border-radius:9999px!important}.rounded-lg{border-radius:var(--radius)!important}.rounded-md{border-radius:calc(var(--radius) - 2px)!important}.rounded-sm{border-radius:calc(var(--radius) - 4px)!important}.rounded-l-md{border-top-left-radius:calc(var(--radius) - 2px)!important;border-bottom-left-radius:calc(var(--radius) - 2px)!important}.rounded-r-md{border-top-right-radius:calc(var(--radius) - 2px)!important;border-bottom-right-radius:calc(var(--radius) - 2px)!important}.rounded-t-lg{border-top-left-radius:var(--radius)!important;border-top-right-radius:var(--radius)!important}.border{border-width:1px!important}.border-0{border-width:0px!important}.border-2{border-width:2px!important}.border-\[1px\]{border-width:1px!important}.border-b{border-bottom-width:1px!important}.border-b-2{border-bottom-width:2px!important}.border-border{border-color:hsl(var(--border))!important}.border-error{--tw-border-opacity: 1 !important;border-color:var(--fallback-er,oklch(var(--er)/var(--tw-border-opacity)))!important}.border-gray-300{--tw-border-opacity: 1 !important;border-color:rgb(209 213 219 / var(--tw-border-opacity))!important}.border-indigo-300{--tw-border-opacity: 1 !important;border-color:rgb(165 180 252 / var(--tw-border-opacity))!important}.border-input{border-color:hsl(var(--input))!important}.border-muted{border-color:hsl(var(--muted))!important}.border-primary{border-color:hsl(var(--primary))!important}.border-ring{border-color:hsl(var(--ring))!important}.border-ring\/60{border-color:hsl(var(--ring) / .6)!important}.border-transparent{border-color:transparent!important}.\!bg-white{background-color:var(--white)!important}.bg-accent{background-color:hsl(var(--accent))!important}.bg-background{background-color:hsl(var(--background))!important}.bg-beta-foreground{background-color:var(--beta-foreground)!important}.bg-blur-shared{background-color:var(--blur-shared)!important}.bg-border{background-color:hsl(var(--border))!important}.bg-chat-send{background-color:var(--chat-send)!important}.bg-destructive{background-color:hsl(var(--destructive))!important}.bg-error-background{background-color:var(--error-background)!important}.bg-foreground{background-color:hsl(var(--foreground))!important}.bg-high-indigo{background-color:var(--high-indigo)!important}.bg-info-background{background-color:var(--info-background)!important}.bg-input{background-color:hsl(var(--input))!important}.bg-muted{background-color:hsl(var(--muted))!important}.bg-popover{background-color:hsl(var(--popover))!important}.bg-primary{background-color:hsl(var(--primary))!important}.bg-ring\/40{background-color:hsl(var(--ring) / .4)!important}.bg-secondary{background-color:hsl(var(--secondary))!important}.bg-status-blue{background-color:var(--status-blue)!important}.bg-status-green{background-color:var(--status-green)!important}.bg-status-red{background-color:var(--status-red)!important}.bg-status-yellow{background-color:var(--status-yellow)!important}.bg-success-background{background-color:var(--success-background)!important}.bg-transparent{background-color:transparent!important}.bg-opacity-50{--tw-bg-opacity: .5 !important}.bg-gradient-to-br{background-image:linear-gradient(to bottom right,var(--tw-gradient-stops))!important}.bg-gradient-to-r{background-image:linear-gradient(to right,var(--tw-gradient-stops))!important}.bg-gradient-to-tr{background-image:linear-gradient(to top right,var(--tw-gradient-stops))!important}.bg-none{background-image:none!important}.from-amber-200{--tw-gradient-from: #fde68a var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(253 230 138 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-amber-700{--tw-gradient-from: #b45309 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(180 83 9 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-blue-100{--tw-gradient-from: #dbeafe var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(219 234 254 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-blue-300{--tw-gradient-from: #93c5fd var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(147 197 253 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-blue-700{--tw-gradient-from: #1d4ed8 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(29 78 216 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-emerald-500{--tw-gradient-from: #10b981 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(16 185 129 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-fuchsia-500{--tw-gradient-from: #d946ef var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(217 70 239 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-fuchsia-600{--tw-gradient-from: #c026d3 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(192 38 211 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-gray-300{--tw-gradient-from: #d1d5db var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(209 213 219 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-gray-800{--tw-gradient-from: #1f2937 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(31 41 55 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-gray-900{--tw-gradient-from: #111827 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(17 24 39 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-green-200{--tw-gradient-from: #bbf7d0 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(187 247 208 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-green-300{--tw-gradient-from: #86efac var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(134 239 172 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-green-500{--tw-gradient-from: #22c55e var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(34 197 94 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-lime-600{--tw-gradient-from: #65a30d var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(101 163 13 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-purple-400{--tw-gradient-from: #c084fc var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(192 132 252 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-red-400{--tw-gradient-from: #f87171 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(248 113 113 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-red-800{--tw-gradient-from: #991b1b var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(153 27 27 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-rose-400{--tw-gradient-from: #fb7185 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(251 113 133 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-rose-500{--tw-gradient-from: #f43f5e var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(244 63 94 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-sky-400{--tw-gradient-from: #38bdf8 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(56 189 248 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-violet-500{--tw-gradient-from: #8b5cf6 var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(139 92 246 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.from-yellow-200{--tw-gradient-from: #fef08a var(--tw-gradient-from-position) !important;--tw-gradient-to: rgb(254 240 138 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to) !important}.via-blue-300{--tw-gradient-to: rgb(147 197 253 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #93c5fd var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-blue-800{--tw-gradient-to: rgb(30 64 175 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #1e40af var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-fuchsia-500{--tw-gradient-to: rgb(217 70 239 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #d946ef var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-fuchsia-600{--tw-gradient-to: rgb(192 38 211 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #c026d3 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-gray-300{--tw-gradient-to: rgb(209 213 219 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #d1d5db var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-green-200{--tw-gradient-to: rgb(187 247 208 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #bbf7d0 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-green-300{--tw-gradient-to: rgb(134 239 172 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #86efac var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-green-400{--tw-gradient-to: rgb(74 222 128 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #4ade80 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-orange-300{--tw-gradient-to: rgb(253 186 116 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #fdba74 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-pink-200{--tw-gradient-to: rgb(251 207 232 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #fbcfe8 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-purple-900{--tw-gradient-to: rgb(88 28 135 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #581c87 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-red-400{--tw-gradient-to: rgb(248 113 113 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #f87171 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-red-500{--tw-gradient-to: rgb(239 68 68 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #ef4444 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-red-600{--tw-gradient-to: rgb(220 38 38 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #dc2626 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-rose-400{--tw-gradient-to: rgb(251 113 133 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #fb7185 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-rose-700{--tw-gradient-to: rgb(190 18 60 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #be123c var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-violet-600{--tw-gradient-to: rgb(124 58 237 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #7c3aed var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-yellow-300{--tw-gradient-to: rgb(253 224 71 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #fde047 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-yellow-400{--tw-gradient-to: rgb(250 204 21 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #facc15 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.via-yellow-600{--tw-gradient-to: rgb(202 138 4 / 0) var(--tw-gradient-to-position) !important;--tw-gradient-stops: var(--tw-gradient-from), #ca8a04 var(--tw-gradient-via-position), var(--tw-gradient-to) !important}.to-blue-500{--tw-gradient-to: #3b82f6 var(--tw-gradient-to-position) !important}.to-fuchsia-500{--tw-gradient-to: #d946ef var(--tw-gradient-to-position) !important}.to-gray-600{--tw-gradient-to: #4b5563 var(--tw-gradient-to-position) !important}.to-gray-900{--tw-gradient-to: #111827 var(--tw-gradient-to-position) !important}.to-green-500{--tw-gradient-to: #22c55e var(--tw-gradient-to-position) !important}.to-green-700{--tw-gradient-to: #15803d var(--tw-gradient-to-position) !important}.to-indigo-500{--tw-gradient-to: #6366f1 var(--tw-gradient-to-position) !important}.to-indigo-700{--tw-gradient-to: #4338ca var(--tw-gradient-to-position) !important}.to-indigo-900{--tw-gradient-to: #312e81 var(--tw-gradient-to-position) !important}.to-lime-400{--tw-gradient-to: #a3e635 var(--tw-gradient-to-position) !important}.to-lime-600{--tw-gradient-to: #65a30d var(--tw-gradient-to-position) !important}.to-orange-300{--tw-gradient-to: #fdba74 var(--tw-gradient-to-position) !important}.to-orange-400{--tw-gradient-to: #fb923c var(--tw-gradient-to-position) !important}.to-orange-600{--tw-gradient-to: #ea580c var(--tw-gradient-to-position) !important}.to-pink-400{--tw-gradient-to: #f472b6 var(--tw-gradient-to-position) !important}.to-pink-600{--tw-gradient-to: #db2777 var(--tw-gradient-to-position) !important}.to-purple-400{--tw-gradient-to: #c084fc var(--tw-gradient-to-position) !important}.to-purple-700{--tw-gradient-to: #7e22ce var(--tw-gradient-to-position) !important}.to-red-500{--tw-gradient-to: #ef4444 var(--tw-gradient-to-position) !important}.to-red-600{--tw-gradient-to: #dc2626 var(--tw-gradient-to-position) !important}.to-rose-800{--tw-gradient-to: #9f1239 var(--tw-gradient-to-position) !important}.to-sky-900{--tw-gradient-to: #0c4a6e var(--tw-gradient-to-position) !important}.to-violet-600{--tw-gradient-to: #7c3aed var(--tw-gradient-to-position) !important}.to-violet-900{--tw-gradient-to: #4c1d95 var(--tw-gradient-to-position) !important}.to-yellow-300{--tw-gradient-to: #fde047 var(--tw-gradient-to-position) !important}.to-yellow-400{--tw-gradient-to: #facc15 var(--tw-gradient-to-position) !important}.to-yellow-500{--tw-gradient-to: #eab308 var(--tw-gradient-to-position) !important}.to-yellow-700{--tw-gradient-to: #a16207 var(--tw-gradient-to-position) !important}.fill-almost-medium-blue{fill:var(--almost-medium-blue)!important}.fill-build-trigger{fill:var(--build-trigger)!important}.fill-current{fill:currentColor!important}.fill-destructive{fill:hsl(var(--destructive))!important}.fill-foreground{fill:hsl(var(--foreground))!important}.stroke-build-trigger{stroke:var(--build-trigger)!important}.stroke-connection{stroke:var(--connection)!important}.stroke-destructive{stroke:hsl(var(--destructive))!important}.stroke-foreground{stroke:hsl(var(--foreground))!important}.stroke-gray-800{stroke:#1f2937!important}.stroke-gray-900{stroke:#111827!important}.stroke-1{stroke-width:1!important}.stroke-\[1\.5\]{stroke-width:1.5!important}.p-0{padding:0!important}.p-0\.5{padding:.125rem!important}.p-1{padding:.25rem!important}.p-1\.5{padding:.375rem!important}.p-2{padding:.5rem!important}.p-2\.5{padding:.625rem!important}.p-3{padding:.75rem!important}.p-4{padding:1rem!important}.p-6{padding:1.5rem!important}.p-8{padding:2rem!important}.px-0{padding-left:0!important;padding-right:0!important}.px-0\.5{padding-left:.125rem!important;padding-right:.125rem!important}.px-1{padding-left:.25rem!important;padding-right:.25rem!important}.px-16{padding-left:4rem!important;padding-right:4rem!important}.px-2{padding-left:.5rem!important;padding-right:.5rem!important}.px-2\.5{padding-left:.625rem!important;padding-right:.625rem!important}.px-3{padding-left:.75rem!important;padding-right:.75rem!important}.px-4{padding-left:1rem!important;padding-right:1rem!important}.px-5{padding-left:1.25rem!important;padding-right:1.25rem!important}.px-6{padding-left:1.5rem!important;padding-right:1.5rem!important}.px-8{padding-left:2rem!important;padding-right:2rem!important}.py-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-1\.5{padding-top:.375rem!important;padding-bottom:.375rem!important}.py-12{padding-top:3rem!important;padding-bottom:3rem!important}.py-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-3{padding-top:.75rem!important;padding-bottom:.75rem!important}.py-4{padding-top:1rem!important;padding-bottom:1rem!important}.py-5{padding-top:1.25rem!important;padding-bottom:1.25rem!important}.py-6{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-8{padding-top:2rem!important;padding-bottom:2rem!important}.pb-16{padding-bottom:4rem!important}.pb-2{padding-bottom:.5rem!important}.pb-4{padding-bottom:1rem!important}.pb-5{padding-bottom:1.25rem!important}.pb-8{padding-bottom:2rem!important}.pl-1{padding-left:.25rem!important}.pl-2{padding-left:.5rem!important}.pl-3{padding-left:.75rem!important}.pl-5{padding-left:1.25rem!important}.pl-8{padding-left:2rem!important}.pr-1{padding-right:.25rem!important}.pr-10{padding-right:2.5rem!important}.pr-12{padding-right:3rem!important}.pr-2{padding-right:.5rem!important}.pr-3{padding-right:.75rem!important}.pr-8{padding-right:2rem!important}.ps-2{padding-inline-start:.5rem!important}.pt-0{padding-top:0!important}.pt-2{padding-top:.5rem!important}.pt-3{padding-top:.75rem!important}.text-left{text-align:left!important}.text-center{text-align:center!important}.text-right{text-align:right!important}.text-start{text-align:start!important}.text-end{text-align:end!important}.align-middle{vertical-align:middle!important}.font-sans{font-family:var(--font-sans),ui-sans-serif,system-ui,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji"!important}.\!text-xs{font-size:.75rem!important;line-height:1rem!important}.text-2xl{font-size:1.5rem!important;line-height:2rem!important}.text-5xl{font-size:3rem!important;line-height:1!important}.text-\[16px\]{font-size:16px!important}.text-\[8px\]{font-size:8px!important}.text-base{font-size:1rem!important;line-height:1.5rem!important}.text-lg{font-size:1.125rem!important;line-height:1.75rem!important}.text-sm{font-size:.875rem!important;line-height:1.25rem!important}.text-xl{font-size:1.25rem!important;line-height:1.75rem!important}.text-xs{font-size:.75rem!important;line-height:1rem!important}.\!font-normal{font-weight:400!important}.font-bold{font-weight:700!important}.font-light{font-weight:300!important}.font-medium{font-weight:500!important}.font-normal{font-weight:400!important}.font-semibold{font-weight:600!important}.italic{font-style:italic!important}.leading-none{line-height:1!important}.leading-tight{line-height:1.25!important}.tracking-tight{letter-spacing:-.025em!important}.tracking-widest{letter-spacing:.1em!important}.\!text-foreground{color:hsl(var(--foreground))!important}.text-almost-medium-blue{color:var(--almost-medium-blue)!important}.text-background{color:hsl(var(--background))!important}.text-black{--tw-text-opacity: 1 !important;color:rgb(0 0 0 / var(--tw-text-opacity))!important}.text-build-trigger{color:var(--build-trigger)!important}.text-card-foreground{color:hsl(var(--card-foreground))!important}.text-component-icon{color:var(--component-icon)!important}.text-current{color:currentColor!important}.text-destructive{color:hsl(var(--destructive))!important}.text-destructive-foreground{color:hsl(var(--destructive-foreground))!important}.text-error-foreground{color:var(--error-foreground)!important}.text-flow-icon{color:var(--flow-icon)!important}.text-foreground{color:hsl(var(--foreground))!important}.text-gray-500{--tw-text-opacity: 1 !important;color:rgb(107 114 128 / var(--tw-text-opacity))!important}.text-gray-800{--tw-text-opacity: 1 !important;color:rgb(31 41 55 / var(--tw-text-opacity))!important}.text-high-indigo{color:var(--high-indigo)!important}.text-info-foreground{color:var(--info-foreground)!important}.text-muted{color:hsl(var(--muted))!important}.text-muted-foreground{color:hsl(var(--muted-foreground))!important}.text-popover-foreground{color:hsl(var(--popover-foreground))!important}.text-primary{color:hsl(var(--primary))!important}.text-primary-foreground{color:hsl(var(--primary-foreground))!important}.text-primary\/80{color:hsl(var(--primary) / .8)!important}.text-ring{color:hsl(var(--ring))!important}.text-secondary-foreground{color:hsl(var(--secondary-foreground))!important}.text-status-blue{color:var(--status-blue)!important}.text-status-green{color:var(--status-green)!important}.text-status-red{color:var(--status-red)!important}.text-success-foreground{color:var(--success-foreground)!important}.underline{text-decoration-line:underline!important}.underline-offset-4{text-underline-offset:4px!important}.\!opacity-100{opacity:1!important}.opacity-0{opacity:0!important}.opacity-100{opacity:1!important}.opacity-50{opacity:.5!important}.opacity-60{opacity:.6!important}.opacity-70{opacity:.7!important}.\!shadow-md{--tw-shadow: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow-inner{--tw-shadow: inset 0 2px 4px 0 rgb(0 0 0 / .05) !important;--tw-shadow-colored: inset 0 2px 4px 0 var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow-lg{--tw-shadow: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow-md{--tw-shadow: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow-sm{--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05) !important;--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow-xl{--tw-shadow: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.outline-none{outline:2px solid transparent!important;outline-offset:2px!important}.outline{outline-style:solid!important}.outline-1{outline-width:1px!important}.outline-ring{outline-color:hsl(var(--ring))!important}.ring-0{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(0px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.ring-1{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.ring-2{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.ring-inset{--tw-ring-inset: inset !important}.ring-primary{--tw-ring-color: hsl(var(--primary)) !important}.ring-ring{--tw-ring-color: hsl(var(--ring)) !important}.ring-offset-background{--tw-ring-offset-color: hsl(var(--background)) !important}.blur{--tw-blur: blur(8px) !important;filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)!important}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)!important}.backdrop-blur-sm{--tw-backdrop-blur: blur(4px) !important;-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)!important;backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)!important}.transition{transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter!important;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter!important;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter!important;transition-timing-function:cubic-bezier(.4,0,.2,1)!important;transition-duration:.15s!important}.transition-all{transition-property:all!important;transition-timing-function:cubic-bezier(.4,0,.2,1)!important;transition-duration:.15s!important}.transition-colors{transition-property:color,background-color,border-color,text-decoration-color,fill,stroke!important;transition-timing-function:cubic-bezier(.4,0,.2,1)!important;transition-duration:.15s!important}.transition-opacity{transition-property:opacity!important;transition-timing-function:cubic-bezier(.4,0,.2,1)!important;transition-duration:.15s!important}.transition-transform{transition-property:transform!important;transition-timing-function:cubic-bezier(.4,0,.2,1)!important;transition-duration:.15s!important}.delay-500{transition-delay:.5s!important}.duration-100{transition-duration:.1s!important}.duration-200{transition-duration:.2s!important}.duration-300{transition-duration:.3s!important}.duration-500{transition-duration:.5s!important}.ease-in{transition-timing-function:cubic-bezier(.4,0,1,1)!important}.ease-in-out{transition-timing-function:cubic-bezier(.4,0,.2,1)!important}.ease-out{transition-timing-function:cubic-bezier(0,0,.2,1)!important}@keyframes enter{0%{opacity:var(--tw-enter-opacity, 1);transform:translate3d(var(--tw-enter-translate-x, 0),var(--tw-enter-translate-y, 0),0) scale3d(var(--tw-enter-scale, 1),var(--tw-enter-scale, 1),var(--tw-enter-scale, 1)) rotate(var(--tw-enter-rotate, 0))}}@keyframes exit{to{opacity:var(--tw-exit-opacity, 1);transform:translate3d(var(--tw-exit-translate-x, 0),var(--tw-exit-translate-y, 0),0) scale3d(var(--tw-exit-scale, 1),var(--tw-exit-scale, 1),var(--tw-exit-scale, 1)) rotate(var(--tw-exit-rotate, 0))}}.animate-in{animation-name:enter!important;animation-duration:.15s!important;--tw-enter-opacity: initial !important;--tw-enter-scale: initial !important;--tw-enter-rotate: initial !important;--tw-enter-translate-x: initial !important;--tw-enter-translate-y: initial !important}.fade-in-50{--tw-enter-opacity: .5 !important}.slide-in-from-top-1{--tw-enter-translate-y: -.25rem !important}.duration-100{animation-duration:.1s!important}.duration-200{animation-duration:.2s!important}.duration-300{animation-duration:.3s!important}.duration-500{animation-duration:.5s!important}.delay-500{animation-delay:.5s!important}.ease-in{animation-timing-function:cubic-bezier(.4,0,1,1)!important}.ease-in-out{animation-timing-function:cubic-bezier(.4,0,.2,1)!important}.ease-out{animation-timing-function:cubic-bezier(0,0,.2,1)!important}.scrollbar-hide{-ms-overflow-style:none!important;scrollbar-width:none!important}.scrollbar-hide::-webkit-scrollbar{display:none!important}.truncate-multiline{display:-webkit-box!important;-webkit-line-clamp:3!important;-webkit-box-orient:vertical!important;overflow:hidden!important;text-overflow:ellipsis!important}.truncate-doubleline{display:-webkit-box!important;-webkit-line-clamp:2!important;-webkit-box-orient:vertical!important;overflow:hidden!important;text-overflow:ellipsis!important}.word-break-break-word{word-break:break-word!important}.password{-webkit-text-security:disc!important;font-family:text-security-disc!important}.stop{animation-play-state:paused!important}.custom-scroll::-webkit-scrollbar{width:8px!important;height:8px!important}.custom-scroll::-webkit-scrollbar-track{background-color:#f1f1f1!important}.custom-scroll::-webkit-scrollbar-thumb{background-color:#ccc!important;border-radius:999px!important}.custom-scroll::-webkit-scrollbar-thumb:hover{background-color:#bbb!important}.custom-scroll{cursor:auto!important}.\!dark .theme-attribution .react-flow__attribution,.dark .theme-attribution .react-flow__attribution{background-color:#fff3!important;padding:0 5px!important}.\!dark .theme-attribution .react-flow__attribution a,.dark .theme-attribution .react-flow__attribution a{color:#000!important}.text-align-last-left{text-align-last:left!important}@keyframes slideDown{0%{height:0}to{height:var(--radix-accordion-content-height)}}@keyframes slideUp{0%{height:var(--radix-accordion-content-height)}to{height:0}}@keyframes gradient-motion-start{0%{stop-color:#9c8aec}50%{stop-color:#ff82b8}80%{stop-color:#ffa564}to{stop-color:#9c8aec}}@keyframes gradient-motion-end{0%{stop-color:#9c8aec}50%{stop-color:#ffa564}80%{stop-color:#ff82b8}to{stop-color:#9c8aec}}.data-\[invalid\]\:label-invalid[data-invalid]{color:hsl(var(--destructive))}:is(.dark .dark\:prose-invert){--tw-prose-body: var(--tw-prose-invert-body);--tw-prose-headings: var(--tw-prose-invert-headings);--tw-prose-lead: var(--tw-prose-invert-lead);--tw-prose-links: var(--tw-prose-invert-links);--tw-prose-bold: var(--tw-prose-invert-bold);--tw-prose-counters: var(--tw-prose-invert-counters);--tw-prose-bullets: var(--tw-prose-invert-bullets);--tw-prose-hr: var(--tw-prose-invert-hr);--tw-prose-quotes: var(--tw-prose-invert-quotes);--tw-prose-quote-borders: var(--tw-prose-invert-quote-borders);--tw-prose-captions: var(--tw-prose-invert-captions);--tw-prose-kbd: var(--tw-prose-invert-kbd);--tw-prose-kbd-shadows: var(--tw-prose-invert-kbd-shadows);--tw-prose-code: var(--tw-prose-invert-code);--tw-prose-pre-code: var(--tw-prose-invert-pre-code);--tw-prose-pre-bg: var(--tw-prose-invert-pre-bg);--tw-prose-th-borders: var(--tw-prose-invert-th-borders);--tw-prose-td-borders: var(--tw-prose-invert-td-borders)}.placeholder\:text-muted-foreground::placeholder{color:hsl(var(--muted-foreground))!important}.hover\:scale-110:hover{--tw-scale-x: 1.1 !important;--tw-scale-y: 1.1 !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.hover\:border-border:hover{border-color:hsl(var(--border))!important}.hover\:bg-accent:hover{background-color:hsl(var(--accent))!important}.hover\:bg-beta-foreground:hover{background-color:var(--beta-foreground)!important}.hover\:bg-border\/80:hover{background-color:hsl(var(--border) / .8)!important}.hover\:bg-destructive\/80:hover{background-color:hsl(var(--destructive) / .8)!important}.hover\:bg-destructive\/90:hover{background-color:hsl(var(--destructive) / .9)!important}.hover\:bg-muted:hover{background-color:hsl(var(--muted))!important}.hover\:bg-muted\/50:hover{background-color:hsl(var(--muted) / .5)!important}.hover\:bg-primary\/80:hover{background-color:hsl(var(--primary) / .8)!important}.hover\:bg-primary\/90:hover{background-color:hsl(var(--primary) / .9)!important}.hover\:bg-secondary-foreground\/5:hover{background-color:hsl(var(--secondary-foreground) / .05)!important}.hover\:bg-secondary\/80:hover{background-color:hsl(var(--secondary) / .8)!important}.hover\:bg-status-red:hover{background-color:var(--status-red)!important}.hover\:bg-transparent:hover{background-color:transparent!important}.hover\:text-accent-foreground:hover{color:hsl(var(--accent-foreground))!important}.hover\:text-destructive:hover{color:hsl(var(--destructive))!important}.hover\:text-gray-600:hover{--tw-text-opacity: 1 !important;color:rgb(75 85 99 / var(--tw-text-opacity))!important}.hover\:text-indigo-500:hover{--tw-text-opacity: 1 !important;color:rgb(99 102 241 / var(--tw-text-opacity))!important}.hover\:text-muted-foreground:hover{color:hsl(var(--muted-foreground))!important}.hover\:text-primary:hover{color:hsl(var(--primary))!important}.hover\:text-status-red:hover{color:var(--status-red)!important}.hover\:underline:hover{text-decoration-line:underline!important}.hover\:opacity-100:hover{opacity:1!important}.hover\:shadow-lg:hover{--tw-shadow: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.hover\:shadow-md:hover{--tw-shadow: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.hover\:shadow-sm:hover{--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05) !important;--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.hover\:outline:hover{outline-style:solid!important}.focus\:z-10:focus{z-index:10!important}.focus\:border-none:focus{border-style:none!important}.focus\:bg-accent:focus{background-color:hsl(var(--accent))!important}.focus\:text-accent-foreground:focus{color:hsl(var(--accent-foreground))!important}.focus\:outline-none:focus{outline:2px solid transparent!important;outline-offset:2px!important}.focus\:outline:focus{outline-style:solid!important}.focus\:ring-1:focus{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.focus\:ring-2:focus{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.focus\:ring-ring:focus{--tw-ring-color: hsl(var(--ring)) !important}.focus\:ring-offset-1:focus{--tw-ring-offset-width: 1px !important}.focus\:ring-offset-2:focus{--tw-ring-offset-width: 2px !important}.focus-visible\:outline-none:focus-visible{outline:2px solid transparent!important;outline-offset:2px!important}.focus-visible\:outline-0:focus-visible{outline-width:0px!important}.focus-visible\:ring-1:focus-visible{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.focus-visible\:ring-2:focus-visible{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.focus-visible\:ring-ring:focus-visible{--tw-ring-color: hsl(var(--ring)) !important}.focus-visible\:ring-offset-2:focus-visible{--tw-ring-offset-width: 2px !important}.focus-visible\:ring-offset-background:focus-visible{--tw-ring-offset-color: hsl(var(--background)) !important}.active\:outline:active{outline-style:solid!important}.disabled\:pointer-events-none:disabled{pointer-events:none!important}.disabled\:cursor-not-allowed:disabled{cursor:not-allowed!important}.disabled\:opacity-50:disabled{opacity:.5!important}.group:hover .group-hover\:opacity-100{opacity:1!important}.peer:disabled~.peer-disabled\:cursor-not-allowed{cursor:not-allowed!important}.peer:disabled~.peer-disabled\:opacity-70{opacity:.7!important}.aria-disabled\:bg-muted\/70[aria-disabled=true]{background-color:hsl(var(--muted) / .7)!important}.aria-selected\:bg-accent[aria-selected=true]{background-color:hsl(var(--accent))!important}.aria-selected\:text-accent-foreground[aria-selected=true]{color:hsl(var(--accent-foreground))!important}.data-\[disabled\]\:pointer-events-none[data-disabled]{pointer-events:none!important}.data-\[side\=bottom\]\:translate-y-1[data-side=bottom]{--tw-translate-y: .25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[side\=left\]\:-translate-x-1[data-side=left]{--tw-translate-x: -.25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[side\=right\]\:translate-x-1[data-side=right]{--tw-translate-x: .25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[side\=top\]\:-translate-y-1[data-side=top]{--tw-translate-y: -.25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[state\=checked\]\:translate-x-5[data-state=checked]{--tw-translate-x: 1.25rem !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[state\=unchecked\]\:translate-x-0[data-state=unchecked]{--tw-translate-x: 0px !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.data-\[state\=active\]\:border[data-state=active],.data-\[state\=inactive\]\:border[data-state=inactive]{border-width:1px!important}.data-\[state\=inactive\]\:border-muted[data-state=inactive]{border-color:hsl(var(--muted))!important}.data-\[state\=active\]\:bg-background[data-state=active]{background-color:hsl(var(--background))!important}.data-\[state\=active\]\:bg-primary-foreground[data-state=active]{background-color:hsl(var(--primary-foreground))!important}.data-\[state\=checked\]\:bg-primary[data-state=checked]{background-color:hsl(var(--primary))!important}.data-\[state\=open\]\:bg-accent[data-state=open]{background-color:hsl(var(--accent))!important}.data-\[state\=selected\]\:bg-muted[data-state=selected]{background-color:hsl(var(--muted))!important}.data-\[state\=unchecked\]\:bg-ring[data-state=unchecked]{background-color:hsl(var(--ring))!important}.data-\[state\=active\]\:text-foreground[data-state=active]{color:hsl(var(--foreground))!important}.data-\[state\=checked\]\:text-primary-foreground[data-state=checked]{color:hsl(var(--primary-foreground))!important}.data-\[state\=open\]\:text-accent-foreground[data-state=open]{color:hsl(var(--accent-foreground))!important}.data-\[state\=open\]\:text-muted-foreground[data-state=open]{color:hsl(var(--muted-foreground))!important}.data-\[disabled\]\:opacity-50[data-disabled]{opacity:.5!important}.data-\[state\=active\]\:shadow-sm[data-state=active]{--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05) !important;--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.data-\[state\=open\]\:animate-in[data-state=open]{animation-name:enter!important;animation-duration:.15s!important;--tw-enter-opacity: initial !important;--tw-enter-scale: initial !important;--tw-enter-rotate: initial !important;--tw-enter-translate-x: initial !important;--tw-enter-translate-y: initial !important}.data-\[state\=closed\]\:animate-out[data-state=closed]{animation-name:exit!important;animation-duration:.15s!important;--tw-exit-opacity: initial !important;--tw-exit-scale: initial !important;--tw-exit-rotate: initial !important;--tw-exit-translate-x: initial !important;--tw-exit-translate-y: initial !important}.data-\[state\=closed\]\:fade-out-0[data-state=closed]{--tw-exit-opacity: 0 !important}.data-\[state\=open\]\:fade-in-0[data-state=open]{--tw-enter-opacity: 0 !important}.data-\[state\=closed\]\:zoom-out-95[data-state=closed]{--tw-exit-scale: .95 !important}.data-\[state\=open\]\:zoom-in-95[data-state=open]{--tw-enter-scale: .95 !important}.data-\[side\=bottom\]\:slide-in-from-top-1[data-side=bottom]{--tw-enter-translate-y: -.25rem !important}.data-\[side\=bottom\]\:slide-in-from-top-2[data-side=bottom]{--tw-enter-translate-y: -.5rem !important}.data-\[side\=left\]\:slide-in-from-right-1[data-side=left]{--tw-enter-translate-x: .25rem !important}.data-\[side\=left\]\:slide-in-from-right-2[data-side=left]{--tw-enter-translate-x: .5rem !important}.data-\[side\=right\]\:slide-in-from-left-1[data-side=right]{--tw-enter-translate-x: -.25rem !important}.data-\[side\=right\]\:slide-in-from-left-2[data-side=right]{--tw-enter-translate-x: -.5rem !important}.data-\[side\=top\]\:slide-in-from-bottom-1[data-side=top]{--tw-enter-translate-y: .25rem !important}.data-\[side\=top\]\:slide-in-from-bottom-2[data-side=top]{--tw-enter-translate-y: .5rem !important}.data-\[state\=closed\]\:slide-out-to-left-1\/2[data-state=closed]{--tw-exit-translate-x: -50% !important}.data-\[state\=closed\]\:slide-out-to-top-\[48\%\][data-state=closed]{--tw-exit-translate-y: -48% !important}.data-\[state\=open\]\:slide-in-from-left-1\/2[data-state=open]{--tw-enter-translate-x: -50% !important}.data-\[state\=open\]\:slide-in-from-top-\[48\%\][data-state=open]{--tw-enter-translate-y: -48% !important}.data-\[state\=inactive\]\:hover\:bg-secondary\/80:hover[data-state=inactive]{background-color:hsl(var(--secondary) / .8)!important}:is(.dark .dark\:border-gray-600){--tw-border-opacity: 1 !important;border-color:rgb(75 85 99 / var(--tw-border-opacity))!important}:is(.dark .dark\:border-b-muted){border-bottom-color:hsl(var(--muted))!important}:is(.dark .dark\:text-gray-300){--tw-text-opacity: 1 !important;color:rgb(209 213 219 / var(--tw-text-opacity))!important}:is(.dark .dark\:text-white){color:var(--white)!important}:is(.dark .dark\:hover\:bg-background\/10:hover){background-color:hsl(var(--background) / .1)!important}@media (min-width: 640px){.sm\:flex-row{flex-direction:row!important}.sm\:items-center{align-items:center!important}.sm\:justify-end{justify-content:flex-end!important}.sm\:space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(.5rem * var(--tw-space-x-reverse))!important;margin-left:calc(.5rem * calc(1 - var(--tw-space-x-reverse)))!important}.sm\:rounded-lg{border-radius:var(--radius)!important}.sm\:px-3{padding-left:.75rem!important;padding-right:.75rem!important}.sm\:text-left{text-align:left!important}}@media (min-width: 768px){.md\:ml-6{margin-left:1.5rem!important}.md\:mt-0{margin-top:0!important}.md\:block{display:block!important}.md\:flex{display:flex!important}.md\:w-full{width:100%!important}.md\:grid-cols-2{grid-template-columns:repeat(2,minmax(0,1fr))!important}.md\:justify-between{justify-content:space-between!important}}@media (min-width: 1024px){.lg\:block{display:block!important}.lg\:flex{display:flex!important}.lg\:w-1\/5{width:20%!important}.lg\:w-\[30\%\]{width:30%!important}.lg\:grid-cols-2{grid-template-columns:repeat(2,minmax(0,1fr))!important}.lg\:grid-cols-3{grid-template-columns:repeat(3,minmax(0,1fr))!important}.lg\:flex-row{flex-direction:row!important}.lg\:flex-col{flex-direction:column!important}.lg\:space-x-0>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(0px * var(--tw-space-x-reverse))!important;margin-left:calc(0px * calc(1 - var(--tw-space-x-reverse)))!important}.lg\:space-x-8>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0 !important;margin-right:calc(2rem * var(--tw-space-x-reverse))!important;margin-left:calc(2rem * calc(1 - var(--tw-space-x-reverse)))!important}.lg\:space-y-0>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(0px * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(0px * var(--tw-space-y-reverse))!important}.lg\:space-y-1>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0 !important;margin-top:calc(.25rem * calc(1 - var(--tw-space-y-reverse)))!important;margin-bottom:calc(.25rem * var(--tw-space-y-reverse))!important}}.\[\&\:has\(\[role\=checkbox\]\)\]\:pr-0:has([role=checkbox]){padding-right:0!important}.\[\&\>button\]\:border-b-border>button{border-bottom-color:hsl(var(--border))!important}.hover\:\[\&\>button\]\:bg-border>button:hover{background-color:hsl(var(--border))!important}.\[\&\[data-state\=open\]\>svg\]\:rotate-180[data-state=open]>svg{--tw-rotate: 180deg !important;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.\[\&_\[cmdk-group-heading\]\]\:px-2 [cmdk-group-heading]{padding-left:.5rem!important;padding-right:.5rem!important}.\[\&_\[cmdk-group-heading\]\]\:py-1\.5 [cmdk-group-heading]{padding-top:.375rem!important;padding-bottom:.375rem!important}.\[\&_\[cmdk-group-heading\]\]\:text-xs [cmdk-group-heading]{font-size:.75rem!important;line-height:1rem!important}.\[\&_\[cmdk-group-heading\]\]\:font-medium [cmdk-group-heading]{font-weight:500!important}.\[\&_\[cmdk-group-heading\]\]\:text-muted-foreground [cmdk-group-heading]{color:hsl(var(--muted-foreground))!important}.\[\&_\[cmdk-group\]\:not\(\[hidden\]\)_\~\[cmdk-group\]\]\:pt-0 [cmdk-group]:not([hidden])~[cmdk-group]{padding-top:0!important}.\[\&_\[cmdk-group\]\]\:px-2 [cmdk-group]{padding-left:.5rem!important;padding-right:.5rem!important}.\[\&_\[cmdk-input-wrapper\]_svg\]\:h-5 [cmdk-input-wrapper] svg{height:1.25rem!important}.\[\&_\[cmdk-input-wrapper\]_svg\]\:w-5 [cmdk-input-wrapper] svg{width:1.25rem!important}.\[\&_\[cmdk-input\]\]\:h-12 [cmdk-input]{height:3rem!important}.\[\&_\[cmdk-item\]\]\:px-2 [cmdk-item]{padding-left:.5rem!important;padding-right:.5rem!important}.\[\&_\[cmdk-item\]\]\:py-3 [cmdk-item]{padding-top:.75rem!important;padding-bottom:.75rem!important}.\[\&_\[cmdk-item\]_svg\]\:h-5 [cmdk-item] svg{height:1.25rem!important}.\[\&_\[cmdk-item\]_svg\]\:w-5 [cmdk-item] svg{width:1.25rem!important}.\[\&_tr\:last-child\]\:border-0 tr:last-child{border-width:0px!important}.\[\&_tr\]\:border-b tr{border-bottom-width:1px!important}body{margin:0;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}code{font-family:source-code-pro,Menlo,Monaco,Consolas,Courier New,monospace}pre{font-family:inherit}.react-flow__pane{cursor:default}.AccordionContent{overflow:hidden}.AccordionContent[data-state=open]{animation:slideDown .3s ease-out}.AccordionContent[data-state=closed]{animation:slideUp .3s ease-out}.gradient-end{animation:gradient-motion-end 3s infinite forwards}.gradient-start{animation:gradient-motion-start 4s infinite forwards}input:-webkit-autofill,input:-webkit-autofill:hover,input:-webkit-autofill:focus,textarea:-webkit-autofill,textarea:-webkit-autofill:hover,textarea:-webkit-autofill:focus,select:-webkit-autofill,select:-webkit-autofill:hover,select:-webkit-autofill:focus{-webkit-text-fill-color:black;box-shadow:0 0 0 1000px #fff6d0 inset;color:#000}.ace_scrollbar::-webkit-scrollbar{height:8px;width:8px}.ace_scrollbar::-webkit-scrollbar-track{background-color:#f1f1f1}.ace_scrollbar::-webkit-scrollbar-thumb{background-color:#ccc;border-radius:999px}.ace_scrollbar::-webkit-scrollbar-thumb:hover{background-color:#bbb;border-radius:999px}
```

### Comparing `langflow-0.6.8/src/backend/langflow/frontend/assets/index-fef5028f.js` & `langflow-0.6.9/src/backend/langflow/frontend/assets/index-3732b41f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
-var F9 = (j, $) => () => ($ || j(($ = {
+var Gp = (j, $) => () => ($ || j(($ = {
     exports: {}
 }).exports, $), $.exports);
-var V9 = F9((exports, module) => {
+var zp = Gp((exports, module) => {
     function _mergeNamespaces(j, $) {
         for (var at = 0; at < $.length; at++) {
             const st = $[at];
             if (typeof st != "string" && !Array.isArray(st)) {
                 for (const ct in st)
                     if (ct !== "default" && !(ct in j)) {
                         const ut = Object.getOwnPropertyDescriptor(st, ct);
@@ -11122,15 +11122,15 @@
                         if (kt = Mn(kt), kt && (Vt || Nt === at)) return kt.replace(ao, "");
                         if (!kt || !(Nt = Ro(Nt))) return kt;
                         var Kt = Yo(kt),
                             tr = g3(Kt, Yo(Nt));
                         return As(Kt, tr).join("")
                     }
 
-                    function e9(kt, Nt) {
+                    function ep(kt, Nt) {
                         var Vt = Dt,
                             Kt = Ht;
                         if (Bn(Nt)) {
                             var tr = "separator" in Nt ? Nt.separator : tr;
                             Vt = "length" in Nt ? Qn(Nt.length) : Vt, Kt = "omission" in Nt ? Ro(Nt.omission) : Kt
                         }
                         kt = Mn(kt);
@@ -11153,89 +11153,89 @@
                         } else if (kt.indexOf(Ro(tr), mr) != mr) {
                             var Gr = xr.lastIndexOf(tr);
                             Gr > -1 && (xr = xr.slice(0, Gr))
                         }
                         return xr + Kt
                     }
 
-                    function t9(kt) {
+                    function tp(kt) {
                         return kt = Mn(kt), kt && go.test(kt) ? kt.replace(zo, C6) : kt
                     }
-                    var r9 = n1(function(kt, Nt, Vt) {
+                    var rp = n1(function(kt, Nt, Vt) {
                             return kt + (Vt ? " " : "") + Nt.toUpperCase()
                         }),
                         o3 = s4("toUpperCase");
 
                     function a6(kt, Nt, Vt) {
                         return kt = Mn(kt), Nt = Vt ? at : Nt, Nt === at ? E6(kt) ? R6(kt) : h6(kt) : kt.match(Nt) || []
                     }
                     var i6 = yn(function(kt, Nt) {
                             try {
                                 return eo(kt, at, Nt)
                             } catch (Vt) {
                                 return e3(Vt) ? Vt : new hn(Vt)
                             }
                         }),
-                        n9 = us(function(kt, Nt) {
+                        np = us(function(kt, Nt) {
                             return $o(Nt, function(Vt) {
                                 Vt = rs(Vt), ls(kt, Vt, Xl(kt[Vt], kt))
                             }), kt
                         });
 
-                    function o9(kt) {
+                    function op(kt) {
                         var Nt = kt == null ? 0 : kt.length,
                             Vt = an();
                         return kt = Nt ? Pn(kt, function(Kt) {
                             if (typeof Kt[1] != "function") throw new Po(dt);
                             return [Vt(Kt[0]), Kt[1]]
                         }) : [], yn(function(Kt) {
                             for (var tr = -1; ++tr < Nt;) {
                                 var lr = kt[tr];
                                 if (eo(lr[0], this, Kt)) return eo(lr[1], this, Kt)
                             }
                         })
                     }
 
-                    function a9(kt) {
+                    function ip(kt) {
                         return Ru(Fo(kt, mt))
                     }
 
                     function a3(kt) {
                         return function() {
                             return kt
                         }
                     }
 
-                    function i9(kt, Nt) {
+                    function sp(kt, Nt) {
                         return kt == null || kt !== kt ? Nt : kt
                     }
-                    var s9 = c4(),
-                        l9 = c4(!0);
+                    var lp = c4(),
+                        cp = c4(!0);
 
                     function Lo(kt) {
                         return kt
                     }
 
                     function i3(kt) {
                         return P3(typeof kt == "function" ? kt : Fo(kt, mt))
                     }
 
-                    function c9(kt) {
+                    function up(kt) {
                         return F3(Fo(kt, mt))
                     }
 
-                    function u9(kt, Nt) {
+                    function dp(kt, Nt) {
                         return V3(kt, Fo(Nt, mt))
                     }
-                    var d9 = yn(function(kt, Nt) {
+                    var fp = yn(function(kt, Nt) {
                             return function(Vt) {
                                 return v1(Vt, kt, Nt)
                             }
                         }),
-                        f9 = yn(function(kt, Nt) {
+                        pp = yn(function(kt, Nt) {
                             return function(Vt) {
                                 return v1(kt, Vt, Nt)
                             }
                         });
 
                     function s3(kt, Nt, Vt) {
                         var Kt = ro(Nt),
@@ -11257,126 +11257,126 @@
                                     }), Dr.__chain__ = Nr, Dr
                                 }
                                 return xr.apply(kt, ys([this.value()], arguments))
                             })
                         }), kt
                     }
 
-                    function p9() {
+                    function hp() {
                         return Sn._ === this && (Sn._ = j6), this
                     }
 
                     function l3() {}
 
-                    function h9(kt) {
+                    function Tp(kt) {
                         return kt = Qn(kt), yn(function(Nt) {
                             return U3(Nt, kt)
                         })
                     }
-                    var m9 = Il(Pn),
-                        T9 = Il(d3),
-                        g9 = Il(P2);
+                    var gp = Il(Pn),
+                        Qp = Il(d3),
+                        vp = Il(P2);
 
                     function s6(kt) {
                         return Gl(kt) ? B2(rs(kt)) : Zu(kt)
                     }
 
-                    function Q9(kt) {
+                    function xp(kt) {
                         return function(Nt) {
                             return kt == null ? at : $s(kt, Nt)
                         }
                     }
-                    var v9 = d4(),
-                        x9 = d4(!0);
+                    var yp = d4(),
+                        bp = d4(!0);
 
                     function c3() {
                         return []
                     }
 
                     function u3() {
                         return !1
                     }
 
-                    function y9() {
+                    function Ep() {
                         return {}
                     }
 
-                    function b9() {
+                    function Sp() {
                         return ""
                     }
 
-                    function E9() {
+                    function Lp() {
                         return !0
                     }
 
-                    function w9(kt, Nt) {
+                    function Ap(kt, Nt) {
                         if (kt = Qn(kt), kt < 1 || kt > Wt) return [];
                         var Vt = Yt,
                             Kt = io(kt, Yt);
                         Nt = an(Nt), kt -= Yt;
                         for (var tr = U2(Kt, Nt); ++Vt < kt;) Nt(Vt);
                         return tr
                     }
 
-                    function S9(kt) {
+                    function Cp(kt) {
                         return gn(kt) ? Pn(kt, rs) : _o(kt) ? [kt] : Eo(A4(Mn(kt)))
                     }
 
-                    function L9(kt) {
+                    function Mp(kt) {
                         var Nt = ++D6;
                         return Mn(kt) + Nt
                     }
-                    var A9 = h2(function(kt, Nt) {
+                    var kp = h2(function(kt, Nt) {
                             return kt + Nt
                         }, 0),
-                        C9 = $l("ceil"),
-                        M9 = h2(function(kt, Nt) {
+                        Rp = $l("ceil"),
+                        _p = h2(function(kt, Nt) {
                             return kt / Nt
                         }, 1),
-                        k9 = $l("floor");
+                        Op = $l("floor");
 
-                    function R9(kt) {
+                    function Np(kt) {
                         return kt && kt.length ? s2(kt, Lo, Ql) : at
                     }
 
-                    function _9(kt, Nt) {
+                    function Dp(kt, Nt) {
                         return kt && kt.length ? s2(kt, an(Nt, 2), Ql) : at
                     }
 
-                    function O9(kt) {
+                    function Hp(kt) {
                         return h3(kt, Lo)
                     }
 
-                    function N9(kt, Nt) {
+                    function jp(kt, Nt) {
                         return h3(kt, an(Nt, 2))
                     }
 
-                    function D9(kt) {
+                    function Ip(kt) {
                         return kt && kt.length ? s2(kt, Lo, Sl) : at
                     }
 
-                    function H9(kt, Nt) {
+                    function $p(kt, Nt) {
                         return kt && kt.length ? s2(kt, an(Nt, 2), Sl) : at
                     }
-                    var j9 = h2(function(kt, Nt) {
+                    var Pp = h2(function(kt, Nt) {
                             return kt * Nt
                         }, 1),
-                        I9 = $l("round"),
-                        $9 = h2(function(kt, Nt) {
+                        Bp = $l("round"),
+                        Fp = h2(function(kt, Nt) {
                             return kt - Nt
                         }, 0);
 
-                    function P9(kt) {
+                    function Vp(kt) {
                         return kt && kt.length ? V2(kt, Lo) : 0
                     }
 
-                    function B9(kt, Nt) {
+                    function Up(kt, Nt) {
                         return kt && kt.length ? V2(kt, an(Nt, 2)) : 0
                     }
-                    return ir.after = u7, ir.ary = I4, ir.assign = Y7, ir.assignIn = X4, ir.assignInWith = A2, ir.assignWith = X7, ir.at = J7, ir.before = $4, ir.bind = Xl, ir.bindAll = n9, ir.bindKey = P4, ir.castArray = b7, ir.chain = D4, ir.chunk = _5, ir.compact = O5, ir.concat = N5, ir.cond = o9, ir.conforms = a9, ir.constant = a3, ir.countBy = F0, ir.create = e8, ir.curry = B4, ir.curryRight = F4, ir.debounce = V4, ir.defaults = t8, ir.defaultsDeep = r8, ir.defer = d7, ir.delay = f7, ir.difference = D5, ir.differenceBy = H5, ir.differenceWith = j5, ir.drop = I5, ir.dropRight = $5, ir.dropRightWhile = P5, ir.dropWhile = B5, ir.fill = F5, ir.filter = U0, ir.flatMap = q0, ir.flatMapDeep = W0, ir.flatMapDepth = Z0, ir.flatten = R4, ir.flattenDeep = V5, ir.flattenDepth = U5, ir.flip = p7, ir.flow = s9, ir.flowRight = l9, ir.fromPairs = G5, ir.functions = c8, ir.functionsIn = u8, ir.groupBy = K0, ir.initial = q5, ir.intersection = W5, ir.intersectionBy = Z5, ir.intersectionWith = K5, ir.invert = f8, ir.invertBy = p8, ir.invokeMap = X0, ir.iteratee = i3, ir.keyBy = J0, ir.keys = ro, ir.keysIn = So, ir.map = y2, ir.mapKeys = m8, ir.mapValues = T8, ir.matches = c9, ir.matchesProperty = u9, ir.memoize = E2, ir.merge = g8, ir.mergeWith = J4, ir.method = d9, ir.methodOf = f9, ir.mixin = s3, ir.negate = w2, ir.nthArg = h9, ir.omit = Q8, ir.omitBy = v8, ir.once = h7, ir.orderBy = _d, ir.over = m9, ir.overArgs = m7, ir.overEvery = T9, ir.overSome = g9, ir.partial = Jl, ir.partialRight = U4, ir.partition = e7, ir.pick = x8, ir.pickBy = e6, ir.property = s6, ir.propertyOf = Q9, ir.pull = e0, ir.pullAll = O4, ir.pullAllBy = t0, ir.pullAllWith = r0, ir.pullAt = n0, ir.range = v9, ir.rangeRight = x9, ir.rearg = T7, ir.reject = n7, ir.remove = o0, ir.rest = g7, ir.reverse = Kl, ir.sampleSize = a7, ir.set = b8, ir.setWith = E8, ir.shuffle = i7, ir.slice = a0, ir.sortBy = c7, ir.sortedUniq = f0, ir.sortedUniqBy = p0, ir.split = z8, ir.spread = Q7, ir.tail = h0, ir.take = m0, ir.takeRight = T0, ir.takeRightWhile = g0, ir.takeWhile = Q0, ir.tap = O0, ir.throttle = v7, ir.thru = x2, ir.toArray = Z4, ir.toPairs = t6, ir.toPairsIn = r6, ir.toPath = S9, ir.toPlainObject = Y4, ir.transform = w8, ir.unary = x7, ir.union = v0, ir.unionBy = x0, ir.unionWith = y0, ir.uniq = b0, ir.uniqBy = E0, ir.uniqWith = w0, ir.unset = S8, ir.unzip = Yl, ir.unzipWith = N4, ir.update = L8, ir.updateWith = A8, ir.values = i1, ir.valuesIn = C8, ir.without = S0, ir.words = a6, ir.wrap = y7, ir.xor = L0, ir.xorBy = A0, ir.xorWith = C0, ir.zip = M0, ir.zipObject = k0, ir.zipObjectDeep = R0, ir.zipWith = _0, ir.entries = t6, ir.entriesIn = r6, ir.extend = X4, ir.extendWith = A2, s3(ir, ir), ir.add = A9, ir.attempt = i6, ir.camelCase = _8, ir.capitalize = n6, ir.ceil = C9, ir.clamp = M8, ir.clone = E7, ir.cloneDeep = S7, ir.cloneDeepWith = L7, ir.cloneWith = w7, ir.conformsTo = A7, ir.deburr = o6, ir.defaultTo = i9, ir.divide = M9, ir.endsWith = O8, ir.eq = Jo, ir.escape = N8, ir.escapeRegExp = D8, ir.every = V0, ir.find = G0, ir.findIndex = M4, ir.findKey = n8, ir.findLast = z0, ir.findLastIndex = k4, ir.findLastKey = o8, ir.floor = k9, ir.forEach = H4, ir.forEachRight = j4, ir.forIn = a8, ir.forInRight = i8, ir.forOwn = s8, ir.forOwnRight = l8, ir.get = r3, ir.gt = C7, ir.gte = M7, ir.has = d8, ir.hasIn = n3, ir.head = _4, ir.identity = Lo, ir.includes = Y0, ir.indexOf = z5, ir.inRange = k8, ir.invoke = h8, ir.isArguments = Fs, ir.isArray = gn, ir.isArrayBuffer = k7, ir.isArrayLike = wo, ir.isArrayLikeObject = zn, ir.isBoolean = R7, ir.isBuffer = Cs, ir.isDate = _7, ir.isElement = O7, ir.isEmpty = N7, ir.isEqual = D7, ir.isEqualWith = H7, ir.isError = e3, ir.isFinite = j7, ir.isFunction = fs, ir.isInteger = G4, ir.isLength = S2, ir.isMap = z4, ir.isMatch = I7, ir.isMatchWith = $7, ir.isNaN = P7, ir.isNative = B7, ir.isNil = V7, ir.isNull = F7, ir.isNumber = q4, ir.isObject = Bn, ir.isObjectLike = Vn, ir.isPlainObject = S1, ir.isRegExp = t3, ir.isSafeInteger = U7, ir.isSet = W4, ir.isString = L2, ir.isSymbol = _o, ir.isTypedArray = a1, ir.isUndefined = G7, ir.isWeakMap = z7, ir.isWeakSet = q7, ir.join = Y5, ir.kebabCase = H8, ir.last = Uo, ir.lastIndexOf = X5, ir.lowerCase = j8, ir.lowerFirst = I8, ir.lt = W7, ir.lte = Z7, ir.max = R9, ir.maxBy = _9, ir.mean = O9, ir.meanBy = N9, ir.min = D9, ir.minBy = H9, ir.stubArray = c3, ir.stubFalse = u3, ir.stubObject = y9, ir.stubString = b9, ir.stubTrue = E9, ir.multiply = j9, ir.nth = J5, ir.noConflict = p9, ir.noop = l3, ir.now = b2, ir.pad = $8, ir.padEnd = P8, ir.padStart = B8, ir.parseInt = F8, ir.random = R8, ir.reduce = t7, ir.reduceRight = r7, ir.repeat = V8, ir.replace = U8, ir.result = y8, ir.round = I9, ir.runInContext = Qr, ir.sample = o7, ir.size = s7, ir.snakeCase = G8, ir.some = l7, ir.sortedIndex = i0, ir.sortedIndexBy = s0, ir.sortedIndexOf = l0, ir.sortedLastIndex = c0, ir.sortedLastIndexBy = u0, ir.sortedLastIndexOf = d0, ir.startCase = q8, ir.startsWith = W8, ir.subtract = $9, ir.sum = P9, ir.sumBy = B9, ir.template = Z8, ir.times = w9, ir.toFinite = ps, ir.toInteger = Qn, ir.toLength = K4, ir.toLower = K8, ir.toNumber = Go, ir.toSafeInteger = K7, ir.toString = Mn, ir.toUpper = Y8, ir.trim = X8, ir.trimEnd = J8, ir.trimStart = _f, ir.truncate = e9, ir.unescape = t9, ir.uniqueId = L9, ir.upperCase = r9, ir.upperFirst = o3, ir.each = H4, ir.eachRight = j4, ir.first = _4, s3(ir, function() {
+                    return ir.after = u7, ir.ary = I4, ir.assign = Y7, ir.assignIn = X4, ir.assignInWith = A2, ir.assignWith = X7, ir.at = J7, ir.before = $4, ir.bind = Xl, ir.bindAll = np, ir.bindKey = P4, ir.castArray = b7, ir.chain = D4, ir.chunk = _5, ir.compact = O5, ir.concat = N5, ir.cond = op, ir.conforms = ip, ir.constant = a3, ir.countBy = F0, ir.create = e8, ir.curry = B4, ir.curryRight = F4, ir.debounce = V4, ir.defaults = t8, ir.defaultsDeep = r8, ir.defer = d7, ir.delay = f7, ir.difference = D5, ir.differenceBy = H5, ir.differenceWith = j5, ir.drop = I5, ir.dropRight = $5, ir.dropRightWhile = P5, ir.dropWhile = B5, ir.fill = F5, ir.filter = U0, ir.flatMap = q0, ir.flatMapDeep = W0, ir.flatMapDepth = Z0, ir.flatten = R4, ir.flattenDeep = V5, ir.flattenDepth = U5, ir.flip = p7, ir.flow = lp, ir.flowRight = cp, ir.fromPairs = G5, ir.functions = c8, ir.functionsIn = u8, ir.groupBy = K0, ir.initial = q5, ir.intersection = W5, ir.intersectionBy = Z5, ir.intersectionWith = K5, ir.invert = f8, ir.invertBy = p8, ir.invokeMap = X0, ir.iteratee = i3, ir.keyBy = J0, ir.keys = ro, ir.keysIn = So, ir.map = y2, ir.mapKeys = m8, ir.mapValues = T8, ir.matches = up, ir.matchesProperty = dp, ir.memoize = E2, ir.merge = g8, ir.mergeWith = J4, ir.method = fp, ir.methodOf = pp, ir.mixin = s3, ir.negate = w2, ir.nthArg = Tp, ir.omit = Q8, ir.omitBy = v8, ir.once = h7, ir.orderBy = _d, ir.over = gp, ir.overArgs = m7, ir.overEvery = Qp, ir.overSome = vp, ir.partial = Jl, ir.partialRight = U4, ir.partition = e7, ir.pick = x8, ir.pickBy = e6, ir.property = s6, ir.propertyOf = xp, ir.pull = e0, ir.pullAll = O4, ir.pullAllBy = t0, ir.pullAllWith = r0, ir.pullAt = n0, ir.range = yp, ir.rangeRight = bp, ir.rearg = T7, ir.reject = n7, ir.remove = o0, ir.rest = g7, ir.reverse = Kl, ir.sampleSize = a7, ir.set = b8, ir.setWith = E8, ir.shuffle = i7, ir.slice = a0, ir.sortBy = c7, ir.sortedUniq = f0, ir.sortedUniqBy = p0, ir.split = z8, ir.spread = Q7, ir.tail = h0, ir.take = m0, ir.takeRight = T0, ir.takeRightWhile = g0, ir.takeWhile = Q0, ir.tap = O0, ir.throttle = v7, ir.thru = x2, ir.toArray = Z4, ir.toPairs = t6, ir.toPairsIn = r6, ir.toPath = Cp, ir.toPlainObject = Y4, ir.transform = w8, ir.unary = x7, ir.union = v0, ir.unionBy = x0, ir.unionWith = y0, ir.uniq = b0, ir.uniqBy = E0, ir.uniqWith = w0, ir.unset = S8, ir.unzip = Yl, ir.unzipWith = N4, ir.update = L8, ir.updateWith = A8, ir.values = i1, ir.valuesIn = C8, ir.without = S0, ir.words = a6, ir.wrap = y7, ir.xor = L0, ir.xorBy = A0, ir.xorWith = C0, ir.zip = M0, ir.zipObject = k0, ir.zipObjectDeep = R0, ir.zipWith = _0, ir.entries = t6, ir.entriesIn = r6, ir.extend = X4, ir.extendWith = A2, s3(ir, ir), ir.add = kp, ir.attempt = i6, ir.camelCase = _8, ir.capitalize = n6, ir.ceil = Rp, ir.clamp = M8, ir.clone = E7, ir.cloneDeep = S7, ir.cloneDeepWith = L7, ir.cloneWith = w7, ir.conformsTo = A7, ir.deburr = o6, ir.defaultTo = sp, ir.divide = _p, ir.endsWith = O8, ir.eq = Jo, ir.escape = N8, ir.escapeRegExp = D8, ir.every = V0, ir.find = G0, ir.findIndex = M4, ir.findKey = n8, ir.findLast = z0, ir.findLastIndex = k4, ir.findLastKey = o8, ir.floor = Op, ir.forEach = H4, ir.forEachRight = j4, ir.forIn = a8, ir.forInRight = i8, ir.forOwn = s8, ir.forOwnRight = l8, ir.get = r3, ir.gt = C7, ir.gte = M7, ir.has = d8, ir.hasIn = n3, ir.head = _4, ir.identity = Lo, ir.includes = Y0, ir.indexOf = z5, ir.inRange = k8, ir.invoke = h8, ir.isArguments = Fs, ir.isArray = gn, ir.isArrayBuffer = k7, ir.isArrayLike = wo, ir.isArrayLikeObject = zn, ir.isBoolean = R7, ir.isBuffer = Cs, ir.isDate = _7, ir.isElement = O7, ir.isEmpty = N7, ir.isEqual = D7, ir.isEqualWith = H7, ir.isError = e3, ir.isFinite = j7, ir.isFunction = fs, ir.isInteger = G4, ir.isLength = S2, ir.isMap = z4, ir.isMatch = I7, ir.isMatchWith = $7, ir.isNaN = P7, ir.isNative = B7, ir.isNil = V7, ir.isNull = F7, ir.isNumber = q4, ir.isObject = Bn, ir.isObjectLike = Vn, ir.isPlainObject = S1, ir.isRegExp = t3, ir.isSafeInteger = U7, ir.isSet = W4, ir.isString = L2, ir.isSymbol = _o, ir.isTypedArray = a1, ir.isUndefined = G7, ir.isWeakMap = z7, ir.isWeakSet = q7, ir.join = Y5, ir.kebabCase = H8, ir.last = Uo, ir.lastIndexOf = X5, ir.lowerCase = j8, ir.lowerFirst = I8, ir.lt = W7, ir.lte = Z7, ir.max = Np, ir.maxBy = Dp, ir.mean = Hp, ir.meanBy = jp, ir.min = Ip, ir.minBy = $p, ir.stubArray = c3, ir.stubFalse = u3, ir.stubObject = Ep, ir.stubString = Sp, ir.stubTrue = Lp, ir.multiply = Pp, ir.nth = J5, ir.noConflict = hp, ir.noop = l3, ir.now = b2, ir.pad = $8, ir.padEnd = P8, ir.padStart = B8, ir.parseInt = F8, ir.random = R8, ir.reduce = t7, ir.reduceRight = r7, ir.repeat = V8, ir.replace = U8, ir.result = y8, ir.round = Bp, ir.runInContext = Qr, ir.sample = o7, ir.size = s7, ir.snakeCase = G8, ir.some = l7, ir.sortedIndex = i0, ir.sortedIndexBy = s0, ir.sortedIndexOf = l0, ir.sortedLastIndex = c0, ir.sortedLastIndexBy = u0, ir.sortedLastIndexOf = d0, ir.startCase = q8, ir.startsWith = W8, ir.subtract = Fp, ir.sum = Vp, ir.sumBy = Up, ir.template = Z8, ir.times = Ap, ir.toFinite = ps, ir.toInteger = Qn, ir.toLength = K4, ir.toLower = K8, ir.toNumber = Go, ir.toSafeInteger = K7, ir.toString = Mn, ir.toUpper = Y8, ir.trim = X8, ir.trimEnd = J8, ir.trimStart = _f, ir.truncate = ep, ir.unescape = tp, ir.uniqueId = Mp, ir.upperCase = rp, ir.upperFirst = o3, ir.each = H4, ir.eachRight = j4, ir.first = _4, s3(ir, function() {
                         var kt = {};
                         return es(ir, function(Nt, Vt) {
                             kn.call(ir.prototype, Vt) || (kt[Vt] = Nt)
                         }), kt
                     }(), {
                         chain: !1
                     }), ir.VERSION = st, $o(["bind", "bindKey", "curry", "curryRight", "partial", "partialRight"], function(kt) {
@@ -18715,92 +18715,1572 @@
                         })
                     })]
                 })
             })
         })
     }
 
-    function CrashErrorComponent({
-        error: j,
-        resetErrorBoundary: $
-    }) {
-        return jsxRuntimeExports.jsx("div", {
-            className: "fixed left-0 top-0 z-50 flex h-full w-full items-center justify-center bg-foreground bg-opacity-50",
-            children: jsxRuntimeExports.jsxs("div", {
-                className: "flex h-1/3 min-h-fit max-w-4xl flex-col justify-evenly rounded-lg bg-background p-8 text-start shadow-lg",
-                children: [jsxRuntimeExports.jsx("h1", {
-                    className: "mb-4 text-3xl text-status-red",
-                    children: "Oops! An unknown error has occurred."
-                }), jsxRuntimeExports.jsx("p", {
-                    className: "mb-4 text-xl text-foreground",
-                    children: "Please click the 'Reset Application' button to restore the application's state. If the error persists, please create an issue on our GitHub page. We apologize for any inconvenience this may have caused."
-                }), jsxRuntimeExports.jsxs("div", {
-                    className: "flex justify-center",
-                    children: [jsxRuntimeExports.jsx("button", {
-                        onClick: $,
-                        className: "mr-4 rounded bg-primary px-4 py-2 font-bold text-background hover:bg-ring",
-                        children: "Reset Application"
-                    }), jsxRuntimeExports.jsx("a", {
-                        href: "https://github.com/logspace-ai/langflow/issues/new",
-                        target: "_blank",
-                        rel: "noopener noreferrer",
-                        className: "rounded bg-status-red px-4 py-2 font-bold text-background hover:bg-error-foreground",
-                        children: "Create Issue"
-                    })]
-                })]
+    function _extends$9() {
+        return _extends$9 = Object.assign ? Object.assign.bind() : function(j) {
+            for (var $ = 1; $ < arguments.length; $++) {
+                var at = arguments[$];
+                for (var st in at) Object.prototype.hasOwnProperty.call(at, st) && (j[st] = at[st])
+            }
+            return j
+        }, _extends$9.apply(this, arguments)
+    }
+
+    function $6ed0406888f73fc4$var$setRef(j, $) {
+        typeof j == "function" ? j($) : j != null && (j.current = $)
+    }
+
+    function $6ed0406888f73fc4$export$43e446d32b3d21af(...j) {
+        return $ => j.forEach(at => $6ed0406888f73fc4$var$setRef(at, $))
+    }
+
+    function $6ed0406888f73fc4$export$c7b2cbe3552a0d05(...j) {
+        return reactExports.useCallback($6ed0406888f73fc4$export$43e446d32b3d21af(...j), j)
+    }
+    const $5e63c961fc1ce211$export$8c6ed5c666ac1360 = reactExports.forwardRef((j, $) => {
+        const {
+            children: at,
+            ...st
+        } = j, ct = reactExports.Children.toArray(at), ut = ct.find($5e63c961fc1ce211$var$isSlottable);
+        if (ut) {
+            const dt = ut.props.children,
+                ft = ct.map(pt => pt === ut ? reactExports.Children.count(dt) > 1 ? reactExports.Children.only(null) : reactExports.isValidElement(dt) ? dt.props.children : null : pt);
+            return reactExports.createElement($5e63c961fc1ce211$var$SlotClone, _extends$9({}, st, {
+                ref: $
+            }), reactExports.isValidElement(dt) ? reactExports.cloneElement(dt, void 0, ft) : null)
+        }
+        return reactExports.createElement($5e63c961fc1ce211$var$SlotClone, _extends$9({}, st, {
+            ref: $
+        }), at)
+    });
+    $5e63c961fc1ce211$export$8c6ed5c666ac1360.displayName = "Slot";
+    const $5e63c961fc1ce211$var$SlotClone = reactExports.forwardRef((j, $) => {
+        const {
+            children: at,
+            ...st
+        } = j;
+        return reactExports.isValidElement(at) ? reactExports.cloneElement(at, {
+            ...$5e63c961fc1ce211$var$mergeProps(st, at.props),
+            ref: $ ? $6ed0406888f73fc4$export$43e446d32b3d21af($, at.ref) : at.ref
+        }) : reactExports.Children.count(at) > 1 ? reactExports.Children.only(null) : null
+    });
+    $5e63c961fc1ce211$var$SlotClone.displayName = "SlotClone";
+    const $5e63c961fc1ce211$export$d9f1ccf0bdb05d45 = ({
+        children: j
+    }) => reactExports.createElement(reactExports.Fragment, null, j);
+
+    function $5e63c961fc1ce211$var$isSlottable(j) {
+        return reactExports.isValidElement(j) && j.type === $5e63c961fc1ce211$export$d9f1ccf0bdb05d45
+    }
+
+    function $5e63c961fc1ce211$var$mergeProps(j, $) {
+        const at = {
+            ...$
+        };
+        for (const st in $) {
+            const ct = j[st],
+                ut = $[st];
+            /^on[A-Z]/.test(st) ? ct && ut ? at[st] = (...ft) => {
+                ut(...ft), ct(...ft)
+            } : ct && (at[st] = ct) : st === "style" ? at[st] = {
+                ...ct,
+                ...ut
+            } : st === "className" && (at[st] = [ct, ut].filter(Boolean).join(" "))
+        }
+        return {
+            ...j,
+            ...at
+        }
+    }
+
+    function r$4(j) {
+        var $, at, st = "";
+        if (typeof j == "string" || typeof j == "number") st += j;
+        else if (typeof j == "object")
+            if (Array.isArray(j))
+                for ($ = 0; $ < j.length; $++) j[$] && (at = r$4(j[$])) && (st && (st += " "), st += at);
+            else
+                for ($ in j) j[$] && (st && (st += " "), st += $);
+        return st
+    }
+
+    function clsx$2() {
+        for (var j, $, at = 0, st = ""; at < arguments.length;)(j = arguments[at++]) && ($ = r$4(j)) && (st && (st += " "), st += $);
+        return st
+    }
+    const falsyToString = j => typeof j == "boolean" ? "".concat(j) : j === 0 ? "0" : j,
+        cx = clsx$2,
+        cva = (j, $) => at => {
+            var st;
+            if (($ == null ? void 0 : $.variants) == null) return cx(j, at == null ? void 0 : at.class, at == null ? void 0 : at.className);
+            const {
+                variants: ct,
+                defaultVariants: ut
+            } = $, dt = Object.keys(ct).map(Tt => {
+                const ht = at == null ? void 0 : at[Tt],
+                    mt = ut == null ? void 0 : ut[Tt];
+                if (ht === null) return null;
+                const Qt = falsyToString(ht) || falsyToString(mt);
+                return ct[Tt][Qt]
+            }), ft = at && Object.entries(at).reduce((Tt, ht) => {
+                let [mt, Qt] = ht;
+                return Qt === void 0 || (Tt[mt] = Qt), Tt
+            }, {}), pt = $ == null || (st = $.compoundVariants) === null || st === void 0 ? void 0 : st.reduce((Tt, ht) => {
+                let {
+                    class: mt,
+                    className: Qt,
+                    ...vt
+                } = ht;
+                return Object.entries(vt).every(xt => {
+                    let [yt, Et] = xt;
+                    return Array.isArray(Et) ? Et.includes({
+                        ...ut,
+                        ...ft
+                    } [yt]) : {
+                        ...ut,
+                        ...ft
+                    } [yt] === Et
+                }) ? [...Tt, mt, Qt] : Tt
+            }, []);
+            return cx(j, dt, pt, at == null ? void 0 : at.class, at == null ? void 0 : at.className)
+        };
+
+    function twJoin() {
+        for (var j = 0, $, at, st = ""; j < arguments.length;)($ = arguments[j++]) && (at = toValue($)) && (st && (st += " "), st += at);
+        return st
+    }
+
+    function toValue(j) {
+        if (typeof j == "string") return j;
+        for (var $, at = "", st = 0; st < j.length; st++) j[st] && ($ = toValue(j[st])) && (at && (at += " "), at += $);
+        return at
+    }
+    var CLASS_PART_SEPARATOR = "-";
+
+    function createClassUtils(j) {
+        var $ = createClassMap(j),
+            at = j.conflictingClassGroups,
+            st = j.conflictingClassGroupModifiers,
+            ct = st === void 0 ? {} : st;
+
+        function ut(ft) {
+            var pt = ft.split(CLASS_PART_SEPARATOR);
+            return pt[0] === "" && pt.length !== 1 && pt.shift(), getGroupRecursive(pt, $) || getGroupIdForArbitraryProperty(ft)
+        }
+
+        function dt(ft, pt) {
+            var Tt = at[ft] || [];
+            return pt && ct[ft] ? [].concat(Tt, ct[ft]) : Tt
+        }
+        return {
+            getClassGroupId: ut,
+            getConflictingClassGroupIds: dt
+        }
+    }
+
+    function getGroupRecursive(j, $) {
+        var dt;
+        if (j.length === 0) return $.classGroupId;
+        var at = j[0],
+            st = $.nextPart.get(at),
+            ct = st ? getGroupRecursive(j.slice(1), st) : void 0;
+        if (ct) return ct;
+        if ($.validators.length !== 0) {
+            var ut = j.join(CLASS_PART_SEPARATOR);
+            return (dt = $.validators.find(function(ft) {
+                var pt = ft.validator;
+                return pt(ut)
+            })) == null ? void 0 : dt.classGroupId
+        }
+    }
+    var arbitraryPropertyRegex = /^\[(.+)\]$/;
+
+    function getGroupIdForArbitraryProperty(j) {
+        if (arbitraryPropertyRegex.test(j)) {
+            var $ = arbitraryPropertyRegex.exec(j)[1],
+                at = $ == null ? void 0 : $.substring(0, $.indexOf(":"));
+            if (at) return "arbitrary.." + at
+        }
+    }
+
+    function createClassMap(j) {
+        var $ = j.theme,
+            at = j.prefix,
+            st = {
+                nextPart: new Map,
+                validators: []
+            },
+            ct = getPrefixedClassGroupEntries(Object.entries(j.classGroups), at);
+        return ct.forEach(function(ut) {
+            var dt = ut[0],
+                ft = ut[1];
+            processClassesRecursively(ft, st, dt, $)
+        }), st
+    }
+
+    function processClassesRecursively(j, $, at, st) {
+        j.forEach(function(ct) {
+            if (typeof ct == "string") {
+                var ut = ct === "" ? $ : getPart($, ct);
+                ut.classGroupId = at;
+                return
+            }
+            if (typeof ct == "function") {
+                if (isThemeGetter(ct)) {
+                    processClassesRecursively(ct(st), $, at, st);
+                    return
+                }
+                $.validators.push({
+                    validator: ct,
+                    classGroupId: at
+                });
+                return
+            }
+            Object.entries(ct).forEach(function(dt) {
+                var ft = dt[0],
+                    pt = dt[1];
+                processClassesRecursively(pt, getPart($, ft), at, st)
             })
         })
     }
 
-    function FetchErrorComponent({
-        message: j,
-        description: $
-    }) {
-        return jsxRuntimeExports.jsxs("div", {
-            role: "status",
-            className: "m-auto flex flex-col items-center",
-            children: [jsxRuntimeExports.jsx(IconComponent, {
-                className: "h-16 w-16",
-                name: "Unplug"
-            }), jsxRuntimeExports.jsx("br", {}), jsxRuntimeExports.jsx("span", {
-                className: "text-lg text-almost-medium-blue",
-                children: j
-            }), jsxRuntimeExports.jsx("span", {
-                className: "text-lg text-almost-medium-blue",
-                children: $
-            })]
-        })
+    function getPart(j, $) {
+        var at = j;
+        return $.split(CLASS_PART_SEPARATOR).forEach(function(st) {
+            at.nextPart.has(st) || at.nextPart.set(st, {
+                nextPart: new Map,
+                validators: []
+            }), at = at.nextPart.get(st)
+        }), at
     }
 
-    function LoadingComponent({
-        remSize: j
-    }) {
-        return jsxRuntimeExports.jsxs("div", {
-            role: "status",
-            className: "flex flex-col items-center justify-center",
-            children: [jsxRuntimeExports.jsxs("svg", {
-                "aria-hidden": "true",
-                className: `w-${j} h-${j} animate-spin fill-almost-medium-blue  text-muted`,
-                viewBox: "0 0 100 101",
-                fill: "none",
-                xmlns: "http://www.w3.org/2000/svg",
-                children: [jsxRuntimeExports.jsx("path", {
-                    d: "M100 50.5908C100 78.2051 77.6142 100.591 50 100.591C22.3858 100.591 0 78.2051 0 50.5908C0 22.9766 22.3858 0.59082 50 0.59082C77.6142 0.59082 100 22.9766 100 50.5908ZM9.08144 50.5908C9.08144 73.1895 27.4013 91.5094 50 91.5094C72.5987 91.5094 90.9186 73.1895 90.9186 50.5908C90.9186 27.9921 72.5987 9.67226 50 9.67226C27.4013 9.67226 9.08144 27.9921 9.08144 50.5908Z",
-                    fill: "currentColor"
-                }), jsxRuntimeExports.jsx("path", {
-                    d: "M93.9676 39.0409C96.393 38.4038 97.8624 35.9116 97.0079 33.5539C95.2932 28.8227 92.871 24.3692 89.8167 20.348C85.8452 15.1192 80.8826 10.7238 75.2124 7.41289C69.5422 4.10194 63.2754 1.94025 56.7698 1.05124C51.7666 0.367541 46.6976 0.446843 41.7345 1.27873C39.2613 1.69328 37.813 4.19778 38.4501 6.62326C39.0873 9.04874 41.5694 10.4717 44.0505 10.1071C47.8511 9.54855 51.7191 9.52689 55.5402 10.0491C60.8642 10.7766 65.9928 12.5457 70.6331 15.2552C75.2735 17.9648 79.3347 21.5619 82.5849 25.841C84.9175 28.9121 86.7997 32.2913 88.1811 35.8758C89.083 38.2158 91.5421 39.6781 93.9676 39.0409Z",
-                    fill: "currentFill"
-                })]
-            }), jsxRuntimeExports.jsx("br", {}), jsxRuntimeExports.jsx("span", {
-                className: "animate-pulse text-lg text-almost-medium-blue",
-                children: "Loading..."
-            })]
-        })
+    function isThemeGetter(j) {
+        return j.isThemeGetter
+    }
+
+    function getPrefixedClassGroupEntries(j, $) {
+        return $ ? j.map(function(at) {
+            var st = at[0],
+                ct = at[1],
+                ut = ct.map(function(dt) {
+                    return typeof dt == "string" ? $ + dt : typeof dt == "object" ? Object.fromEntries(Object.entries(dt).map(function(ft) {
+                        var pt = ft[0],
+                            Tt = ft[1];
+                        return [$ + pt, Tt]
+                    })) : dt
+                });
+            return [st, ut]
+        }) : j
+    }
+
+    function createLruCache(j) {
+        if (j < 1) return {
+            get: function() {},
+            set: function() {}
+        };
+        var $ = 0,
+            at = new Map,
+            st = new Map;
+
+        function ct(ut, dt) {
+            at.set(ut, dt), $++, $ > j && ($ = 0, st = at, at = new Map)
+        }
+        return {
+            get: function(dt) {
+                var ft = at.get(dt);
+                if (ft !== void 0) return ft;
+                if ((ft = st.get(dt)) !== void 0) return ct(dt, ft), ft
+            },
+            set: function(dt, ft) {
+                at.has(dt) ? at.set(dt, ft) : ct(dt, ft)
+            }
+        }
+    }
+    var IMPORTANT_MODIFIER = "!";
+
+    function createSplitModifiers(j) {
+        var $ = j.separator || ":",
+            at = $.length === 1,
+            st = $[0],
+            ct = $.length;
+        return function(dt) {
+            for (var ft = [], pt = 0, Tt = 0, ht, mt = 0; mt < dt.length; mt++) {
+                var Qt = dt[mt];
+                if (pt === 0) {
+                    if (Qt === st && (at || dt.slice(mt, mt + ct) === $)) {
+                        ft.push(dt.slice(Tt, mt)), Tt = mt + ct;
+                        continue
+                    }
+                    if (Qt === "/") {
+                        ht = mt;
+                        continue
+                    }
+                }
+                Qt === "[" ? pt++ : Qt === "]" && pt--
+            }
+            var vt = ft.length === 0 ? dt : dt.substring(Tt),
+                xt = vt.startsWith(IMPORTANT_MODIFIER),
+                yt = xt ? vt.substring(1) : vt,
+                Et = ht && ht > Tt ? ht - Tt : void 0;
+            return {
+                modifiers: ft,
+                hasImportantModifier: xt,
+                baseClassName: yt,
+                maybePostfixModifierPosition: Et
+            }
+        }
+    }
+
+    function sortModifiers(j) {
+        if (j.length <= 1) return j;
+        var $ = [],
+            at = [];
+        return j.forEach(function(st) {
+            var ct = st[0] === "[";
+            ct ? ($.push.apply($, at.sort().concat([st])), at = []) : at.push(st)
+        }), $.push.apply($, at.sort()), $
+    }
+
+    function createConfigUtils(j) {
+        return {
+            cache: createLruCache(j.cacheSize),
+            splitModifiers: createSplitModifiers(j),
+            ...createClassUtils(j)
+        }
+    }
+    var SPLIT_CLASSES_REGEX = /\s+/;
+
+    function mergeClassList(j, $) {
+        var at = $.splitModifiers,
+            st = $.getClassGroupId,
+            ct = $.getConflictingClassGroupIds,
+            ut = new Set;
+        return j.trim().split(SPLIT_CLASSES_REGEX).map(function(dt) {
+            var ft = at(dt),
+                pt = ft.modifiers,
+                Tt = ft.hasImportantModifier,
+                ht = ft.baseClassName,
+                mt = ft.maybePostfixModifierPosition,
+                Qt = st(mt ? ht.substring(0, mt) : ht),
+                vt = !!mt;
+            if (!Qt) {
+                if (!mt) return {
+                    isTailwindClass: !1,
+                    originalClassName: dt
+                };
+                if (Qt = st(ht), !Qt) return {
+                    isTailwindClass: !1,
+                    originalClassName: dt
+                };
+                vt = !1
+            }
+            var xt = sortModifiers(pt).join(":"),
+                yt = Tt ? xt + IMPORTANT_MODIFIER : xt;
+            return {
+                isTailwindClass: !0,
+                modifierId: yt,
+                classGroupId: Qt,
+                originalClassName: dt,
+                hasPostfixModifier: vt
+            }
+        }).reverse().filter(function(dt) {
+            if (!dt.isTailwindClass) return !0;
+            var ft = dt.modifierId,
+                pt = dt.classGroupId,
+                Tt = dt.hasPostfixModifier,
+                ht = ft + pt;
+            return ut.has(ht) ? !1 : (ut.add(ht), ct(pt, Tt).forEach(function(mt) {
+                return ut.add(ft + mt)
+            }), !0)
+        }).reverse().map(function(dt) {
+            return dt.originalClassName
+        }).join(" ")
+    }
+
+    function createTailwindMerge() {
+        for (var j = arguments.length, $ = new Array(j), at = 0; at < j; at++) $[at] = arguments[at];
+        var st, ct, ut, dt = ft;
+
+        function ft(Tt) {
+            var ht = $[0],
+                mt = $.slice(1),
+                Qt = mt.reduce(function(vt, xt) {
+                    return xt(vt)
+                }, ht());
+            return st = createConfigUtils(Qt), ct = st.cache.get, ut = st.cache.set, dt = pt, pt(Tt)
+        }
+
+        function pt(Tt) {
+            var ht = ct(Tt);
+            if (ht) return ht;
+            var mt = mergeClassList(Tt, st);
+            return ut(Tt, mt), mt
+        }
+        return function() {
+            return dt(twJoin.apply(null, arguments))
+        }
+    }
+
+    function fromTheme(j) {
+        var $ = function(st) {
+            return st[j] || []
+        };
+        return $.isThemeGetter = !0, $
+    }
+    var arbitraryValueRegex = /^\[(?:([a-z-]+):)?(.+)\]$/i,
+        fractionRegex = /^\d+\/\d+$/,
+        stringLengths = new Set(["px", "full", "screen"]),
+        tshirtUnitRegex = /^(\d+(\.\d+)?)?(xs|sm|md|lg|xl)$/,
+        lengthUnitRegex = /\d+(%|px|r?em|[sdl]?v([hwib]|min|max)|pt|pc|in|cm|mm|cap|ch|ex|r?lh|cq(w|h|i|b|min|max))|\b(calc|min|max|clamp)\(.+\)|^0$/,
+        shadowRegex = /^-?((\d+)?\.?(\d+)[a-z]+|0)_-?((\d+)?\.?(\d+)[a-z]+|0)/;
+
+    function isLength(j) {
+        return isNumber$2(j) || stringLengths.has(j) || fractionRegex.test(j) || isArbitraryLength(j)
+    }
+
+    function isArbitraryLength(j) {
+        return getIsArbitraryValue(j, "length", isLengthOnly)
+    }
+
+    function isArbitrarySize(j) {
+        return getIsArbitraryValue(j, "size", isNever)
+    }
+
+    function isArbitraryPosition(j) {
+        return getIsArbitraryValue(j, "position", isNever)
+    }
+
+    function isArbitraryUrl(j) {
+        return getIsArbitraryValue(j, "url", isUrl$1)
+    }
+
+    function isArbitraryNumber(j) {
+        return getIsArbitraryValue(j, "number", isNumber$2)
+    }
+
+    function isNumber$2(j) {
+        return !Number.isNaN(Number(j))
+    }
+
+    function isPercent$1(j) {
+        return j.endsWith("%") && isNumber$2(j.slice(0, -1))
+    }
+
+    function isInteger(j) {
+        return isIntegerOnly(j) || getIsArbitraryValue(j, "number", isIntegerOnly)
+    }
+
+    function isArbitraryValue(j) {
+        return arbitraryValueRegex.test(j)
+    }
+
+    function isAny() {
+        return !0
+    }
+
+    function isTshirtSize(j) {
+        return tshirtUnitRegex.test(j)
+    }
+
+    function isArbitraryShadow(j) {
+        return getIsArbitraryValue(j, "", isShadow)
+    }
+
+    function getIsArbitraryValue(j, $, at) {
+        var st = arbitraryValueRegex.exec(j);
+        return st ? st[1] ? st[1] === $ : at(st[2]) : !1
+    }
+
+    function isLengthOnly(j) {
+        return lengthUnitRegex.test(j)
+    }
+
+    function isNever() {
+        return !1
+    }
+
+    function isUrl$1(j) {
+        return j.startsWith("url(")
+    }
+
+    function isIntegerOnly(j) {
+        return Number.isInteger(Number(j))
+    }
+
+    function isShadow(j) {
+        return shadowRegex.test(j)
+    }
+
+    function getDefaultConfig() {
+        var j = fromTheme("colors"),
+            $ = fromTheme("spacing"),
+            at = fromTheme("blur"),
+            st = fromTheme("brightness"),
+            ct = fromTheme("borderColor"),
+            ut = fromTheme("borderRadius"),
+            dt = fromTheme("borderSpacing"),
+            ft = fromTheme("borderWidth"),
+            pt = fromTheme("contrast"),
+            Tt = fromTheme("grayscale"),
+            ht = fromTheme("hueRotate"),
+            mt = fromTheme("invert"),
+            Qt = fromTheme("gap"),
+            vt = fromTheme("gradientColorStops"),
+            xt = fromTheme("gradientColorStopPositions"),
+            yt = fromTheme("inset"),
+            Et = fromTheme("margin"),
+            bt = fromTheme("opacity"),
+            wt = fromTheme("padding"),
+            At = fromTheme("saturate"),
+            Ct = fromTheme("scale"),
+            Mt = fromTheme("sepia"),
+            St = fromTheme("skew"),
+            Rt = fromTheme("space"),
+            _t = fromTheme("translate"),
+            Ot = function() {
+                return ["auto", "contain", "none"]
+            },
+            Dt = function() {
+                return ["auto", "hidden", "clip", "visible", "scroll"]
+            },
+            Ht = function() {
+                return ["auto", isArbitraryValue, $]
+            },
+            $t = function() {
+                return [isArbitraryValue, $]
+            },
+            Pt = function() {
+                return ["", isLength]
+            },
+            jt = function() {
+                return ["auto", isNumber$2, isArbitraryValue]
+            },
+            Bt = function() {
+                return ["bottom", "center", "left", "left-bottom", "left-top", "right", "right-bottom", "right-top", "top"]
+            },
+            Ft = function() {
+                return ["solid", "dashed", "dotted", "double", "none"]
+            },
+            zt = function() {
+                return ["normal", "multiply", "screen", "overlay", "darken", "lighten", "color-dodge", "color-burn", "hard-light", "soft-light", "difference", "exclusion", "hue", "saturation", "color", "luminosity", "plus-lighter"]
+            },
+            Wt = function() {
+                return ["start", "end", "center", "between", "around", "evenly", "stretch"]
+            },
+            qt = function() {
+                return ["", "0", isArbitraryValue]
+            },
+            Ut = function() {
+                return ["auto", "avoid", "all", "avoid-page", "page", "left", "right", "column"]
+            },
+            Yt = function() {
+                return [isNumber$2, isArbitraryNumber]
+            },
+            Xt = function() {
+                return [isNumber$2, isArbitraryValue]
+            };
+        return {
+            cacheSize: 500,
+            theme: {
+                colors: [isAny],
+                spacing: [isLength],
+                blur: ["none", "", isTshirtSize, isArbitraryValue],
+                brightness: Yt(),
+                borderColor: [j],
+                borderRadius: ["none", "", "full", isTshirtSize, isArbitraryValue],
+                borderSpacing: $t(),
+                borderWidth: Pt(),
+                contrast: Yt(),
+                grayscale: qt(),
+                hueRotate: Xt(),
+                invert: qt(),
+                gap: $t(),
+                gradientColorStops: [j],
+                gradientColorStopPositions: [isPercent$1, isArbitraryLength],
+                inset: Ht(),
+                margin: Ht(),
+                opacity: Yt(),
+                padding: $t(),
+                saturate: Yt(),
+                scale: Yt(),
+                sepia: qt(),
+                skew: Xt(),
+                space: $t(),
+                translate: $t()
+            },
+            classGroups: {
+                aspect: [{
+                    aspect: ["auto", "square", "video", isArbitraryValue]
+                }],
+                container: ["container"],
+                columns: [{
+                    columns: [isTshirtSize]
+                }],
+                "break-after": [{
+                    "break-after": Ut()
+                }],
+                "break-before": [{
+                    "break-before": Ut()
+                }],
+                "break-inside": [{
+                    "break-inside": ["auto", "avoid", "avoid-page", "avoid-column"]
+                }],
+                "box-decoration": [{
+                    "box-decoration": ["slice", "clone"]
+                }],
+                box: [{
+                    box: ["border", "content"]
+                }],
+                display: ["block", "inline-block", "inline", "flex", "inline-flex", "table", "inline-table", "table-caption", "table-cell", "table-column", "table-column-group", "table-footer-group", "table-header-group", "table-row-group", "table-row", "flow-root", "grid", "inline-grid", "contents", "list-item", "hidden"],
+                float: [{
+                    float: ["right", "left", "none"]
+                }],
+                clear: [{
+                    clear: ["left", "right", "both", "none"]
+                }],
+                isolation: ["isolate", "isolation-auto"],
+                "object-fit": [{
+                    object: ["contain", "cover", "fill", "none", "scale-down"]
+                }],
+                "object-position": [{
+                    object: [].concat(Bt(), [isArbitraryValue])
+                }],
+                overflow: [{
+                    overflow: Dt()
+                }],
+                "overflow-x": [{
+                    "overflow-x": Dt()
+                }],
+                "overflow-y": [{
+                    "overflow-y": Dt()
+                }],
+                overscroll: [{
+                    overscroll: Ot()
+                }],
+                "overscroll-x": [{
+                    "overscroll-x": Ot()
+                }],
+                "overscroll-y": [{
+                    "overscroll-y": Ot()
+                }],
+                position: ["static", "fixed", "absolute", "relative", "sticky"],
+                inset: [{
+                    inset: [yt]
+                }],
+                "inset-x": [{
+                    "inset-x": [yt]
+                }],
+                "inset-y": [{
+                    "inset-y": [yt]
+                }],
+                start: [{
+                    start: [yt]
+                }],
+                end: [{
+                    end: [yt]
+                }],
+                top: [{
+                    top: [yt]
+                }],
+                right: [{
+                    right: [yt]
+                }],
+                bottom: [{
+                    bottom: [yt]
+                }],
+                left: [{
+                    left: [yt]
+                }],
+                visibility: ["visible", "invisible", "collapse"],
+                z: [{
+                    z: ["auto", isInteger]
+                }],
+                basis: [{
+                    basis: Ht()
+                }],
+                "flex-direction": [{
+                    flex: ["row", "row-reverse", "col", "col-reverse"]
+                }],
+                "flex-wrap": [{
+                    flex: ["wrap", "wrap-reverse", "nowrap"]
+                }],
+                flex: [{
+                    flex: ["1", "auto", "initial", "none", isArbitraryValue]
+                }],
+                grow: [{
+                    grow: qt()
+                }],
+                shrink: [{
+                    shrink: qt()
+                }],
+                order: [{
+                    order: ["first", "last", "none", isInteger]
+                }],
+                "grid-cols": [{
+                    "grid-cols": [isAny]
+                }],
+                "col-start-end": [{
+                    col: ["auto", {
+                        span: ["full", isInteger]
+                    }, isArbitraryValue]
+                }],
+                "col-start": [{
+                    "col-start": jt()
+                }],
+                "col-end": [{
+                    "col-end": jt()
+                }],
+                "grid-rows": [{
+                    "grid-rows": [isAny]
+                }],
+                "row-start-end": [{
+                    row: ["auto", {
+                        span: [isInteger]
+                    }, isArbitraryValue]
+                }],
+                "row-start": [{
+                    "row-start": jt()
+                }],
+                "row-end": [{
+                    "row-end": jt()
+                }],
+                "grid-flow": [{
+                    "grid-flow": ["row", "col", "dense", "row-dense", "col-dense"]
+                }],
+                "auto-cols": [{
+                    "auto-cols": ["auto", "min", "max", "fr", isArbitraryValue]
+                }],
+                "auto-rows": [{
+                    "auto-rows": ["auto", "min", "max", "fr", isArbitraryValue]
+                }],
+                gap: [{
+                    gap: [Qt]
+                }],
+                "gap-x": [{
+                    "gap-x": [Qt]
+                }],
+                "gap-y": [{
+                    "gap-y": [Qt]
+                }],
+                "justify-content": [{
+                    justify: ["normal"].concat(Wt())
+                }],
+                "justify-items": [{
+                    "justify-items": ["start", "end", "center", "stretch"]
+                }],
+                "justify-self": [{
+                    "justify-self": ["auto", "start", "end", "center", "stretch"]
+                }],
+                "align-content": [{
+                    content: ["normal"].concat(Wt(), ["baseline"])
+                }],
+                "align-items": [{
+                    items: ["start", "end", "center", "baseline", "stretch"]
+                }],
+                "align-self": [{
+                    self: ["auto", "start", "end", "center", "stretch", "baseline"]
+                }],
+                "place-content": [{
+                    "place-content": [].concat(Wt(), ["baseline"])
+                }],
+                "place-items": [{
+                    "place-items": ["start", "end", "center", "baseline", "stretch"]
+                }],
+                "place-self": [{
+                    "place-self": ["auto", "start", "end", "center", "stretch"]
+                }],
+                p: [{
+                    p: [wt]
+                }],
+                px: [{
+                    px: [wt]
+                }],
+                py: [{
+                    py: [wt]
+                }],
+                ps: [{
+                    ps: [wt]
+                }],
+                pe: [{
+                    pe: [wt]
+                }],
+                pt: [{
+                    pt: [wt]
+                }],
+                pr: [{
+                    pr: [wt]
+                }],
+                pb: [{
+                    pb: [wt]
+                }],
+                pl: [{
+                    pl: [wt]
+                }],
+                m: [{
+                    m: [Et]
+                }],
+                mx: [{
+                    mx: [Et]
+                }],
+                my: [{
+                    my: [Et]
+                }],
+                ms: [{
+                    ms: [Et]
+                }],
+                me: [{
+                    me: [Et]
+                }],
+                mt: [{
+                    mt: [Et]
+                }],
+                mr: [{
+                    mr: [Et]
+                }],
+                mb: [{
+                    mb: [Et]
+                }],
+                ml: [{
+                    ml: [Et]
+                }],
+                "space-x": [{
+                    "space-x": [Rt]
+                }],
+                "space-x-reverse": ["space-x-reverse"],
+                "space-y": [{
+                    "space-y": [Rt]
+                }],
+                "space-y-reverse": ["space-y-reverse"],
+                w: [{
+                    w: ["auto", "min", "max", "fit", isArbitraryValue, $]
+                }],
+                "min-w": [{
+                    "min-w": ["min", "max", "fit", isArbitraryValue, isLength]
+                }],
+                "max-w": [{
+                    "max-w": ["0", "none", "full", "min", "max", "fit", "prose", {
+                        screen: [isTshirtSize]
+                    }, isTshirtSize, isArbitraryValue]
+                }],
+                h: [{
+                    h: [isArbitraryValue, $, "auto", "min", "max", "fit"]
+                }],
+                "min-h": [{
+                    "min-h": ["min", "max", "fit", isArbitraryValue, isLength]
+                }],
+                "max-h": [{
+                    "max-h": [isArbitraryValue, $, "min", "max", "fit"]
+                }],
+                "font-size": [{
+                    text: ["base", isTshirtSize, isArbitraryLength]
+                }],
+                "font-smoothing": ["antialiased", "subpixel-antialiased"],
+                "font-style": ["italic", "not-italic"],
+                "font-weight": [{
+                    font: ["thin", "extralight", "light", "normal", "medium", "semibold", "bold", "extrabold", "black", isArbitraryNumber]
+                }],
+                "font-family": [{
+                    font: [isAny]
+                }],
+                "fvn-normal": ["normal-nums"],
+                "fvn-ordinal": ["ordinal"],
+                "fvn-slashed-zero": ["slashed-zero"],
+                "fvn-figure": ["lining-nums", "oldstyle-nums"],
+                "fvn-spacing": ["proportional-nums", "tabular-nums"],
+                "fvn-fraction": ["diagonal-fractions", "stacked-fractons"],
+                tracking: [{
+                    tracking: ["tighter", "tight", "normal", "wide", "wider", "widest", isArbitraryValue]
+                }],
+                "line-clamp": [{
+                    "line-clamp": ["none", isNumber$2, isArbitraryNumber]
+                }],
+                leading: [{
+                    leading: ["none", "tight", "snug", "normal", "relaxed", "loose", isArbitraryValue, isLength]
+                }],
+                "list-image": [{
+                    "list-image": ["none", isArbitraryValue]
+                }],
+                "list-style-type": [{
+                    list: ["none", "disc", "decimal", isArbitraryValue]
+                }],
+                "list-style-position": [{
+                    list: ["inside", "outside"]
+                }],
+                "placeholder-color": [{
+                    placeholder: [j]
+                }],
+                "placeholder-opacity": [{
+                    "placeholder-opacity": [bt]
+                }],
+                "text-alignment": [{
+                    text: ["left", "center", "right", "justify", "start", "end"]
+                }],
+                "text-color": [{
+                    text: [j]
+                }],
+                "text-opacity": [{
+                    "text-opacity": [bt]
+                }],
+                "text-decoration": ["underline", "overline", "line-through", "no-underline"],
+                "text-decoration-style": [{
+                    decoration: [].concat(Ft(), ["wavy"])
+                }],
+                "text-decoration-thickness": [{
+                    decoration: ["auto", "from-font", isLength]
+                }],
+                "underline-offset": [{
+                    "underline-offset": ["auto", isArbitraryValue, isLength]
+                }],
+                "text-decoration-color": [{
+                    decoration: [j]
+                }],
+                "text-transform": ["uppercase", "lowercase", "capitalize", "normal-case"],
+                "text-overflow": ["truncate", "text-ellipsis", "text-clip"],
+                indent: [{
+                    indent: $t()
+                }],
+                "vertical-align": [{
+                    align: ["baseline", "top", "middle", "bottom", "text-top", "text-bottom", "sub", "super", isArbitraryValue]
+                }],
+                whitespace: [{
+                    whitespace: ["normal", "nowrap", "pre", "pre-line", "pre-wrap", "break-spaces"]
+                }],
+                break: [{
+                    break: ["normal", "words", "all", "keep"]
+                }],
+                hyphens: [{
+                    hyphens: ["none", "manual", "auto"]
+                }],
+                content: [{
+                    content: ["none", isArbitraryValue]
+                }],
+                "bg-attachment": [{
+                    bg: ["fixed", "local", "scroll"]
+                }],
+                "bg-clip": [{
+                    "bg-clip": ["border", "padding", "content", "text"]
+                }],
+                "bg-opacity": [{
+                    "bg-opacity": [bt]
+                }],
+                "bg-origin": [{
+                    "bg-origin": ["border", "padding", "content"]
+                }],
+                "bg-position": [{
+                    bg: [].concat(Bt(), [isArbitraryPosition])
+                }],
+                "bg-repeat": [{
+                    bg: ["no-repeat", {
+                        repeat: ["", "x", "y", "round", "space"]
+                    }]
+                }],
+                "bg-size": [{
+                    bg: ["auto", "cover", "contain", isArbitrarySize]
+                }],
+                "bg-image": [{
+                    bg: ["none", {
+                        "gradient-to": ["t", "tr", "r", "br", "b", "bl", "l", "tl"]
+                    }, isArbitraryUrl]
+                }],
+                "bg-color": [{
+                    bg: [j]
+                }],
+                "gradient-from-pos": [{
+                    from: [xt]
+                }],
+                "gradient-via-pos": [{
+                    via: [xt]
+                }],
+                "gradient-to-pos": [{
+                    to: [xt]
+                }],
+                "gradient-from": [{
+                    from: [vt]
+                }],
+                "gradient-via": [{
+                    via: [vt]
+                }],
+                "gradient-to": [{
+                    to: [vt]
+                }],
+                rounded: [{
+                    rounded: [ut]
+                }],
+                "rounded-s": [{
+                    "rounded-s": [ut]
+                }],
+                "rounded-e": [{
+                    "rounded-e": [ut]
+                }],
+                "rounded-t": [{
+                    "rounded-t": [ut]
+                }],
+                "rounded-r": [{
+                    "rounded-r": [ut]
+                }],
+                "rounded-b": [{
+                    "rounded-b": [ut]
+                }],
+                "rounded-l": [{
+                    "rounded-l": [ut]
+                }],
+                "rounded-ss": [{
+                    "rounded-ss": [ut]
+                }],
+                "rounded-se": [{
+                    "rounded-se": [ut]
+                }],
+                "rounded-ee": [{
+                    "rounded-ee": [ut]
+                }],
+                "rounded-es": [{
+                    "rounded-es": [ut]
+                }],
+                "rounded-tl": [{
+                    "rounded-tl": [ut]
+                }],
+                "rounded-tr": [{
+                    "rounded-tr": [ut]
+                }],
+                "rounded-br": [{
+                    "rounded-br": [ut]
+                }],
+                "rounded-bl": [{
+                    "rounded-bl": [ut]
+                }],
+                "border-w": [{
+                    border: [ft]
+                }],
+                "border-w-x": [{
+                    "border-x": [ft]
+                }],
+                "border-w-y": [{
+                    "border-y": [ft]
+                }],
+                "border-w-s": [{
+                    "border-s": [ft]
+                }],
+                "border-w-e": [{
+                    "border-e": [ft]
+                }],
+                "border-w-t": [{
+                    "border-t": [ft]
+                }],
+                "border-w-r": [{
+                    "border-r": [ft]
+                }],
+                "border-w-b": [{
+                    "border-b": [ft]
+                }],
+                "border-w-l": [{
+                    "border-l": [ft]
+                }],
+                "border-opacity": [{
+                    "border-opacity": [bt]
+                }],
+                "border-style": [{
+                    border: [].concat(Ft(), ["hidden"])
+                }],
+                "divide-x": [{
+                    "divide-x": [ft]
+                }],
+                "divide-x-reverse": ["divide-x-reverse"],
+                "divide-y": [{
+                    "divide-y": [ft]
+                }],
+                "divide-y-reverse": ["divide-y-reverse"],
+                "divide-opacity": [{
+                    "divide-opacity": [bt]
+                }],
+                "divide-style": [{
+                    divide: Ft()
+                }],
+                "border-color": [{
+                    border: [ct]
+                }],
+                "border-color-x": [{
+                    "border-x": [ct]
+                }],
+                "border-color-y": [{
+                    "border-y": [ct]
+                }],
+                "border-color-t": [{
+                    "border-t": [ct]
+                }],
+                "border-color-r": [{
+                    "border-r": [ct]
+                }],
+                "border-color-b": [{
+                    "border-b": [ct]
+                }],
+                "border-color-l": [{
+                    "border-l": [ct]
+                }],
+                "divide-color": [{
+                    divide: [ct]
+                }],
+                "outline-style": [{
+                    outline: [""].concat(Ft())
+                }],
+                "outline-offset": [{
+                    "outline-offset": [isArbitraryValue, isLength]
+                }],
+                "outline-w": [{
+                    outline: [isLength]
+                }],
+                "outline-color": [{
+                    outline: [j]
+                }],
+                "ring-w": [{
+                    ring: Pt()
+                }],
+                "ring-w-inset": ["ring-inset"],
+                "ring-color": [{
+                    ring: [j]
+                }],
+                "ring-opacity": [{
+                    "ring-opacity": [bt]
+                }],
+                "ring-offset-w": [{
+                    "ring-offset": [isLength]
+                }],
+                "ring-offset-color": [{
+                    "ring-offset": [j]
+                }],
+                shadow: [{
+                    shadow: ["", "inner", "none", isTshirtSize, isArbitraryShadow]
+                }],
+                "shadow-color": [{
+                    shadow: [isAny]
+                }],
+                opacity: [{
+                    opacity: [bt]
+                }],
+                "mix-blend": [{
+                    "mix-blend": zt()
+                }],
+                "bg-blend": [{
+                    "bg-blend": zt()
+                }],
+                filter: [{
+                    filter: ["", "none"]
+                }],
+                blur: [{
+                    blur: [at]
+                }],
+                brightness: [{
+                    brightness: [st]
+                }],
+                contrast: [{
+                    contrast: [pt]
+                }],
+                "drop-shadow": [{
+                    "drop-shadow": ["", "none", isTshirtSize, isArbitraryValue]
+                }],
+                grayscale: [{
+                    grayscale: [Tt]
+                }],
+                "hue-rotate": [{
+                    "hue-rotate": [ht]
+                }],
+                invert: [{
+                    invert: [mt]
+                }],
+                saturate: [{
+                    saturate: [At]
+                }],
+                sepia: [{
+                    sepia: [Mt]
+                }],
+                "backdrop-filter": [{
+                    "backdrop-filter": ["", "none"]
+                }],
+                "backdrop-blur": [{
+                    "backdrop-blur": [at]
+                }],
+                "backdrop-brightness": [{
+                    "backdrop-brightness": [st]
+                }],
+                "backdrop-contrast": [{
+                    "backdrop-contrast": [pt]
+                }],
+                "backdrop-grayscale": [{
+                    "backdrop-grayscale": [Tt]
+                }],
+                "backdrop-hue-rotate": [{
+                    "backdrop-hue-rotate": [ht]
+                }],
+                "backdrop-invert": [{
+                    "backdrop-invert": [mt]
+                }],
+                "backdrop-opacity": [{
+                    "backdrop-opacity": [bt]
+                }],
+                "backdrop-saturate": [{
+                    "backdrop-saturate": [At]
+                }],
+                "backdrop-sepia": [{
+                    "backdrop-sepia": [Mt]
+                }],
+                "border-collapse": [{
+                    border: ["collapse", "separate"]
+                }],
+                "border-spacing": [{
+                    "border-spacing": [dt]
+                }],
+                "border-spacing-x": [{
+                    "border-spacing-x": [dt]
+                }],
+                "border-spacing-y": [{
+                    "border-spacing-y": [dt]
+                }],
+                "table-layout": [{
+                    table: ["auto", "fixed"]
+                }],
+                caption: [{
+                    caption: ["top", "bottom"]
+                }],
+                transition: [{
+                    transition: ["none", "all", "", "colors", "opacity", "shadow", "transform", isArbitraryValue]
+                }],
+                duration: [{
+                    duration: Xt()
+                }],
+                ease: [{
+                    ease: ["linear", "in", "out", "in-out", isArbitraryValue]
+                }],
+                delay: [{
+                    delay: Xt()
+                }],
+                animate: [{
+                    animate: ["none", "spin", "ping", "pulse", "bounce", isArbitraryValue]
+                }],
+                transform: [{
+                    transform: ["", "gpu", "none"]
+                }],
+                scale: [{
+                    scale: [Ct]
+                }],
+                "scale-x": [{
+                    "scale-x": [Ct]
+                }],
+                "scale-y": [{
+                    "scale-y": [Ct]
+                }],
+                rotate: [{
+                    rotate: [isInteger, isArbitraryValue]
+                }],
+                "translate-x": [{
+                    "translate-x": [_t]
+                }],
+                "translate-y": [{
+                    "translate-y": [_t]
+                }],
+                "skew-x": [{
+                    "skew-x": [St]
+                }],
+                "skew-y": [{
+                    "skew-y": [St]
+                }],
+                "transform-origin": [{
+                    origin: ["center", "top", "top-right", "right", "bottom-right", "bottom", "bottom-left", "left", "top-left", isArbitraryValue]
+                }],
+                accent: [{
+                    accent: ["auto", j]
+                }],
+                appearance: ["appearance-none"],
+                cursor: [{
+                    cursor: ["auto", "default", "pointer", "wait", "text", "move", "help", "not-allowed", "none", "context-menu", "progress", "cell", "crosshair", "vertical-text", "alias", "copy", "no-drop", "grab", "grabbing", "all-scroll", "col-resize", "row-resize", "n-resize", "e-resize", "s-resize", "w-resize", "ne-resize", "nw-resize", "se-resize", "sw-resize", "ew-resize", "ns-resize", "nesw-resize", "nwse-resize", "zoom-in", "zoom-out", isArbitraryValue]
+                }],
+                "caret-color": [{
+                    caret: [j]
+                }],
+                "pointer-events": [{
+                    "pointer-events": ["none", "auto"]
+                }],
+                resize: [{
+                    resize: ["none", "y", "x", ""]
+                }],
+                "scroll-behavior": [{
+                    scroll: ["auto", "smooth"]
+                }],
+                "scroll-m": [{
+                    "scroll-m": $t()
+                }],
+                "scroll-mx": [{
+                    "scroll-mx": $t()
+                }],
+                "scroll-my": [{
+                    "scroll-my": $t()
+                }],
+                "scroll-ms": [{
+                    "scroll-ms": $t()
+                }],
+                "scroll-me": [{
+                    "scroll-me": $t()
+                }],
+                "scroll-mt": [{
+                    "scroll-mt": $t()
+                }],
+                "scroll-mr": [{
+                    "scroll-mr": $t()
+                }],
+                "scroll-mb": [{
+                    "scroll-mb": $t()
+                }],
+                "scroll-ml": [{
+                    "scroll-ml": $t()
+                }],
+                "scroll-p": [{
+                    "scroll-p": $t()
+                }],
+                "scroll-px": [{
+                    "scroll-px": $t()
+                }],
+                "scroll-py": [{
+                    "scroll-py": $t()
+                }],
+                "scroll-ps": [{
+                    "scroll-ps": $t()
+                }],
+                "scroll-pe": [{
+                    "scroll-pe": $t()
+                }],
+                "scroll-pt": [{
+                    "scroll-pt": $t()
+                }],
+                "scroll-pr": [{
+                    "scroll-pr": $t()
+                }],
+                "scroll-pb": [{
+                    "scroll-pb": $t()
+                }],
+                "scroll-pl": [{
+                    "scroll-pl": $t()
+                }],
+                "snap-align": [{
+                    snap: ["start", "end", "center", "align-none"]
+                }],
+                "snap-stop": [{
+                    snap: ["normal", "always"]
+                }],
+                "snap-type": [{
+                    snap: ["none", "x", "y", "both"]
+                }],
+                "snap-strictness": [{
+                    snap: ["mandatory", "proximity"]
+                }],
+                touch: [{
+                    touch: ["auto", "none", "pinch-zoom", "manipulation", {
+                        pan: ["x", "left", "right", "y", "up", "down"]
+                    }]
+                }],
+                select: [{
+                    select: ["none", "text", "all", "auto"]
+                }],
+                "will-change": [{
+                    "will-change": ["auto", "scroll", "contents", "transform", isArbitraryValue]
+                }],
+                fill: [{
+                    fill: [j, "none"]
+                }],
+                "stroke-w": [{
+                    stroke: [isLength, isArbitraryNumber]
+                }],
+                stroke: [{
+                    stroke: [j, "none"]
+                }],
+                sr: ["sr-only", "not-sr-only"]
+            },
+            conflictingClassGroups: {
+                overflow: ["overflow-x", "overflow-y"],
+                overscroll: ["overscroll-x", "overscroll-y"],
+                inset: ["inset-x", "inset-y", "start", "end", "top", "right", "bottom", "left"],
+                "inset-x": ["right", "left"],
+                "inset-y": ["top", "bottom"],
+                flex: ["basis", "grow", "shrink"],
+                gap: ["gap-x", "gap-y"],
+                p: ["px", "py", "ps", "pe", "pt", "pr", "pb", "pl"],
+                px: ["pr", "pl"],
+                py: ["pt", "pb"],
+                m: ["mx", "my", "ms", "me", "mt", "mr", "mb", "ml"],
+                mx: ["mr", "ml"],
+                my: ["mt", "mb"],
+                "font-size": ["leading"],
+                "fvn-normal": ["fvn-ordinal", "fvn-slashed-zero", "fvn-figure", "fvn-spacing", "fvn-fraction"],
+                "fvn-ordinal": ["fvn-normal"],
+                "fvn-slashed-zero": ["fvn-normal"],
+                "fvn-figure": ["fvn-normal"],
+                "fvn-spacing": ["fvn-normal"],
+                "fvn-fraction": ["fvn-normal"],
+                rounded: ["rounded-s", "rounded-e", "rounded-t", "rounded-r", "rounded-b", "rounded-l", "rounded-ss", "rounded-se", "rounded-ee", "rounded-es", "rounded-tl", "rounded-tr", "rounded-br", "rounded-bl"],
+                "rounded-s": ["rounded-ss", "rounded-es"],
+                "rounded-e": ["rounded-se", "rounded-ee"],
+                "rounded-t": ["rounded-tl", "rounded-tr"],
+                "rounded-r": ["rounded-tr", "rounded-br"],
+                "rounded-b": ["rounded-br", "rounded-bl"],
+                "rounded-l": ["rounded-tl", "rounded-bl"],
+                "border-spacing": ["border-spacing-x", "border-spacing-y"],
+                "border-w": ["border-w-s", "border-w-e", "border-w-t", "border-w-r", "border-w-b", "border-w-l"],
+                "border-w-x": ["border-w-r", "border-w-l"],
+                "border-w-y": ["border-w-t", "border-w-b"],
+                "border-color": ["border-color-t", "border-color-r", "border-color-b", "border-color-l"],
+                "border-color-x": ["border-color-r", "border-color-l"],
+                "border-color-y": ["border-color-t", "border-color-b"],
+                "scroll-m": ["scroll-mx", "scroll-my", "scroll-ms", "scroll-me", "scroll-mt", "scroll-mr", "scroll-mb", "scroll-ml"],
+                "scroll-mx": ["scroll-mr", "scroll-ml"],
+                "scroll-my": ["scroll-mt", "scroll-mb"],
+                "scroll-p": ["scroll-px", "scroll-py", "scroll-ps", "scroll-pe", "scroll-pt", "scroll-pr", "scroll-pb", "scroll-pl"],
+                "scroll-px": ["scroll-pr", "scroll-pl"],
+                "scroll-py": ["scroll-pt", "scroll-pb"]
+            },
+            conflictingClassGroupModifiers: {
+                "font-size": ["leading"]
+            }
+        }
     }
-    const INVALID_CHARACTERS = [" ", ",", ".", ":", ";", "!", "?", "/", "\\", "(", ")", "[", "]", `
+    var twMerge = createTailwindMerge(getDefaultConfig);
+    const DESCRIPTIONS = ["Chain the Words, Master Language!", "Language Architect at Work!", "Empowering Language Engineering.", "Craft Language Connections Here.", "Create, Connect, Converse.", "Smart Chains, Smarter Conversations.", "Bridging Prompts for Brilliance.", "Language Models, Unleashed.", "Your Hub for Text Generation.", "Promptly Ingenious!", "Building Linguistic Labyrinths.", "Create, Chain, Communicate.", "Connect the Dots, Craft Language.", "Interactive Language Weaving.", "Generate, Innovate, Communicate.", "Conversation Catalyst Engine.", "Language Chainlink Master.", "Design Dialogues with Langflow.", "Nurture NLP Nodes Here.", "Conversational Cartography Unlocked.", "Design, Develop, Dialogize.", "Unleashing Linguistic Creativity.", "Graph Your Way to Great Conversations.", "The Power of Language at Your Fingertips.", "Sculpting Language with Precision.", "Where Language Meets Logic.", "Building Intelligent Interactions.", "Your Passport to Linguistic Landscapes.", "Create, Curate, Communicate with Langflow.", "Flow into the Future of Language.", "Mapping Meaningful Conversations.", "Unravel the Art of Articulation.", "Language Engineering Excellence.", "Navigate the Networks of Conversation.", "Crafting Conversations, One Node at a Time.", "The Pinnacle of Prompt Generation.", "Language Models, Mapped and Mastered.", "Powerful Prompts, Perfectly Positioned.", "Innovation in Interaction with Langflow.", "Your Toolkit for Text Generation.", "Unfolding Linguistic Possibilities.", "Building Powerful Solutions with Language Models.", "Uncover Business Opportunities with NLP.", "Harness the Power of Conversational AI.", "Transform Your Business with Smart Dialogues.", "Craft Meaningful Interactions, Generate Value.", "Unleashing Business Potential through Language Engineering.", "Empowering Enterprises with Intelligent Interactions.", "Driving Innovation in Business Communication.", "Catalyzing Business Growth through Conversational AI.", "Text Generation Meets Business Transformation.", "Navigate the Linguistic Landscape, Discover Opportunities.", "Create Powerful Connections, Boost Business Value.", "Empowering Communication, Enabling Opportunities.", "Advanced NLP for Groundbreaking Business Solutions.", "Innovation in Interaction, Revolution in Revenue.", "Maximize Impact with Intelligent Conversations.", "Beyond Text Generation - Unleashing Business Opportunities.", "Unlock the Power of AI in Your Business Conversations.", "Crafting Dialogues that Drive Business Success.", "Engineered for Excellence, Built for Business."],
+        ADJECTIVES = ["admiring", "adoring", "agitated", "amazing", "angry", "awesome", "backstabbing", "berserk", "big", "boring", "clever", "cocky", "compassionate", "condescending", "cranky", "desperate", "determined", "distracted", "dreamy", "drunk", "ecstatic", "elated", "elegant", "evil", "fervent", "focused", "furious", "gigantic", "gloomy", "goofy", "grave", "happy", "high", "hopeful", "hungry", "insane", "jolly", "jovial", "kickass", "lonely", "loving", "mad", "modest", "naughty", "nauseous", "nostalgic", "pedantic", "pensive", "prickly", "reverent", "romantic", "sad", "serene", "sharp", "sick", "silly", "sleepy", "small", "stoic", "stupefied", "suspicious", "tender", "thirsty", "tiny", "trusting", "bubbly", "charming", "cheerful", "comical", "dazzling", "delighted", "dynamic", "effervescent", "enthusiastic", "exuberant", "fluffy", "friendly", "funky", "giddy", "giggly", "gleeful", "goofy", "graceful", "grinning", "hilarious", "inquisitive", "joyous", "jubilant", "lively", "mirthful", "mischievous", "optimistic", "peppy", "perky", "playful", "quirky", "radiant", "sassy", "silly", "spirited", "sprightly", "twinkly", "upbeat", "vibrant", "witty", "zany", "zealous"],
+        NOUNS = ["albattani", "allen", "almeida", "archimedes", "ardinghelli", "aryabhata", "austin", "babbage", "banach", "bardeen", "bartik", "bassi", "bell", "bhabha", "bhaskara", "blackwell", "bohr", "booth", "borg", "bose", "boyd", "brahmagupta", "brattain", "brown", "carson", "chandrasekhar", "colden", "cori", "cray", "curie", "darwin", "davinci", "dijkstra", "dubinsky", "easley", "einstein", "elion", "engelbart", "euclid", "euler", "fermat", "fermi", "feynman", "franklin", "galileo", "gates", "goldberg", "goldstine", "goldwasser", "golick", "goodall", "hamilton", "hawking", "heisenberg", "heyrovsky", "hodgkin", "hoover", "hopper", "hugle", "hypatia", "jang", "jennings", "jepsen", "joliot", "jones", "kalam", "kare", "keller", "khorana", "kilby", "kirch", "knuth", "kowalevski", "lalande", "lamarr", "leakey", "leavitt", "lichterman", "liskov", "lovelace", "lumiere", "mahavira", "mayer", "mccarthy", "mcclintock", "mclean", "mcnulty", "meitner", "meninsky", "mestorf", "minsky", "mirzakhani", "morse", "murdock", "newton", "nobel", "noether", "northcutt", "noyce", "panini", "pare", "pasteur", "payne", "perlman", "pike", "poincare", "poitras", "ptolemy", "raman", "ramanujan", "ride", "ritchie", "roentgen", "rosalind", "saha", "sammet", "shaw", "shirley", "shockley", "sinoussi", "snyder", "spence", "stallman", "stonebraker", "swanson", "swartz", "swirles", "tesla", "thompson", "torvalds", "turing", "varahamihira", "visvesvaraya", "volhard", "wescoff", "williams", "wilson", "wing", "wozniak", "wright", "yalow", "yonath", "coulomb", "degrasse", "dewey", "edison", "eratosthenes", "faraday", "galton", "gauss", "herschel", "hubble", "joule", "kaku", "kepler", "khayyam", "lavoisier", "maxwell", "mendel", "mendeleev", "ohm", "pascal", "planck", "riemann", "schrodinger", "sagan", "tesla", "tyson", "volta", "watt", "weber", "wien", "zoBell", "zuse", "carroll"];
+    var shortUniqueId = {
+        exports: {}
+    };
+    (function(j) {
+        var $ = (() => {
+            var at = Object.defineProperty,
+                st = Object.getOwnPropertySymbols,
+                ct = Object.prototype.hasOwnProperty,
+                ut = Object.prototype.propertyIsEnumerable,
+                dt = (Et, bt, wt) => bt in Et ? at(Et, bt, {
+                    enumerable: !0,
+                    configurable: !0,
+                    writable: !0,
+                    value: wt
+                }) : Et[bt] = wt,
+                ft = (Et, bt) => {
+                    for (var wt in bt || (bt = {})) ct.call(bt, wt) && dt(Et, wt, bt[wt]);
+                    if (st)
+                        for (var wt of st(bt)) ut.call(bt, wt) && dt(Et, wt, bt[wt]);
+                    return Et
+                },
+                pt = Et => at(Et, "__esModule", {
+                    value: !0
+                }),
+                Tt = (Et, bt) => {
+                    pt(Et);
+                    for (var wt in bt) at(Et, wt, {
+                        get: bt[wt],
+                        enumerable: !0
+                    })
+                },
+                ht = {};
+            Tt(ht, {
+                DEFAULT_UUID_LENGTH: () => Qt,
+                default: () => yt
+            });
+            var mt = "4.4.4",
+                Qt = 6,
+                vt = {
+                    dictionary: "alphanum",
+                    shuffle: !0,
+                    debug: !1,
+                    length: Qt
+                },
+                xt = class extends Function {
+                    constructor(Et = {}) {
+                        super(), this.dictIndex = 0, this.dictRange = [], this.lowerBound = 0, this.upperBound = 0, this.dictLength = 0, this._digit_first_ascii = 48, this._digit_last_ascii = 58, this._alpha_lower_first_ascii = 97, this._alpha_lower_last_ascii = 123, this._hex_last_ascii = 103, this._alpha_upper_first_ascii = 65, this._alpha_upper_last_ascii = 91, this._number_dict_ranges = {
+                            digits: [this._digit_first_ascii, this._digit_last_ascii]
+                        }, this._alpha_dict_ranges = {
+                            lowerCase: [this._alpha_lower_first_ascii, this._alpha_lower_last_ascii],
+                            upperCase: [this._alpha_upper_first_ascii, this._alpha_upper_last_ascii]
+                        }, this._alpha_lower_dict_ranges = {
+                            lowerCase: [this._alpha_lower_first_ascii, this._alpha_lower_last_ascii]
+                        }, this._alpha_upper_dict_ranges = {
+                            upperCase: [this._alpha_upper_first_ascii, this._alpha_upper_last_ascii]
+                        }, this._alphanum_dict_ranges = {
+                            digits: [this._digit_first_ascii, this._digit_last_ascii],
+                            lowerCase: [this._alpha_lower_first_ascii, this._alpha_lower_last_ascii],
+                            upperCase: [this._alpha_upper_first_ascii, this._alpha_upper_last_ascii]
+                        }, this._alphanum_lower_dict_ranges = {
+                            digits: [this._digit_first_ascii, this._digit_last_ascii],
+                            lowerCase: [this._alpha_lower_first_ascii, this._alpha_lower_last_ascii]
+                        }, this._alphanum_upper_dict_ranges = {
+                            digits: [this._digit_first_ascii, this._digit_last_ascii],
+                            upperCase: [this._alpha_upper_first_ascii, this._alpha_upper_last_ascii]
+                        }, this._hex_dict_ranges = {
+                            decDigits: [this._digit_first_ascii, this._digit_last_ascii],
+                            alphaDigits: [this._alpha_lower_first_ascii, this._hex_last_ascii]
+                        }, this.log = (...Mt) => {
+                            const St = [...Mt];
+                            if (St[0] = `[short-unique-id] ${Mt[0]}`, this.debug === !0 && typeof console < "u" && console !== null) return console.log(...St)
+                        }, this.setDictionary = (Mt, St) => {
+                            let Rt;
+                            if (Mt && Array.isArray(Mt) && Mt.length > 1) Rt = Mt;
+                            else {
+                                Rt = [];
+                                let _t;
+                                this.dictIndex = _t = 0;
+                                const Ot = `_${Mt}_dict_ranges`,
+                                    Dt = this[Ot];
+                                Object.keys(Dt).forEach(Ht => {
+                                    const $t = Ht;
+                                    for (this.dictRange = Dt[$t], this.lowerBound = this.dictRange[0], this.upperBound = this.dictRange[1], this.dictIndex = _t = this.lowerBound; this.lowerBound <= this.upperBound ? _t < this.upperBound : _t > this.upperBound; this.dictIndex = this.lowerBound <= this.upperBound ? _t += 1 : _t -= 1) Rt.push(String.fromCharCode(this.dictIndex))
+                                })
+                            }
+                            St && (Rt = Rt.sort(() => Math.random() - .5)), this.dict = Rt, this.dictLength = this.dict.length, this.counter = 0
+                        }, this.seq = () => this.sequentialUUID(), this.sequentialUUID = () => {
+                            let Mt, St, Rt = "";
+                            Mt = this.counter;
+                            do St = Mt % this.dictLength, Mt = Math.trunc(Mt / this.dictLength), Rt += this.dict[St]; while (Mt !== 0);
+                            return this.counter += 1, Rt
+                        }, this.randomUUID = (Mt = this.uuidLength || Qt) => {
+                            let St, Rt, _t;
+                            if (Mt === null || typeof Mt > "u" || Mt < 1) throw new Error("Invalid UUID Length Provided");
+                            for (St = "", _t = 0; _t < Mt; _t += 1) Rt = parseInt((Math.random() * this.dictLength).toFixed(0), 10) % this.dictLength, St += this.dict[Rt];
+                            return St
+                        }, this.availableUUIDs = (Mt = this.uuidLength) => parseFloat(Math.pow([...new Set(this.dict)].length, Mt).toFixed(0)), this.approxMaxBeforeCollision = (Mt = this.availableUUIDs(this.uuidLength)) => parseFloat(Math.sqrt(Math.PI / 2 * Mt).toFixed(20)), this.collisionProbability = (Mt = this.availableUUIDs(this.uuidLength), St = this.uuidLength) => parseFloat((this.approxMaxBeforeCollision(Mt) / this.availableUUIDs(St)).toFixed(20)), this.uniqueness = (Mt = this.availableUUIDs(this.uuidLength)) => {
+                            const St = parseFloat((1 - this.approxMaxBeforeCollision(Mt) / Mt).toFixed(20));
+                            return St > 1 ? 1 : St < 0 ? 0 : St
+                        }, this.getVersion = () => this.version, this.stamp = Mt => {
+                            if (typeof Mt != "number" || Mt < 10) throw new Error("Param finalLength must be number greater than 10");
+                            const St = Math.floor(+new Date / 1e3).toString(16),
+                                Rt = Mt - 9,
+                                _t = Math.round(Math.random() * (Rt > 15 ? 15 : Rt)),
+                                Ot = this.randomUUID(Rt);
+                            return `${Ot.substr(0,_t)}${St}${Ot.substr(_t)}${_t.toString(16)}`
+                        }, this.parseStamp = Mt => {
+                            if (Mt.length < 10) throw new Error("Stamp length invalid");
+                            const St = parseInt(Mt.substr(Mt.length - 1, 1), 16);
+                            return new Date(parseInt(Mt.substr(St, 8), 16) * 1e3)
+                        };
+                        const bt = ft(ft({}, vt), Et);
+                        this.counter = 0, this.debug = !1, this.dict = [], this.version = mt;
+                        const {
+                            dictionary: wt,
+                            shuffle: At,
+                            length: Ct
+                        } = bt;
+                        return this.uuidLength = Ct, this.setDictionary(wt, At), this.debug = bt.debug, this.log(this.dict), this.log(`Generator instantiated with Dictionary Size ${this.dictLength}`), new Proxy(this, {
+                            apply: (Mt, St, Rt) => this.randomUUID(...Rt)
+                        })
+                    }
+                },
+                yt = xt;
+            return yt.default = xt, ht
+        })();
+        j.exports = $.default, typeof window < "u" && ($ = $.default)
+    })(shortUniqueId);
+    var shortUniqueIdExports = shortUniqueId.exports;
+    const ShortUniqueId = getDefaultExportFromCjs(shortUniqueIdExports),
+        INVALID_CHARACTERS = [" ", ",", ".", ":", ";", "!", "?", "/", "\\", "(", ")", "[", "]", `
 `],
         regexHighlight = /\{([^}]+)\}/g,
         specialCharsRegex = /[!@#$%^&*()\-_=+[\]{}|;:'",.<>/?\\`´]/,
         MAX_WORDS_HIGHLIGHT = 79,
         limitScrollFieldsModal = 10,
         EXPORT_DIALOG_SUBTITLE = "Export flow as JSON file.",
         SETTINGS_DIALOG_SUBTITLE = "Edit details about your project.",
@@ -18845,173 +20325,14 @@
         API_PAGE_PARAGRAPH_1 = "Your secret API keys are listed below. Please note that we do not display your secret API keys again after you generate them.",
         API_PAGE_PARAGRAPH_2 = "Do not share your API key with others, or expose it in the browser or other client-side code.",
         API_PAGE_USER_KEYS = "This user does not have any keys assigned at the moment.",
         LAST_USED_SPAN_1 = "The last time this key was used.",
         LAST_USED_SPAN_2 = "Accurate to within the hour from the most recent usage.",
         LANGFLOW_SUPPORTED_TYPES = new Set(["str", "bool", "float", "code", "prompt", "file", "int", "dict", "NestedDict"]),
         priorityFields = new Set(["code", "template"]);
-    /*!
-     * cookie
-     * Copyright(c) 2012-2014 Roman Shtylman
-     * Copyright(c) 2015 Douglas Christopher Wilson
-     * MIT Licensed
-     */
-    var parse_1 = parse$a,
-        serialize_1 = serialize$2,
-        decode$3 = decodeURIComponent,
-        encode$4 = encodeURIComponent,
-        fieldContentRegExp = /^[\u0009\u0020-\u007e\u0080-\u00ff]+$/;
-
-    function parse$a(j, $) {
-        if (typeof j != "string") throw new TypeError("argument str must be a string");
-        for (var at = {}, st = $ || {}, ct = j.split(";"), ut = st.decode || decode$3, dt = 0; dt < ct.length; dt++) {
-            var ft = ct[dt],
-                pt = ft.indexOf("=");
-            if (!(pt < 0)) {
-                var Tt = ft.substring(0, pt).trim();
-                if (at[Tt] == null) {
-                    var ht = ft.substring(pt + 1, ft.length).trim();
-                    ht[0] === '"' && (ht = ht.slice(1, -1)), at[Tt] = tryDecode(ht, ut)
-                }
-            }
-        }
-        return at
-    }
-
-    function serialize$2(j, $, at) {
-        var st = at || {},
-            ct = st.encode || encode$4;
-        if (typeof ct != "function") throw new TypeError("option encode is invalid");
-        if (!fieldContentRegExp.test(j)) throw new TypeError("argument name is invalid");
-        var ut = ct($);
-        if (ut && !fieldContentRegExp.test(ut)) throw new TypeError("argument val is invalid");
-        var dt = j + "=" + ut;
-        if (st.maxAge != null) {
-            var ft = st.maxAge - 0;
-            if (isNaN(ft) || !isFinite(ft)) throw new TypeError("option maxAge is invalid");
-            dt += "; Max-Age=" + Math.floor(ft)
-        }
-        if (st.domain) {
-            if (!fieldContentRegExp.test(st.domain)) throw new TypeError("option domain is invalid");
-            dt += "; Domain=" + st.domain
-        }
-        if (st.path) {
-            if (!fieldContentRegExp.test(st.path)) throw new TypeError("option path is invalid");
-            dt += "; Path=" + st.path
-        }
-        if (st.expires) {
-            if (typeof st.expires.toUTCString != "function") throw new TypeError("option expires is invalid");
-            dt += "; Expires=" + st.expires.toUTCString()
-        }
-        if (st.httpOnly && (dt += "; HttpOnly"), st.secure && (dt += "; Secure"), st.sameSite) {
-            var pt = typeof st.sameSite == "string" ? st.sameSite.toLowerCase() : st.sameSite;
-            switch (pt) {
-                case !0:
-                    dt += "; SameSite=Strict";
-                    break;
-                case "lax":
-                    dt += "; SameSite=Lax";
-                    break;
-                case "strict":
-                    dt += "; SameSite=Strict";
-                    break;
-                case "none":
-                    dt += "; SameSite=None";
-                    break;
-                default:
-                    throw new TypeError("option sameSite is invalid")
-            }
-        }
-        return dt
-    }
-
-    function tryDecode(j, $) {
-        try {
-            return $(j)
-        } catch {
-            return j
-        }
-    }
-
-    function hasDocumentCookie() {
-        return typeof document == "object" && typeof document.cookie == "string"
-    }
-
-    function parseCookies(j, $) {
-        return typeof j == "string" ? parse_1(j, $) : typeof j == "object" && j !== null ? j : {}
-    }
-
-    function isParsingCookie(j, $) {
-        return typeof $ > "u" && ($ = !j || j[0] !== "{" && j[0] !== "[" && j[0] !== '"'), !$
-    }
-
-    function readCookie(j, $) {
-        $ === void 0 && ($ = {});
-        var at = cleanupCookieValue(j);
-        if (isParsingCookie(at, $.doNotParse)) try {
-            return JSON.parse(at)
-        } catch {}
-        return j
-    }
-
-    function cleanupCookieValue(j) {
-        return j && j[0] === "j" && j[1] === ":" ? j.substr(2) : j
-    }
-    var __assign$G = globalThis && globalThis.__assign || function() {
-            return __assign$G = Object.assign || function(j) {
-                for (var $, at = 1, st = arguments.length; at < st; at++) {
-                    $ = arguments[at];
-                    for (var ct in $) Object.prototype.hasOwnProperty.call($, ct) && (j[ct] = $[ct])
-                }
-                return j
-            }, __assign$G.apply(this, arguments)
-        },
-        Cookies = function() {
-            function j($, at) {
-                var st = this;
-                this.changeListeners = [], this.HAS_DOCUMENT_COOKIE = !1, this.cookies = parseCookies($, at), new Promise(function() {
-                    st.HAS_DOCUMENT_COOKIE = hasDocumentCookie()
-                }).catch(function() {})
-            }
-            return j.prototype._updateBrowserValues = function($) {
-                this.HAS_DOCUMENT_COOKIE && (this.cookies = parse_1(document.cookie, $))
-            }, j.prototype._emitChange = function($) {
-                for (var at = 0; at < this.changeListeners.length; ++at) this.changeListeners[at]($)
-            }, j.prototype.get = function($, at, st) {
-                return at === void 0 && (at = {}), this._updateBrowserValues(st), readCookie(this.cookies[$], at)
-            }, j.prototype.getAll = function($, at) {
-                $ === void 0 && ($ = {}), this._updateBrowserValues(at);
-                var st = {};
-                for (var ct in this.cookies) st[ct] = readCookie(this.cookies[ct], $);
-                return st
-            }, j.prototype.set = function($, at, st) {
-                var ct;
-                typeof at == "object" && (at = JSON.stringify(at)), this.cookies = __assign$G(__assign$G({}, this.cookies), (ct = {}, ct[$] = at, ct)), this.HAS_DOCUMENT_COOKIE && (document.cookie = serialize_1($, at, st)), this._emitChange({
-                    name: $,
-                    value: at,
-                    options: st
-                })
-            }, j.prototype.remove = function($, at) {
-                var st = at = __assign$G(__assign$G({}, at), {
-                    expires: new Date(1970, 1, 1, 0, 0, 1),
-                    maxAge: 0
-                });
-                this.cookies = __assign$G({}, this.cookies), delete this.cookies[$], this.HAS_DOCUMENT_COOKIE && (document.cookie = serialize_1($, "", st)), this._emitChange({
-                    name: $,
-                    value: void 0,
-                    options: at
-                })
-            }, j.prototype.addChangeListener = function($) {
-                this.changeListeners.push($)
-            }, j.prototype.removeChangeListener = function($) {
-                var at = this.changeListeners.indexOf($);
-                at >= 0 && this.changeListeners.splice(at, 1)
-            }, j
-        }();
-    const Cookies$1 = Cookies;
 
     function bind(j, $) {
         return function() {
             return j.apply($, arguments)
         }
     }
     const {
@@ -19032,15 +20353,15 @@
 
     function isArrayBufferView(j) {
         let $;
         return typeof ArrayBuffer < "u" && ArrayBuffer.isView ? $ = ArrayBuffer.isView(j) : $ = j && j.buffer && isArrayBuffer(j.buffer), $
     }
     const isString$1 = typeOfTest("string"),
         isFunction$2 = typeOfTest("function"),
-        isNumber$2 = typeOfTest("number"),
+        isNumber$1 = typeOfTest("number"),
         isObject$3 = j => j !== null && typeof j == "object",
         isBoolean = j => j === !0 || j === !1,
         isPlainObject$3 = j => {
             if (kindOf(j) !== "object") return !1;
             const $ = getPrototypeOf$1(j);
             return ($ === null || $ === Object.prototype || Object.getPrototypeOf($) === null) && !(Symbol.toStringTag in j) && !(Symbol.iterator in j)
         },
@@ -19121,15 +20442,15 @@
             const st = j.indexOf($, at);
             return st !== -1 && st === at
         },
         toArray$1 = j => {
             if (!j) return null;
             if (isArray$3(j)) return j;
             let $ = j.length;
-            if (!isNumber$2($)) return null;
+            if (!isNumber$1($)) return null;
             const at = new Array($);
             for (; $-- > 0;) at[$] = j[$];
             return at
         },
         isTypedArray = (j => $ => j && $ instanceof j)(typeof Uint8Array < "u" && getPrototypeOf$1(Uint8Array)),
         forEachEntry = (j, $) => {
             const st = (j && j[Symbol.iterator]).call(j);
@@ -19231,15 +20552,15 @@
         utils$1 = {
             isArray: isArray$3,
             isArrayBuffer,
             isBuffer: isBuffer$2,
             isFormData,
             isArrayBufferView,
             isString: isString$1,
-            isNumber: isNumber$2,
+            isNumber: isNumber$1,
             isBoolean,
             isObject: isObject$3,
             isPlainObject: isPlainObject$3,
             isUndefined: isUndefined$1,
             isDate: isDate$1,
             isFile,
             isBlob,
@@ -19390,15 +20711,15 @@
                 }), mt.pop()
             }
         }
         if (!utils$1.isObject(j)) throw new TypeError("data must be an object");
         return vt(j), $
     }
 
-    function encode$3(j) {
+    function encode$4(j) {
         const $ = {
             "!": "%21",
             "'": "%27",
             "(": "%28",
             ")": "%29",
             "~": "%7E",
             "%20": "+",
@@ -19414,28 +20735,28 @@
     }
     const prototype = AxiosURLSearchParams.prototype;
     prototype.append = function($, at) {
         this._pairs.push([$, at])
     };
     prototype.toString = function($) {
         const at = $ ? function(st) {
-            return $.call(this, st, encode$3)
-        } : encode$3;
+            return $.call(this, st, encode$4)
+        } : encode$4;
         return this._pairs.map(function(ct) {
             return at(ct[0]) + "=" + at(ct[1])
         }, "").join("&")
     };
 
-    function encode$2(j) {
+    function encode$3(j) {
         return encodeURIComponent(j).replace(/%3A/gi, ":").replace(/%24/g, "$").replace(/%2C/gi, ",").replace(/%20/g, "+").replace(/%5B/gi, "[").replace(/%5D/gi, "]")
     }
 
     function buildURL(j, $, at) {
         if (!$) return j;
-        const st = at && at.encode || encode$2,
+        const st = at && at.encode || encode$3,
             ct = at && at.serialize;
         let ut;
         if (ct ? ut = ct($, at) : ut = utils$1.isURLSearchParams($) ? $.toString() : new AxiosURLSearchParams($, at).toString(st), ut) {
             const dt = j.indexOf("#");
             dt !== -1 && (j = j.slice(0, dt)), j += (j.indexOf("?") === -1 ? "?" : "&") + ut
         }
         return j
@@ -20418,15 +21739,174 @@
     axios.isAxiosError = isAxiosError;
     axios.mergeConfig = mergeConfig;
     axios.AxiosHeaders = AxiosHeaders$1;
     axios.formToJSON = j => formDataToJSON(utils$1.isHTMLForm(j) ? new FormData(j) : j);
     axios.getAdapter = adapters.getAdapter;
     axios.HttpStatusCode = HttpStatusCode$1;
     axios.default = axios;
-    const axios$1 = axios,
+    const axios$1 = axios;
+    /*!
+     * cookie
+     * Copyright(c) 2012-2014 Roman Shtylman
+     * Copyright(c) 2015 Douglas Christopher Wilson
+     * MIT Licensed
+     */
+    var parse_1 = parse$a,
+        serialize_1 = serialize$2,
+        decode$3 = decodeURIComponent,
+        encode$2 = encodeURIComponent,
+        fieldContentRegExp = /^[\u0009\u0020-\u007e\u0080-\u00ff]+$/;
+
+    function parse$a(j, $) {
+        if (typeof j != "string") throw new TypeError("argument str must be a string");
+        for (var at = {}, st = $ || {}, ct = j.split(";"), ut = st.decode || decode$3, dt = 0; dt < ct.length; dt++) {
+            var ft = ct[dt],
+                pt = ft.indexOf("=");
+            if (!(pt < 0)) {
+                var Tt = ft.substring(0, pt).trim();
+                if (at[Tt] == null) {
+                    var ht = ft.substring(pt + 1, ft.length).trim();
+                    ht[0] === '"' && (ht = ht.slice(1, -1)), at[Tt] = tryDecode(ht, ut)
+                }
+            }
+        }
+        return at
+    }
+
+    function serialize$2(j, $, at) {
+        var st = at || {},
+            ct = st.encode || encode$2;
+        if (typeof ct != "function") throw new TypeError("option encode is invalid");
+        if (!fieldContentRegExp.test(j)) throw new TypeError("argument name is invalid");
+        var ut = ct($);
+        if (ut && !fieldContentRegExp.test(ut)) throw new TypeError("argument val is invalid");
+        var dt = j + "=" + ut;
+        if (st.maxAge != null) {
+            var ft = st.maxAge - 0;
+            if (isNaN(ft) || !isFinite(ft)) throw new TypeError("option maxAge is invalid");
+            dt += "; Max-Age=" + Math.floor(ft)
+        }
+        if (st.domain) {
+            if (!fieldContentRegExp.test(st.domain)) throw new TypeError("option domain is invalid");
+            dt += "; Domain=" + st.domain
+        }
+        if (st.path) {
+            if (!fieldContentRegExp.test(st.path)) throw new TypeError("option path is invalid");
+            dt += "; Path=" + st.path
+        }
+        if (st.expires) {
+            if (typeof st.expires.toUTCString != "function") throw new TypeError("option expires is invalid");
+            dt += "; Expires=" + st.expires.toUTCString()
+        }
+        if (st.httpOnly && (dt += "; HttpOnly"), st.secure && (dt += "; Secure"), st.sameSite) {
+            var pt = typeof st.sameSite == "string" ? st.sameSite.toLowerCase() : st.sameSite;
+            switch (pt) {
+                case !0:
+                    dt += "; SameSite=Strict";
+                    break;
+                case "lax":
+                    dt += "; SameSite=Lax";
+                    break;
+                case "strict":
+                    dt += "; SameSite=Strict";
+                    break;
+                case "none":
+                    dt += "; SameSite=None";
+                    break;
+                default:
+                    throw new TypeError("option sameSite is invalid")
+            }
+        }
+        return dt
+    }
+
+    function tryDecode(j, $) {
+        try {
+            return $(j)
+        } catch {
+            return j
+        }
+    }
+
+    function hasDocumentCookie() {
+        return typeof document == "object" && typeof document.cookie == "string"
+    }
+
+    function parseCookies(j, $) {
+        return typeof j == "string" ? parse_1(j, $) : typeof j == "object" && j !== null ? j : {}
+    }
+
+    function isParsingCookie(j, $) {
+        return typeof $ > "u" && ($ = !j || j[0] !== "{" && j[0] !== "[" && j[0] !== '"'), !$
+    }
+
+    function readCookie(j, $) {
+        $ === void 0 && ($ = {});
+        var at = cleanupCookieValue(j);
+        if (isParsingCookie(at, $.doNotParse)) try {
+            return JSON.parse(at)
+        } catch {}
+        return j
+    }
+
+    function cleanupCookieValue(j) {
+        return j && j[0] === "j" && j[1] === ":" ? j.substr(2) : j
+    }
+    var __assign$G = globalThis && globalThis.__assign || function() {
+            return __assign$G = Object.assign || function(j) {
+                for (var $, at = 1, st = arguments.length; at < st; at++) {
+                    $ = arguments[at];
+                    for (var ct in $) Object.prototype.hasOwnProperty.call($, ct) && (j[ct] = $[ct])
+                }
+                return j
+            }, __assign$G.apply(this, arguments)
+        },
+        Cookies = function() {
+            function j($, at) {
+                var st = this;
+                this.changeListeners = [], this.HAS_DOCUMENT_COOKIE = !1, this.cookies = parseCookies($, at), new Promise(function() {
+                    st.HAS_DOCUMENT_COOKIE = hasDocumentCookie()
+                }).catch(function() {})
+            }
+            return j.prototype._updateBrowserValues = function($) {
+                this.HAS_DOCUMENT_COOKIE && (this.cookies = parse_1(document.cookie, $))
+            }, j.prototype._emitChange = function($) {
+                for (var at = 0; at < this.changeListeners.length; ++at) this.changeListeners[at]($)
+            }, j.prototype.get = function($, at, st) {
+                return at === void 0 && (at = {}), this._updateBrowserValues(st), readCookie(this.cookies[$], at)
+            }, j.prototype.getAll = function($, at) {
+                $ === void 0 && ($ = {}), this._updateBrowserValues(at);
+                var st = {};
+                for (var ct in this.cookies) st[ct] = readCookie(this.cookies[ct], $);
+                return st
+            }, j.prototype.set = function($, at, st) {
+                var ct;
+                typeof at == "object" && (at = JSON.stringify(at)), this.cookies = __assign$G(__assign$G({}, this.cookies), (ct = {}, ct[$] = at, ct)), this.HAS_DOCUMENT_COOKIE && (document.cookie = serialize_1($, at, st)), this._emitChange({
+                    name: $,
+                    value: at,
+                    options: st
+                })
+            }, j.prototype.remove = function($, at) {
+                var st = at = __assign$G(__assign$G({}, at), {
+                    expires: new Date(1970, 1, 1, 0, 0, 1),
+                    maxAge: 0
+                });
+                this.cookies = __assign$G({}, this.cookies), delete this.cookies[$], this.HAS_DOCUMENT_COOKIE && (document.cookie = serialize_1($, "", st)), this._emitChange({
+                    name: $,
+                    value: void 0,
+                    options: at
+                })
+            }, j.prototype.addChangeListener = function($) {
+                this.changeListeners.push($)
+            }, j.prototype.removeChangeListener = function($) {
+                var at = this.changeListeners.indexOf($);
+                at >= 0 && this.changeListeners.splice(at, 1)
+            }, j
+        }();
+    const Cookies$1 = Cookies,
         createStoreImpl = j => {
             let $;
             const at = new Set,
                 st = (ht, mt) => {
                     const Qt = typeof ht == "function" ? ht($) : ht;
                     if (!Object.is(Qt, $)) {
                         const vt = $;
@@ -20482,29 +21962,29 @@
                     value: at,
                     getSnapshot: $
                 }
             }),
             ct = st[0].inst,
             ut = st[1];
         return n$2(function() {
-            ct.value = at, ct.getSnapshot = $, r$4(ct) && ut({
+            ct.value = at, ct.getSnapshot = $, r$3(ct) && ut({
                 inst: ct
             })
         }, [j, at, $]), m$1(function() {
-            return r$4(ct) && ut({
+            return r$3(ct) && ut({
                 inst: ct
             }), j(function() {
-                r$4(ct) && ut({
+                r$3(ct) && ut({
                     inst: ct
                 })
             })
         }, [j]), p$3(at), at
     }
 
-    function r$4(j) {
+    function r$3(j) {
         var $ = j.getSnapshot;
         j = j.value;
         try {
             var at = $();
             return !k$1(j, at)
         } catch {
             return !0
@@ -20530,15 +22010,15 @@
     var h$3 = reactExports,
         n$1 = shimExports;
 
     function p$2(j, $) {
         return j === $ && (j !== 0 || 1 / j === 1 / $) || j !== j && $ !== $
     }
     var q$1 = typeof Object.is == "function" ? Object.is : p$2,
-        r$3 = n$1.useSyncExternalStore,
+        r$2 = n$1.useSyncExternalStore,
         t$1 = h$3.useRef,
         u$1 = h$3.useEffect,
         v$1 = h$3.useMemo,
         w = h$3.useDebugValue;
     withSelector_production_min.useSyncExternalStoreWithSelector = function(j, $, at, st, ct) {
         var ut = t$1(null);
         if (ut.current === null) {
@@ -20565,15 +22045,15 @@
                 ht, mt, Qt = at === void 0 ? null : at;
             return [function() {
                 return pt($())
             }, Qt === null ? void 0 : function() {
                 return pt(Qt())
             }]
         }, [$, at, st, ct]);
-        var ft = r$3(j, ut[0], ut[1]);
+        var ft = r$2(j, ut[0], ut[1]);
         return u$1(function() {
             dt.hasValue = !0, dt.value = ft
         }, [ft]), w(ft), ft
     };
     withSelector.exports = withSelector_production_min;
     var withSelectorExports = withSelector.exports;
     const useSyncExternalStoreExports = getDefaultExportFromCjs(withSelectorExports),
@@ -20685,2763 +22165,14 @@
             },
             setLoading: at => {
                 j({
                     loading: at
                 })
             }
         })),
-        api = axios$1.create({
-            baseURL: ""
-        });
-
-    function ApiInterceptor() {
-        const j = useAlertStore(ft => ft.setErrorData);
-        let {
-            accessToken: $,
-            login: at,
-            logout: st,
-            authenticationErrorCount: ct,
-            autoLogin: ut
-        } = reactExports.useContext(AuthContext);
-        useNavigate();
-        const dt = new Cookies$1;
-        return reactExports.useEffect(() => {
-            const ft = api.interceptors.response.use(ht => ht, async ht => {
-                    var mt, Qt, vt, xt, yt, Et, bt, wt;
-                    if (((mt = ht.response) == null ? void 0 : mt.status) === 401) {
-                        const At = dt.get("access_token_lf");
-                        if (At && !ut) {
-                            ct = ct + 1, ct > 3 && (ct = 0, st());
-                            try {
-                                const Ct = await renewAccessToken();
-                                if ((Qt = Ct == null ? void 0 : Ct.data) != null && Qt.access_token && ((vt = Ct == null ? void 0 : Ct.data) != null && vt.refresh_token) && at((xt = Ct == null ? void 0 : Ct.data) == null ? void 0 : xt.access_token), (yt = ht == null ? void 0 : ht.config) != null && yt.headers) return delete ht.config.headers.Authorization, ht.config.headers.Authorization = `Bearer ${dt.get("access_token_lf")}`, await axios$1.request(ht.config)
-                            } catch (Ct) {
-                                axios$1.isAxiosError(Ct) && ((Et = Ct.response) == null ? void 0 : Et.status) === 401 || console.error(Ct), st()
-                            }
-                        }
-                        if (!At && ((wt = (bt = ht == null ? void 0 : ht.config) == null ? void 0 : bt.url) != null && wt.includes("login"))) return Promise.reject(ht);
-                        st()
-                    } else return Promise.reject(ht)
-                }),
-                pt = ht => {
-                    const mt = ["https://raw.githubusercontent.com/logspace-ai/langflow_examples/main/examples", "https://api.github.com/repos/logspace-ai/langflow_examples/contents/examples", "https://api.github.com/repos/logspace-ai/langflow", "auto_login"],
-                        Qt = ["auto_login"];
-                    try {
-                        const vt = new URL(ht),
-                            xt = mt.some(Et => vt.origin === new URL(Et).origin),
-                            yt = Qt.some(Et => vt.pathname.includes(Et));
-                        return xt || yt
-                    } catch {
-                        return !1
-                    }
-                },
-                Tt = api.interceptors.request.use(ht => {
-                    const mt = dt.get("access_token_lf");
-                    return mt && !pt(ht == null ? void 0 : ht.url) && (ht.headers.Authorization = `Bearer ${mt}`), ht
-                }, ht => Promise.reject(ht));
-            return () => {
-                api.interceptors.response.eject(ft), api.interceptors.request.eject(Tt)
-            }
-        }, [$, j]), null
-    }
-    async function getAll() {
-        return await api.get(`${BASE_URL_API}all`)
-    }
-    const GITHUB_API_URL = "https://api.github.com";
-    async function getRepoStars(j, $) {
-        try {
-            return (await api.get(`${GITHUB_API_URL}/repos/${j}/${$}`)).data.stargazers_count
-        } catch (at) {
-            return console.error("Error fetching repository data:", at), null
-        }
-    }
-    async function postValidateCode(j) {
-        return await api.post(`${BASE_URL_API}validate/code`, {
-            code: j
-        })
-    }
-    async function postValidatePrompt(j, $, at) {
-        return api.post(`${BASE_URL_API}validate/prompt`, {
-            name: j,
-            template: $,
-            frontend_node: at
-        })
-    }
-    async function saveFlowToDatabase(j) {
-        try {
-            const $ = await api.post(`${BASE_URL_API}flows/`, {
-                name: j.name,
-                data: j.data,
-                description: j.description,
-                is_component: j.is_component
-            });
-            if ($.status !== 201) throw new Error(`HTTP error! status: ${$.status}`);
-            return $.data
-        } catch ($) {
-            throw console.error($), $
-        }
-    }
-    async function updateFlowInDatabase(j) {
-        try {
-            const $ = await api.patch(`${BASE_URL_API}flows/${j.id}`, {
-                name: j.name,
-                data: j.data,
-                description: j.description
-            });
-            if (($ == null ? void 0 : $.status) !== 200) throw new Error(`HTTP error! status: ${$==null?void 0:$.status}`);
-            return $.data
-        } catch ($) {
-            throw console.error($), $
-        }
-    }
-    async function readFlowsFromDatabase() {
-        try {
-            const j = await api.get(`${BASE_URL_API}flows/`);
-            if ((j == null ? void 0 : j.status) !== 200) throw new Error(`HTTP error! status: ${j==null?void 0:j.status}`);
-            return j.data
-        } catch (j) {
-            throw console.error(j), j
-        }
-    }
-    async function downloadFlowsFromDatabase() {
-        try {
-            const j = await api.get(`${BASE_URL_API}flows/download/`);
-            if ((j == null ? void 0 : j.status) !== 200) throw new Error(`HTTP error! status: ${j==null?void 0:j.status}`);
-            return j.data
-        } catch (j) {
-            throw console.error(j), j
-        }
-    }
-    async function uploadFlowsToDatabase(j) {
-        try {
-            const $ = await api.post(`${BASE_URL_API}flows/upload/`, j);
-            if (($ == null ? void 0 : $.status) !== 201) throw new Error(`HTTP error! status: ${$==null?void 0:$.status}`);
-            return $.data
-        } catch ($) {
-            throw console.error($), $
-        }
-    }
-    async function deleteFlowFromDatabase(j) {
-        try {
-            const $ = await api.delete(`${BASE_URL_API}flows/${j}`);
-            if ($.status !== 200) throw new Error(`HTTP error! status: ${$.status}`);
-            return $.data
-        } catch ($) {
-            throw console.error($), $
-        }
-    }
-    async function getVersion() {
-        return (await api.get(`${BASE_URL_API}version`)).data
-    }
-    async function getHealth() {
-        return await api.get("/health")
-    }
-    async function getBuildStatus(j) {
-        return await api.get(`${BASE_URL_API}build/${j}/status`)
-    }
-    async function postBuildInit(j) {
-        return await api.post(`${BASE_URL_API}build/init/${j.id}`, j)
-    }
-    async function uploadFile(j, $) {
-        const at = new FormData;
-        return at.append("file", j), await api.post(`${BASE_URL_API}upload/${$}`, at)
-    }
-    async function postCustomComponent(j, $) {
-        return await api.post(`${BASE_URL_API}custom_component`, {
-            code: j,
-            frontend_node: $
-        })
-    }
-    async function postCustomComponentUpdate(j, $) {
-        return await api.post(`${BASE_URL_API}custom_component/update`, {
-            code: j,
-            field: $
-        })
-    }
-    async function onLogin(j) {
-        try {
-            const $ = await api.post(`${BASE_URL_API}login`, new URLSearchParams({
-                username: j.username,
-                password: j.password
-            }).toString(), {
-                headers: {
-                    "Content-Type": "application/x-www-form-urlencoded"
-                }
-            });
-            if ($.status === 200) return $.data
-        } catch ($) {
-            throw $
-        }
-    }
-    async function autoLogin() {
-        try {
-            const j = await api.get(`${BASE_URL_API}auto_login`);
-            if (j.status === 200) return j.data
-        } catch (j) {
-            throw j
-        }
-    }
-    async function renewAccessToken() {
-        try {
-            return await api.post(`${BASE_URL_API}refresh`)
-        } catch (j) {
-            throw j
-        }
-    }
-    async function getLoggedUser() {
-        try {
-            const j = await api.get(`${BASE_URL_API}users/whoami`);
-            if (j.status === 200) return j.data
-        } catch (j) {
-            throw j
-        }
-        return null
-    }
-    async function addUser(j) {
-        try {
-            const $ = await api.post(`${BASE_URL_API}users/`, j);
-            if ($.status !== 201) throw new Error($.data.detail);
-            return $.data
-        } catch ($) {
-            throw $
-        }
-    }
-    async function getUsersPage(j, $) {
-        try {
-            const at = await api.get(`${BASE_URL_API}users/?skip=${j}&limit=${$}`);
-            if (at.status === 200) return at.data
-        } catch (at) {
-            throw at
-        }
-        return []
-    }
-    async function deleteUser(j) {
-        try {
-            const $ = await api.delete(`${BASE_URL_API}users/${j}`);
-            if ($.status === 200) return $.data
-        } catch ($) {
-            throw $
-        }
-    }
-    async function updateUser(j, $) {
-        try {
-            const at = await api.patch(`${BASE_URL_API}users/${j}`, $);
-            if (at.status === 200) return at.data
-        } catch (at) {
-            throw at
-        }
-    }
-    async function resetPassword(j, $) {
-        try {
-            const at = await api.patch(`${BASE_URL_API}users/${j}/reset-password`, $);
-            if (at.status === 200) return at.data
-        } catch (at) {
-            throw at
-        }
-    }
-    async function getApiKey() {
-        try {
-            const j = await api.get(`${BASE_URL_API}api_key/`);
-            if (j.status === 200) return j.data
-        } catch (j) {
-            throw j
-        }
-    }
-    async function createApiKey(j) {
-        try {
-            const $ = await api.post(`${BASE_URL_API}api_key/`, {
-                name: j
-            });
-            if ($.status === 200) return $.data
-        } catch ($) {
-            throw $
-        }
-    }
-    async function deleteApiKey(j) {
-        try {
-            const $ = await api.delete(`${BASE_URL_API}api_key/${j}`);
-            if ($.status === 200) return $.data
-        } catch ($) {
-            throw $
-        }
-    }
-    async function addApiKeyStore(j) {
-        try {
-            const $ = await api.post(`${BASE_URL_API}api_key/store`, {
-                api_key: j
-            });
-            if ($.status === 200) return $.data
-        } catch ($) {
-            throw $
-        }
-    }
-    async function saveFlowStore(j, $, at = !1) {
-        try {
-            const st = await api.post(`${BASE_URL_API}store/components/`, {
-                name: j.name,
-                data: j.data,
-                description: j.description,
-                is_component: j.is_component,
-                parent: j.parent,
-                tags: $,
-                private: !at,
-                status: at ? "Public" : "Private",
-                last_tested_version: j.last_tested_version
-            });
-            if (st.status !== 201) throw new Error(`HTTP error! status: ${st.status}`);
-            return st.data
-        } catch (st) {
-            throw console.error(st), st
-        }
-    }
-    async function getStoreComponents({
-        component_id: j = null,
-        page: $ = 1,
-        limit: at = 9999999,
-        is_component: st = null,
-        sort: ct = "-count(liked_by)",
-        tags: ut = [],
-        liked: dt = null,
-        isPrivate: ft = null,
-        search: pt = null,
-        filterByUser: Tt = null,
-        fields: ht = null
-    }) {
-        try {
-            let mt = `${BASE_URL_API}store/components/`;
-            const Qt = [];
-            j != null && Qt.push(`component_id=${j}`), pt != null && Qt.push(`search=${pt}`), ft != null && Qt.push(`private=${ft}`), ut != null && ut.length > 0 && Qt.push(`tags=${ut.join(encodeURIComponent(","))}`), ht != null && ht.length > 0 && Qt.push(`fields=${ht.join(encodeURIComponent(","))}`), ct != null ? Qt.push(`sort=${ct}`) : Qt.push("sort=-count(liked_by)"), dt != null && Qt.push(`liked=${dt}`), Tt != null && Qt.push(`filter_by_user=${Tt}`), $ !== void 0 && Qt.push(`page=${$??1}`), at !== void 0 && Qt.push(`limit=${at??9999999}`), st != null && Qt.push(`is_component=${st}`), Qt.length > 0 && (mt += `?${Qt.join("&")}`);
-            const vt = await api.get(mt);
-            if (vt.status === 200) return vt.data
-        } catch (mt) {
-            throw mt
-        }
-    }
-    async function getComponent(j) {
-        try {
-            const $ = await api.get(`${BASE_URL_API}store/components/${j}`);
-            if ($.status === 200) return $.data
-        } catch ($) {
-            throw $
-        }
-    }
-    async function checkHasApiKey() {
-        try {
-            const j = await api.get(`${BASE_URL_API}store/check/api_key`);
-            if ((j == null ? void 0 : j.status) === 200) return j.data
-        } catch (j) {
-            throw j
-        }
-    }
-    async function checkHasStore() {
-        try {
-            const j = await api.get(`${BASE_URL_API}store/check/`);
-            if ((j == null ? void 0 : j.status) === 200) return j.data
-        } catch (j) {
-            throw j
-        }
-    }
-    async function getStoreTags() {
-        try {
-            const j = await api.get(`${BASE_URL_API}store/tags`);
-            if (j.status === 200) return j.data
-        } catch (j) {
-            throw j
-        }
-    }
-    const postLikeComponent = j => api.post(`${BASE_URL_API}store/users/likes/${j}`);
-    async function updateFlowStore(j, $, at = !1, st) {
-        try {
-            const ct = await api.patch(`${BASE_URL_API}store/components/${st}`, {
-                name: j.name,
-                data: j.data,
-                description: j.description,
-                is_component: j.is_component,
-                parent: j.parent,
-                tags: $,
-                private: !at,
-                last_tested_version: j.last_tested_version
-            });
-            if (ct.status !== 201) throw new Error(`HTTP error! status: ${ct.status}`);
-            return ct.data
-        } catch (ct) {
-            throw console.error(ct), ct
-        }
-    }
-    async function requestLogout() {
-        try {
-            return (await api.post(`${BASE_URL_API}logout`)).data
-        } catch (j) {
-            throw console.error(j), j
-        }
-    }
-    var shortUniqueId = {
-        exports: {}
-    };
-    (function(j) {
-        var $ = (() => {
-            var at = Object.defineProperty,
-                st = Object.getOwnPropertySymbols,
-                ct = Object.prototype.hasOwnProperty,
-                ut = Object.prototype.propertyIsEnumerable,
-                dt = (Et, bt, wt) => bt in Et ? at(Et, bt, {
-                    enumerable: !0,
-                    configurable: !0,
-                    writable: !0,
-                    value: wt
-                }) : Et[bt] = wt,
-                ft = (Et, bt) => {
-                    for (var wt in bt || (bt = {})) ct.call(bt, wt) && dt(Et, wt, bt[wt]);
-                    if (st)
-                        for (var wt of st(bt)) ut.call(bt, wt) && dt(Et, wt, bt[wt]);
-                    return Et
-                },
-                pt = Et => at(Et, "__esModule", {
-                    value: !0
-                }),
-                Tt = (Et, bt) => {
-                    pt(Et);
-                    for (var wt in bt) at(Et, wt, {
-                        get: bt[wt],
-                        enumerable: !0
-                    })
-                },
-                ht = {};
-            Tt(ht, {
-                DEFAULT_UUID_LENGTH: () => Qt,
-                default: () => yt
-            });
-            var mt = "4.4.4",
-                Qt = 6,
-                vt = {
-                    dictionary: "alphanum",
-                    shuffle: !0,
-                    debug: !1,
-                    length: Qt
-                },
-                xt = class extends Function {
-                    constructor(Et = {}) {
-                        super(), this.dictIndex = 0, this.dictRange = [], this.lowerBound = 0, this.upperBound = 0, this.dictLength = 0, this._digit_first_ascii = 48, this._digit_last_ascii = 58, this._alpha_lower_first_ascii = 97, this._alpha_lower_last_ascii = 123, this._hex_last_ascii = 103, this._alpha_upper_first_ascii = 65, this._alpha_upper_last_ascii = 91, this._number_dict_ranges = {
-                            digits: [this._digit_first_ascii, this._digit_last_ascii]
-                        }, this._alpha_dict_ranges = {
-                            lowerCase: [this._alpha_lower_first_ascii, this._alpha_lower_last_ascii],
-                            upperCase: [this._alpha_upper_first_ascii, this._alpha_upper_last_ascii]
-                        }, this._alpha_lower_dict_ranges = {
-                            lowerCase: [this._alpha_lower_first_ascii, this._alpha_lower_last_ascii]
-                        }, this._alpha_upper_dict_ranges = {
-                            upperCase: [this._alpha_upper_first_ascii, this._alpha_upper_last_ascii]
-                        }, this._alphanum_dict_ranges = {
-                            digits: [this._digit_first_ascii, this._digit_last_ascii],
-                            lowerCase: [this._alpha_lower_first_ascii, this._alpha_lower_last_ascii],
-                            upperCase: [this._alpha_upper_first_ascii, this._alpha_upper_last_ascii]
-                        }, this._alphanum_lower_dict_ranges = {
-                            digits: [this._digit_first_ascii, this._digit_last_ascii],
-                            lowerCase: [this._alpha_lower_first_ascii, this._alpha_lower_last_ascii]
-                        }, this._alphanum_upper_dict_ranges = {
-                            digits: [this._digit_first_ascii, this._digit_last_ascii],
-                            upperCase: [this._alpha_upper_first_ascii, this._alpha_upper_last_ascii]
-                        }, this._hex_dict_ranges = {
-                            decDigits: [this._digit_first_ascii, this._digit_last_ascii],
-                            alphaDigits: [this._alpha_lower_first_ascii, this._hex_last_ascii]
-                        }, this.log = (...Mt) => {
-                            const St = [...Mt];
-                            if (St[0] = `[short-unique-id] ${Mt[0]}`, this.debug === !0 && typeof console < "u" && console !== null) return console.log(...St)
-                        }, this.setDictionary = (Mt, St) => {
-                            let Rt;
-                            if (Mt && Array.isArray(Mt) && Mt.length > 1) Rt = Mt;
-                            else {
-                                Rt = [];
-                                let _t;
-                                this.dictIndex = _t = 0;
-                                const Ot = `_${Mt}_dict_ranges`,
-                                    Dt = this[Ot];
-                                Object.keys(Dt).forEach(Ht => {
-                                    const $t = Ht;
-                                    for (this.dictRange = Dt[$t], this.lowerBound = this.dictRange[0], this.upperBound = this.dictRange[1], this.dictIndex = _t = this.lowerBound; this.lowerBound <= this.upperBound ? _t < this.upperBound : _t > this.upperBound; this.dictIndex = this.lowerBound <= this.upperBound ? _t += 1 : _t -= 1) Rt.push(String.fromCharCode(this.dictIndex))
-                                })
-                            }
-                            St && (Rt = Rt.sort(() => Math.random() - .5)), this.dict = Rt, this.dictLength = this.dict.length, this.counter = 0
-                        }, this.seq = () => this.sequentialUUID(), this.sequentialUUID = () => {
-                            let Mt, St, Rt = "";
-                            Mt = this.counter;
-                            do St = Mt % this.dictLength, Mt = Math.trunc(Mt / this.dictLength), Rt += this.dict[St]; while (Mt !== 0);
-                            return this.counter += 1, Rt
-                        }, this.randomUUID = (Mt = this.uuidLength || Qt) => {
-                            let St, Rt, _t;
-                            if (Mt === null || typeof Mt > "u" || Mt < 1) throw new Error("Invalid UUID Length Provided");
-                            for (St = "", _t = 0; _t < Mt; _t += 1) Rt = parseInt((Math.random() * this.dictLength).toFixed(0), 10) % this.dictLength, St += this.dict[Rt];
-                            return St
-                        }, this.availableUUIDs = (Mt = this.uuidLength) => parseFloat(Math.pow([...new Set(this.dict)].length, Mt).toFixed(0)), this.approxMaxBeforeCollision = (Mt = this.availableUUIDs(this.uuidLength)) => parseFloat(Math.sqrt(Math.PI / 2 * Mt).toFixed(20)), this.collisionProbability = (Mt = this.availableUUIDs(this.uuidLength), St = this.uuidLength) => parseFloat((this.approxMaxBeforeCollision(Mt) / this.availableUUIDs(St)).toFixed(20)), this.uniqueness = (Mt = this.availableUUIDs(this.uuidLength)) => {
-                            const St = parseFloat((1 - this.approxMaxBeforeCollision(Mt) / Mt).toFixed(20));
-                            return St > 1 ? 1 : St < 0 ? 0 : St
-                        }, this.getVersion = () => this.version, this.stamp = Mt => {
-                            if (typeof Mt != "number" || Mt < 10) throw new Error("Param finalLength must be number greater than 10");
-                            const St = Math.floor(+new Date / 1e3).toString(16),
-                                Rt = Mt - 9,
-                                _t = Math.round(Math.random() * (Rt > 15 ? 15 : Rt)),
-                                Ot = this.randomUUID(Rt);
-                            return `${Ot.substr(0,_t)}${St}${Ot.substr(_t)}${_t.toString(16)}`
-                        }, this.parseStamp = Mt => {
-                            if (Mt.length < 10) throw new Error("Stamp length invalid");
-                            const St = parseInt(Mt.substr(Mt.length - 1, 1), 16);
-                            return new Date(parseInt(Mt.substr(St, 8), 16) * 1e3)
-                        };
-                        const bt = ft(ft({}, vt), Et);
-                        this.counter = 0, this.debug = !1, this.dict = [], this.version = mt;
-                        const {
-                            dictionary: wt,
-                            shuffle: At,
-                            length: Ct
-                        } = bt;
-                        return this.uuidLength = Ct, this.setDictionary(wt, At), this.debug = bt.debug, this.log(this.dict), this.log(`Generator instantiated with Dictionary Size ${this.dictLength}`), new Proxy(this, {
-                            apply: (Mt, St, Rt) => this.randomUUID(...Rt)
-                        })
-                    }
-                },
-                yt = xt;
-            return yt.default = xt, ht
-        })();
-        j.exports = $.default, typeof window < "u" && ($ = $.default)
-    })(shortUniqueId);
-    var shortUniqueIdExports = shortUniqueId.exports;
-    const ShortUniqueId = getDefaultExportFromCjs(shortUniqueIdExports);
-
-    function r$2(j) {
-        var $, at, st = "";
-        if (typeof j == "string" || typeof j == "number") st += j;
-        else if (typeof j == "object")
-            if (Array.isArray(j))
-                for ($ = 0; $ < j.length; $++) j[$] && (at = r$2(j[$])) && (st && (st += " "), st += at);
-            else
-                for ($ in j) j[$] && (st && (st += " "), st += $);
-        return st
-    }
-
-    function clsx$2() {
-        for (var j, $, at = 0, st = ""; at < arguments.length;)(j = arguments[at++]) && ($ = r$2(j)) && (st && (st += " "), st += $);
-        return st
-    }
-
-    function twJoin() {
-        for (var j = 0, $, at, st = ""; j < arguments.length;)($ = arguments[j++]) && (at = toValue($)) && (st && (st += " "), st += at);
-        return st
-    }
-
-    function toValue(j) {
-        if (typeof j == "string") return j;
-        for (var $, at = "", st = 0; st < j.length; st++) j[st] && ($ = toValue(j[st])) && (at && (at += " "), at += $);
-        return at
-    }
-    var CLASS_PART_SEPARATOR = "-";
-
-    function createClassUtils(j) {
-        var $ = createClassMap(j),
-            at = j.conflictingClassGroups,
-            st = j.conflictingClassGroupModifiers,
-            ct = st === void 0 ? {} : st;
-
-        function ut(ft) {
-            var pt = ft.split(CLASS_PART_SEPARATOR);
-            return pt[0] === "" && pt.length !== 1 && pt.shift(), getGroupRecursive(pt, $) || getGroupIdForArbitraryProperty(ft)
-        }
-
-        function dt(ft, pt) {
-            var Tt = at[ft] || [];
-            return pt && ct[ft] ? [].concat(Tt, ct[ft]) : Tt
-        }
-        return {
-            getClassGroupId: ut,
-            getConflictingClassGroupIds: dt
-        }
-    }
-
-    function getGroupRecursive(j, $) {
-        var dt;
-        if (j.length === 0) return $.classGroupId;
-        var at = j[0],
-            st = $.nextPart.get(at),
-            ct = st ? getGroupRecursive(j.slice(1), st) : void 0;
-        if (ct) return ct;
-        if ($.validators.length !== 0) {
-            var ut = j.join(CLASS_PART_SEPARATOR);
-            return (dt = $.validators.find(function(ft) {
-                var pt = ft.validator;
-                return pt(ut)
-            })) == null ? void 0 : dt.classGroupId
-        }
-    }
-    var arbitraryPropertyRegex = /^\[(.+)\]$/;
-
-    function getGroupIdForArbitraryProperty(j) {
-        if (arbitraryPropertyRegex.test(j)) {
-            var $ = arbitraryPropertyRegex.exec(j)[1],
-                at = $ == null ? void 0 : $.substring(0, $.indexOf(":"));
-            if (at) return "arbitrary.." + at
-        }
-    }
-
-    function createClassMap(j) {
-        var $ = j.theme,
-            at = j.prefix,
-            st = {
-                nextPart: new Map,
-                validators: []
-            },
-            ct = getPrefixedClassGroupEntries(Object.entries(j.classGroups), at);
-        return ct.forEach(function(ut) {
-            var dt = ut[0],
-                ft = ut[1];
-            processClassesRecursively(ft, st, dt, $)
-        }), st
-    }
-
-    function processClassesRecursively(j, $, at, st) {
-        j.forEach(function(ct) {
-            if (typeof ct == "string") {
-                var ut = ct === "" ? $ : getPart($, ct);
-                ut.classGroupId = at;
-                return
-            }
-            if (typeof ct == "function") {
-                if (isThemeGetter(ct)) {
-                    processClassesRecursively(ct(st), $, at, st);
-                    return
-                }
-                $.validators.push({
-                    validator: ct,
-                    classGroupId: at
-                });
-                return
-            }
-            Object.entries(ct).forEach(function(dt) {
-                var ft = dt[0],
-                    pt = dt[1];
-                processClassesRecursively(pt, getPart($, ft), at, st)
-            })
-        })
-    }
-
-    function getPart(j, $) {
-        var at = j;
-        return $.split(CLASS_PART_SEPARATOR).forEach(function(st) {
-            at.nextPart.has(st) || at.nextPart.set(st, {
-                nextPart: new Map,
-                validators: []
-            }), at = at.nextPart.get(st)
-        }), at
-    }
-
-    function isThemeGetter(j) {
-        return j.isThemeGetter
-    }
-
-    function getPrefixedClassGroupEntries(j, $) {
-        return $ ? j.map(function(at) {
-            var st = at[0],
-                ct = at[1],
-                ut = ct.map(function(dt) {
-                    return typeof dt == "string" ? $ + dt : typeof dt == "object" ? Object.fromEntries(Object.entries(dt).map(function(ft) {
-                        var pt = ft[0],
-                            Tt = ft[1];
-                        return [$ + pt, Tt]
-                    })) : dt
-                });
-            return [st, ut]
-        }) : j
-    }
-
-    function createLruCache(j) {
-        if (j < 1) return {
-            get: function() {},
-            set: function() {}
-        };
-        var $ = 0,
-            at = new Map,
-            st = new Map;
-
-        function ct(ut, dt) {
-            at.set(ut, dt), $++, $ > j && ($ = 0, st = at, at = new Map)
-        }
-        return {
-            get: function(dt) {
-                var ft = at.get(dt);
-                if (ft !== void 0) return ft;
-                if ((ft = st.get(dt)) !== void 0) return ct(dt, ft), ft
-            },
-            set: function(dt, ft) {
-                at.has(dt) ? at.set(dt, ft) : ct(dt, ft)
-            }
-        }
-    }
-    var IMPORTANT_MODIFIER = "!";
-
-    function createSplitModifiers(j) {
-        var $ = j.separator || ":",
-            at = $.length === 1,
-            st = $[0],
-            ct = $.length;
-        return function(dt) {
-            for (var ft = [], pt = 0, Tt = 0, ht, mt = 0; mt < dt.length; mt++) {
-                var Qt = dt[mt];
-                if (pt === 0) {
-                    if (Qt === st && (at || dt.slice(mt, mt + ct) === $)) {
-                        ft.push(dt.slice(Tt, mt)), Tt = mt + ct;
-                        continue
-                    }
-                    if (Qt === "/") {
-                        ht = mt;
-                        continue
-                    }
-                }
-                Qt === "[" ? pt++ : Qt === "]" && pt--
-            }
-            var vt = ft.length === 0 ? dt : dt.substring(Tt),
-                xt = vt.startsWith(IMPORTANT_MODIFIER),
-                yt = xt ? vt.substring(1) : vt,
-                Et = ht && ht > Tt ? ht - Tt : void 0;
-            return {
-                modifiers: ft,
-                hasImportantModifier: xt,
-                baseClassName: yt,
-                maybePostfixModifierPosition: Et
-            }
-        }
-    }
-
-    function sortModifiers(j) {
-        if (j.length <= 1) return j;
-        var $ = [],
-            at = [];
-        return j.forEach(function(st) {
-            var ct = st[0] === "[";
-            ct ? ($.push.apply($, at.sort().concat([st])), at = []) : at.push(st)
-        }), $.push.apply($, at.sort()), $
-    }
-
-    function createConfigUtils(j) {
-        return {
-            cache: createLruCache(j.cacheSize),
-            splitModifiers: createSplitModifiers(j),
-            ...createClassUtils(j)
-        }
-    }
-    var SPLIT_CLASSES_REGEX = /\s+/;
-
-    function mergeClassList(j, $) {
-        var at = $.splitModifiers,
-            st = $.getClassGroupId,
-            ct = $.getConflictingClassGroupIds,
-            ut = new Set;
-        return j.trim().split(SPLIT_CLASSES_REGEX).map(function(dt) {
-            var ft = at(dt),
-                pt = ft.modifiers,
-                Tt = ft.hasImportantModifier,
-                ht = ft.baseClassName,
-                mt = ft.maybePostfixModifierPosition,
-                Qt = st(mt ? ht.substring(0, mt) : ht),
-                vt = !!mt;
-            if (!Qt) {
-                if (!mt) return {
-                    isTailwindClass: !1,
-                    originalClassName: dt
-                };
-                if (Qt = st(ht), !Qt) return {
-                    isTailwindClass: !1,
-                    originalClassName: dt
-                };
-                vt = !1
-            }
-            var xt = sortModifiers(pt).join(":"),
-                yt = Tt ? xt + IMPORTANT_MODIFIER : xt;
-            return {
-                isTailwindClass: !0,
-                modifierId: yt,
-                classGroupId: Qt,
-                originalClassName: dt,
-                hasPostfixModifier: vt
-            }
-        }).reverse().filter(function(dt) {
-            if (!dt.isTailwindClass) return !0;
-            var ft = dt.modifierId,
-                pt = dt.classGroupId,
-                Tt = dt.hasPostfixModifier,
-                ht = ft + pt;
-            return ut.has(ht) ? !1 : (ut.add(ht), ct(pt, Tt).forEach(function(mt) {
-                return ut.add(ft + mt)
-            }), !0)
-        }).reverse().map(function(dt) {
-            return dt.originalClassName
-        }).join(" ")
-    }
-
-    function createTailwindMerge() {
-        for (var j = arguments.length, $ = new Array(j), at = 0; at < j; at++) $[at] = arguments[at];
-        var st, ct, ut, dt = ft;
-
-        function ft(Tt) {
-            var ht = $[0],
-                mt = $.slice(1),
-                Qt = mt.reduce(function(vt, xt) {
-                    return xt(vt)
-                }, ht());
-            return st = createConfigUtils(Qt), ct = st.cache.get, ut = st.cache.set, dt = pt, pt(Tt)
-        }
-
-        function pt(Tt) {
-            var ht = ct(Tt);
-            if (ht) return ht;
-            var mt = mergeClassList(Tt, st);
-            return ut(Tt, mt), mt
-        }
-        return function() {
-            return dt(twJoin.apply(null, arguments))
-        }
-    }
-
-    function fromTheme(j) {
-        var $ = function(st) {
-            return st[j] || []
-        };
-        return $.isThemeGetter = !0, $
-    }
-    var arbitraryValueRegex = /^\[(?:([a-z-]+):)?(.+)\]$/i,
-        fractionRegex = /^\d+\/\d+$/,
-        stringLengths = new Set(["px", "full", "screen"]),
-        tshirtUnitRegex = /^(\d+(\.\d+)?)?(xs|sm|md|lg|xl)$/,
-        lengthUnitRegex = /\d+(%|px|r?em|[sdl]?v([hwib]|min|max)|pt|pc|in|cm|mm|cap|ch|ex|r?lh|cq(w|h|i|b|min|max))|\b(calc|min|max|clamp)\(.+\)|^0$/,
-        shadowRegex = /^-?((\d+)?\.?(\d+)[a-z]+|0)_-?((\d+)?\.?(\d+)[a-z]+|0)/;
-
-    function isLength(j) {
-        return isNumber$1(j) || stringLengths.has(j) || fractionRegex.test(j) || isArbitraryLength(j)
-    }
-
-    function isArbitraryLength(j) {
-        return getIsArbitraryValue(j, "length", isLengthOnly)
-    }
-
-    function isArbitrarySize(j) {
-        return getIsArbitraryValue(j, "size", isNever)
-    }
-
-    function isArbitraryPosition(j) {
-        return getIsArbitraryValue(j, "position", isNever)
-    }
-
-    function isArbitraryUrl(j) {
-        return getIsArbitraryValue(j, "url", isUrl$1)
-    }
-
-    function isArbitraryNumber(j) {
-        return getIsArbitraryValue(j, "number", isNumber$1)
-    }
-
-    function isNumber$1(j) {
-        return !Number.isNaN(Number(j))
-    }
-
-    function isPercent$1(j) {
-        return j.endsWith("%") && isNumber$1(j.slice(0, -1))
-    }
-
-    function isInteger(j) {
-        return isIntegerOnly(j) || getIsArbitraryValue(j, "number", isIntegerOnly)
-    }
-
-    function isArbitraryValue(j) {
-        return arbitraryValueRegex.test(j)
-    }
-
-    function isAny() {
-        return !0
-    }
-
-    function isTshirtSize(j) {
-        return tshirtUnitRegex.test(j)
-    }
-
-    function isArbitraryShadow(j) {
-        return getIsArbitraryValue(j, "", isShadow)
-    }
-
-    function getIsArbitraryValue(j, $, at) {
-        var st = arbitraryValueRegex.exec(j);
-        return st ? st[1] ? st[1] === $ : at(st[2]) : !1
-    }
-
-    function isLengthOnly(j) {
-        return lengthUnitRegex.test(j)
-    }
-
-    function isNever() {
-        return !1
-    }
-
-    function isUrl$1(j) {
-        return j.startsWith("url(")
-    }
-
-    function isIntegerOnly(j) {
-        return Number.isInteger(Number(j))
-    }
-
-    function isShadow(j) {
-        return shadowRegex.test(j)
-    }
-
-    function getDefaultConfig() {
-        var j = fromTheme("colors"),
-            $ = fromTheme("spacing"),
-            at = fromTheme("blur"),
-            st = fromTheme("brightness"),
-            ct = fromTheme("borderColor"),
-            ut = fromTheme("borderRadius"),
-            dt = fromTheme("borderSpacing"),
-            ft = fromTheme("borderWidth"),
-            pt = fromTheme("contrast"),
-            Tt = fromTheme("grayscale"),
-            ht = fromTheme("hueRotate"),
-            mt = fromTheme("invert"),
-            Qt = fromTheme("gap"),
-            vt = fromTheme("gradientColorStops"),
-            xt = fromTheme("gradientColorStopPositions"),
-            yt = fromTheme("inset"),
-            Et = fromTheme("margin"),
-            bt = fromTheme("opacity"),
-            wt = fromTheme("padding"),
-            At = fromTheme("saturate"),
-            Ct = fromTheme("scale"),
-            Mt = fromTheme("sepia"),
-            St = fromTheme("skew"),
-            Rt = fromTheme("space"),
-            _t = fromTheme("translate"),
-            Ot = function() {
-                return ["auto", "contain", "none"]
-            },
-            Dt = function() {
-                return ["auto", "hidden", "clip", "visible", "scroll"]
-            },
-            Ht = function() {
-                return ["auto", isArbitraryValue, $]
-            },
-            $t = function() {
-                return [isArbitraryValue, $]
-            },
-            Pt = function() {
-                return ["", isLength]
-            },
-            jt = function() {
-                return ["auto", isNumber$1, isArbitraryValue]
-            },
-            Bt = function() {
-                return ["bottom", "center", "left", "left-bottom", "left-top", "right", "right-bottom", "right-top", "top"]
-            },
-            Ft = function() {
-                return ["solid", "dashed", "dotted", "double", "none"]
-            },
-            zt = function() {
-                return ["normal", "multiply", "screen", "overlay", "darken", "lighten", "color-dodge", "color-burn", "hard-light", "soft-light", "difference", "exclusion", "hue", "saturation", "color", "luminosity", "plus-lighter"]
-            },
-            Wt = function() {
-                return ["start", "end", "center", "between", "around", "evenly", "stretch"]
-            },
-            qt = function() {
-                return ["", "0", isArbitraryValue]
-            },
-            Ut = function() {
-                return ["auto", "avoid", "all", "avoid-page", "page", "left", "right", "column"]
-            },
-            Yt = function() {
-                return [isNumber$1, isArbitraryNumber]
-            },
-            Xt = function() {
-                return [isNumber$1, isArbitraryValue]
-            };
-        return {
-            cacheSize: 500,
-            theme: {
-                colors: [isAny],
-                spacing: [isLength],
-                blur: ["none", "", isTshirtSize, isArbitraryValue],
-                brightness: Yt(),
-                borderColor: [j],
-                borderRadius: ["none", "", "full", isTshirtSize, isArbitraryValue],
-                borderSpacing: $t(),
-                borderWidth: Pt(),
-                contrast: Yt(),
-                grayscale: qt(),
-                hueRotate: Xt(),
-                invert: qt(),
-                gap: $t(),
-                gradientColorStops: [j],
-                gradientColorStopPositions: [isPercent$1, isArbitraryLength],
-                inset: Ht(),
-                margin: Ht(),
-                opacity: Yt(),
-                padding: $t(),
-                saturate: Yt(),
-                scale: Yt(),
-                sepia: qt(),
-                skew: Xt(),
-                space: $t(),
-                translate: $t()
-            },
-            classGroups: {
-                aspect: [{
-                    aspect: ["auto", "square", "video", isArbitraryValue]
-                }],
-                container: ["container"],
-                columns: [{
-                    columns: [isTshirtSize]
-                }],
-                "break-after": [{
-                    "break-after": Ut()
-                }],
-                "break-before": [{
-                    "break-before": Ut()
-                }],
-                "break-inside": [{
-                    "break-inside": ["auto", "avoid", "avoid-page", "avoid-column"]
-                }],
-                "box-decoration": [{
-                    "box-decoration": ["slice", "clone"]
-                }],
-                box: [{
-                    box: ["border", "content"]
-                }],
-                display: ["block", "inline-block", "inline", "flex", "inline-flex", "table", "inline-table", "table-caption", "table-cell", "table-column", "table-column-group", "table-footer-group", "table-header-group", "table-row-group", "table-row", "flow-root", "grid", "inline-grid", "contents", "list-item", "hidden"],
-                float: [{
-                    float: ["right", "left", "none"]
-                }],
-                clear: [{
-                    clear: ["left", "right", "both", "none"]
-                }],
-                isolation: ["isolate", "isolation-auto"],
-                "object-fit": [{
-                    object: ["contain", "cover", "fill", "none", "scale-down"]
-                }],
-                "object-position": [{
-                    object: [].concat(Bt(), [isArbitraryValue])
-                }],
-                overflow: [{
-                    overflow: Dt()
-                }],
-                "overflow-x": [{
-                    "overflow-x": Dt()
-                }],
-                "overflow-y": [{
-                    "overflow-y": Dt()
-                }],
-                overscroll: [{
-                    overscroll: Ot()
-                }],
-                "overscroll-x": [{
-                    "overscroll-x": Ot()
-                }],
-                "overscroll-y": [{
-                    "overscroll-y": Ot()
-                }],
-                position: ["static", "fixed", "absolute", "relative", "sticky"],
-                inset: [{
-                    inset: [yt]
-                }],
-                "inset-x": [{
-                    "inset-x": [yt]
-                }],
-                "inset-y": [{
-                    "inset-y": [yt]
-                }],
-                start: [{
-                    start: [yt]
-                }],
-                end: [{
-                    end: [yt]
-                }],
-                top: [{
-                    top: [yt]
-                }],
-                right: [{
-                    right: [yt]
-                }],
-                bottom: [{
-                    bottom: [yt]
-                }],
-                left: [{
-                    left: [yt]
-                }],
-                visibility: ["visible", "invisible", "collapse"],
-                z: [{
-                    z: ["auto", isInteger]
-                }],
-                basis: [{
-                    basis: Ht()
-                }],
-                "flex-direction": [{
-                    flex: ["row", "row-reverse", "col", "col-reverse"]
-                }],
-                "flex-wrap": [{
-                    flex: ["wrap", "wrap-reverse", "nowrap"]
-                }],
-                flex: [{
-                    flex: ["1", "auto", "initial", "none", isArbitraryValue]
-                }],
-                grow: [{
-                    grow: qt()
-                }],
-                shrink: [{
-                    shrink: qt()
-                }],
-                order: [{
-                    order: ["first", "last", "none", isInteger]
-                }],
-                "grid-cols": [{
-                    "grid-cols": [isAny]
-                }],
-                "col-start-end": [{
-                    col: ["auto", {
-                        span: ["full", isInteger]
-                    }, isArbitraryValue]
-                }],
-                "col-start": [{
-                    "col-start": jt()
-                }],
-                "col-end": [{
-                    "col-end": jt()
-                }],
-                "grid-rows": [{
-                    "grid-rows": [isAny]
-                }],
-                "row-start-end": [{
-                    row: ["auto", {
-                        span: [isInteger]
-                    }, isArbitraryValue]
-                }],
-                "row-start": [{
-                    "row-start": jt()
-                }],
-                "row-end": [{
-                    "row-end": jt()
-                }],
-                "grid-flow": [{
-                    "grid-flow": ["row", "col", "dense", "row-dense", "col-dense"]
-                }],
-                "auto-cols": [{
-                    "auto-cols": ["auto", "min", "max", "fr", isArbitraryValue]
-                }],
-                "auto-rows": [{
-                    "auto-rows": ["auto", "min", "max", "fr", isArbitraryValue]
-                }],
-                gap: [{
-                    gap: [Qt]
-                }],
-                "gap-x": [{
-                    "gap-x": [Qt]
-                }],
-                "gap-y": [{
-                    "gap-y": [Qt]
-                }],
-                "justify-content": [{
-                    justify: ["normal"].concat(Wt())
-                }],
-                "justify-items": [{
-                    "justify-items": ["start", "end", "center", "stretch"]
-                }],
-                "justify-self": [{
-                    "justify-self": ["auto", "start", "end", "center", "stretch"]
-                }],
-                "align-content": [{
-                    content: ["normal"].concat(Wt(), ["baseline"])
-                }],
-                "align-items": [{
-                    items: ["start", "end", "center", "baseline", "stretch"]
-                }],
-                "align-self": [{
-                    self: ["auto", "start", "end", "center", "stretch", "baseline"]
-                }],
-                "place-content": [{
-                    "place-content": [].concat(Wt(), ["baseline"])
-                }],
-                "place-items": [{
-                    "place-items": ["start", "end", "center", "baseline", "stretch"]
-                }],
-                "place-self": [{
-                    "place-self": ["auto", "start", "end", "center", "stretch"]
-                }],
-                p: [{
-                    p: [wt]
-                }],
-                px: [{
-                    px: [wt]
-                }],
-                py: [{
-                    py: [wt]
-                }],
-                ps: [{
-                    ps: [wt]
-                }],
-                pe: [{
-                    pe: [wt]
-                }],
-                pt: [{
-                    pt: [wt]
-                }],
-                pr: [{
-                    pr: [wt]
-                }],
-                pb: [{
-                    pb: [wt]
-                }],
-                pl: [{
-                    pl: [wt]
-                }],
-                m: [{
-                    m: [Et]
-                }],
-                mx: [{
-                    mx: [Et]
-                }],
-                my: [{
-                    my: [Et]
-                }],
-                ms: [{
-                    ms: [Et]
-                }],
-                me: [{
-                    me: [Et]
-                }],
-                mt: [{
-                    mt: [Et]
-                }],
-                mr: [{
-                    mr: [Et]
-                }],
-                mb: [{
-                    mb: [Et]
-                }],
-                ml: [{
-                    ml: [Et]
-                }],
-                "space-x": [{
-                    "space-x": [Rt]
-                }],
-                "space-x-reverse": ["space-x-reverse"],
-                "space-y": [{
-                    "space-y": [Rt]
-                }],
-                "space-y-reverse": ["space-y-reverse"],
-                w: [{
-                    w: ["auto", "min", "max", "fit", isArbitraryValue, $]
-                }],
-                "min-w": [{
-                    "min-w": ["min", "max", "fit", isArbitraryValue, isLength]
-                }],
-                "max-w": [{
-                    "max-w": ["0", "none", "full", "min", "max", "fit", "prose", {
-                        screen: [isTshirtSize]
-                    }, isTshirtSize, isArbitraryValue]
-                }],
-                h: [{
-                    h: [isArbitraryValue, $, "auto", "min", "max", "fit"]
-                }],
-                "min-h": [{
-                    "min-h": ["min", "max", "fit", isArbitraryValue, isLength]
-                }],
-                "max-h": [{
-                    "max-h": [isArbitraryValue, $, "min", "max", "fit"]
-                }],
-                "font-size": [{
-                    text: ["base", isTshirtSize, isArbitraryLength]
-                }],
-                "font-smoothing": ["antialiased", "subpixel-antialiased"],
-                "font-style": ["italic", "not-italic"],
-                "font-weight": [{
-                    font: ["thin", "extralight", "light", "normal", "medium", "semibold", "bold", "extrabold", "black", isArbitraryNumber]
-                }],
-                "font-family": [{
-                    font: [isAny]
-                }],
-                "fvn-normal": ["normal-nums"],
-                "fvn-ordinal": ["ordinal"],
-                "fvn-slashed-zero": ["slashed-zero"],
-                "fvn-figure": ["lining-nums", "oldstyle-nums"],
-                "fvn-spacing": ["proportional-nums", "tabular-nums"],
-                "fvn-fraction": ["diagonal-fractions", "stacked-fractons"],
-                tracking: [{
-                    tracking: ["tighter", "tight", "normal", "wide", "wider", "widest", isArbitraryValue]
-                }],
-                "line-clamp": [{
-                    "line-clamp": ["none", isNumber$1, isArbitraryNumber]
-                }],
-                leading: [{
-                    leading: ["none", "tight", "snug", "normal", "relaxed", "loose", isArbitraryValue, isLength]
-                }],
-                "list-image": [{
-                    "list-image": ["none", isArbitraryValue]
-                }],
-                "list-style-type": [{
-                    list: ["none", "disc", "decimal", isArbitraryValue]
-                }],
-                "list-style-position": [{
-                    list: ["inside", "outside"]
-                }],
-                "placeholder-color": [{
-                    placeholder: [j]
-                }],
-                "placeholder-opacity": [{
-                    "placeholder-opacity": [bt]
-                }],
-                "text-alignment": [{
-                    text: ["left", "center", "right", "justify", "start", "end"]
-                }],
-                "text-color": [{
-                    text: [j]
-                }],
-                "text-opacity": [{
-                    "text-opacity": [bt]
-                }],
-                "text-decoration": ["underline", "overline", "line-through", "no-underline"],
-                "text-decoration-style": [{
-                    decoration: [].concat(Ft(), ["wavy"])
-                }],
-                "text-decoration-thickness": [{
-                    decoration: ["auto", "from-font", isLength]
-                }],
-                "underline-offset": [{
-                    "underline-offset": ["auto", isArbitraryValue, isLength]
-                }],
-                "text-decoration-color": [{
-                    decoration: [j]
-                }],
-                "text-transform": ["uppercase", "lowercase", "capitalize", "normal-case"],
-                "text-overflow": ["truncate", "text-ellipsis", "text-clip"],
-                indent: [{
-                    indent: $t()
-                }],
-                "vertical-align": [{
-                    align: ["baseline", "top", "middle", "bottom", "text-top", "text-bottom", "sub", "super", isArbitraryValue]
-                }],
-                whitespace: [{
-                    whitespace: ["normal", "nowrap", "pre", "pre-line", "pre-wrap", "break-spaces"]
-                }],
-                break: [{
-                    break: ["normal", "words", "all", "keep"]
-                }],
-                hyphens: [{
-                    hyphens: ["none", "manual", "auto"]
-                }],
-                content: [{
-                    content: ["none", isArbitraryValue]
-                }],
-                "bg-attachment": [{
-                    bg: ["fixed", "local", "scroll"]
-                }],
-                "bg-clip": [{
-                    "bg-clip": ["border", "padding", "content", "text"]
-                }],
-                "bg-opacity": [{
-                    "bg-opacity": [bt]
-                }],
-                "bg-origin": [{
-                    "bg-origin": ["border", "padding", "content"]
-                }],
-                "bg-position": [{
-                    bg: [].concat(Bt(), [isArbitraryPosition])
-                }],
-                "bg-repeat": [{
-                    bg: ["no-repeat", {
-                        repeat: ["", "x", "y", "round", "space"]
-                    }]
-                }],
-                "bg-size": [{
-                    bg: ["auto", "cover", "contain", isArbitrarySize]
-                }],
-                "bg-image": [{
-                    bg: ["none", {
-                        "gradient-to": ["t", "tr", "r", "br", "b", "bl", "l", "tl"]
-                    }, isArbitraryUrl]
-                }],
-                "bg-color": [{
-                    bg: [j]
-                }],
-                "gradient-from-pos": [{
-                    from: [xt]
-                }],
-                "gradient-via-pos": [{
-                    via: [xt]
-                }],
-                "gradient-to-pos": [{
-                    to: [xt]
-                }],
-                "gradient-from": [{
-                    from: [vt]
-                }],
-                "gradient-via": [{
-                    via: [vt]
-                }],
-                "gradient-to": [{
-                    to: [vt]
-                }],
-                rounded: [{
-                    rounded: [ut]
-                }],
-                "rounded-s": [{
-                    "rounded-s": [ut]
-                }],
-                "rounded-e": [{
-                    "rounded-e": [ut]
-                }],
-                "rounded-t": [{
-                    "rounded-t": [ut]
-                }],
-                "rounded-r": [{
-                    "rounded-r": [ut]
-                }],
-                "rounded-b": [{
-                    "rounded-b": [ut]
-                }],
-                "rounded-l": [{
-                    "rounded-l": [ut]
-                }],
-                "rounded-ss": [{
-                    "rounded-ss": [ut]
-                }],
-                "rounded-se": [{
-                    "rounded-se": [ut]
-                }],
-                "rounded-ee": [{
-                    "rounded-ee": [ut]
-                }],
-                "rounded-es": [{
-                    "rounded-es": [ut]
-                }],
-                "rounded-tl": [{
-                    "rounded-tl": [ut]
-                }],
-                "rounded-tr": [{
-                    "rounded-tr": [ut]
-                }],
-                "rounded-br": [{
-                    "rounded-br": [ut]
-                }],
-                "rounded-bl": [{
-                    "rounded-bl": [ut]
-                }],
-                "border-w": [{
-                    border: [ft]
-                }],
-                "border-w-x": [{
-                    "border-x": [ft]
-                }],
-                "border-w-y": [{
-                    "border-y": [ft]
-                }],
-                "border-w-s": [{
-                    "border-s": [ft]
-                }],
-                "border-w-e": [{
-                    "border-e": [ft]
-                }],
-                "border-w-t": [{
-                    "border-t": [ft]
-                }],
-                "border-w-r": [{
-                    "border-r": [ft]
-                }],
-                "border-w-b": [{
-                    "border-b": [ft]
-                }],
-                "border-w-l": [{
-                    "border-l": [ft]
-                }],
-                "border-opacity": [{
-                    "border-opacity": [bt]
-                }],
-                "border-style": [{
-                    border: [].concat(Ft(), ["hidden"])
-                }],
-                "divide-x": [{
-                    "divide-x": [ft]
-                }],
-                "divide-x-reverse": ["divide-x-reverse"],
-                "divide-y": [{
-                    "divide-y": [ft]
-                }],
-                "divide-y-reverse": ["divide-y-reverse"],
-                "divide-opacity": [{
-                    "divide-opacity": [bt]
-                }],
-                "divide-style": [{
-                    divide: Ft()
-                }],
-                "border-color": [{
-                    border: [ct]
-                }],
-                "border-color-x": [{
-                    "border-x": [ct]
-                }],
-                "border-color-y": [{
-                    "border-y": [ct]
-                }],
-                "border-color-t": [{
-                    "border-t": [ct]
-                }],
-                "border-color-r": [{
-                    "border-r": [ct]
-                }],
-                "border-color-b": [{
-                    "border-b": [ct]
-                }],
-                "border-color-l": [{
-                    "border-l": [ct]
-                }],
-                "divide-color": [{
-                    divide: [ct]
-                }],
-                "outline-style": [{
-                    outline: [""].concat(Ft())
-                }],
-                "outline-offset": [{
-                    "outline-offset": [isArbitraryValue, isLength]
-                }],
-                "outline-w": [{
-                    outline: [isLength]
-                }],
-                "outline-color": [{
-                    outline: [j]
-                }],
-                "ring-w": [{
-                    ring: Pt()
-                }],
-                "ring-w-inset": ["ring-inset"],
-                "ring-color": [{
-                    ring: [j]
-                }],
-                "ring-opacity": [{
-                    "ring-opacity": [bt]
-                }],
-                "ring-offset-w": [{
-                    "ring-offset": [isLength]
-                }],
-                "ring-offset-color": [{
-                    "ring-offset": [j]
-                }],
-                shadow: [{
-                    shadow: ["", "inner", "none", isTshirtSize, isArbitraryShadow]
-                }],
-                "shadow-color": [{
-                    shadow: [isAny]
-                }],
-                opacity: [{
-                    opacity: [bt]
-                }],
-                "mix-blend": [{
-                    "mix-blend": zt()
-                }],
-                "bg-blend": [{
-                    "bg-blend": zt()
-                }],
-                filter: [{
-                    filter: ["", "none"]
-                }],
-                blur: [{
-                    blur: [at]
-                }],
-                brightness: [{
-                    brightness: [st]
-                }],
-                contrast: [{
-                    contrast: [pt]
-                }],
-                "drop-shadow": [{
-                    "drop-shadow": ["", "none", isTshirtSize, isArbitraryValue]
-                }],
-                grayscale: [{
-                    grayscale: [Tt]
-                }],
-                "hue-rotate": [{
-                    "hue-rotate": [ht]
-                }],
-                invert: [{
-                    invert: [mt]
-                }],
-                saturate: [{
-                    saturate: [At]
-                }],
-                sepia: [{
-                    sepia: [Mt]
-                }],
-                "backdrop-filter": [{
-                    "backdrop-filter": ["", "none"]
-                }],
-                "backdrop-blur": [{
-                    "backdrop-blur": [at]
-                }],
-                "backdrop-brightness": [{
-                    "backdrop-brightness": [st]
-                }],
-                "backdrop-contrast": [{
-                    "backdrop-contrast": [pt]
-                }],
-                "backdrop-grayscale": [{
-                    "backdrop-grayscale": [Tt]
-                }],
-                "backdrop-hue-rotate": [{
-                    "backdrop-hue-rotate": [ht]
-                }],
-                "backdrop-invert": [{
-                    "backdrop-invert": [mt]
-                }],
-                "backdrop-opacity": [{
-                    "backdrop-opacity": [bt]
-                }],
-                "backdrop-saturate": [{
-                    "backdrop-saturate": [At]
-                }],
-                "backdrop-sepia": [{
-                    "backdrop-sepia": [Mt]
-                }],
-                "border-collapse": [{
-                    border: ["collapse", "separate"]
-                }],
-                "border-spacing": [{
-                    "border-spacing": [dt]
-                }],
-                "border-spacing-x": [{
-                    "border-spacing-x": [dt]
-                }],
-                "border-spacing-y": [{
-                    "border-spacing-y": [dt]
-                }],
-                "table-layout": [{
-                    table: ["auto", "fixed"]
-                }],
-                caption: [{
-                    caption: ["top", "bottom"]
-                }],
-                transition: [{
-                    transition: ["none", "all", "", "colors", "opacity", "shadow", "transform", isArbitraryValue]
-                }],
-                duration: [{
-                    duration: Xt()
-                }],
-                ease: [{
-                    ease: ["linear", "in", "out", "in-out", isArbitraryValue]
-                }],
-                delay: [{
-                    delay: Xt()
-                }],
-                animate: [{
-                    animate: ["none", "spin", "ping", "pulse", "bounce", isArbitraryValue]
-                }],
-                transform: [{
-                    transform: ["", "gpu", "none"]
-                }],
-                scale: [{
-                    scale: [Ct]
-                }],
-                "scale-x": [{
-                    "scale-x": [Ct]
-                }],
-                "scale-y": [{
-                    "scale-y": [Ct]
-                }],
-                rotate: [{
-                    rotate: [isInteger, isArbitraryValue]
-                }],
-                "translate-x": [{
-                    "translate-x": [_t]
-                }],
-                "translate-y": [{
-                    "translate-y": [_t]
-                }],
-                "skew-x": [{
-                    "skew-x": [St]
-                }],
-                "skew-y": [{
-                    "skew-y": [St]
-                }],
-                "transform-origin": [{
-                    origin: ["center", "top", "top-right", "right", "bottom-right", "bottom", "bottom-left", "left", "top-left", isArbitraryValue]
-                }],
-                accent: [{
-                    accent: ["auto", j]
-                }],
-                appearance: ["appearance-none"],
-                cursor: [{
-                    cursor: ["auto", "default", "pointer", "wait", "text", "move", "help", "not-allowed", "none", "context-menu", "progress", "cell", "crosshair", "vertical-text", "alias", "copy", "no-drop", "grab", "grabbing", "all-scroll", "col-resize", "row-resize", "n-resize", "e-resize", "s-resize", "w-resize", "ne-resize", "nw-resize", "se-resize", "sw-resize", "ew-resize", "ns-resize", "nesw-resize", "nwse-resize", "zoom-in", "zoom-out", isArbitraryValue]
-                }],
-                "caret-color": [{
-                    caret: [j]
-                }],
-                "pointer-events": [{
-                    "pointer-events": ["none", "auto"]
-                }],
-                resize: [{
-                    resize: ["none", "y", "x", ""]
-                }],
-                "scroll-behavior": [{
-                    scroll: ["auto", "smooth"]
-                }],
-                "scroll-m": [{
-                    "scroll-m": $t()
-                }],
-                "scroll-mx": [{
-                    "scroll-mx": $t()
-                }],
-                "scroll-my": [{
-                    "scroll-my": $t()
-                }],
-                "scroll-ms": [{
-                    "scroll-ms": $t()
-                }],
-                "scroll-me": [{
-                    "scroll-me": $t()
-                }],
-                "scroll-mt": [{
-                    "scroll-mt": $t()
-                }],
-                "scroll-mr": [{
-                    "scroll-mr": $t()
-                }],
-                "scroll-mb": [{
-                    "scroll-mb": $t()
-                }],
-                "scroll-ml": [{
-                    "scroll-ml": $t()
-                }],
-                "scroll-p": [{
-                    "scroll-p": $t()
-                }],
-                "scroll-px": [{
-                    "scroll-px": $t()
-                }],
-                "scroll-py": [{
-                    "scroll-py": $t()
-                }],
-                "scroll-ps": [{
-                    "scroll-ps": $t()
-                }],
-                "scroll-pe": [{
-                    "scroll-pe": $t()
-                }],
-                "scroll-pt": [{
-                    "scroll-pt": $t()
-                }],
-                "scroll-pr": [{
-                    "scroll-pr": $t()
-                }],
-                "scroll-pb": [{
-                    "scroll-pb": $t()
-                }],
-                "scroll-pl": [{
-                    "scroll-pl": $t()
-                }],
-                "snap-align": [{
-                    snap: ["start", "end", "center", "align-none"]
-                }],
-                "snap-stop": [{
-                    snap: ["normal", "always"]
-                }],
-                "snap-type": [{
-                    snap: ["none", "x", "y", "both"]
-                }],
-                "snap-strictness": [{
-                    snap: ["mandatory", "proximity"]
-                }],
-                touch: [{
-                    touch: ["auto", "none", "pinch-zoom", "manipulation", {
-                        pan: ["x", "left", "right", "y", "up", "down"]
-                    }]
-                }],
-                select: [{
-                    select: ["none", "text", "all", "auto"]
-                }],
-                "will-change": [{
-                    "will-change": ["auto", "scroll", "contents", "transform", isArbitraryValue]
-                }],
-                fill: [{
-                    fill: [j, "none"]
-                }],
-                "stroke-w": [{
-                    stroke: [isLength, isArbitraryNumber]
-                }],
-                stroke: [{
-                    stroke: [j, "none"]
-                }],
-                sr: ["sr-only", "not-sr-only"]
-            },
-            conflictingClassGroups: {
-                overflow: ["overflow-x", "overflow-y"],
-                overscroll: ["overscroll-x", "overscroll-y"],
-                inset: ["inset-x", "inset-y", "start", "end", "top", "right", "bottom", "left"],
-                "inset-x": ["right", "left"],
-                "inset-y": ["top", "bottom"],
-                flex: ["basis", "grow", "shrink"],
-                gap: ["gap-x", "gap-y"],
-                p: ["px", "py", "ps", "pe", "pt", "pr", "pb", "pl"],
-                px: ["pr", "pl"],
-                py: ["pt", "pb"],
-                m: ["mx", "my", "ms", "me", "mt", "mr", "mb", "ml"],
-                mx: ["mr", "ml"],
-                my: ["mt", "mb"],
-                "font-size": ["leading"],
-                "fvn-normal": ["fvn-ordinal", "fvn-slashed-zero", "fvn-figure", "fvn-spacing", "fvn-fraction"],
-                "fvn-ordinal": ["fvn-normal"],
-                "fvn-slashed-zero": ["fvn-normal"],
-                "fvn-figure": ["fvn-normal"],
-                "fvn-spacing": ["fvn-normal"],
-                "fvn-fraction": ["fvn-normal"],
-                rounded: ["rounded-s", "rounded-e", "rounded-t", "rounded-r", "rounded-b", "rounded-l", "rounded-ss", "rounded-se", "rounded-ee", "rounded-es", "rounded-tl", "rounded-tr", "rounded-br", "rounded-bl"],
-                "rounded-s": ["rounded-ss", "rounded-es"],
-                "rounded-e": ["rounded-se", "rounded-ee"],
-                "rounded-t": ["rounded-tl", "rounded-tr"],
-                "rounded-r": ["rounded-tr", "rounded-br"],
-                "rounded-b": ["rounded-br", "rounded-bl"],
-                "rounded-l": ["rounded-tl", "rounded-bl"],
-                "border-spacing": ["border-spacing-x", "border-spacing-y"],
-                "border-w": ["border-w-s", "border-w-e", "border-w-t", "border-w-r", "border-w-b", "border-w-l"],
-                "border-w-x": ["border-w-r", "border-w-l"],
-                "border-w-y": ["border-w-t", "border-w-b"],
-                "border-color": ["border-color-t", "border-color-r", "border-color-b", "border-color-l"],
-                "border-color-x": ["border-color-r", "border-color-l"],
-                "border-color-y": ["border-color-t", "border-color-b"],
-                "scroll-m": ["scroll-mx", "scroll-my", "scroll-ms", "scroll-me", "scroll-mt", "scroll-mr", "scroll-mb", "scroll-ml"],
-                "scroll-mx": ["scroll-mr", "scroll-ml"],
-                "scroll-my": ["scroll-mt", "scroll-mb"],
-                "scroll-p": ["scroll-px", "scroll-py", "scroll-ps", "scroll-pe", "scroll-pt", "scroll-pr", "scroll-pb", "scroll-pl"],
-                "scroll-px": ["scroll-pr", "scroll-pl"],
-                "scroll-py": ["scroll-pt", "scroll-pb"]
-            },
-            conflictingClassGroupModifiers: {
-                "font-size": ["leading"]
-            }
-        }
-    }
-    var twMerge = createTailwindMerge(getDefaultConfig);
-    const DESCRIPTIONS = ["Chain the Words, Master Language!", "Language Architect at Work!", "Empowering Language Engineering.", "Craft Language Connections Here.", "Create, Connect, Converse.", "Smart Chains, Smarter Conversations.", "Bridging Prompts for Brilliance.", "Language Models, Unleashed.", "Your Hub for Text Generation.", "Promptly Ingenious!", "Building Linguistic Labyrinths.", "Create, Chain, Communicate.", "Connect the Dots, Craft Language.", "Interactive Language Weaving.", "Generate, Innovate, Communicate.", "Conversation Catalyst Engine.", "Language Chainlink Master.", "Design Dialogues with Langflow.", "Nurture NLP Nodes Here.", "Conversational Cartography Unlocked.", "Design, Develop, Dialogize.", "Unleashing Linguistic Creativity.", "Graph Your Way to Great Conversations.", "The Power of Language at Your Fingertips.", "Sculpting Language with Precision.", "Where Language Meets Logic.", "Building Intelligent Interactions.", "Your Passport to Linguistic Landscapes.", "Create, Curate, Communicate with Langflow.", "Flow into the Future of Language.", "Mapping Meaningful Conversations.", "Unravel the Art of Articulation.", "Language Engineering Excellence.", "Navigate the Networks of Conversation.", "Crafting Conversations, One Node at a Time.", "The Pinnacle of Prompt Generation.", "Language Models, Mapped and Mastered.", "Powerful Prompts, Perfectly Positioned.", "Innovation in Interaction with Langflow.", "Your Toolkit for Text Generation.", "Unfolding Linguistic Possibilities.", "Building Powerful Solutions with Language Models.", "Uncover Business Opportunities with NLP.", "Harness the Power of Conversational AI.", "Transform Your Business with Smart Dialogues.", "Craft Meaningful Interactions, Generate Value.", "Unleashing Business Potential through Language Engineering.", "Empowering Enterprises with Intelligent Interactions.", "Driving Innovation in Business Communication.", "Catalyzing Business Growth through Conversational AI.", "Text Generation Meets Business Transformation.", "Navigate the Linguistic Landscape, Discover Opportunities.", "Create Powerful Connections, Boost Business Value.", "Empowering Communication, Enabling Opportunities.", "Advanced NLP for Groundbreaking Business Solutions.", "Innovation in Interaction, Revolution in Revenue.", "Maximize Impact with Intelligent Conversations.", "Beyond Text Generation - Unleashing Business Opportunities.", "Unlock the Power of AI in Your Business Conversations.", "Crafting Dialogues that Drive Business Success.", "Engineered for Excellence, Built for Business."],
-        ADJECTIVES = ["admiring", "adoring", "agitated", "amazing", "angry", "awesome", "backstabbing", "berserk", "big", "boring", "clever", "cocky", "compassionate", "condescending", "cranky", "desperate", "determined", "distracted", "dreamy", "drunk", "ecstatic", "elated", "elegant", "evil", "fervent", "focused", "furious", "gigantic", "gloomy", "goofy", "grave", "happy", "high", "hopeful", "hungry", "insane", "jolly", "jovial", "kickass", "lonely", "loving", "mad", "modest", "naughty", "nauseous", "nostalgic", "pedantic", "pensive", "prickly", "reverent", "romantic", "sad", "serene", "sharp", "sick", "silly", "sleepy", "small", "stoic", "stupefied", "suspicious", "tender", "thirsty", "tiny", "trusting", "bubbly", "charming", "cheerful", "comical", "dazzling", "delighted", "dynamic", "effervescent", "enthusiastic", "exuberant", "fluffy", "friendly", "funky", "giddy", "giggly", "gleeful", "goofy", "graceful", "grinning", "hilarious", "inquisitive", "joyous", "jubilant", "lively", "mirthful", "mischievous", "optimistic", "peppy", "perky", "playful", "quirky", "radiant", "sassy", "silly", "spirited", "sprightly", "twinkly", "upbeat", "vibrant", "witty", "zany", "zealous"],
-        NOUNS = ["albattani", "allen", "almeida", "archimedes", "ardinghelli", "aryabhata", "austin", "babbage", "banach", "bardeen", "bartik", "bassi", "bell", "bhabha", "bhaskara", "blackwell", "bohr", "booth", "borg", "bose", "boyd", "brahmagupta", "brattain", "brown", "carson", "chandrasekhar", "colden", "cori", "cray", "curie", "darwin", "davinci", "dijkstra", "dubinsky", "easley", "einstein", "elion", "engelbart", "euclid", "euler", "fermat", "fermi", "feynman", "franklin", "galileo", "gates", "goldberg", "goldstine", "goldwasser", "golick", "goodall", "hamilton", "hawking", "heisenberg", "heyrovsky", "hodgkin", "hoover", "hopper", "hugle", "hypatia", "jang", "jennings", "jepsen", "joliot", "jones", "kalam", "kare", "keller", "khorana", "kilby", "kirch", "knuth", "kowalevski", "lalande", "lamarr", "leakey", "leavitt", "lichterman", "liskov", "lovelace", "lumiere", "mahavira", "mayer", "mccarthy", "mcclintock", "mclean", "mcnulty", "meitner", "meninsky", "mestorf", "minsky", "mirzakhani", "morse", "murdock", "newton", "nobel", "noether", "northcutt", "noyce", "panini", "pare", "pasteur", "payne", "perlman", "pike", "poincare", "poitras", "ptolemy", "raman", "ramanujan", "ride", "ritchie", "roentgen", "rosalind", "saha", "sammet", "shaw", "shirley", "shockley", "sinoussi", "snyder", "spence", "stallman", "stonebraker", "swanson", "swartz", "swirles", "tesla", "thompson", "torvalds", "turing", "varahamihira", "visvesvaraya", "volhard", "wescoff", "williams", "wilson", "wing", "wozniak", "wright", "yalow", "yonath", "coulomb", "degrasse", "dewey", "edison", "eratosthenes", "faraday", "galton", "gauss", "herschel", "hubble", "joule", "kaku", "kepler", "khayyam", "lavoisier", "maxwell", "mendel", "mendeleev", "ohm", "pascal", "planck", "riemann", "schrodinger", "sagan", "tesla", "tyson", "volta", "watt", "weber", "wien", "zoBell", "zuse", "carroll"];
-
-    function classNames(...j) {
-        return j.filter(Boolean).join(" ")
-    }
-
-    function cn(...j) {
-        return twMerge(clsx$2(j))
-    }
-
-    function toTitleCase(j) {
-        return j ? j.split("_").map((at, st) => checkUpperWords(st === 0 ? at[0].toUpperCase() + at.slice(1).toLowerCase() : at.toLowerCase())).join(" ").split("-").map((at, st) => checkUpperWords(st === 0 ? at[0].toUpperCase() + at.slice(1).toLowerCase() : at.toLowerCase())).join(" ") : ""
-    }
-    const upperCaseWords = ["llm", "uri"];
-
-    function checkUpperWords(j) {
-        return j.split(" ").map(at => upperCaseWords.includes(at.toLowerCase()) ? at.toUpperCase() : at[0].toUpperCase() + at.slice(1).toLowerCase()).join(" ")
-    }
-    const isWrappedWithClass$1 = (j, $) => j.target.closest(`.${$}`);
-
-    function groupByFamily(j, $, at, st) {
-        var ht;
-        const ct = new Set($.split(`
-`));
-        let ut = [],
-            dt = [],
-            ft = new Map;
-        const pt = new Set(["str", "bool", "float", "code", "prompt", "file", "int"]),
-            Tt = mt => mt.type && mt.show && (!pt.has(mt.type) && ct.has(mt.type) || mt.input_types && mt.input_types.some(Qt => ct.has(Qt)));
-        if (st)
-            for (const mt of st) {
-                if (mt.data.node.flow) break;
-                const Qt = mt.data,
-                    vt = ft.get(Qt.type);
-                ft.set(Qt.type, {
-                    hasBaseClassInTemplate: (vt == null ? void 0 : vt.hasBaseClassInTemplate) || Object.values(Qt.node.template).some(Tt),
-                    hasBaseClassInBaseClasses: (vt == null ? void 0 : vt.hasBaseClassInBaseClasses) || Qt.node.base_classes.some(xt => ct.has(xt)),
-                    displayName: (ht = Qt.node) == null ? void 0 : ht.display_name
-                })
-            }
-        for (const [mt, Qt] of Object.entries(j)) {
-            let vt = [],
-                xt = [];
-            for (const [Et, bt] of Object.entries(Qt)) {
-                let wt = ft.get(Et);
-                wt || (wt = {
-                    hasBaseClassInTemplate: Object.values(bt.template).some(Tt),
-                    hasBaseClassInBaseClasses: bt.base_classes.some(At => ct.has(At)),
-                    displayName: bt == null ? void 0 : bt.display_name
-                }), wt.hasBaseClassInTemplate && vt.push({
-                    node: Et,
-                    displayName: wt.displayName
-                }), wt.hasBaseClassInBaseClasses && xt.push({
-                    node: Et,
-                    displayName: wt.displayName
-                })
-            }
-            const yt = Object.keys(Qt).length;
-            vt.length && ut.push({
-                category: mt,
-                nodes: vt,
-                full: vt.length === yt
-            }), xt.length && dt.push({
-                category: mt,
-                nodes: xt,
-                full: xt.length === yt
-            })
-        }
-        return at ? dt.map(mt => ({
-            family: mt.category,
-            type: mt.full ? "" : mt.nodes.map(Qt => Qt.node).join(", "),
-            display_name: ""
-        })) : ut.map(mt => ({
-            family: mt.category,
-            type: mt.full ? "" : mt.nodes.map(Qt => Qt.node).join(", "),
-            display_name: mt.nodes.map(Qt => Qt.displayName).join(", ")
-        }))
-    }
-
-    function buildInputs(j) {
-        return j && j.input_keys && Object.keys(j.input_keys).length > 0 ? JSON.stringify(j.input_keys) : '{"input": "message"}'
-    }
-
-    function getRandomElement(j) {
-        return j[Math.floor(Math.random() * j.length)]
-    }
-
-    function getRandomDescription() {
-        return getRandomElement(DESCRIPTIONS)
-    }
-
-    function getRandomName(j = 0, $ = !1, at = 3) {
-        const st = ADJECTIVES,
-            ct = NOUNS,
-            ut = getRandomElement(st),
-            dt = getRandomElement(ct);
-        if (ut === "boring" && dt === "wozniak") {
-            if (j < at) return getRandomName(j + 1, $, at);
-            console.warn("Max retries reached, returning as is")
-        }
-        if (j > 0 && $) {
-            const pt = Math.floor(Math.random() * 10);
-            return `${ut}_${dt}${pt}`
-        }
-        let ft = $ ? `${ut}_${dt}` : `${ut} ${dt}`;
-        return toTitleCase(ft)
-    }
-
-    function varHighlightHTML({
-        name: j
-    }) {
-        return `<span class="font-semibold chat-message-highlight">{${j}}</span>`
-    }
-
-    function buildTweakObject(j) {
-        return j.forEach(at => {
-            Object.keys(at).forEach(st => {
-                for (let ct in at[st]) try {
-                    at[st][ct] = JSON.parse(at[st][ct])
-                } catch {}
-            })
-        }), JSON.stringify(j.at(-1), null, 2)
-    }
-
-    function getChatInputField(j, $) {
-        let at = "text";
-        return $ && $.input_keys && (at = Object.keys($.input_keys)[0]), at
-    }
-
-    function getPythonApiCode(j, $, at, st) {
-        const ct = j.id,
-            ut = buildTweaks(j),
-            dt = buildInputs(st);
-        return `import requests
-from typing import Optional
-
-BASE_API_URL = "${window.location.protocol}//${window.location.host}/api/v1/process"
-FLOW_ID = "${ct}"
-# You can tweak the flow by adding a tweaks dictionary
-# e.g {"OpenAI-XXXXX": {"model_name": "gpt-4"}}
-TWEAKS = ${at&&at.length>0?buildTweakObject(at):JSON.stringify(ut,null,2)}
-
-def run_flow(inputs: dict, flow_id: str, tweaks: Optional[dict] = None${$?"":", api_key: Optional[str] = None"}) -> dict:
-    """
-    Run a flow with a given message and optional tweaks.
-
-    :param message: The message to send to the flow
-    :param flow_id: The ID of the flow to run
-    :param tweaks: Optional tweaks to customize the flow
-    :return: The JSON response from the flow
-    """
-    api_url = f"{BASE_API_URL}/{flow_id}"
-
-    payload = {"inputs": inputs}
-    headers = None
-    if tweaks:
-        payload["tweaks"] = tweaks
-    if api_key:
-        headers = {"x-api-key": api_key}
-    response = requests.post(api_url, json=payload, headers=headers)
-    return response.json()
-
-# Setup any tweaks you want to apply to the flow
-inputs = ${dt}
-${$?"":'api_key = "<your api key>"'}
-print(run_flow(inputs, flow_id=FLOW_ID, tweaks=TWEAKS${$?"":", api_key=api_key"}))`
-    }
-
-    function getCurlCode(j, $, at, st) {
-        const ct = j.id,
-            ut = buildTweaks(j),
-            dt = buildInputs(st);
-        return `curl -X POST \\
-  ${window.location.protocol}//${window.location.host}/api/v1/process/${ct} \\
-  -H 'Content-Type: application/json'\\${$?"":`
-  -H 'x-api-key: <your api key>'\\`}
-  -d '{"inputs": ${dt}, "tweaks": ${at&&at.length>0?buildTweakObject(at):JSON.stringify(ut,null,2)}}'`
-    }
-
-    function getPythonCode(j, $, at) {
-        const st = j.name,
-            ct = buildTweaks(j),
-            ut = buildInputs(at);
-        return `from langflow import load_flow_from_json
-TWEAKS = ${$&&$.length>0?buildTweakObject($):JSON.stringify(ct,null,2)}
-flow = load_flow_from_json("${st}.json", tweaks=TWEAKS)
-# Now you can use it like any chain
-inputs = ${ut}
-flow(inputs)`
-    }
-
-    function getWidgetCode(j, $, at) {
-        const st = j.id,
-            ct = j.name,
-            ut = buildInputs(at);
-        let dt = getChatInputField(j, at);
-        return `<script src="https://cdn.jsdelivr.net/gh/logspace-ai/langflow-embedded-chat@main/dist/build/static/js/bundle.min.js"><\/script>
-
-<!-- chat_inputs: Stringified JSON with all the input keys and its values. The value of the key that is defined
-as chat_input_field will be overwritten by the chat message.
-chat_input_field: Input key that you want the chat to send the user message with. -->
-<langflow-chat
-  window_title="${ct}"
-  flow_id="${st}"
-  ${at?`chat_inputs='${ut}'
-  chat_input_field="${dt}"
-  `:""}host_url="http://localhost:7860"${$?"":`
-  api_key="..."`}
-
-></langflow-chat>`
-    }
-
-    function tabsArray(j, $) {
-        if ($) return $ === 0 ? [{
-            name: "cURL",
-            mode: "bash",
-            image: "https://curl.se/logo/curl-symbol-transparent.png",
-            language: "sh",
-            code: j[0]
-        }, {
-            name: "Python API",
-            mode: "python",
-            image: "https://images.squarespace-cdn.com/content/v1/5df3d8c5d2be5962e4f87890/1628015119369-OY4TV3XJJ53ECO0W2OLQ/Python+API+Training+Logo.png?format=1000w",
-            language: "py",
-            code: j[1]
-        }, {
-            name: "Python Code",
-            mode: "python",
-            image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
-            language: "py",
-            code: j[2]
-        }, {
-            name: "Chat Widget HTML",
-            description: "Insert this code anywhere in your &lt;body&gt; tag. To use with react and other libs, check our <a class='link-color' href='https://langflow.org/guidelines/widget'>documentation</a>.",
-            mode: "html",
-            image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
-            language: "py",
-            code: j[3]
-        }] : [{
-            name: "cURL",
-            mode: "bash",
-            image: "https://curl.se/logo/curl-symbol-transparent.png",
-            language: "sh",
-            code: j[0]
-        }, {
-            name: "Python API",
-            mode: "python",
-            image: "https://images.squarespace-cdn.com/content/v1/5df3d8c5d2be5962e4f87890/1628015119369-OY4TV3XJJ53ECO0W2OLQ/Python+API+Training+Logo.png?format=1000w",
-            language: "py",
-            code: j[1]
-        }, {
-            name: "Python Code",
-            mode: "python",
-            language: "py",
-            image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
-            code: j[2]
-        }, {
-            name: "Chat Widget HTML",
-            description: "Insert this code anywhere in your &lt;body&gt; tag. To use with react and other libs, check our <a class='link-color' href='https://langflow.org/guidelines/widget'>documentation</a>.",
-            mode: "html",
-            image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
-            language: "py",
-            code: j[3]
-        }, {
-            name: "Tweaks",
-            mode: "python",
-            image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
-            language: "py",
-            code: j[4]
-        }]
-    }
-
-    function removeCountFromString(j) {
-        const $ = /\s*\(\w+\)\s*$/;
-        return j.replace($, "").trim()
-    }
-
-    function createRandomKey(j, $) {
-        return removeCountFromString(j) + ` (${$})`
-    }
-
-    function sensitiveSort(j, $) {
-        const at = /(.+) \((\w+)\)/,
-            st = j.match(at),
-            ct = $.match(at);
-        if (st && ct) {
-            const ut = st[1],
-                dt = ct[1];
-            if (ut !== dt) return ut.localeCompare(dt);
-            const ft = parseInt(st[2]),
-                pt = parseInt(ct[2]);
-            return ft - pt
-        } else return j.localeCompare($)
-    }
-
-    function getFieldTitle(j, $) {
-        return j[$].display_name ? j[$].display_name : j[$].name ? toTitleCase(j[$].name) : toTitleCase($)
-    }
-    const uid = new ShortUniqueId({
-        length: 5
-    });
-
-    function cleanEdges(j, $) {
-        let at = lodashExports.cloneDeep($);
-        return $.forEach(st => {
-            var pt, Tt, ht, mt;
-            const ct = j.find(Qt => Qt.id === st.source),
-                ut = j.find(Qt => Qt.id === st.target);
-            if (!ct || !ut) {
-                at = at.filter(Qt => Qt.id !== st.id);
-                return
-            }
-            const dt = st.sourceHandle,
-                ft = st.targetHandle;
-            if (ft) {
-                const vt = scapeJSONParse(ft).fieldName,
-                    xt = {
-                        type: (pt = ut.data.node.template[vt]) == null ? void 0 : pt.type,
-                        fieldName: vt,
-                        id: ut.data.id,
-                        inputTypes: (Tt = ut.data.node.template[vt]) == null ? void 0 : Tt.input_types
-                    };
-                (ht = ut.data.node.template[vt]) != null && ht.proxy && (xt.proxy = (mt = ut.data.node.template[vt]) == null ? void 0 : mt.proxy), scapedJSONStringfy(xt) !== ft && (at = at.filter(yt => yt.id !== st.id))
-            }
-            if (dt) {
-                const Qt = {
-                    id: ct.data.id,
-                    baseClasses: ct.data.node.base_classes,
-                    dataType: ct.data.type
-                };
-                scapedJSONStringfy(Qt) !== dt && (at = at.filter(vt => vt.id !== st.id))
-            }
-        }), at
-    }
-
-    function isValidConnection({
-        source: j,
-        target: $,
-        sourceHandle: at,
-        targetHandle: st
-    }, ct, ut) {
-        var pt, Tt, ht;
-        const dt = scapeJSONParse(st),
-            ft = scapeJSONParse(at);
-        if ((pt = dt.inputTypes) != null && pt.some(mt => mt === ft.dataType) || ft.baseClasses.some(mt => {
-                var Qt;
-                return ((Qt = dt.inputTypes) == null ? void 0 : Qt.some(vt => vt === mt)) || mt === dt.type
-            })) {
-            let mt = (ht = (Tt = ct.find(Qt => Qt.id === $)) == null ? void 0 : Tt.data) == null ? void 0 : ht.node;
-            if (mt) {
-                if (!mt.template[dt.fieldName].list && !ut.find(Qt => Qt.targetHandle === st) || mt.template[dt.fieldName].list) return !0
-            } else if (!ut.find(Qt => Qt.targetHandle === st)) return !0
-        }
-        return !1
-    }
-
-    function removeApiKeys(j) {
-        let $ = lodashExports.cloneDeep(j);
-        return $.data.nodes.forEach(at => {
-            for (const st in at.data.node.template) at.data.node.template[st].password && (at.data.node.template[st].value = "")
-        }), $
-    }
-    const processFlows = (j, $ = !0) => {
-            let at = {};
-            return j.forEach(st => {
-                try {
-                    if (!st.data) return;
-                    if (st.data && st.is_component) {
-                        st.data.nodes[0].data.node.display_name = st.name, at[createRandomKey(st.data.nodes[0].data.type, uid())] = lodashExports.cloneDeep(st.data.nodes[0].data.node);
-                        return
-                    }
-                    $ || processDataFromFlow(st, !1)
-                } catch (ct) {
-                    console.log(ct)
-                }
-            }), {
-                data: at,
-                flows: j
-            }
-        },
-        processDataFromFlow = (j, $ = !0) => {
-            let at = j != null && j.data ? j.data : null;
-            return at && (processFlowEdges(j), updateEdges(at.edges), $ && updateIds(at)), at
-        };
-
-    function updateIds(j) {
-        let $ = {};
-        return j.nodes && j.nodes.forEach(at => {
-            var ct;
-            let st = getNodeId((ct = at.data.node) != null && ct.flow ? "GroupNode" : at.data.type);
-            $[at.id] = st, at.id = st, at.data.id = st
-        }), j.edges && j.edges.forEach(at => {
-            var ut, dt, ft, pt;
-            at.source = $[at.source], at.target = $[at.target];
-            const st = scapeJSONParse(at.sourceHandle);
-            at.sourceHandle = scapedJSONStringfy({
-                ...st,
-                id: at.source
-            }), (dt = (ut = at.data) == null ? void 0 : ut.sourceHandle) != null && dt.id && (at.data.sourceHandle.id = at.source);
-            const ct = scapeJSONParse(at.targetHandle);
-            at.targetHandle = scapedJSONStringfy({
-                ...ct,
-                id: at.target
-            }), (pt = (ft = at.data) == null ? void 0 : ft.targetHandle) != null && pt.id && (at.data.targetHandle.id = at.target), at.id = "reactflow__edge-" + at.source + at.sourceHandle + "-" + at.target + at.targetHandle
-        }), $
-    }
-
-    function buildTweaks(j) {
-        return j.data.nodes.reduce(($, at) => ($[at.data.id] = {}, $), {})
-    }
-
-    function validateNode(j, $) {
-        var ct, ut;
-        if (!((ut = (ct = j.data) == null ? void 0 : ct.node) != null && ut.template) || !Object.keys(j.data.node.template)) return ["We've noticed a potential issue with a node in the flow. Please review it and, if necessary, submit a bug report with your exported flow file. Thank you for your help!"];
-        const {
-            type: at,
-            node: {
-                template: st
-            }
-        } = j.data;
-        return Object.keys(st).reduce((dt, ft) => (st[ft].required && st[ft].show && (st[ft].value === void 0 || st[ft].value === null || st[ft].value === "") && !$.some(pt => scapeJSONParse(pt.targetHandle).fieldName === ft && scapeJSONParse(pt.targetHandle).id === j.id) ? dt.push(`${at} is missing ${getFieldTitle(st,ft)}.`) : st[ft].type === "dict" && st[ft].required && st[ft].show && (st[ft].value !== void 0 || st[ft].value !== null || st[ft].value !== "") && (hasDuplicateKeys(st[ft].value) && dt.push(`${at} (${getFieldTitle(st,ft)}) contains duplicate keys with the same values.`), hasEmptyKey(st[ft].value) && dt.push(`${at} (${getFieldTitle(st,ft)}) field must not be empty.`)), dt), [])
-    }
-
-    function validateNodes(j, $) {
-        return j.length === 0 ? ["No nodes found in the flow. Please add at least one node to the flow."] : j.flatMap(at => validateNode(at, $))
-    }
-
-    function updateEdges(j) {
-        j && j.forEach($ => {
-            const at = scapeJSONParse($.targetHandle);
-            $.className = (at.type === "Text" ? "stroke-gray-800 " : "stroke-gray-900 ") + " stroke-connection", $.animated = at.type === "Text"
-        })
-    }
-
-    function addVersionToDuplicates(j, $) {
-        const at = $.map(ut => ut.name);
-        let st = j.name,
-            ct = 1;
-        for (; at.includes(st);) st = `${j.name} (${ct})`, ct++;
-        return st
-    }
-
-    function updateEdgesHandleIds({
-        edges: j,
-        nodes: $
-    }) {
-        let at = lodashExports.cloneDeep(j);
-        return at.forEach(st => {
-            const ct = st.source,
-                ut = st.target,
-                dt = $.find(vt => vt.id === ct),
-                ft = $.find(vt => vt.id === ut);
-            let pt = st.sourceHandle,
-                Tt = st.targetHandle,
-                ht, mt;
-            if (Tt && ft) {
-                let vt = Tt.split("|")[1];
-                mt = {
-                    type: ft.data.node.template[vt].type,
-                    fieldName: vt,
-                    id: ft.data.id,
-                    inputTypes: ft.data.node.template[vt].input_types
-                }
-            }
-            pt && dt && (ht = {
-                id: dt.data.id,
-                baseClasses: dt.data.node.base_classes,
-                dataType: dt.data.type
-            }), st.sourceHandle = scapedJSONStringfy(ht), st.targetHandle = scapedJSONStringfy(mt);
-            const Qt = {
-                sourceHandle: scapeJSONParse(st.sourceHandle),
-                targetHandle: scapeJSONParse(st.targetHandle)
-            };
-            st.data = Qt
-        }), at
-    }
-
-    function handleKeyDown$1(j, $, at) {
-        (typeof $ == "string" && (j.metaKey === !0 || j.ctrlKey === !0) && j.key === "Backspace" && ($ === at || ($ == null ? void 0 : $.charAt(($ == null ? void 0 : $.length) - 1)) === " " || specialCharsRegex.test($ == null ? void 0 : $.charAt(($ == null ? void 0 : $.length) - 1))) || navigator.userAgent.toUpperCase().includes("MAC") && j.ctrlKey === !0 && j.key === "Backspace") && (j.preventDefault(), j.stopPropagation()), j.ctrlKey === !0 && j.key === "Backspace" && $ === at && (j.preventDefault(), j.stopPropagation())
-    }
-
-    function handleOnlyIntegerInput(j) {
-        (j.key === "." || j.key === "-" || j.key === "," || j.key === "e" || j.key === "E" || j.key === "+") && j.preventDefault()
-    }
-
-    function convertObjToArray(j) {
-        if (typeof j == "string" && (j = JSON.parse(j)), Array.isArray(j)) return j;
-        let $ = [];
-        if (typeof j == "object") {
-            for (const at in j)
-                if (Object.prototype.hasOwnProperty.call(j, at)) {
-                    const st = {};
-                    st[at] = j[at], $.push(st)
-                }
-        }
-        return $
-    }
-
-    function convertArrayToObj(j) {
-        if (!Array.isArray(j)) return j;
-        let $ = {};
-        for (const at of j)
-            for (const st in at) at.hasOwnProperty(st) && ($[st] = at[st]);
-        return $
-    }
-
-    function hasDuplicateKeys(j) {
-        const $ = {};
-        Array.isArray(j) || (j = [{
-            "": ""
-        }]);
-        for (const at of j)
-            for (const st in at) {
-                if ($[st]) return !0;
-                $[st] = !0
-            }
-        return !1
-    }
-
-    function hasEmptyKey(j) {
-        Array.isArray(j) || (j = []);
-        for (const $ of j)
-            for (const at in $)
-                if ($.hasOwnProperty(at) && at === "") return !0;
-        return !1
-    }
-
-    function convertValuesToNumbers(j) {
-        return j.map($ => {
-            const at = {};
-            for (const st in $)
-                if ($.hasOwnProperty(st)) {
-                    let ct = $[st];
-                    /^\d+$/.test(ct) && (ct = ct == null ? void 0 : ct.toString().trim()), at[st] = ct === "" || isNaN(ct) ? ct.toString() : Number(ct)
-                } return at
-        })
-    }
-
-    function scapedJSONStringfy(j) {
-        return customStringify(j).replace(/"/g, "œ")
-    }
-
-    function scapeJSONParse(j) {
-        let $ = j.replace(/œ/g, '"');
-        return JSON.parse($)
-    }
-
-    function checkOldEdgesHandles(j) {
-        return j.some($ => !$.sourceHandle || !$.targetHandle || !$.sourceHandle.includes("{") || !$.targetHandle.includes("{"))
-    }
-
-    function customStringify(j) {
-        return typeof j > "u" ? "null" : j === null || typeof j != "object" ? j instanceof Date ? `"${j.toISOString()}"` : JSON.stringify(j) : Array.isArray(j) ? `[${j.map(ct=>customStringify(ct)).join(",")}]` : `{${Object.keys(j).sort().map(st=>`"${st}":${customStringify(j[st])}`).join(",")}}`
-    }
-
-    function getMiddlePoint(j) {
-        let $ = 0,
-            at = 0;
-        j.forEach(dt => {
-            $ += dt.position.x, at += dt.position.y
-        });
-        const st = j.length,
-            ct = $ / st,
-            ut = at / st;
-        return {
-            x: ct,
-            y: ut
-        }
-    }
-
-    function getNodeId(j) {
-        return j + "-" + uid()
-    }
-
-    function getHandleId(j, $, at, st) {
-        return "reactflow__edge-" + j + $ + "-" + at + st
-    }
-
-    function generateFlow(j, $, at, st) {
-        const ct = {
-                nodes: $,
-                edges: at,
-                viewport: {
-                    zoom: 1,
-                    x: 0,
-                    y: 0
-                }
-            },
-            ut = new ShortUniqueId({
-                length: 5
-            });
-        return ct.edges = j.edges.filter(ft => j.nodes.some(pt => pt.id === ft.target) && j.nodes.some(pt => pt.id === ft.source)), ct.nodes = j.nodes, {
-            newFlow: {
-                data: ct,
-                is_component: !1,
-                name: st,
-                description: "",
-                id: ut()
-            },
-            removedEdges: at.filter(ft => (j.nodes.some(pt => pt.id === ft.target) || j.nodes.some(pt => pt.id === ft.source)) && ct.edges.every(pt => pt.id !== ft.id))
-        }
-    }
-
-    function reconnectEdges(j, $) {
-        let at = lodashExports.cloneDeep($);
-        if (!j.data.node.flow) return [];
-        const {
-            nodes: st,
-            edges: ct
-        } = j.data.node.flow.data, ut = findLastNode(j.data.node.flow.data);
-        return at.forEach(dt => {
-            if (ut && dt.source === ut.id) {
-                dt.source = j.id;
-                let ft = scapeJSONParse(dt.sourceHandle);
-                ft.id = j.id, dt.sourceHandle = scapedJSONStringfy(ft), dt.data.sourceHandle = ft
-            }
-            if (st.some(ft => ft.id === dt.target)) {
-                const ft = st.find(mt => mt.id === dt.target);
-                console.log("targetNode", ft);
-                const pt = scapeJSONParse(dt.targetHandle);
-                console.log("targetHandle", pt);
-                const Tt = {
-                    id: ft.id,
-                    field: pt.fieldName
-                };
-                let ht = lodashExports.cloneDeep(pt);
-                ht.id = j.id, ht.proxy = Tt, dt.target = j.id, ht.fieldName = pt.fieldName + "_" + ft.id, dt.targetHandle = scapedJSONStringfy(ht), dt.data.targetHandle = ht
-            }
-        }), at
-    }
-
-    function findLastNode({
-        nodes: j,
-        edges: $
-    }) {
-        return j.find(st => !$.some(ct => ct.source === st.id))
-    }
-
-    function updateFlowPosition(j, $) {
-        const at = getMiddlePoint($.data.nodes);
-        let st = {
-            x: j.x - at.x,
-            y: j.y - at.y
-        };
-        return {
-            ...$,
-            data: {
-                ...$.data,
-                nodes: $.data.nodes.map(ct => ({
-                    ...ct,
-                    position: {
-                        x: ct.position.x + st.x,
-                        y: ct.position.y + st.y
-                    }
-                }))
-            }
-        }
-    }
-
-    function validateSelection(j, $) {
-        j.edges.length === 0 && (j.edges = $);
-        let at = new Set(j.nodes.map(ut => ut.id)),
-            st = j.edges.filter(ut => at.has(ut.source) && at.has(ut.target));
-        j.edges = st;
-        let ct = [];
-        return j.nodes.length < 2 && ct.push("Please select more than one node"), j.nodes.filter(ut => !j.edges.some(dt => dt.source === ut.id)).length > 1 && ct.push("Please select only one node with free outputs"), j.nodes.some(ut => !j.edges.some(dt => dt.target === ut.id) && !j.edges.some(dt => dt.source === ut.id)) && ct.push("Please select only nodes that are connected"), ct
-    }
-
-    function updateGroupNodeTemplate(j) {
-        return Object.keys(j).forEach($ => {
-            let at = j[$].type,
-                st = j[$].input_types;
-            LANGFLOW_SUPPORTED_TYPES.has(at) && !j[$].required && !st && (j[$].advanced = !0), at === "code" && (j[$].show = !1)
-        }), j
-    }
-
-    function mergeNodeTemplates({
-        nodes: j,
-        edges: $
-    }) {
-        let at = {};
-        return j.forEach(st => {
-            let ct = lodashExports.cloneDeep(st.data.node.template);
-            Object.keys(ct).filter(ut => ut.charAt(0) !== "_").forEach(ut => {
-                isHandleConnected($, ut, ct[ut], st.id) || (at[ut + "_" + st.id] = ct[ut], at[ut + "_" + st.id].proxy = {
-                    id: st.id,
-                    field: ut
-                }, st.type === "groupNode" ? at[ut + "_" + st.id].display_name = st.data.node.flow.name + " - " + ct[ut].name : at[ut + "_" + st.id].display_name = ct[ut].display_name ? ct[ut].display_name : ct[ut].name ? toTitleCase(ct[ut].name) : toTitleCase(ut))
-            })
-        }), at
-    }
-
-    function isHandleConnected(j, $, at, st) {
-        if (at.proxy) {
-            if (j.some(ct => ct.targetHandle === scapedJSONStringfy({
-                    type: at.type,
-                    fieldName: $,
-                    id: st,
-                    proxy: {
-                        id: at.proxy.id,
-                        field: at.proxy.field
-                    },
-                    inputTypes: at.input_types
-                }))) return !0
-        } else if (j.some(ct => ct.targetHandle === scapedJSONStringfy({
-                type: at.type,
-                fieldName: $,
-                id: st,
-                inputTypes: at.input_types
-            }))) return !0;
-        return !1
-    }
-
-    function generateNodeTemplate(j) {
-        let $ = mergeNodeTemplates({
-            nodes: j.data.nodes,
-            edges: j.data.edges
-        });
-        return updateGroupNodeTemplate($), $
-    }
-
-    function generateNodeFromFlow(j, $) {
-        const {
-            nodes: at
-        } = j.data, st = lodashExports.cloneDeep(findLastNode(j.data)), ct = getMiddlePoint(at);
-        let ut = lodashExports.cloneDeep(j);
-        const dt = $(st == null ? void 0 : st.data.type);
-        return {
-            data: {
-                id: dt,
-                type: st == null ? void 0 : st.data.type,
-                node: {
-                    output_types: st.data.node.output_types,
-                    display_name: "Group",
-                    documentation: "",
-                    base_classes: st.data.node.base_classes,
-                    description: "",
-                    template: generateNodeTemplate(ut),
-                    flow: ut
-                }
-            },
-            id: dt,
-            position: ct,
-            type: "genericNode"
-        }
-    }
-
-    function updateProxyIdsOnTemplate(j, $) {
-        Object.keys(j).forEach(at => {
-            j[at].proxy && $[j[at].proxy.id] && (j[at].proxy.id = $[j[at].proxy.id])
-        })
-    }
-
-    function updateEdgesIds(j, $) {
-        j.forEach(at => {
-            let st = at.data.targetHandle;
-            st.proxy && $[st.proxy.id] && (st.proxy.id = $[st.proxy.id]), at.data.targetHandle = st, at.targetHandle = scapedJSONStringfy(st)
-        })
-    }
-
-    function processFlowEdges(j) {
-        if (!(!j.data || !j.data.edges)) {
-            if (checkOldEdgesHandles(j.data.edges)) {
-                const $ = updateEdgesHandleIds(j.data);
-                j.data.edges = $
-            }
-            j.data.edges.forEach($ => {
-                $.className = "", $.style = {
-                    stroke: "#555"
-                }
-            })
-        }
-    }
-
-    function expandGroupNode(j, $, at, st, ct, ut, dt) {
-        var xt;
-        const ft = updateIds($.data);
-        updateProxyIdsOnTemplate(at, ft);
-        let pt = ct;
-        updateEdgesIds(pt, ft);
-        const Tt = lodashExports.cloneDeep((xt = $ == null ? void 0 : $.data) == null ? void 0 : xt.nodes),
-            ht = lodashExports.cloneDeep($.data.edges);
-        let mt = [];
-        pt.forEach(yt => {
-            var bt, wt, At;
-            let Et = lodashExports.cloneDeep(yt);
-            if (Et.target === j) {
-                const Ct = Et.data.targetHandle;
-                if (Ct.proxy) {
-                    let Mt = Ct.type,
-                        St = Ct.proxy.field,
-                        Rt = Ct.proxy.id,
-                        _t = Ct.inputTypes,
-                        Ot = Tt.find(Dt => Dt.id === Rt);
-                    if (Ot) {
-                        Et.target = Rt;
-                        let Dt = {
-                            fieldName: St,
-                            type: Mt,
-                            id: Rt,
-                            inputTypes: _t
-                        };
-                        (bt = Ot.data.node) != null && bt.flow && (Dt.proxy = {
-                            field: (wt = Ot.data.node.template[St].proxy) == null ? void 0 : wt.field,
-                            id: (At = Ot.data.node.template[St].proxy) == null ? void 0 : At.id
-                        }), Et.data.targetHandle = Dt, Et.targetHandle = scapedJSONStringfy(Dt)
-                    }
-                }
-            }
-            if (Et.source === j) {
-                const Ct = lodashExports.cloneDeep(findLastNode($.data));
-                Et.source = Ct.id;
-                let Mt = scapeJSONParse(Et.sourceHandle);
-                Mt.id = Ct.id, Et.data.sourceHandle = Mt, Et.sourceHandle = scapedJSONStringfy(Mt)
-            }(yt.target === j || yt.source === j) && mt.push(Et)
-        }), Object.keys(at).forEach(yt => {
-            let {
-                field: Et,
-                id: bt
-            } = at[yt].proxy, wt = Tt.findIndex(At => At.id === bt);
-            if (wt !== -1) {
-                let At, Ct, Mt = Tt[wt].data.node.template[Et].show,
-                    St = Tt[wt].data.node.template[Et].advanced;
-                Tt[wt].data.node.template[Et].display_name ? Ct = Tt[wt].data.node.template[Et].display_name : Ct = Tt[wt].data.node.template[Et].name, Tt[wt].data.node.template[Et].proxy && (At = Tt[wt].data.node.template[Et].proxy), Tt[wt].data.node.template[Et] = at[yt], Tt[wt].data.node.template[Et].show = Mt, Tt[wt].data.node.template[Et].advanced = St, Tt[wt].data.node.template[Et].display_name = Ct, At ? Tt[wt].data.node.template[Et].proxy = At : delete Tt[wt].data.node.template[Et].proxy
-            }
-        });
-        const Qt = [...st.filter(yt => yt.id !== j), ...Tt],
-            vt = [...ct.filter(yt => yt.target !== j && yt.source !== j), ...ht, ...mt];
-        ut(Qt), dt(vt)
-    }
-
-    function createFlowComponent(j, $) {
-        var st, ct;
-        return {
-            data: {
-                edges: [],
-                nodes: [{
-                    data: {
-                        ...j,
-                        node: {
-                            ...j.node,
-                            official: !1
-                        }
-                    },
-                    id: j.id,
-                    position: {
-                        x: 0,
-                        y: 0
-                    },
-                    type: "genericNode"
-                }],
-                viewport: {
-                    x: 1,
-                    y: 1,
-                    zoom: 1
-                }
-            },
-            description: ((st = j.node) == null ? void 0 : st.description) || "",
-            name: ((ct = j.node) == null ? void 0 : ct.display_name) || j.type || "",
-            id: j.id || "",
-            is_component: !0,
-            last_tested_version: $
-        }
-    }
-
-    function downloadNode(j) {
-        const $ = document.createElement("a"),
-            at = new Blob([JSON.stringify(j)], {
-                type: "application/json"
-            });
-        $.href = URL.createObjectURL(at), $.download = `${j.name}.json`, $.click()
-    }
-
-    function removeFileNameFromComponents(j) {
-        j.data.nodes.forEach($ => {
-            var at;
-            Object.keys($.data.node.template).forEach(st => {
-                var ct;
-                ((ct = $.data.node) == null ? void 0 : ct.template[st].type) === "file" && ($.data.node.template[st].value = "")
-            }), (at = $.data.node) != null && at.flow && removeFileNameFromComponents($.data.node.flow)
-        })
-    }
-
-    function typesGenerator(j) {
-        return Object.keys(j).reverse().reduce(($, at) => (Object.keys(j[at]).forEach(st => {
-            var ct;
-            $[st] = at, (ct = j[at][st].base_classes) == null || ct.forEach(ut => {
-                $[ut] = at
-            })
-        }), $), {})
-    }
-
-    function templatesGenerator(j) {
-        return Object.keys(j).reduce(($, at) => (Object.keys(j[at]).forEach(st => {
-            j[at][st].flow || ($[st] = j[at][st])
-        }), $), {})
-    }
-
-    function downloadFlow(j, $, at) {
-        let st = lodashExports.cloneDeep(j);
-        removeFileNameFromComponents(st);
-        const ct = `data:text/json;chatset=utf-8,${encodeURIComponent(JSON.stringify({...st,name:$,description:at}))}`,
-            ut = document.createElement("a");
-        ut.href = ct, ut.download = `${$&&$!=""?$:j.name}.json`, ut.click()
-    }
-
-    function downloadFlows() {
-        downloadFlowsFromDatabase().then(j => {
-            const $ = `data:text/json;chatset=utf-8,${encodeURIComponent(JSON.stringify(j))}`,
-                at = document.createElement("a");
-            at.href = $, at.download = "flows.json", at.click()
-        })
-    }
-    const createNewFlow = (j, $) => ({
-            description: ($ == null ? void 0 : $.description) ?? getRandomDescription(),
-            name: $ != null && $.name ? $.name : "Untitled document",
-            data: j,
-            id: "",
-            is_component: ($ == null ? void 0 : $.is_component) ?? !1
-        }),
         useDarkStore = create$9(j => ({
             dark: JSON.parse(window.localStorage.getItem("isDark")) ?? !1,
             stars: 0,
             version: "",
             setDark: $ => j(() => ({
                 dark: $
             })),
@@ -28300,15 +27031,15 @@
         },
         viewChanged = (j, $) => j.x !== $.x || j.y !== $.y || j.zoom !== $.k,
         eventToFlowTransform = j => ({
             x: j.x,
             y: j.y,
             zoom: j.k
         }),
-        isWrappedWithClass = (j, $) => j.target.closest(`.${$}`),
+        isWrappedWithClass$1 = (j, $) => j.target.closest(`.${$}`),
         isRightClickPan = (j, $) => $ === 2 && Array.isArray(j) && j.includes(2),
         wheelDelta = j => {
             const $ = j.ctrlKey && isMacOs() ? 10 : 1;
             return -j.deltaY * (j.deltaMode === 1 ? .05 : j.deltaMode ? 1 : .002) * $
         },
         selector$a = j => ({
             d3Zoom: j.d3Zoom,
@@ -28376,15 +27107,15 @@
                         d3ZoomHandler: Yt.on("wheel.zoom"),
                         transform: [Jt.x, Jt.y, Jt.k],
                         domNode: Ot.current.closest(".react-flow")
                     })
                 }
             }, []), reactExports.useEffect(() => {
                 $t && Ht && (dt && !Bt && !jt ? $t.on("wheel.zoom", qt => {
-                    if (isWrappedWithClass(qt, At)) return !1;
+                    if (isWrappedWithClass$1(qt, At)) return !1;
                     qt.preventDefault(), qt.stopImmediatePropagation();
                     const Ut = $t.property("__zoom").k || 1,
                         Yt = isMacOs();
                     if (qt.ctrlKey && ut && Yt) {
                         const ur = pointer(qt),
                             dr = wheelDelta(qt),
                             Tr = Ut * Math.pow(2, dr);
@@ -28405,15 +27136,15 @@
                         } = St.getState();
                     clearTimeout(Wt.current), zt.current || (zt.current = !0, $ == null || $(qt, rr), nr == null || nr(rr)), zt.current && (j == null || j(qt, rr), er == null || er(rr), Wt.current = setTimeout(() => {
                         at == null || at(qt, rr), ar == null || ar(rr), zt.current = !1
                     }, 150))
                 }, {
                     passive: !1
                 }) : typeof Pt < "u" && $t.on("wheel.zoom", function(qt, Ut) {
-                    if (!bt || isWrappedWithClass(qt, At)) return null;
+                    if (!bt || isWrappedWithClass$1(qt, At)) return null;
                     qt.preventDefault(), Pt.call(this, qt, Ut)
                 }, {
                     passive: !1
                 }))
             }, [jt, dt, pt, $t, Ht, Pt, Bt, ut, bt, At, $, j, at]), reactExports.useEffect(() => {
                 Ht && Ht.on("start", qt => {
                     var Xt, Zt;
@@ -28454,16 +27185,16 @@
                         }, dt ? 150 : 0)
                     }
                 })
             }, [Ht, dt, mt, at, st]), reactExports.useEffect(() => {
                 Ht && Ht.filter(qt => {
                     const Ut = Bt || ct,
                         Yt = ut && qt.ctrlKey;
-                    if ((mt === !0 || Array.isArray(mt) && mt.includes(1)) && qt.button === 1 && qt.type === "mousedown" && (isWrappedWithClass(qt, "react-flow__node") || isWrappedWithClass(qt, "react-flow__edge"))) return !0;
-                    if (!mt && !Ut && !dt && !Tt && !ut || jt || !Tt && qt.type === "dblclick" || isWrappedWithClass(qt, At) && qt.type === "wheel" || isWrappedWithClass(qt, Ct) && (qt.type !== "wheel" || dt && qt.type === "wheel" && !Bt) || !ut && qt.ctrlKey && qt.type === "wheel" || !Ut && !dt && !Yt && qt.type === "wheel" || !mt && (qt.type === "mousedown" || qt.type === "touchstart") || Array.isArray(mt) && !mt.includes(qt.button) && (qt.type === "mousedown" || qt.type === "touchstart")) return !1;
+                    if ((mt === !0 || Array.isArray(mt) && mt.includes(1)) && qt.button === 1 && qt.type === "mousedown" && (isWrappedWithClass$1(qt, "react-flow__node") || isWrappedWithClass$1(qt, "react-flow__edge"))) return !0;
+                    if (!mt && !Ut && !dt && !Tt && !ut || jt || !Tt && qt.type === "dblclick" || isWrappedWithClass$1(qt, At) && qt.type === "wheel" || isWrappedWithClass$1(qt, Ct) && (qt.type !== "wheel" || dt && qt.type === "wheel" && !Bt) || !ut && qt.ctrlKey && qt.type === "wheel" || !Ut && !dt && !Yt && qt.type === "wheel" || !mt && (qt.type === "mousedown" || qt.type === "touchstart") || Array.isArray(mt) && !mt.includes(qt.button) && (qt.type === "mousedown" || qt.type === "touchstart")) return !1;
                     const Xt = Array.isArray(mt) && mt.includes(qt.button) || !qt.button || qt.button <= 1;
                     return (!qt.ctrlKey || qt.type === "wheel") && Xt
                 })
             }, [jt, Ht, ct, ut, dt, Tt, mt, ht, Bt]), $3DjNB$react.createElement("div", {
                 className: "react-flow__renderer",
                 ref: Ot,
                 style: containerStyle
@@ -31993,14 +30724,1522 @@
                 setApiKey: yt,
                 apiKey: xt,
                 storeApiKey: At
             },
             children: j
         })
     }
+    const api = axios$1.create({
+        baseURL: ""
+    });
+
+    function ApiInterceptor() {
+        const j = useAlertStore(ft => ft.setErrorData);
+        let {
+            accessToken: $,
+            login: at,
+            logout: st,
+            authenticationErrorCount: ct,
+            autoLogin: ut
+        } = reactExports.useContext(AuthContext);
+        useNavigate();
+        const dt = new Cookies$1;
+        return reactExports.useEffect(() => {
+            const ft = api.interceptors.response.use(ht => ht, async ht => {
+                    var mt, Qt, vt, xt, yt, Et, bt, wt;
+                    if (((mt = ht.response) == null ? void 0 : mt.status) === 401) {
+                        const At = dt.get("access_token_lf");
+                        if (At && !ut) {
+                            ct = ct + 1, ct > 3 && (ct = 0, st());
+                            try {
+                                const Ct = await renewAccessToken();
+                                if ((Qt = Ct == null ? void 0 : Ct.data) != null && Qt.access_token && ((vt = Ct == null ? void 0 : Ct.data) != null && vt.refresh_token) && at((xt = Ct == null ? void 0 : Ct.data) == null ? void 0 : xt.access_token), (yt = ht == null ? void 0 : ht.config) != null && yt.headers) return delete ht.config.headers.Authorization, ht.config.headers.Authorization = `Bearer ${dt.get("access_token_lf")}`, await axios$1.request(ht.config)
+                            } catch (Ct) {
+                                axios$1.isAxiosError(Ct) && ((Et = Ct.response) == null ? void 0 : Et.status) === 401 || console.error(Ct), st()
+                            }
+                        }
+                        if (!At && ((wt = (bt = ht == null ? void 0 : ht.config) == null ? void 0 : bt.url) != null && wt.includes("login"))) return Promise.reject(ht);
+                        st()
+                    } else return Promise.reject(ht)
+                }),
+                pt = ht => {
+                    const mt = ["https://raw.githubusercontent.com/logspace-ai/langflow_examples/main/examples", "https://api.github.com/repos/logspace-ai/langflow_examples/contents/examples", "https://api.github.com/repos/logspace-ai/langflow", "auto_login"],
+                        Qt = ["auto_login"];
+                    try {
+                        const vt = new URL(ht),
+                            xt = mt.some(Et => vt.origin === new URL(Et).origin),
+                            yt = Qt.some(Et => vt.pathname.includes(Et));
+                        return xt || yt
+                    } catch {
+                        return !1
+                    }
+                },
+                Tt = api.interceptors.request.use(ht => {
+                    const mt = dt.get("access_token_lf");
+                    return mt && !pt(ht == null ? void 0 : ht.url) && (ht.headers.Authorization = `Bearer ${mt}`), ht
+                }, ht => Promise.reject(ht));
+            return () => {
+                api.interceptors.response.eject(ft), api.interceptors.request.eject(Tt)
+            }
+        }, [$, j]), null
+    }
+    async function getAll() {
+        return await api.get(`${BASE_URL_API}all`)
+    }
+    const GITHUB_API_URL = "https://api.github.com";
+    async function getRepoStars(j, $) {
+        try {
+            return (await api.get(`${GITHUB_API_URL}/repos/${j}/${$}`)).data.stargazers_count
+        } catch (at) {
+            return console.error("Error fetching repository data:", at), null
+        }
+    }
+    async function postValidateCode(j) {
+        return await api.post(`${BASE_URL_API}validate/code`, {
+            code: j
+        })
+    }
+    async function postValidatePrompt(j, $, at) {
+        return api.post(`${BASE_URL_API}validate/prompt`, {
+            name: j,
+            template: $,
+            frontend_node: at
+        })
+    }
+    async function saveFlowToDatabase(j) {
+        try {
+            const $ = await api.post(`${BASE_URL_API}flows/`, {
+                name: j.name,
+                data: j.data,
+                description: j.description,
+                is_component: j.is_component
+            });
+            if ($.status !== 201) throw new Error(`HTTP error! status: ${$.status}`);
+            return $.data
+        } catch ($) {
+            throw console.error($), $
+        }
+    }
+    async function updateFlowInDatabase(j) {
+        try {
+            const $ = await api.patch(`${BASE_URL_API}flows/${j.id}`, {
+                name: j.name,
+                data: j.data,
+                description: j.description
+            });
+            if (($ == null ? void 0 : $.status) !== 200) throw new Error(`HTTP error! status: ${$==null?void 0:$.status}`);
+            return $.data
+        } catch ($) {
+            throw console.error($), $
+        }
+    }
+    async function readFlowsFromDatabase() {
+        try {
+            const j = await api.get(`${BASE_URL_API}flows/`);
+            if ((j == null ? void 0 : j.status) !== 200) throw new Error(`HTTP error! status: ${j==null?void 0:j.status}`);
+            return j.data
+        } catch (j) {
+            throw console.error(j), j
+        }
+    }
+    async function downloadFlowsFromDatabase() {
+        try {
+            const j = await api.get(`${BASE_URL_API}flows/download/`);
+            if ((j == null ? void 0 : j.status) !== 200) throw new Error(`HTTP error! status: ${j==null?void 0:j.status}`);
+            return j.data
+        } catch (j) {
+            throw console.error(j), j
+        }
+    }
+    async function uploadFlowsToDatabase(j) {
+        try {
+            const $ = await api.post(`${BASE_URL_API}flows/upload/`, j);
+            if (($ == null ? void 0 : $.status) !== 201) throw new Error(`HTTP error! status: ${$==null?void 0:$.status}`);
+            return $.data
+        } catch ($) {
+            throw console.error($), $
+        }
+    }
+    async function deleteFlowFromDatabase(j) {
+        try {
+            const $ = await api.delete(`${BASE_URL_API}flows/${j}`);
+            if ($.status !== 200) throw new Error(`HTTP error! status: ${$.status}`);
+            return $.data
+        } catch ($) {
+            throw console.error($), $
+        }
+    }
+    async function getVersion() {
+        return (await api.get(`${BASE_URL_API}version`)).data
+    }
+    async function getHealth() {
+        return await api.get("/health")
+    }
+    async function getBuildStatus(j) {
+        return await api.get(`${BASE_URL_API}build/${j}/status`)
+    }
+    async function postBuildInit(j) {
+        return await api.post(`${BASE_URL_API}build/init/${j.id}`, j)
+    }
+    async function uploadFile(j, $) {
+        const at = new FormData;
+        return at.append("file", j), await api.post(`${BASE_URL_API}upload/${$}`, at)
+    }
+    async function postCustomComponent(j, $) {
+        return await api.post(`${BASE_URL_API}custom_component`, {
+            code: j,
+            frontend_node: $
+        })
+    }
+    async function postCustomComponentUpdate(j, $) {
+        return await api.post(`${BASE_URL_API}custom_component/update`, {
+            code: j,
+            field: $
+        })
+    }
+    async function onLogin(j) {
+        try {
+            const $ = await api.post(`${BASE_URL_API}login`, new URLSearchParams({
+                username: j.username,
+                password: j.password
+            }).toString(), {
+                headers: {
+                    "Content-Type": "application/x-www-form-urlencoded"
+                }
+            });
+            if ($.status === 200) return $.data
+        } catch ($) {
+            throw $
+        }
+    }
+    async function autoLogin() {
+        try {
+            const j = await api.get(`${BASE_URL_API}auto_login`);
+            if (j.status === 200) return j.data
+        } catch (j) {
+            throw j
+        }
+    }
+    async function renewAccessToken() {
+        try {
+            return await api.post(`${BASE_URL_API}refresh`)
+        } catch (j) {
+            throw j
+        }
+    }
+    async function getLoggedUser() {
+        try {
+            const j = await api.get(`${BASE_URL_API}users/whoami`);
+            if (j.status === 200) return j.data
+        } catch (j) {
+            throw j
+        }
+        return null
+    }
+    async function addUser(j) {
+        try {
+            const $ = await api.post(`${BASE_URL_API}users/`, j);
+            if ($.status !== 201) throw new Error($.data.detail);
+            return $.data
+        } catch ($) {
+            throw $
+        }
+    }
+    async function getUsersPage(j, $) {
+        try {
+            const at = await api.get(`${BASE_URL_API}users/?skip=${j}&limit=${$}`);
+            if (at.status === 200) return at.data
+        } catch (at) {
+            throw at
+        }
+        return []
+    }
+    async function deleteUser(j) {
+        try {
+            const $ = await api.delete(`${BASE_URL_API}users/${j}`);
+            if ($.status === 200) return $.data
+        } catch ($) {
+            throw $
+        }
+    }
+    async function updateUser(j, $) {
+        try {
+            const at = await api.patch(`${BASE_URL_API}users/${j}`, $);
+            if (at.status === 200) return at.data
+        } catch (at) {
+            throw at
+        }
+    }
+    async function resetPassword(j, $) {
+        try {
+            const at = await api.patch(`${BASE_URL_API}users/${j}/reset-password`, $);
+            if (at.status === 200) return at.data
+        } catch (at) {
+            throw at
+        }
+    }
+    async function getApiKey() {
+        try {
+            const j = await api.get(`${BASE_URL_API}api_key/`);
+            if (j.status === 200) return j.data
+        } catch (j) {
+            throw j
+        }
+    }
+    async function createApiKey(j) {
+        try {
+            const $ = await api.post(`${BASE_URL_API}api_key/`, {
+                name: j
+            });
+            if ($.status === 200) return $.data
+        } catch ($) {
+            throw $
+        }
+    }
+    async function deleteApiKey(j) {
+        try {
+            const $ = await api.delete(`${BASE_URL_API}api_key/${j}`);
+            if ($.status === 200) return $.data
+        } catch ($) {
+            throw $
+        }
+    }
+    async function addApiKeyStore(j) {
+        try {
+            const $ = await api.post(`${BASE_URL_API}api_key/store`, {
+                api_key: j
+            });
+            if ($.status === 200) return $.data
+        } catch ($) {
+            throw $
+        }
+    }
+    async function saveFlowStore(j, $, at = !1) {
+        try {
+            const st = await api.post(`${BASE_URL_API}store/components/`, {
+                name: j.name,
+                data: j.data,
+                description: j.description,
+                is_component: j.is_component,
+                parent: j.parent,
+                tags: $,
+                private: !at,
+                status: at ? "Public" : "Private",
+                last_tested_version: j.last_tested_version
+            });
+            if (st.status !== 201) throw new Error(`HTTP error! status: ${st.status}`);
+            return st.data
+        } catch (st) {
+            throw console.error(st), st
+        }
+    }
+    async function getStoreComponents({
+        component_id: j = null,
+        page: $ = 1,
+        limit: at = 9999999,
+        is_component: st = null,
+        sort: ct = "-count(liked_by)",
+        tags: ut = [],
+        liked: dt = null,
+        isPrivate: ft = null,
+        search: pt = null,
+        filterByUser: Tt = null,
+        fields: ht = null
+    }) {
+        try {
+            let mt = `${BASE_URL_API}store/components/`;
+            const Qt = [];
+            j != null && Qt.push(`component_id=${j}`), pt != null && Qt.push(`search=${pt}`), ft != null && Qt.push(`private=${ft}`), ut != null && ut.length > 0 && Qt.push(`tags=${ut.join(encodeURIComponent(","))}`), ht != null && ht.length > 0 && Qt.push(`fields=${ht.join(encodeURIComponent(","))}`), ct != null ? Qt.push(`sort=${ct}`) : Qt.push("sort=-count(liked_by)"), dt != null && Qt.push(`liked=${dt}`), Tt != null && Qt.push(`filter_by_user=${Tt}`), $ !== void 0 && Qt.push(`page=${$??1}`), at !== void 0 && Qt.push(`limit=${at??9999999}`), st != null && Qt.push(`is_component=${st}`), Qt.length > 0 && (mt += `?${Qt.join("&")}`);
+            const vt = await api.get(mt);
+            if (vt.status === 200) return vt.data
+        } catch (mt) {
+            throw mt
+        }
+    }
+    async function getComponent(j) {
+        try {
+            const $ = await api.get(`${BASE_URL_API}store/components/${j}`);
+            if ($.status === 200) return $.data
+        } catch ($) {
+            throw $
+        }
+    }
+    async function checkHasApiKey() {
+        try {
+            const j = await api.get(`${BASE_URL_API}store/check/api_key`);
+            if ((j == null ? void 0 : j.status) === 200) return j.data
+        } catch (j) {
+            throw j
+        }
+    }
+    async function checkHasStore() {
+        try {
+            const j = await api.get(`${BASE_URL_API}store/check/`);
+            if ((j == null ? void 0 : j.status) === 200) return j.data
+        } catch (j) {
+            throw j
+        }
+    }
+    async function getStoreTags() {
+        try {
+            const j = await api.get(`${BASE_URL_API}store/tags`);
+            if (j.status === 200) return j.data
+        } catch (j) {
+            throw j
+        }
+    }
+    const postLikeComponent = j => api.post(`${BASE_URL_API}store/users/likes/${j}`);
+    async function updateFlowStore(j, $, at = !1, st) {
+        try {
+            const ct = await api.patch(`${BASE_URL_API}store/components/${st}`, {
+                name: j.name,
+                data: j.data,
+                description: j.description,
+                is_component: j.is_component,
+                parent: j.parent,
+                tags: $,
+                private: !at,
+                last_tested_version: j.last_tested_version
+            });
+            if (ct.status !== 201) throw new Error(`HTTP error! status: ${ct.status}`);
+            return ct.data
+        } catch (ct) {
+            throw console.error(ct), ct
+        }
+    }
+    async function requestLogout() {
+        try {
+            return (await api.post(`${BASE_URL_API}logout`)).data
+        } catch (j) {
+            throw console.error(j), j
+        }
+    }
+    const uid = new ShortUniqueId({
+        length: 5
+    });
+
+    function cleanEdges(j, $) {
+        let at = lodashExports.cloneDeep($);
+        return $.forEach(st => {
+            var pt, Tt, ht, mt;
+            const ct = j.find(Qt => Qt.id === st.source),
+                ut = j.find(Qt => Qt.id === st.target);
+            if (!ct || !ut) {
+                at = at.filter(Qt => Qt.id !== st.id);
+                return
+            }
+            const dt = st.sourceHandle,
+                ft = st.targetHandle;
+            if (ft) {
+                const vt = scapeJSONParse(ft).fieldName,
+                    xt = {
+                        type: (pt = ut.data.node.template[vt]) == null ? void 0 : pt.type,
+                        fieldName: vt,
+                        id: ut.data.id,
+                        inputTypes: (Tt = ut.data.node.template[vt]) == null ? void 0 : Tt.input_types
+                    };
+                (ht = ut.data.node.template[vt]) != null && ht.proxy && (xt.proxy = (mt = ut.data.node.template[vt]) == null ? void 0 : mt.proxy), scapedJSONStringfy(xt) !== ft && (at = at.filter(yt => yt.id !== st.id))
+            }
+            if (dt) {
+                const Qt = {
+                    id: ct.data.id,
+                    baseClasses: ct.data.node.base_classes,
+                    dataType: ct.data.type
+                };
+                scapedJSONStringfy(Qt) !== dt && (at = at.filter(vt => vt.id !== st.id))
+            }
+        }), at
+    }
+
+    function isValidConnection({
+        source: j,
+        target: $,
+        sourceHandle: at,
+        targetHandle: st
+    }, ct, ut) {
+        var pt, Tt, ht;
+        const dt = scapeJSONParse(st),
+            ft = scapeJSONParse(at);
+        if ((pt = dt.inputTypes) != null && pt.some(mt => mt === ft.dataType) || ft.baseClasses.some(mt => {
+                var Qt;
+                return ((Qt = dt.inputTypes) == null ? void 0 : Qt.some(vt => vt === mt)) || mt === dt.type
+            })) {
+            let mt = (ht = (Tt = ct.find(Qt => Qt.id === $)) == null ? void 0 : Tt.data) == null ? void 0 : ht.node;
+            if (mt) {
+                if (!mt.template[dt.fieldName].list && !ut.find(Qt => Qt.targetHandle === st) || mt.template[dt.fieldName].list) return !0
+            } else if (!ut.find(Qt => Qt.targetHandle === st)) return !0
+        }
+        return !1
+    }
+
+    function removeApiKeys(j) {
+        let $ = lodashExports.cloneDeep(j);
+        return $.data.nodes.forEach(at => {
+            for (const st in at.data.node.template) at.data.node.template[st].password && (at.data.node.template[st].value = "")
+        }), $
+    }
+    const processFlows = (j, $ = !0) => {
+            let at = {};
+            return j.forEach(st => {
+                try {
+                    if (!st.data) return;
+                    if (st.data && st.is_component) {
+                        st.data.nodes[0].data.node.display_name = st.name, at[createRandomKey(st.data.nodes[0].data.type, uid())] = lodashExports.cloneDeep(st.data.nodes[0].data.node);
+                        return
+                    }
+                    $ || processDataFromFlow(st, !1)
+                } catch (ct) {
+                    console.log(ct)
+                }
+            }), {
+                data: at,
+                flows: j
+            }
+        },
+        processDataFromFlow = (j, $ = !0) => {
+            let at = j != null && j.data ? j.data : null;
+            return at && (processFlowEdges(j), updateEdges(at.edges), $ && updateIds(at)), at
+        };
+
+    function updateIds(j) {
+        let $ = {};
+        return j.nodes && j.nodes.forEach(at => {
+            var ct;
+            let st = getNodeId((ct = at.data.node) != null && ct.flow ? "GroupNode" : at.data.type);
+            $[at.id] = st, at.id = st, at.data.id = st
+        }), j.edges && j.edges.forEach(at => {
+            var ut, dt, ft, pt;
+            at.source = $[at.source], at.target = $[at.target];
+            const st = scapeJSONParse(at.sourceHandle);
+            at.sourceHandle = scapedJSONStringfy({
+                ...st,
+                id: at.source
+            }), (dt = (ut = at.data) == null ? void 0 : ut.sourceHandle) != null && dt.id && (at.data.sourceHandle.id = at.source);
+            const ct = scapeJSONParse(at.targetHandle);
+            at.targetHandle = scapedJSONStringfy({
+                ...ct,
+                id: at.target
+            }), (pt = (ft = at.data) == null ? void 0 : ft.targetHandle) != null && pt.id && (at.data.targetHandle.id = at.target), at.id = "reactflow__edge-" + at.source + at.sourceHandle + "-" + at.target + at.targetHandle
+        }), $
+    }
+
+    function buildTweaks(j) {
+        return j.data.nodes.reduce(($, at) => ($[at.data.id] = {}, $), {})
+    }
+
+    function validateNode(j, $) {
+        var ct, ut;
+        if (!((ut = (ct = j.data) == null ? void 0 : ct.node) != null && ut.template) || !Object.keys(j.data.node.template)) return ["We've noticed a potential issue with a node in the flow. Please review it and, if necessary, submit a bug report with your exported flow file. Thank you for your help!"];
+        const {
+            type: at,
+            node: {
+                template: st
+            }
+        } = j.data;
+        return Object.keys(st).reduce((dt, ft) => (st[ft].required && st[ft].show && (st[ft].value === void 0 || st[ft].value === null || st[ft].value === "") && !$.some(pt => scapeJSONParse(pt.targetHandle).fieldName === ft && scapeJSONParse(pt.targetHandle).id === j.id) ? dt.push(`${at} is missing ${getFieldTitle(st,ft)}.`) : st[ft].type === "dict" && st[ft].required && st[ft].show && (st[ft].value !== void 0 || st[ft].value !== null || st[ft].value !== "") && (hasDuplicateKeys(st[ft].value) && dt.push(`${at} (${getFieldTitle(st,ft)}) contains duplicate keys with the same values.`), hasEmptyKey(st[ft].value) && dt.push(`${at} (${getFieldTitle(st,ft)}) field must not be empty.`)), dt), [])
+    }
+
+    function validateNodes(j, $) {
+        return j.length === 0 ? ["No nodes found in the flow. Please add at least one node to the flow."] : j.flatMap(at => validateNode(at, $))
+    }
+
+    function updateEdges(j) {
+        j && j.forEach($ => {
+            const at = scapeJSONParse($.targetHandle);
+            $.className = (at.type === "Text" ? "stroke-gray-800 " : "stroke-gray-900 ") + " stroke-connection", $.animated = at.type === "Text"
+        })
+    }
+
+    function addVersionToDuplicates(j, $) {
+        const at = $.map(ut => ut.name);
+        let st = j.name,
+            ct = 1;
+        for (; at.includes(st);) st = `${j.name} (${ct})`, ct++;
+        return st
+    }
+
+    function updateEdgesHandleIds({
+        edges: j,
+        nodes: $
+    }) {
+        let at = lodashExports.cloneDeep(j);
+        return at.forEach(st => {
+            const ct = st.source,
+                ut = st.target,
+                dt = $.find(vt => vt.id === ct),
+                ft = $.find(vt => vt.id === ut);
+            let pt = st.sourceHandle,
+                Tt = st.targetHandle,
+                ht, mt;
+            if (Tt && ft) {
+                let vt = Tt.split("|")[1];
+                mt = {
+                    type: ft.data.node.template[vt].type,
+                    fieldName: vt,
+                    id: ft.data.id,
+                    inputTypes: ft.data.node.template[vt].input_types
+                }
+            }
+            pt && dt && (ht = {
+                id: dt.data.id,
+                baseClasses: dt.data.node.base_classes,
+                dataType: dt.data.type
+            }), st.sourceHandle = scapedJSONStringfy(ht), st.targetHandle = scapedJSONStringfy(mt);
+            const Qt = {
+                sourceHandle: scapeJSONParse(st.sourceHandle),
+                targetHandle: scapeJSONParse(st.targetHandle)
+            };
+            st.data = Qt
+        }), at
+    }
+
+    function handleKeyDown$1(j, $, at) {
+        (typeof $ == "string" && (j.metaKey === !0 || j.ctrlKey === !0) && j.key === "Backspace" && ($ === at || ($ == null ? void 0 : $.charAt(($ == null ? void 0 : $.length) - 1)) === " " || specialCharsRegex.test($ == null ? void 0 : $.charAt(($ == null ? void 0 : $.length) - 1))) || navigator.userAgent.toUpperCase().includes("MAC") && j.ctrlKey === !0 && j.key === "Backspace") && (j.preventDefault(), j.stopPropagation()), j.ctrlKey === !0 && j.key === "Backspace" && $ === at && (j.preventDefault(), j.stopPropagation())
+    }
+
+    function handleOnlyIntegerInput(j) {
+        (j.key === "." || j.key === "-" || j.key === "," || j.key === "e" || j.key === "E" || j.key === "+") && j.preventDefault()
+    }
+
+    function convertObjToArray(j) {
+        if (typeof j == "string" && (j = JSON.parse(j)), Array.isArray(j)) return j;
+        let $ = [];
+        if (typeof j == "object") {
+            for (const at in j)
+                if (Object.prototype.hasOwnProperty.call(j, at)) {
+                    const st = {};
+                    st[at] = j[at], $.push(st)
+                }
+        }
+        return $
+    }
+
+    function convertArrayToObj(j) {
+        if (!Array.isArray(j)) return j;
+        let $ = {};
+        for (const at of j)
+            for (const st in at) at.hasOwnProperty(st) && ($[st] = at[st]);
+        return $
+    }
+
+    function hasDuplicateKeys(j) {
+        const $ = {};
+        Array.isArray(j) || (j = [{
+            "": ""
+        }]);
+        for (const at of j)
+            for (const st in at) {
+                if ($[st]) return !0;
+                $[st] = !0
+            }
+        return !1
+    }
+
+    function hasEmptyKey(j) {
+        Array.isArray(j) || (j = []);
+        for (const $ of j)
+            for (const at in $)
+                if ($.hasOwnProperty(at) && at === "") return !0;
+        return !1
+    }
+
+    function convertValuesToNumbers(j) {
+        return j.map($ => {
+            const at = {};
+            for (const st in $)
+                if ($.hasOwnProperty(st)) {
+                    let ct = $[st];
+                    /^\d+$/.test(ct) && (ct = ct == null ? void 0 : ct.toString().trim()), at[st] = ct === "" || isNaN(ct) ? ct.toString() : Number(ct)
+                } return at
+        })
+    }
+
+    function scapedJSONStringfy(j) {
+        return customStringify(j).replace(/"/g, "œ")
+    }
+
+    function scapeJSONParse(j) {
+        let $ = j.replace(/œ/g, '"');
+        return JSON.parse($)
+    }
+
+    function checkOldEdgesHandles(j) {
+        return j.some($ => !$.sourceHandle || !$.targetHandle || !$.sourceHandle.includes("{") || !$.targetHandle.includes("{"))
+    }
+
+    function customStringify(j) {
+        return typeof j > "u" ? "null" : j === null || typeof j != "object" ? j instanceof Date ? `"${j.toISOString()}"` : JSON.stringify(j) : Array.isArray(j) ? `[${j.map(ct=>customStringify(ct)).join(",")}]` : `{${Object.keys(j).sort().map(st=>`"${st}":${customStringify(j[st])}`).join(",")}}`
+    }
+
+    function getMiddlePoint(j) {
+        let $ = 0,
+            at = 0;
+        j.forEach(dt => {
+            $ += dt.position.x, at += dt.position.y
+        });
+        const st = j.length,
+            ct = $ / st,
+            ut = at / st;
+        return {
+            x: ct,
+            y: ut
+        }
+    }
+
+    function getNodeId(j) {
+        return j + "-" + uid()
+    }
+
+    function getHandleId(j, $, at, st) {
+        return "reactflow__edge-" + j + $ + "-" + at + st
+    }
+
+    function generateFlow(j, $, at, st) {
+        const ct = {
+                nodes: $,
+                edges: at,
+                viewport: {
+                    zoom: 1,
+                    x: 0,
+                    y: 0
+                }
+            },
+            ut = new ShortUniqueId({
+                length: 5
+            });
+        return ct.edges = j.edges.filter(ft => j.nodes.some(pt => pt.id === ft.target) && j.nodes.some(pt => pt.id === ft.source)), ct.nodes = j.nodes, {
+            newFlow: {
+                data: ct,
+                is_component: !1,
+                name: st,
+                description: "",
+                id: ut()
+            },
+            removedEdges: at.filter(ft => (j.nodes.some(pt => pt.id === ft.target) || j.nodes.some(pt => pt.id === ft.source)) && ct.edges.every(pt => pt.id !== ft.id))
+        }
+    }
+
+    function reconnectEdges(j, $) {
+        let at = lodashExports.cloneDeep($);
+        if (!j.data.node.flow) return [];
+        const {
+            nodes: st,
+            edges: ct
+        } = j.data.node.flow.data, ut = findLastNode(j.data.node.flow.data);
+        return at.forEach(dt => {
+            if (ut && dt.source === ut.id) {
+                dt.source = j.id;
+                let ft = scapeJSONParse(dt.sourceHandle);
+                ft.id = j.id, dt.sourceHandle = scapedJSONStringfy(ft), dt.data.sourceHandle = ft
+            }
+            if (st.some(ft => ft.id === dt.target)) {
+                const ft = st.find(mt => mt.id === dt.target);
+                console.log("targetNode", ft);
+                const pt = scapeJSONParse(dt.targetHandle);
+                console.log("targetHandle", pt);
+                const Tt = {
+                    id: ft.id,
+                    field: pt.fieldName
+                };
+                let ht = lodashExports.cloneDeep(pt);
+                ht.id = j.id, ht.proxy = Tt, dt.target = j.id, ht.fieldName = pt.fieldName + "_" + ft.id, dt.targetHandle = scapedJSONStringfy(ht), dt.data.targetHandle = ht
+            }
+        }), at
+    }
+
+    function findLastNode({
+        nodes: j,
+        edges: $
+    }) {
+        return j.find(st => !$.some(ct => ct.source === st.id))
+    }
+
+    function updateFlowPosition(j, $) {
+        const at = getMiddlePoint($.data.nodes);
+        let st = {
+            x: j.x - at.x,
+            y: j.y - at.y
+        };
+        return {
+            ...$,
+            data: {
+                ...$.data,
+                nodes: $.data.nodes.map(ct => ({
+                    ...ct,
+                    position: {
+                        x: ct.position.x + st.x,
+                        y: ct.position.y + st.y
+                    }
+                }))
+            }
+        }
+    }
+
+    function validateSelection(j, $) {
+        j.edges.length === 0 && (j.edges = $);
+        let at = new Set(j.nodes.map(ut => ut.id)),
+            st = j.edges.filter(ut => at.has(ut.source) && at.has(ut.target));
+        j.edges = st;
+        let ct = [];
+        return j.nodes.length < 2 && ct.push("Please select more than one node"), j.nodes.filter(ut => !j.edges.some(dt => dt.source === ut.id)).length > 1 && ct.push("Please select only one node with free outputs"), j.nodes.some(ut => !j.edges.some(dt => dt.target === ut.id) && !j.edges.some(dt => dt.source === ut.id)) && ct.push("Please select only nodes that are connected"), ct
+    }
+
+    function updateGroupNodeTemplate(j) {
+        return Object.keys(j).forEach($ => {
+            let at = j[$].type,
+                st = j[$].input_types;
+            LANGFLOW_SUPPORTED_TYPES.has(at) && !j[$].required && !st && (j[$].advanced = !0), at === "code" && (j[$].show = !1)
+        }), j
+    }
+
+    function mergeNodeTemplates({
+        nodes: j,
+        edges: $
+    }) {
+        let at = {};
+        return j.forEach(st => {
+            let ct = lodashExports.cloneDeep(st.data.node.template);
+            Object.keys(ct).filter(ut => ut.charAt(0) !== "_").forEach(ut => {
+                isHandleConnected($, ut, ct[ut], st.id) || (at[ut + "_" + st.id] = ct[ut], at[ut + "_" + st.id].proxy = {
+                    id: st.id,
+                    field: ut
+                }, st.type === "groupNode" ? at[ut + "_" + st.id].display_name = st.data.node.flow.name + " - " + ct[ut].name : at[ut + "_" + st.id].display_name = ct[ut].display_name ? ct[ut].display_name : ct[ut].name ? toTitleCase(ct[ut].name) : toTitleCase(ut))
+            })
+        }), at
+    }
+
+    function isHandleConnected(j, $, at, st) {
+        if (at.proxy) {
+            if (j.some(ct => ct.targetHandle === scapedJSONStringfy({
+                    type: at.type,
+                    fieldName: $,
+                    id: st,
+                    proxy: {
+                        id: at.proxy.id,
+                        field: at.proxy.field
+                    },
+                    inputTypes: at.input_types
+                }))) return !0
+        } else if (j.some(ct => ct.targetHandle === scapedJSONStringfy({
+                type: at.type,
+                fieldName: $,
+                id: st,
+                inputTypes: at.input_types
+            }))) return !0;
+        return !1
+    }
+
+    function generateNodeTemplate(j) {
+        let $ = mergeNodeTemplates({
+            nodes: j.data.nodes,
+            edges: j.data.edges
+        });
+        return updateGroupNodeTemplate($), $
+    }
+
+    function generateNodeFromFlow(j, $) {
+        const {
+            nodes: at
+        } = j.data, st = lodashExports.cloneDeep(findLastNode(j.data)), ct = getMiddlePoint(at);
+        let ut = lodashExports.cloneDeep(j);
+        const dt = $(st == null ? void 0 : st.data.type);
+        return {
+            data: {
+                id: dt,
+                type: st == null ? void 0 : st.data.type,
+                node: {
+                    output_types: st.data.node.output_types,
+                    display_name: "Group",
+                    documentation: "",
+                    base_classes: st.data.node.base_classes,
+                    description: "",
+                    template: generateNodeTemplate(ut),
+                    flow: ut
+                }
+            },
+            id: dt,
+            position: ct,
+            type: "genericNode"
+        }
+    }
+
+    function updateProxyIdsOnTemplate(j, $) {
+        Object.keys(j).forEach(at => {
+            j[at].proxy && $[j[at].proxy.id] && (j[at].proxy.id = $[j[at].proxy.id])
+        })
+    }
+
+    function updateEdgesIds(j, $) {
+        j.forEach(at => {
+            let st = at.data.targetHandle;
+            st.proxy && $[st.proxy.id] && (st.proxy.id = $[st.proxy.id]), at.data.targetHandle = st, at.targetHandle = scapedJSONStringfy(st)
+        })
+    }
+
+    function processFlowEdges(j) {
+        if (!(!j.data || !j.data.edges)) {
+            if (checkOldEdgesHandles(j.data.edges)) {
+                const $ = updateEdgesHandleIds(j.data);
+                j.data.edges = $
+            }
+            j.data.edges.forEach($ => {
+                $.className = "", $.style = {
+                    stroke: "#555"
+                }
+            })
+        }
+    }
+
+    function expandGroupNode(j, $, at, st, ct, ut, dt) {
+        var xt;
+        const ft = updateIds($.data);
+        updateProxyIdsOnTemplate(at, ft);
+        let pt = ct;
+        updateEdgesIds(pt, ft);
+        const Tt = lodashExports.cloneDeep((xt = $ == null ? void 0 : $.data) == null ? void 0 : xt.nodes),
+            ht = lodashExports.cloneDeep($.data.edges);
+        let mt = [];
+        pt.forEach(yt => {
+            var bt, wt, At;
+            let Et = lodashExports.cloneDeep(yt);
+            if (Et.target === j) {
+                const Ct = Et.data.targetHandle;
+                if (Ct.proxy) {
+                    let Mt = Ct.type,
+                        St = Ct.proxy.field,
+                        Rt = Ct.proxy.id,
+                        _t = Ct.inputTypes,
+                        Ot = Tt.find(Dt => Dt.id === Rt);
+                    if (Ot) {
+                        Et.target = Rt;
+                        let Dt = {
+                            fieldName: St,
+                            type: Mt,
+                            id: Rt,
+                            inputTypes: _t
+                        };
+                        (bt = Ot.data.node) != null && bt.flow && (Dt.proxy = {
+                            field: (wt = Ot.data.node.template[St].proxy) == null ? void 0 : wt.field,
+                            id: (At = Ot.data.node.template[St].proxy) == null ? void 0 : At.id
+                        }), Et.data.targetHandle = Dt, Et.targetHandle = scapedJSONStringfy(Dt)
+                    }
+                }
+            }
+            if (Et.source === j) {
+                const Ct = lodashExports.cloneDeep(findLastNode($.data));
+                Et.source = Ct.id;
+                let Mt = scapeJSONParse(Et.sourceHandle);
+                Mt.id = Ct.id, Et.data.sourceHandle = Mt, Et.sourceHandle = scapedJSONStringfy(Mt)
+            }(yt.target === j || yt.source === j) && mt.push(Et)
+        }), Object.keys(at).forEach(yt => {
+            let {
+                field: Et,
+                id: bt
+            } = at[yt].proxy, wt = Tt.findIndex(At => At.id === bt);
+            if (wt !== -1) {
+                let At, Ct, Mt = Tt[wt].data.node.template[Et].show,
+                    St = Tt[wt].data.node.template[Et].advanced;
+                Tt[wt].data.node.template[Et].display_name ? Ct = Tt[wt].data.node.template[Et].display_name : Ct = Tt[wt].data.node.template[Et].name, Tt[wt].data.node.template[Et].proxy && (At = Tt[wt].data.node.template[Et].proxy), Tt[wt].data.node.template[Et] = at[yt], Tt[wt].data.node.template[Et].show = Mt, Tt[wt].data.node.template[Et].advanced = St, Tt[wt].data.node.template[Et].display_name = Ct, At ? Tt[wt].data.node.template[Et].proxy = At : delete Tt[wt].data.node.template[Et].proxy
+            }
+        });
+        const Qt = [...st.filter(yt => yt.id !== j), ...Tt],
+            vt = [...ct.filter(yt => yt.target !== j && yt.source !== j), ...ht, ...mt];
+        ut(Qt), dt(vt)
+    }
+
+    function createFlowComponent(j, $) {
+        var st, ct;
+        return {
+            data: {
+                edges: [],
+                nodes: [{
+                    data: {
+                        ...j,
+                        node: {
+                            ...j.node,
+                            official: !1
+                        }
+                    },
+                    id: j.id,
+                    position: {
+                        x: 0,
+                        y: 0
+                    },
+                    type: "genericNode"
+                }],
+                viewport: {
+                    x: 1,
+                    y: 1,
+                    zoom: 1
+                }
+            },
+            description: ((st = j.node) == null ? void 0 : st.description) || "",
+            name: ((ct = j.node) == null ? void 0 : ct.display_name) || j.type || "",
+            id: j.id || "",
+            is_component: !0,
+            last_tested_version: $
+        }
+    }
+
+    function downloadNode(j) {
+        const $ = document.createElement("a"),
+            at = new Blob([JSON.stringify(j)], {
+                type: "application/json"
+            });
+        $.href = URL.createObjectURL(at), $.download = `${j.name}.json`, $.click()
+    }
+
+    function removeFileNameFromComponents(j) {
+        j.data.nodes.forEach($ => {
+            var at;
+            Object.keys($.data.node.template).forEach(st => {
+                var ct;
+                ((ct = $.data.node) == null ? void 0 : ct.template[st].type) === "file" && ($.data.node.template[st].value = "")
+            }), (at = $.data.node) != null && at.flow && removeFileNameFromComponents($.data.node.flow)
+        })
+    }
+
+    function typesGenerator(j) {
+        return Object.keys(j).reverse().reduce(($, at) => (Object.keys(j[at]).forEach(st => {
+            var ct;
+            $[st] = at, (ct = j[at][st].base_classes) == null || ct.forEach(ut => {
+                $[ut] = at
+            })
+        }), $), {})
+    }
+
+    function templatesGenerator(j) {
+        return Object.keys(j).reduce(($, at) => (Object.keys(j[at]).forEach(st => {
+            j[at][st].flow || ($[st] = j[at][st])
+        }), $), {})
+    }
+
+    function downloadFlow(j, $, at) {
+        let st = lodashExports.cloneDeep(j);
+        removeFileNameFromComponents(st);
+        const ct = `data:text/json;chatset=utf-8,${encodeURIComponent(JSON.stringify({...st,name:$,description:at}))}`,
+            ut = document.createElement("a");
+        ut.href = ct, ut.download = `${$&&$!=""?$:j.name}.json`, ut.click()
+    }
+
+    function downloadFlows() {
+        downloadFlowsFromDatabase().then(j => {
+            const $ = `data:text/json;chatset=utf-8,${encodeURIComponent(JSON.stringify(j))}`,
+                at = document.createElement("a");
+            at.href = $, at.download = "flows.json", at.click()
+        })
+    }
+    const createNewFlow = (j, $) => ({
+        description: ($ == null ? void 0 : $.description) ?? getRandomDescription(),
+        name: $ != null && $.name ? $.name : "Untitled document",
+        data: j,
+        id: "",
+        is_component: ($ == null ? void 0 : $.is_component) ?? !1
+    });
+
+    function classNames(...j) {
+        return j.filter(Boolean).join(" ")
+    }
+
+    function cn(...j) {
+        return twMerge(clsx$2(j))
+    }
+
+    function toTitleCase(j) {
+        return j ? j.split("_").map((at, st) => checkUpperWords(st === 0 ? at[0].toUpperCase() + at.slice(1).toLowerCase() : at.toLowerCase())).join(" ").split("-").map((at, st) => checkUpperWords(st === 0 ? at[0].toUpperCase() + at.slice(1).toLowerCase() : at.toLowerCase())).join(" ") : ""
+    }
+    const upperCaseWords = ["llm", "uri"];
+
+    function checkUpperWords(j) {
+        return j.split(" ").map(at => upperCaseWords.includes(at.toLowerCase()) ? at.toUpperCase() : at[0].toUpperCase() + at.slice(1).toLowerCase()).join(" ")
+    }
+    const isWrappedWithClass = (j, $) => j.target.closest(`.${$}`);
+
+    function groupByFamily(j, $, at, st) {
+        var ht;
+        const ct = new Set($.split(`
+`));
+        let ut = [],
+            dt = [],
+            ft = new Map;
+        const pt = new Set(["str", "bool", "float", "code", "prompt", "file", "int"]),
+            Tt = mt => mt.type && mt.show && (!pt.has(mt.type) && ct.has(mt.type) || mt.input_types && mt.input_types.some(Qt => ct.has(Qt)));
+        if (st)
+            for (const mt of st) {
+                if (mt.data.node.flow) break;
+                const Qt = mt.data,
+                    vt = ft.get(Qt.type);
+                ft.set(Qt.type, {
+                    hasBaseClassInTemplate: (vt == null ? void 0 : vt.hasBaseClassInTemplate) || Object.values(Qt.node.template).some(Tt),
+                    hasBaseClassInBaseClasses: (vt == null ? void 0 : vt.hasBaseClassInBaseClasses) || Qt.node.base_classes.some(xt => ct.has(xt)),
+                    displayName: (ht = Qt.node) == null ? void 0 : ht.display_name
+                })
+            }
+        for (const [mt, Qt] of Object.entries(j)) {
+            let vt = [],
+                xt = [];
+            for (const [Et, bt] of Object.entries(Qt)) {
+                let wt = ft.get(Et);
+                wt || (wt = {
+                    hasBaseClassInTemplate: Object.values(bt.template).some(Tt),
+                    hasBaseClassInBaseClasses: bt.base_classes.some(At => ct.has(At)),
+                    displayName: bt == null ? void 0 : bt.display_name
+                }), wt.hasBaseClassInTemplate && vt.push({
+                    node: Et,
+                    displayName: wt.displayName
+                }), wt.hasBaseClassInBaseClasses && xt.push({
+                    node: Et,
+                    displayName: wt.displayName
+                })
+            }
+            const yt = Object.keys(Qt).length;
+            vt.length && ut.push({
+                category: mt,
+                nodes: vt,
+                full: vt.length === yt
+            }), xt.length && dt.push({
+                category: mt,
+                nodes: xt,
+                full: xt.length === yt
+            })
+        }
+        return at ? dt.map(mt => ({
+            family: mt.category,
+            type: mt.full ? "" : mt.nodes.map(Qt => Qt.node).join(", "),
+            display_name: ""
+        })) : ut.map(mt => ({
+            family: mt.category,
+            type: mt.full ? "" : mt.nodes.map(Qt => Qt.node).join(", "),
+            display_name: mt.nodes.map(Qt => Qt.displayName).join(", ")
+        }))
+    }
+
+    function buildInputs(j) {
+        return j && j.input_keys && Object.keys(j.input_keys).length > 0 ? JSON.stringify(j.input_keys) : '{"input": "message"}'
+    }
+
+    function getRandomElement(j) {
+        return j[Math.floor(Math.random() * j.length)]
+    }
+
+    function getRandomDescription() {
+        return getRandomElement(DESCRIPTIONS)
+    }
+
+    function getRandomName(j = 0, $ = !1, at = 3) {
+        const st = ADJECTIVES,
+            ct = NOUNS,
+            ut = getRandomElement(st),
+            dt = getRandomElement(ct);
+        if (ut === "boring" && dt === "wozniak") {
+            if (j < at) return getRandomName(j + 1, $, at);
+            console.warn("Max retries reached, returning as is")
+        }
+        if (j > 0 && $) {
+            const pt = Math.floor(Math.random() * 10);
+            return `${ut}_${dt}${pt}`
+        }
+        let ft = $ ? `${ut}_${dt}` : `${ut} ${dt}`;
+        return toTitleCase(ft)
+    }
+
+    function varHighlightHTML({
+        name: j
+    }) {
+        return `<span class="font-semibold chat-message-highlight">{${j}}</span>`
+    }
+
+    function buildTweakObject(j) {
+        return j.forEach(at => {
+            Object.keys(at).forEach(st => {
+                for (let ct in at[st]) try {
+                    at[st][ct] = JSON.parse(at[st][ct])
+                } catch {}
+            })
+        }), JSON.stringify(j.at(-1), null, 2)
+    }
+
+    function getChatInputField(j, $) {
+        let at = "text";
+        return $ && $.input_keys && (at = Object.keys($.input_keys)[0]), at
+    }
+
+    function getPythonApiCode(j, $, at, st) {
+        const ct = j.id,
+            ut = buildTweaks(j),
+            dt = buildInputs(st);
+        return `import requests
+from typing import Optional
+
+BASE_API_URL = "${window.location.protocol}//${window.location.host}/api/v1/process"
+FLOW_ID = "${ct}"
+# You can tweak the flow by adding a tweaks dictionary
+# e.g {"OpenAI-XXXXX": {"model_name": "gpt-4"}}
+TWEAKS = ${at&&at.length>0?buildTweakObject(at):JSON.stringify(ut,null,2)}
+
+def run_flow(inputs: dict, flow_id: str, tweaks: Optional[dict] = None${$?"":", api_key: Optional[str] = None"}) -> dict:
+    """
+    Run a flow with a given message and optional tweaks.
+
+    :param message: The message to send to the flow
+    :param flow_id: The ID of the flow to run
+    :param tweaks: Optional tweaks to customize the flow
+    :return: The JSON response from the flow
+    """
+    api_url = f"{BASE_API_URL}/{flow_id}"
+
+    payload = {"inputs": inputs}
+    headers = None
+    if tweaks:
+        payload["tweaks"] = tweaks
+    if api_key:
+        headers = {"x-api-key": api_key}
+    response = requests.post(api_url, json=payload, headers=headers)
+    return response.json()
+
+# Setup any tweaks you want to apply to the flow
+inputs = ${dt}
+${$?"":'api_key = "<your api key>"'}
+print(run_flow(inputs, flow_id=FLOW_ID, tweaks=TWEAKS${$?"":", api_key=api_key"}))`
+    }
+
+    function getCurlCode(j, $, at, st) {
+        const ct = j.id,
+            ut = buildTweaks(j),
+            dt = buildInputs(st);
+        return `curl -X POST \\
+  ${window.location.protocol}//${window.location.host}/api/v1/process/${ct} \\
+  -H 'Content-Type: application/json'\\${$?"":`
+  -H 'x-api-key: <your api key>'\\`}
+  -d '{"inputs": ${dt}, "tweaks": ${at&&at.length>0?buildTweakObject(at):JSON.stringify(ut,null,2)}}'`
+    }
+
+    function getPythonCode(j, $, at) {
+        const st = j.name,
+            ct = buildTweaks(j),
+            ut = buildInputs(at);
+        return `from langflow import load_flow_from_json
+TWEAKS = ${$&&$.length>0?buildTweakObject($):JSON.stringify(ct,null,2)}
+flow = load_flow_from_json("${st}.json", tweaks=TWEAKS)
+# Now you can use it like any chain
+inputs = ${ut}
+flow(inputs)`
+    }
+
+    function getWidgetCode(j, $, at) {
+        const st = j.id,
+            ct = j.name,
+            ut = buildInputs(at);
+        let dt = getChatInputField(j, at);
+        return `<script src="https://cdn.jsdelivr.net/gh/logspace-ai/langflow-embedded-chat@main/dist/build/static/js/bundle.min.js"><\/script>
+
+<!-- chat_inputs: Stringified JSON with all the input keys and its values. The value of the key that is defined
+as chat_input_field will be overwritten by the chat message.
+chat_input_field: Input key that you want the chat to send the user message with. -->
+<langflow-chat
+  window_title="${ct}"
+  flow_id="${st}"
+  ${at?`chat_inputs='${ut}'
+  chat_input_field="${dt}"
+  `:""}host_url="http://localhost:7860"${$?"":`
+  api_key="..."`}
+
+></langflow-chat>`
+    }
+
+    function tabsArray(j, $) {
+        if ($) return $ === 0 ? [{
+            name: "cURL",
+            mode: "bash",
+            image: "https://curl.se/logo/curl-symbol-transparent.png",
+            language: "sh",
+            code: j[0]
+        }, {
+            name: "Python API",
+            mode: "python",
+            image: "https://images.squarespace-cdn.com/content/v1/5df3d8c5d2be5962e4f87890/1628015119369-OY4TV3XJJ53ECO0W2OLQ/Python+API+Training+Logo.png?format=1000w",
+            language: "py",
+            code: j[1]
+        }, {
+            name: "Python Code",
+            mode: "python",
+            image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
+            language: "py",
+            code: j[2]
+        }, {
+            name: "Chat Widget HTML",
+            description: "Insert this code anywhere in your &lt;body&gt; tag. To use with react and other libs, check our <a class='link-color' href='https://langflow.org/guidelines/widget'>documentation</a>.",
+            mode: "html",
+            image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
+            language: "py",
+            code: j[3]
+        }] : [{
+            name: "cURL",
+            mode: "bash",
+            image: "https://curl.se/logo/curl-symbol-transparent.png",
+            language: "sh",
+            code: j[0]
+        }, {
+            name: "Python API",
+            mode: "python",
+            image: "https://images.squarespace-cdn.com/content/v1/5df3d8c5d2be5962e4f87890/1628015119369-OY4TV3XJJ53ECO0W2OLQ/Python+API+Training+Logo.png?format=1000w",
+            language: "py",
+            code: j[1]
+        }, {
+            name: "Python Code",
+            mode: "python",
+            language: "py",
+            image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
+            code: j[2]
+        }, {
+            name: "Chat Widget HTML",
+            description: "Insert this code anywhere in your &lt;body&gt; tag. To use with react and other libs, check our <a class='link-color' href='https://langflow.org/guidelines/widget'>documentation</a>.",
+            mode: "html",
+            image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
+            language: "py",
+            code: j[3]
+        }, {
+            name: "Tweaks",
+            mode: "python",
+            image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
+            language: "py",
+            code: j[4]
+        }]
+    }
+
+    function removeCountFromString(j) {
+        const $ = /\s*\(\w+\)\s*$/;
+        return j.replace($, "").trim()
+    }
+
+    function createRandomKey(j, $) {
+        return removeCountFromString(j) + ` (${$})`
+    }
+
+    function sensitiveSort(j, $) {
+        const at = /(.+) \((\w+)\)/,
+            st = j.match(at),
+            ct = $.match(at);
+        if (st && ct) {
+            const ut = st[1],
+                dt = ct[1];
+            if (ut !== dt) return ut.localeCompare(dt);
+            const ft = parseInt(st[2]),
+                pt = parseInt(ct[2]);
+            return ft - pt
+        } else return j.localeCompare($)
+    }
+
+    function getFieldTitle(j, $) {
+        return j[$].display_name ? j[$].display_name : j[$].name ? toTitleCase(j[$].name) : toTitleCase($)
+    }
+    const buttonVariants = cva("inline-flex items-center justify-center rounded-md text-sm font-medium transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:opacity-50 disabled:pointer-events-none ring-offset-background", {
+            variants: {
+                variant: {
+                    default: "bg-primary text-primary-foreground hover:bg-primary/90",
+                    destructive: "bg-destructive text-destructive-foreground hover:bg-destructive/90",
+                    outline: "border border-input hover:bg-accent hover:text-accent-foreground",
+                    primary: "border bg-background text-secondary-foreground hover:bg-secondary-foreground/5 dark:hover:bg-background/10 hover:shadow-sm",
+                    secondary: "border border-muted bg-muted text-secondary-foreground hover:bg-secondary-foreground/5",
+                    ghost: "hover:bg-accent hover:text-accent-foreground",
+                    link: "underline-offset-4 hover:underline text-primary"
+                },
+                size: {
+                    default: "h-10 py-2 px-4",
+                    sm: "h-9 px-3 rounded-md",
+                    xs: "py-1 px-1 rounded-md",
+                    lg: "h-11 px-8 rounded-md"
+                }
+            },
+            defaultVariants: {
+                variant: "default",
+                size: "default"
+            }
+        }),
+        Button = reactExports.forwardRef(({
+            className: j,
+            variant: $,
+            size: at,
+            asChild: st = !1,
+            ...ct
+        }, ut) => {
+            const dt = st ? $5e63c961fc1ce211$export$8c6ed5c666ac1360 : "button";
+            return jsxRuntimeExports.jsx(dt, {
+                className: cn(buttonVariants({
+                    variant: $,
+                    size: at,
+                    className: j
+                })),
+                ref: ut,
+                ...ct
+            })
+        });
+    Button.displayName = "Button";
+    const Card = reactExports.forwardRef(({
+        className: j,
+        ...$
+    }, at) => jsxRuntimeExports.jsx("div", {
+        ref: at,
+        className: cn("flex flex-col justify-between rounded-lg border bg-muted text-card-foreground shadow-sm transition-all hover:shadow-lg", j),
+        ...$
+    }));
+    Card.displayName = "Card";
+    const CardHeader = reactExports.forwardRef(({
+        className: j,
+        ...$
+    }, at) => jsxRuntimeExports.jsx("div", {
+        ref: at,
+        className: cn("flex flex-col space-y-1.5 p-4", j),
+        ...$
+    }));
+    CardHeader.displayName = "CardHeader";
+    const CardTitle = reactExports.forwardRef(({
+        className: j,
+        ...$
+    }, at) => jsxRuntimeExports.jsx("h3", {
+        ref: at,
+        className: cn("text-base font-semibold leading-tight tracking-tight", j),
+        ...$
+    }));
+    CardTitle.displayName = "CardTitle";
+    const CardDescription = reactExports.forwardRef(({
+        className: j,
+        ...$
+    }, at) => jsxRuntimeExports.jsx("div", {
+        ref: at,
+        className: cn("text-sm text-muted-foreground", j),
+        ...$
+    }));
+    CardDescription.displayName = "CardDescription";
+    const CardContent = reactExports.forwardRef(({
+        className: j,
+        ...$
+    }, at) => jsxRuntimeExports.jsx("div", {
+        ref: at,
+        className: cn("p-4 pt-0", j),
+        ...$
+    }));
+    CardContent.displayName = "CardContent";
+    const CardFooter = reactExports.forwardRef(({
+        className: j,
+        ...$
+    }, at) => jsxRuntimeExports.jsx("div", {
+        ref: at,
+        className: cn(" flex items-center p-4 pt-0", j),
+        ...$
+    }));
+    CardFooter.displayName = "CardFooter";
+
+    function CrashErrorComponent({
+        error: j,
+        resetErrorBoundary: $
+    }) {
+        return jsxRuntimeExports.jsx("div", {
+            className: "z-50 flex h-screen w-screen items-center justify-center bg-foreground bg-opacity-50",
+            children: jsxRuntimeExports.jsx("div", {
+                className: "flex h-screen w-screen flex-col  bg-background text-start shadow-lg",
+                children: jsxRuntimeExports.jsx("div", {
+                    className: "m-auto grid w-1/2 justify-center gap-5 text-center",
+                    children: jsxRuntimeExports.jsxs(Card, {
+                        className: "p-8",
+                        children: [jsxRuntimeExports.jsxs(CardHeader, {
+                            children: [jsxRuntimeExports.jsx("div", {
+                                className: "m-auto",
+                                children: jsxRuntimeExports.jsx(XCircle, {
+                                    strokeWidth: 1.5,
+                                    className: "h-16 w-16"
+                                })
+                            }), jsxRuntimeExports.jsx("div", {
+                                children: jsxRuntimeExports.jsx("p", {
+                                    className: "mb-4 text-xl text-foreground",
+                                    children: "Sorry, we found an unexpected error!"
+                                })
+                            })]
+                        }), jsxRuntimeExports.jsx(CardContent, {
+                            className: "grid",
+                            children: jsxRuntimeExports.jsx("div", {
+                                children: jsxRuntimeExports.jsxs("p", {
+                                    children: ["Please report errors with detailed tracebacks on the", " ", jsxRuntimeExports.jsx("a", {
+                                        href: "https://github.com/logspace-ai/langflow/issues",
+                                        target: "_blank",
+                                        rel: "noopener noreferrer",
+                                        className: "font-medium  hover:underline ",
+                                        children: "GitHub Issues"
+                                    }), " ", "page.", jsxRuntimeExports.jsx("br", {}), "Thank you!"]
+                                })
+                            })
+                        }), jsxRuntimeExports.jsx(CardFooter, {
+                            children: jsxRuntimeExports.jsxs("div", {
+                                className: "m-auto mt-4 flex justify-center",
+                                children: [jsxRuntimeExports.jsx(Button, {
+                                    onClick: $,
+                                    children: "Restart Langflow"
+                                }), jsxRuntimeExports.jsx("a", {
+                                    href: "https://github.com/logspace-ai/langflow/issues/new",
+                                    target: "_blank",
+                                    rel: "noopener noreferrer",
+                                    children: jsxRuntimeExports.jsx(Button, {
+                                        className: "ml-3",
+                                        variant: "outline",
+                                        children: "Report on GitHub"
+                                    })
+                                })]
+                            })
+                        })]
+                    })
+                })
+            })
+        })
+    }
+
+    function FetchErrorComponent({
+        message: j,
+        description: $
+    }) {
+        return jsxRuntimeExports.jsxs("div", {
+            role: "status",
+            className: "m-auto flex flex-col items-center",
+            children: [jsxRuntimeExports.jsx(IconComponent, {
+                className: "h-16 w-16",
+                name: "Unplug"
+            }), jsxRuntimeExports.jsx("br", {}), jsxRuntimeExports.jsx("span", {
+                className: "text-lg text-almost-medium-blue",
+                children: j
+            }), jsxRuntimeExports.jsx("span", {
+                className: "text-lg text-almost-medium-blue",
+                children: $
+            })]
+        })
+    }
+
+    function LoadingComponent({
+        remSize: j
+    }) {
+        return jsxRuntimeExports.jsxs("div", {
+            role: "status",
+            className: "flex flex-col items-center justify-center",
+            children: [jsxRuntimeExports.jsxs("svg", {
+                "aria-hidden": "true",
+                className: `w-${j} h-${j} animate-spin fill-almost-medium-blue  text-muted`,
+                viewBox: "0 0 100 101",
+                fill: "none",
+                xmlns: "http://www.w3.org/2000/svg",
+                children: [jsxRuntimeExports.jsx("path", {
+                    d: "M100 50.5908C100 78.2051 77.6142 100.591 50 100.591C22.3858 100.591 0 78.2051 0 50.5908C0 22.9766 22.3858 0.59082 50 0.59082C77.6142 0.59082 100 22.9766 100 50.5908ZM9.08144 50.5908C9.08144 73.1895 27.4013 91.5094 50 91.5094C72.5987 91.5094 90.9186 73.1895 90.9186 50.5908C90.9186 27.9921 72.5987 9.67226 50 9.67226C27.4013 9.67226 9.08144 27.9921 9.08144 50.5908Z",
+                    fill: "currentColor"
+                }), jsxRuntimeExports.jsx("path", {
+                    d: "M93.9676 39.0409C96.393 38.4038 97.8624 35.9116 97.0079 33.5539C95.2932 28.8227 92.871 24.3692 89.8167 20.348C85.8452 15.1192 80.8826 10.7238 75.2124 7.41289C69.5422 4.10194 63.2754 1.94025 56.7698 1.05124C51.7666 0.367541 46.6976 0.446843 41.7345 1.27873C39.2613 1.69328 37.813 4.19778 38.4501 6.62326C39.0873 9.04874 41.5694 10.4717 44.0505 10.1071C47.8511 9.54855 51.7191 9.52689 55.5402 10.0491C60.8642 10.7766 65.9928 12.5457 70.6331 15.2552C75.2735 17.9648 79.3347 21.5619 82.5849 25.841C84.9175 28.9121 86.7997 32.2913 88.1811 35.8758C89.083 38.2158 91.5421 39.6781 93.9676 39.0409Z",
+                    fill: "currentFill"
+                })]
+            }), jsxRuntimeExports.jsx("br", {}), jsxRuntimeExports.jsx("span", {
+                className: "animate-pulse text-lg text-almost-medium-blue",
+                children: "Loading..."
+            })]
+        })
+    }
     const ProtectedAdminRoute = ({
             children: j
         }) => {
             const {
                 isAdmin: $,
                 isAuthenticated: at,
                 logout: st,
@@ -32086,24 +32325,14 @@
         StoreGuard = ({
             children: j
         }) => useStoreStore(at => at.hasStore) ? j : jsxRuntimeExports.jsx(Navigate, {
             to: "/flows",
             replace: !0
         });
 
-    function _extends$9() {
-        return _extends$9 = Object.assign ? Object.assign.bind() : function(j) {
-            for (var $ = 1; $ < arguments.length; $++) {
-                var at = arguments[$];
-                for (var st in at) Object.prototype.hasOwnProperty.call(at, st) && (j[st] = at[st])
-            }
-            return j
-        }, _extends$9.apply(this, arguments)
-    }
-
     function $ae6933e535247d3d$export$7d15b64cf5a3a4c4(j, [$, at]) {
         return Math.min(at, Math.max($, j))
     }
 
     function $e42e1063c40fb3ef$export$b9ecd428b558ff10(j, $, {
         checkForDefaultPrevented: at = !0
     } = {}) {
@@ -32178,81 +32407,14 @@
                     [`__scope${$.scopeName}`]: dt
                 }), [dt])
             }
         };
         return at.scopeName = $.scopeName, at
     }
 
-    function $6ed0406888f73fc4$var$setRef(j, $) {
-        typeof j == "function" ? j($) : j != null && (j.current = $)
-    }
-
-    function $6ed0406888f73fc4$export$43e446d32b3d21af(...j) {
-        return $ => j.forEach(at => $6ed0406888f73fc4$var$setRef(at, $))
-    }
-
-    function $6ed0406888f73fc4$export$c7b2cbe3552a0d05(...j) {
-        return reactExports.useCallback($6ed0406888f73fc4$export$43e446d32b3d21af(...j), j)
-    }
-    const $5e63c961fc1ce211$export$8c6ed5c666ac1360 = reactExports.forwardRef((j, $) => {
-        const {
-            children: at,
-            ...st
-        } = j, ct = reactExports.Children.toArray(at), ut = ct.find($5e63c961fc1ce211$var$isSlottable);
-        if (ut) {
-            const dt = ut.props.children,
-                ft = ct.map(pt => pt === ut ? reactExports.Children.count(dt) > 1 ? reactExports.Children.only(null) : reactExports.isValidElement(dt) ? dt.props.children : null : pt);
-            return reactExports.createElement($5e63c961fc1ce211$var$SlotClone, _extends$9({}, st, {
-                ref: $
-            }), reactExports.isValidElement(dt) ? reactExports.cloneElement(dt, void 0, ft) : null)
-        }
-        return reactExports.createElement($5e63c961fc1ce211$var$SlotClone, _extends$9({}, st, {
-            ref: $
-        }), at)
-    });
-    $5e63c961fc1ce211$export$8c6ed5c666ac1360.displayName = "Slot";
-    const $5e63c961fc1ce211$var$SlotClone = reactExports.forwardRef((j, $) => {
-        const {
-            children: at,
-            ...st
-        } = j;
-        return reactExports.isValidElement(at) ? reactExports.cloneElement(at, {
-            ...$5e63c961fc1ce211$var$mergeProps(st, at.props),
-            ref: $ ? $6ed0406888f73fc4$export$43e446d32b3d21af($, at.ref) : at.ref
-        }) : reactExports.Children.count(at) > 1 ? reactExports.Children.only(null) : null
-    });
-    $5e63c961fc1ce211$var$SlotClone.displayName = "SlotClone";
-    const $5e63c961fc1ce211$export$d9f1ccf0bdb05d45 = ({
-        children: j
-    }) => reactExports.createElement(reactExports.Fragment, null, j);
-
-    function $5e63c961fc1ce211$var$isSlottable(j) {
-        return reactExports.isValidElement(j) && j.type === $5e63c961fc1ce211$export$d9f1ccf0bdb05d45
-    }
-
-    function $5e63c961fc1ce211$var$mergeProps(j, $) {
-        const at = {
-            ...$
-        };
-        for (const st in $) {
-            const ct = j[st],
-                ut = $[st];
-            /^on[A-Z]/.test(st) ? ct && ut ? at[st] = (...ft) => {
-                ut(...ft), ct(...ft)
-            } : ct && (at[st] = ct) : st === "style" ? at[st] = {
-                ...ct,
-                ...ut
-            } : st === "className" && (at[st] = [ct, ut].filter(Boolean).join(" "))
-        }
-        return {
-            ...j,
-            ...at
-        }
-    }
-
     function $e02a7d9cb1dc128c$export$c74125a8e3af6bb2(j) {
         const $ = j + "CollectionProvider",
             [at, st] = $c512c27ab02ef895$export$50c7b4e9d9f19c1($),
             [ct, ut] = at($, {
                 collectionRef: {
                     current: null
                 },
@@ -35762,92 +35924,14 @@
         ...$
     }, at) => jsxRuntimeExports.jsx($cc7e05a45900e73f$export$1ff3c3f08ae963c0, {
         ref: at,
         className: cn("-mx-1 my-1 h-px bg-muted", j),
         ...$
     }));
     SelectSeparator$1.displayName = $cc7e05a45900e73f$export$1ff3c3f08ae963c0.displayName;
-    const falsyToString = j => typeof j == "boolean" ? "".concat(j) : j === 0 ? "0" : j,
-        cx = clsx$2,
-        cva = (j, $) => at => {
-            var st;
-            if (($ == null ? void 0 : $.variants) == null) return cx(j, at == null ? void 0 : at.class, at == null ? void 0 : at.className);
-            const {
-                variants: ct,
-                defaultVariants: ut
-            } = $, dt = Object.keys(ct).map(Tt => {
-                const ht = at == null ? void 0 : at[Tt],
-                    mt = ut == null ? void 0 : ut[Tt];
-                if (ht === null) return null;
-                const Qt = falsyToString(ht) || falsyToString(mt);
-                return ct[Tt][Qt]
-            }), ft = at && Object.entries(at).reduce((Tt, ht) => {
-                let [mt, Qt] = ht;
-                return Qt === void 0 || (Tt[mt] = Qt), Tt
-            }, {}), pt = $ == null || (st = $.compoundVariants) === null || st === void 0 ? void 0 : st.reduce((Tt, ht) => {
-                let {
-                    class: mt,
-                    className: Qt,
-                    ...vt
-                } = ht;
-                return Object.entries(vt).every(xt => {
-                    let [yt, Et] = xt;
-                    return Array.isArray(Et) ? Et.includes({
-                        ...ut,
-                        ...ft
-                    } [yt]) : {
-                        ...ut,
-                        ...ft
-                    } [yt] === Et
-                }) ? [...Tt, mt, Qt] : Tt
-            }, []);
-            return cx(j, dt, pt, at == null ? void 0 : at.class, at == null ? void 0 : at.className)
-        },
-        buttonVariants = cva("inline-flex items-center justify-center rounded-md text-sm font-medium transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:opacity-50 disabled:pointer-events-none ring-offset-background", {
-            variants: {
-                variant: {
-                    default: "bg-primary text-primary-foreground hover:bg-primary/90",
-                    destructive: "bg-destructive text-destructive-foreground hover:bg-destructive/90",
-                    outline: "border border-input hover:bg-accent hover:text-accent-foreground",
-                    primary: "border bg-background text-secondary-foreground hover:bg-secondary-foreground/5 dark:hover:bg-background/10 hover:shadow-sm",
-                    secondary: "border border-muted bg-muted text-secondary-foreground hover:bg-secondary-foreground/5",
-                    ghost: "hover:bg-accent hover:text-accent-foreground",
-                    link: "underline-offset-4 hover:underline text-primary"
-                },
-                size: {
-                    default: "h-10 py-2 px-4",
-                    sm: "h-9 px-3 rounded-md",
-                    xs: "py-1 px-1 rounded-md",
-                    lg: "h-11 px-8 rounded-md"
-                }
-            },
-            defaultVariants: {
-                variant: "default",
-                size: "default"
-            }
-        }),
-        Button = reactExports.forwardRef(({
-            className: j,
-            variant: $,
-            size: at,
-            asChild: st = !1,
-            ...ct
-        }, ut) => {
-            const dt = st ? $5e63c961fc1ce211$export$8c6ed5c666ac1360 : "button";
-            return jsxRuntimeExports.jsx(dt, {
-                className: cn(buttonVariants({
-                    variant: $,
-                    size: at,
-                    className: j
-                })),
-                ref: ut,
-                ...ct
-            })
-        });
-    Button.displayName = "Button";
 
     function PaginatorComponent({
         pageSize: j = 12,
         pageIndex: $ = 1,
         rowsCount: at = [12, 24, 48, 96],
         totalRowsCount: st = 0,
         paginate: ct,
@@ -70790,15 +70874,15 @@
                                 className: "h-4 w-4"
                             })
                         })
                     }), ft && jsxRuntimeExports.jsx(ShadTooltip, {
                         content: !pt || !Tt ? "Set a valid API key to share this component." : "Share",
                         side: "top",
                         children: jsxRuntimeExports.jsx("button", {
-                            className: classNames("relative -ml-px inline-flex items-center bg-background px-2 py-2 text-foreground shadow-md ring-1 ring-inset ring-ring  transition-all duration-500 ease-in-out hover:bg-muted focus:z-10", !pt || !Tt ? " text-muted-foreground cursor-not-allowed" : ""),
+                            className: classNames("relative -ml-px inline-flex items-center bg-background px-2 py-2 text-foreground shadow-md ring-1 ring-inset ring-ring  transition-all duration-500 ease-in-out hover:bg-muted focus:z-10", !pt || !Tt ? " cursor-not-allowed text-muted-foreground" : ""),
                             onClick: Zt => {
                                 Zt.preventDefault(), pt && ft && Tt && _t(!0)
                             },
                             children: jsxRuntimeExports.jsx(IconComponent, {
                                 name: "Share3",
                                 className: "-m-1 h-6 w-6"
                             })
@@ -157014,18 +157098,18 @@
                 x: 0,
                 y: 0
             }),
             [$t, Pt] = reactExports.useState(null);
         reactExports.useEffect(() => {
             const sr = Mr => {
                     var _r;
-                    isWrappedWithClass$1(Mr, "noundo") || ((Mr.key === "y" || Mr.key === "z" && Mr.shiftKey) && (Mr.ctrlKey || Mr.metaKey) ? (Mr.preventDefault(), Ct()) : Mr.key === "z" && (Mr.ctrlKey || Mr.metaKey) && (Mr.preventDefault(), At())), !isWrappedWithClass$1(Mr, "nocopy") && ((_r = window.getSelection()) == null ? void 0 : _r.toString().length) === 0 && ((Mr.ctrlKey || Mr.metaKey) && Mr.key === "c" && $t ? (Mr.preventDefault(), Ot(_$1.cloneDeep($t))) : (Mr.ctrlKey || Mr.metaKey) && Mr.key === "x" && $t ? (Mr.preventDefault(), Ot(_$1.cloneDeep($t), !0)) : (Mr.ctrlKey || Mr.metaKey) && Mr.key === "v" && _t ? (Mr.preventDefault(), Mt(), St(_t, {
+                    isWrappedWithClass(Mr, "noundo") || ((Mr.key === "y" || Mr.key === "z" && Mr.shiftKey) && (Mr.ctrlKey || Mr.metaKey) ? (Mr.preventDefault(), Ct()) : Mr.key === "z" && (Mr.ctrlKey || Mr.metaKey) && (Mr.preventDefault(), At())), !isWrappedWithClass(Mr, "nocopy") && ((_r = window.getSelection()) == null ? void 0 : _r.toString().length) === 0 && ((Mr.ctrlKey || Mr.metaKey) && Mr.key === "c" && $t ? (Mr.preventDefault(), Ot(_$1.cloneDeep($t))) : (Mr.ctrlKey || Mr.metaKey) && Mr.key === "x" && $t ? (Mr.preventDefault(), Ot(_$1.cloneDeep($t), !0)) : (Mr.ctrlKey || Mr.metaKey) && Mr.key === "v" && _t ? (Mr.preventDefault(), Mt(), St(_t, {
                         x: Ht.current.x,
                         y: Ht.current.y
-                    })) : (Mr.ctrlKey || Mr.metaKey) && Mr.key === "g" && $t && Mr.preventDefault()), isWrappedWithClass$1(Mr, "nodelete") || (Mr.key === "Delete" || Mr.key === "Backspace") && $t && (Mr.preventDefault(), Mt(), bt($t.nodes.map(tn => tn.id)), wt($t.edges.map(tn => tn.id)))
+                    })) : (Mr.ctrlKey || Mr.metaKey) && Mr.key === "g" && $t && Mr.preventDefault()), isWrappedWithClass(Mr, "nodelete") || (Mr.key === "Delete" || Mr.key === "Backspace") && $t && (Mr.preventDefault(), Mt(), bt($t.nodes.map(tn => tn.id)), wt($t.edges.map(tn => tn.id)))
                 },
                 Cr = Mr => {
                     Ht.current = {
                         x: Mr.clientX,
                         y: Mr.clientY
                     }
                 };
@@ -157476,68 +157560,14 @@
                             children: "Delete"
                         })]
                     })
                 })]
             })]
         })
     }
-    const Card = reactExports.forwardRef(({
-        className: j,
-        ...$
-    }, at) => jsxRuntimeExports.jsx("div", {
-        ref: at,
-        className: cn("flex flex-col justify-between rounded-lg border bg-muted text-card-foreground shadow-sm transition-all hover:shadow-lg", j),
-        ...$
-    }));
-    Card.displayName = "Card";
-    const CardHeader = reactExports.forwardRef(({
-        className: j,
-        ...$
-    }, at) => jsxRuntimeExports.jsx("div", {
-        ref: at,
-        className: cn("flex flex-col space-y-1.5 p-4", j),
-        ...$
-    }));
-    CardHeader.displayName = "CardHeader";
-    const CardTitle = reactExports.forwardRef(({
-        className: j,
-        ...$
-    }, at) => jsxRuntimeExports.jsx("h3", {
-        ref: at,
-        className: cn("text-base font-semibold leading-tight tracking-tight", j),
-        ...$
-    }));
-    CardTitle.displayName = "CardTitle";
-    const CardDescription = reactExports.forwardRef(({
-        className: j,
-        ...$
-    }, at) => jsxRuntimeExports.jsx("div", {
-        ref: at,
-        className: cn("text-sm text-muted-foreground", j),
-        ...$
-    }));
-    CardDescription.displayName = "CardDescription";
-    const CardContent = reactExports.forwardRef(({
-        className: j,
-        ...$
-    }, at) => jsxRuntimeExports.jsx("div", {
-        ref: at,
-        className: cn("p-4 pt-0", j),
-        ...$
-    }));
-    CardContent.displayName = "CardContent";
-    const CardFooter = reactExports.forwardRef(({
-        className: j,
-        ...$
-    }, at) => jsxRuntimeExports.jsx("div", {
-        ref: at,
-        className: cn(" flex items-center p-4 pt-0", j),
-        ...$
-    }));
-    CardFooter.displayName = "CardFooter";
 
     function CollectionCardComponent({
         data: j,
         authorized: $ = !0,
         disabled: at = !1,
         button: st,
         onDelete: ct
@@ -159155,8 +159185,8 @@
         classes = "",
         root = client.createRoot(document.getElementById("root"));
     root.render(jsxRuntimeExports.jsx(ContextWrapper, {
         children: jsxRuntimeExports.jsx(App, {})
     }));
     reportWebVitals()
 });
-export default V9();
+export default zp();
```

### Comparing `langflow-0.6.8/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png` & `langflow-0.6.9/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/frontend/assets/robot-95e1b00d.png` & `langflow-0.6.9/src/backend/langflow/frontend/assets/robot-95e1b00d.png`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js` & `langflow-0.6.9/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/frontend/favicon.ico` & `langflow-0.6.9/src/backend/langflow/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/frontend/index.html` & `langflow-0.6.9/src/backend/langflow/frontend/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <link rel="icon" href="/favicon.ico" />
     <script src="/node_modules/ace-builds/src-min-noconflict/ace.js" type="text/javascript"></script>
     <title>Langflow</title>
-  <script type="module" crossorigin src="/assets/index-fef5028f.js"></script>
-  <link rel="stylesheet" href="/assets/index-c6d7fba2.css">
+  <script type="module" crossorigin src="/assets/index-3732b41f.js"></script>
+  <link rel="stylesheet" href="/assets/index-e7ca4585.css">
 </head>
 <body id='body' style="width: 100%; height:100%">
     <noscript>You need to enable JavaScript to run this app.</noscript>
     <div style="width: 100vw; height:100vh" id='root'></div>
     
 </body>
 </html>
```

### Comparing `langflow-0.6.8/src/backend/langflow/graph/__init__.py` & `langflow-0.6.9/src/backend/langflow/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/graph/edge/base.py` & `langflow-0.6.9/src/backend/langflow/graph/edge/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/graph/graph/base.py` & `langflow-0.6.9/src/backend/langflow/graph/graph/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/graph/graph/constants.py` & `langflow-0.6.9/src/backend/langflow/graph/graph/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/graph/graph/utils.py` & `langflow-0.6.9/src/backend/langflow/graph/graph/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/graph/utils.py` & `langflow-0.6.9/src/backend/langflow/graph/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/graph/vertex/base.py` & `langflow-0.6.9/src/backend/langflow/graph/vertex/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/graph/vertex/types.py` & `langflow-0.6.9/src/backend/langflow/graph/vertex/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/agents/base.py` & `langflow-0.6.9/src/backend/langflow/interface/agents/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/agents/custom.py` & `langflow-0.6.9/src/backend/langflow/interface/agents/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/agents/prebuilt.py` & `langflow-0.6.9/src/backend/langflow/interface/agents/prebuilt.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/base.py` & `langflow-0.6.9/src/backend/langflow/interface/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/chains/base.py` & `langflow-0.6.9/src/backend/langflow/interface/chains/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/chains/custom.py` & `langflow-0.6.9/src/backend/langflow/interface/chains/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/custom/base.py` & `langflow-0.6.9/src/backend/langflow/interface/custom/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/custom/code_parser/code_parser.py` & `langflow-0.6.9/src/backend/langflow/interface/custom/code_parser/code_parser.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/custom/code_parser/utils.py` & `langflow-0.6.9/src/backend/langflow/interface/custom/code_parser/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/custom/custom_component/component.py` & `langflow-0.6.9/src/backend/langflow/interface/custom/custom_component/component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/custom/custom_component/custom_component.py` & `langflow-0.6.9/src/backend/langflow/interface/custom/custom_component/custom_component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/custom/directory_reader/directory_reader.py` & `langflow-0.6.9/src/backend/langflow/interface/custom/directory_reader/directory_reader.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/custom/directory_reader/utils.py` & `langflow-0.6.9/src/backend/langflow/interface/custom/directory_reader/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/custom/schema.py` & `langflow-0.6.9/src/backend/langflow/interface/custom/schema.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/custom/utils.py` & `langflow-0.6.9/src/backend/langflow/interface/custom/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/custom_lists.py` & `langflow-0.6.9/src/backend/langflow/interface/custom_lists.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/document_loaders/base.py` & `langflow-0.6.9/src/backend/langflow/interface/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/embeddings/base.py` & `langflow-0.6.9/src/backend/langflow/interface/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/importing/utils.py` & `langflow-0.6.9/src/backend/langflow/interface/importing/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/initialize/loading.py` & `langflow-0.6.9/src/backend/langflow/interface/initialize/loading.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/initialize/utils.py` & `langflow-0.6.9/src/backend/langflow/interface/initialize/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/initialize/vector_store.py` & `langflow-0.6.9/src/backend/langflow/interface/initialize/vector_store.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/listing.py` & `langflow-0.6.9/src/backend/langflow/interface/listing.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/llms/base.py` & `langflow-0.6.9/src/backend/langflow/interface/llms/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/memories/base.py` & `langflow-0.6.9/src/backend/langflow/interface/memories/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/output_parsers/base.py` & `langflow-0.6.9/src/backend/langflow/interface/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/prompts/base.py` & `langflow-0.6.9/src/backend/langflow/interface/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/prompts/custom.py` & `langflow-0.6.9/src/backend/langflow/interface/prompts/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/retrievers/base.py` & `langflow-0.6.9/src/backend/langflow/interface/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/run.py` & `langflow-0.6.9/src/backend/langflow/interface/run.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/text_splitters/base.py` & `langflow-0.6.9/src/backend/langflow/interface/text_splitters/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/toolkits/base.py` & `langflow-0.6.9/src/backend/langflow/interface/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/tools/base.py` & `langflow-0.6.9/src/backend/langflow/interface/tools/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/tools/constants.py` & `langflow-0.6.9/src/backend/langflow/interface/tools/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/tools/custom.py` & `langflow-0.6.9/src/backend/langflow/interface/tools/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/tools/util.py` & `langflow-0.6.9/src/backend/langflow/interface/tools/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/types.py` & `langflow-0.6.9/src/backend/langflow/interface/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/utilities/base.py` & `langflow-0.6.9/src/backend/langflow/interface/utilities/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/utils.py` & `langflow-0.6.9/src/backend/langflow/interface/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/vector_store/base.py` & `langflow-0.6.9/src/backend/langflow/interface/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/interface/wrappers/base.py` & `langflow-0.6.9/src/backend/langflow/interface/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/main.py` & `langflow-0.6.9/src/backend/langflow/main.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/processing/base.py` & `langflow-0.6.9/src/backend/langflow/processing/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/processing/load.py` & `langflow-0.6.9/src/backend/langflow/processing/load.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/processing/process.py` & `langflow-0.6.9/src/backend/langflow/processing/process.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/server.py` & `langflow-0.6.9/src/backend/langflow/server.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/auth/utils.py` & `langflow-0.6.9/src/backend/langflow/services/auth/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/cache/base.py` & `langflow-0.6.9/src/backend/langflow/services/cache/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/cache/factory.py` & `langflow-0.6.9/src/backend/langflow/services/cache/factory.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/cache/service.py` & `langflow-0.6.9/src/backend/langflow/services/cache/service.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/cache/utils.py` & `langflow-0.6.9/src/backend/langflow/services/cache/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/chat/cache.py` & `langflow-0.6.9/src/backend/langflow/services/chat/cache.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/chat/service.py` & `langflow-0.6.9/src/backend/langflow/services/chat/service.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/chat/utils.py` & `langflow-0.6.9/src/backend/langflow/services/chat/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/credentials/service.py` & `langflow-0.6.9/src/backend/langflow/services/credentials/service.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/factory.py` & `langflow-0.6.9/src/backend/langflow/services/database/factory.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/models/api_key/crud.py` & `langflow-0.6.9/src/backend/langflow/services/database/models/api_key/crud.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/models/api_key/model.py` & `langflow-0.6.9/src/backend/langflow/services/database/models/api_key/model.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/models/base.py` & `langflow-0.6.9/src/backend/langflow/services/database/models/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/models/component/model.py` & `langflow-0.6.9/src/backend/langflow/services/database/models/component/model.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/models/credential/model.py` & `langflow-0.6.9/src/backend/langflow/services/database/models/credential/model.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/models/flow/model.py` & `langflow-0.6.9/src/backend/langflow/services/database/models/flow/model.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/models/user/crud.py` & `langflow-0.6.9/src/backend/langflow/services/database/models/user/crud.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/models/user/model.py` & `langflow-0.6.9/src/backend/langflow/services/database/models/user/model.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/service.py` & `langflow-0.6.9/src/backend/langflow/services/database/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import time
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import sqlalchemy as sa
 from alembic import command, util
 from alembic.config import Config
+from loguru import logger
+from sqlalchemy import inspect
+from sqlalchemy.exc import OperationalError
+from sqlmodel import Session, SQLModel, create_engine, select, text
+
 from langflow.services.base import Service
 from langflow.services.database import models  # noqa
 from langflow.services.database.models.user.crud import get_user_by_username
 from langflow.services.database.utils import Result, TableResults
 from langflow.services.deps import get_settings_service
 from langflow.services.utils import teardown_superuser
-from loguru import logger
-from sqlalchemy import inspect
-from sqlalchemy.exc import OperationalError
-from sqlmodel import Session, SQLModel, create_engine, select, text
 
 if TYPE_CHECKING:
     from sqlalchemy.engine import Engine
 
 
 class DatabaseService(Service):
     name = "database_service"
@@ -106,59 +107,63 @@
 
         for table in legacy_tables:
             if table in inspector.get_table_names():
                 logger.warning(f"Legacy table exists: {table}")
 
         return True
 
-    def init_alembic(self):
+    def init_alembic(self, alembic_cfg):
         logger.info("Initializing alembic")
-        alembic_cfg = Config()
-        alembic_cfg.set_main_option("script_location", str(self.script_location))
-        alembic_cfg.set_main_option("sqlalchemy.url", self.database_url)
-        command.stamp(alembic_cfg, "head")
-        # command.upgrade(alembic_cfg, "head")
+        command.ensure_version(alembic_cfg)
+        # alembic_cfg.attributes["connection"].commit()
+        command.upgrade(alembic_cfg, "head")
         logger.info("Alembic initialized")
 
     def run_migrations(self, fix=False):
         # First we need to check if alembic has been initialized
         # If not, we need to initialize it
         # if not self.script_location.exists(): # this is not the correct way to check if alembic has been initialized
         # We need to check if the alembic_version table exists
         # if not, we need to initialize alembic
+        alembic_cfg = Config()
+        # alembic_cfg.attributes["connection"] = session
+        alembic_cfg.set_main_option("script_location", str(self.script_location))
+        alembic_cfg.set_main_option("sqlalchemy.url", self.database_url)
+        should_initialize_alembic = False
         with Session(self.engine) as session:
             # If the table does not exist it throws an error
             # so we need to catch it
             try:
                 session.exec(text("SELECT * FROM alembic_version"))
             except Exception:
                 logger.info("Alembic not initialized")
-                try:
-                    self.init_alembic()
-                except Exception as exc:
-                    logger.error(f"Error initializing alembic: {exc}")
-                    raise RuntimeError("Error initializing alembic") from exc
+                should_initialize_alembic = True
+
             else:
                 logger.info("Alembic already initialized")
+        if should_initialize_alembic:
+            try:
+                self.init_alembic(alembic_cfg)
+            except Exception as exc:
+                logger.error(f"Error initializing alembic: {exc}")
+                raise RuntimeError("Error initializing alembic") from exc
 
         logger.info(f"Running DB migrations in {self.script_location}")
-        alembic_cfg = Config()
-        alembic_cfg.set_main_option("script_location", str(self.script_location))
-        alembic_cfg.set_main_option("sqlalchemy.url", self.database_url)
+
         try:
             command.check(alembic_cfg)
         except Exception as exc:
             if isinstance(exc, (util.exc.CommandError, util.exc.AutogenerateDiffsDetected)):
                 command.upgrade(alembic_cfg, "head")
                 time.sleep(3)
 
         try:
             command.check(alembic_cfg)
         except util.exc.AutogenerateDiffsDetected as e:
-            logger.exception("AutogenerateDiffsDetected: {exc}")
+            logger.error("AutogenerateDiffsDetected: {exc}")
             if not fix:
                 raise RuntimeError(
                     "Something went wrong running migrations. Please, run `langflow migration --fix`"
                 ) from e
 
         if fix:
             self.try_downgrade_upgrade_until_success(alembic_cfg)
```

### Comparing `langflow-0.6.8/src/backend/langflow/services/database/utils.py` & `langflow-0.6.9/src/backend/langflow/services/database/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/deps.py` & `langflow-0.6.9/src/backend/langflow/services/deps.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/manager.py` & `langflow-0.6.9/src/backend/langflow/services/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/plugins/langfuse_plugin.py` & `langflow-0.6.9/src/backend/langflow/services/plugins/langfuse_plugin.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/plugins/service.py` & `langflow-0.6.9/src/backend/langflow/services/plugins/service.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/schema.py` & `langflow-0.6.9/src/backend/langflow/services/schema.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/session/service.py` & `langflow-0.6.9/src/backend/langflow/services/session/service.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/session/utils.py` & `langflow-0.6.9/src/backend/langflow/services/session/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/settings/auth.py` & `langflow-0.6.9/src/backend/langflow/services/settings/auth.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/settings/base.py` & `langflow-0.6.9/src/backend/langflow/services/settings/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/settings/service.py` & `langflow-0.6.9/src/backend/langflow/services/settings/service.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/settings/utils.py` & `langflow-0.6.9/src/backend/langflow/services/settings/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/store/exceptions.py` & `langflow-0.6.9/src/backend/langflow/services/store/exceptions.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/store/schema.py` & `langflow-0.6.9/src/backend/langflow/services/store/schema.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/store/service.py` & `langflow-0.6.9/src/backend/langflow/services/store/service.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/store/utils.py` & `langflow-0.6.9/src/backend/langflow/services/store/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/task/backends/anyio.py` & `langflow-0.6.9/src/backend/langflow/services/task/backends/anyio.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/task/backends/celery.py` & `langflow-0.6.9/src/backend/langflow/services/task/backends/celery.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/task/service.py` & `langflow-0.6.9/src/backend/langflow/services/task/service.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/task/utils.py` & `langflow-0.6.9/src/backend/langflow/services/task/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/services/utils.py` & `langflow-0.6.9/src/backend/langflow/services/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,32 @@
+from loguru import logger
+from sqlmodel import Session, select
+
 from langflow.services.auth.utils import create_super_user, verify_password
 from langflow.services.database.utils import initialize_database
 from langflow.services.manager import service_manager
 from langflow.services.schema import ServiceType
-from langflow.services.settings.constants import DEFAULT_SUPERUSER, DEFAULT_SUPERUSER_PASSWORD
-from loguru import logger
-from sqlmodel import Session, select
+from langflow.services.settings.constants import (
+    DEFAULT_SUPERUSER,
+    DEFAULT_SUPERUSER_PASSWORD,
+)
 
 from .deps import get_db_service, get_session, get_settings_service
 
 
 def get_factories_and_deps():
     from langflow.services.auth import factory as auth_factory
     from langflow.services.cache import factory as cache_factory
     from langflow.services.chat import factory as chat_factory
     from langflow.services.credentials import factory as credentials_factory
     from langflow.services.database import factory as database_factory
     from langflow.services.plugins import factory as plugins_factory
-    from langflow.services.session import factory as session_service_factory  # type: ignore
+    from langflow.services.session import (
+        factory as session_service_factory,
+    )  # type: ignore
     from langflow.services.settings import factory as settings_factory
     from langflow.services.store import factory as store_factory
     from langflow.services.task import factory as task_factory
 
     return [
         (settings_factory.SettingsServiceFactory(), []),
         (
@@ -39,15 +45,18 @@
         (task_factory.TaskServiceFactory(), []),
         (
             session_service_factory.SessionServiceFactory(),
             [ServiceType.CACHE_SERVICE],
         ),
         (plugins_factory.PluginServiceFactory(), [ServiceType.SETTINGS_SERVICE]),
         (store_factory.StoreServiceFactory(), [ServiceType.SETTINGS_SERVICE]),
-        (credentials_factory.CredentialServiceFactory(), [ServiceType.SETTINGS_SERVICE]),
+        (
+            credentials_factory.CredentialServiceFactory(),
+            [ServiceType.SETTINGS_SERVICE],
+        ),
     ]
 
 
 def get_or_create_super_user(session: Session, username, password, is_default):
     from langflow.services.database.models.user.model import User
 
     user = session.exec(select(User).where(User.username == username)).first()
@@ -169,15 +178,17 @@
 
 
 def initialize_session_service():
     """
     Initialize the session manager.
     """
     from langflow.services.cache import factory as cache_factory
-    from langflow.services.session import factory as session_service_factory  # type: ignore
+    from langflow.services.session import (
+        factory as session_service_factory,
+    )  # type: ignore
 
     initialize_settings_service()
 
     service_manager.register_factory(cache_factory.CacheServiceFactory(), dependencies=[ServiceType.SETTINGS_SERVICE])
 
     service_manager.register_factory(
         session_service_factory.SessionServiceFactory(),
@@ -198,15 +209,15 @@
 
     # Test cache connection
     service_manager.get(ServiceType.CACHE_SERVICE)
     # Setup the superuser
     try:
         initialize_database(fix_migration=fix_migration)
     except Exception as exc:
-        logger.exception(exc)
+        logger.error(exc)
         raise exc
     setup_superuser(service_manager.get(ServiceType.SETTINGS_SERVICE), next(get_session()))
     try:
         get_db_service().migrate_flows_if_auto_login()
     except Exception as exc:
         logger.error(f"Error migrating flows: {exc}")
         raise RuntimeError("Error migrating flows") from exc
```

### Comparing `langflow-0.6.8/src/backend/langflow/settings.py` & `langflow-0.6.9/src/backend/langflow/settings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/field/base.py` & `langflow-0.6.9/src/backend/langflow/template/field/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/agents.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/agents.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/base.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/chains.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/chains.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/constants.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/custom_components.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/custom_components.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/documentloaders.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/documentloaders.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/embeddings.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/embeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/formatter/field_formatters.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/formatter/field_formatters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/llms.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/llms.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/memories.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/memories.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/prompts.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/prompts.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/retrievers.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/retrievers.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/textsplitters.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/textsplitters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/tools.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/tools.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/utilities.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/utilities.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/frontend_node/vectorstores.py` & `langflow-0.6.9/src/backend/langflow/template/frontend_node/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/template/template/base.py` & `langflow-0.6.9/src/backend/langflow/template/template/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/utils/constants.py` & `langflow-0.6.9/src/backend/langflow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/utils/logger.py` & `langflow-0.6.9/src/backend/langflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/utils/payload.py` & `langflow-0.6.9/src/backend/langflow/utils/payload.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/utils/util.py` & `langflow-0.6.9/src/backend/langflow/utils/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/utils/validate.py` & `langflow-0.6.9/src/backend/langflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/src/backend/langflow/worker.py` & `langflow-0.6.9/src/backend/langflow/worker.py`

 * *Files identical despite different names*

### Comparing `langflow-0.6.8/PKG-INFO` & `langflow-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 0.6.8
+Version: 0.6.9
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Carlos Coelho
```

