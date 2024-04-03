# Comparing `tmp/chat_cli_anything-0.1.3.tar.gz` & `tmp/chat_cli_anything-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_cli_anything-0.1.3.tar", max compression
+gzip compressed data, was "chat_cli_anything-0.1.4.tar", max compression
```

## Comparing `chat_cli_anything-0.1.3.tar` & `chat_cli_anything-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-13 16:33:27.236056 chat_cli_anything-0.1.3/LICENSE
--rw-r--r--   0        0        0     6607 2024-04-02 02:18:28.290235 chat_cli_anything-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-03-20 12:50:07.078680 chat_cli_anything-0.1.3/chat_cli_anything/__init__.py
--rw-r--r--   0        0        0    28955 2024-04-03 08:40:52.276963 chat_cli_anything-0.1.3/chat_cli_anything/ask.py
--rw-r--r--   0        0        0     6896 2024-04-03 05:20:02.168901 chat_cli_anything-0.1.3/chat_cli_anything/config.py
--rw-r--r--   0        0        0     7928 2024-04-03 05:20:24.146595 chat_cli_anything-0.1.3/chat_cli_anything/db.py
--rw-r--r--   0        0        0     1616 2024-04-01 13:09:38.160887 chat_cli_anything-0.1.3/chat_cli_anything/embedding.py
--rw-r--r--   0        0        0     2798 2024-04-03 06:48:40.337190 chat_cli_anything-0.1.3/chat_cli_anything/loader.py
--rw-r--r--   0        0        0     2714 2024-04-03 07:17:55.368638 chat_cli_anything-0.1.3/chat_cli_anything/request.py
--rw-r--r--   0        0        0      729 2024-03-31 17:35:50.217211 chat_cli_anything-0.1.3/chat_cli_anything/rerank.py
--rw-r--r--   0        0        0     1868 2024-04-01 08:49:00.737620 chat_cli_anything-0.1.3/chat_cli_anything/service.py
--rw-r--r--   0        0        0     1050 2024-04-02 06:30:30.360008 chat_cli_anything-0.1.3/chat_cli_anything/util.py
--rw-r--r--   0        0        0     1448 2024-04-03 07:05:53.661098 chat_cli_anything-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8110 1970-01-01 00:00:00.000000 chat_cli_anything-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-13 16:33:27.236056 chat_cli_anything-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7696 2024-04-03 09:54:05.392800 chat_cli_anything-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 12:50:07.078680 chat_cli_anything-0.1.4/chat_cli_anything/__init__.py
+-rw-r--r--   0        0        0    28974 2024-04-03 09:59:28.022343 chat_cli_anything-0.1.4/chat_cli_anything/ask.py
+-rw-r--r--   0        0        0     6896 2024-04-03 05:20:02.168901 chat_cli_anything-0.1.4/chat_cli_anything/config.py
+-rw-r--r--   0        0        0     7876 2024-04-03 09:16:53.301015 chat_cli_anything-0.1.4/chat_cli_anything/db.py
+-rw-r--r--   0        0        0     1621 2024-04-03 09:17:55.507727 chat_cli_anything-0.1.4/chat_cli_anything/embedding.py
+-rw-r--r--   0        0        0     2798 2024-04-03 06:48:40.337190 chat_cli_anything-0.1.4/chat_cli_anything/loader.py
+-rw-r--r--   0        0        0     2714 2024-04-03 07:17:55.368638 chat_cli_anything-0.1.4/chat_cli_anything/request.py
+-rw-r--r--   0        0        0      729 2024-03-31 17:35:50.217211 chat_cli_anything-0.1.4/chat_cli_anything/rerank.py
+-rw-r--r--   0        0        0     1868 2024-04-01 08:49:00.737620 chat_cli_anything-0.1.4/chat_cli_anything/service.py
+-rw-r--r--   0        0        0     1050 2024-04-02 06:30:30.360008 chat_cli_anything-0.1.4/chat_cli_anything/util.py
+-rw-r--r--   0        0        0     1465 2024-04-03 10:15:53.523917 chat_cli_anything-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9237 1970-01-01 00:00:00.000000 chat_cli_anything-0.1.4/PKG-INFO
```

### Comparing `chat_cli_anything-0.1.3/LICENSE` & `chat_cli_anything-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.3/README.md` & `chat_cli_anything-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,363 +1,417 @@
 ![chat-cli-anything](./logo.png)
 
 # Chat-Cli-Anything
 
-Interact with GPT-like services from the command line, supports local RAG, and pipe input.
+Interact with GPT-like services from the command line, supporting local RAG and pipe input.
+
+Why:
+① A significant portion of a developer's time is spent interacting with the system through the terminal. When encountering issues in the terminal, they expect to resolve them without having to switch to a search engine or another application.
+② By combining the language model's excellent text capabilities and text processing abilities, it helps us achieve code generation, explanation, and translation, as well as document Q&A, beyond simple searches.
 
 ## Tutorial
 
 1. Installation
 
 ```shell
 pip install "chat-cli-anything[all]"
 ```
 
-To simplify command length, set command aliases (optional)
+To simplify command length, you can set command aliases (optional):
 
 ```shell
+# put this in your ~/.bashrc or ~/.zshrc
 alias config="cc-config"
 alias code="cc-code"
 alias chat="cc-chat"
 alias db="cc-db"
 alias service="cc-service"
 ```
 
 2. Add LLM provider
 
 ```
 cc-config add "openai" "https://api.openai.com/v1"  --api-key "your-api-key"
 ```
 
-If command aliases are set
+If command aliases are already set:
 
 ```
 config add "openai" "https://api.openai.com/v1"  --api-key "your-api-key"
 ```
 
 3. Start Using
 
-*example1* Normal question
+**Example 1**: General question
 
 ```
 cc-ask "Who is the author of the science fiction novel 'Three Body'?"
 ```
 
-*example2* Using pipe
+```
+cc-ask "How to get the memory size occupied by a process in Linux?"
+```
+
+**Example 2**: Using pipe
 
 ```
 cat names_of_diseases.txt | cc-ask "What are the most common types of diseases among the names listed?"
 ```
 
-*example3* Interactive questioning
+**Example 3**: Interactive questioning
 
 ```
 cc-chat "What is the capital of France?"
 ```
 
-*example4* Local RAG
+**Example 4**: Local document Q&A
 
-step 1: Digest text to build a local database
+```
+cc-ask "Which school did the candidate graduate from?" -f resume.pdf
+```
+
+**Example 5**: Local document collection
+
+Step 1: Digest text to build a local database
 
 ```
-cc-db ingest "/path/to/西游记.txt" -n xiyouji
+# d2light code
+cc-db ingest "/path/to/detectron2-light" -n d2light
 ```
 
-step 2: Ask a question
+Step 2: Ask a question
 
 ```
 # for open question, '-a/--advance' option would be helpful
-cc-ask -d xiyouji "孙悟空一打白骨精的时候说了啥" -a
+cc-ask -d d2light "DETR implementation" -a
 ```
 
+**Example 6**: Code review
 
-## Commands
+```
+# Explain line by line
+cc-code review /path/to/your/code.py -l
+
+# If the code is lengthy, continue generating
+cc-code review /path/to/your/code.py -l -c
+```
+
+## Command Explanation
 
 ### cc-config
+
 Configure LLM provider
 
 #### 1. Add LLM provider
 
 ```
 cc-config add [OPTIONS] NAME BASE_URL
 
 Options:
   --model TEXT
   --api-key TEXT
   --proxy TEXT
   --help          Show this message and exit.
 ```
 
-example:
+Example:
 
 ```
 cc-config add "openai" "https://api.openai.com/v1"  --model "gpt-3.5-turbo-1106" --api-key "sk-xxxxxxxxxxx"
 ```
 
 #### 2. Test provider
+
 ```
 cc-config ping [OPTIONS] NAME
 
-  Switch to a different configuration and save the change.
+Switch to a different configuration and save the change.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### 3. List all providers
 
 ```
 cc-config list [OPTIONS]
 
-  List all configurations.
+List all configurations.
 
 Options:
   -s, --show-api-key
   --help              Show this message and exit.
 ```
-The default api-key is hidden, use `-s/--show-api-key` to display the key.
+
+The default api-key is hidden; use `-s/--show-api-key` to display the key.
 
 #### 4. Remove provider
+
 ```
 cc-config remove [OPTIONS] [NAME]
 
-  Remove a configuration.
+Remove a configuration.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### 5. Switch active provider
+
 ```
 ask.py cc-config switch [OPTIONS] NAME
 
-  Switch to a different configuration and save the change.
+Switch to a different configuration and save the change.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### 6. Load configuration file
+
 ```
 Import configurations.
 
 Options:
-  -o, --override  Whether override original config.
+  -o, --override  Whether to override the original config.
   --help          Show this message and exit.
 ```
 
 #### 7. Export configuration file
+
 ```
 ask.py cc-config dump [OPTIONS] PATH
 
-  Export current configurations.
+Export current configurations.
 
 Options:
-  -o, --override  Whether override existing file.
+  -o, --override  Whether to override the existing file.
   --help          Show this message and exit.
 ```
 
 ### cc-ask
 
 Perform a question-answering task
+
 ```
 cc-ask [OPTIONS] QUERY
 
-  Start a chat session with the given query.
+Start a chat session with the given query.
 
 Options:
   -d, --db TEXT        Name of database.
   -f, --filename TEXT  Name of file.
   -r, --rerank         Whether to rerank the results.
   -s, --show-chunks    Whether to show the related chunks retrieved from
-                       database.
-  -a, --advance        Whether to use advance RAG.
+                       the database.
+  -a, --advance        Whether to use advanced RAG.
   --help               Show this message and exit.
 ```
 
 ### cc-chat
+
 Interactive Q&A
+
 ```
 cc-chat [OPTIONS] [QUERY]
 
-  Interactive chat. Enter '/quit' to exit
+Interactive chat. Enter '/quit' to exit.
 
 Options:
-  -d, --db TEXT          name of database.
-  -f, --filename TEXT    Name of file.
+  -d, --db TEXT          Name of the database.
+  -f, --filename TEXT    Name of the file.
   -n, --not-interactive
   -s, --show-history
   -c, --clear
   --help                 Show this message and exit.
 ```
 
 ### cc-code
+
 Some common commands for code based on cc-ask.
 
 #### Code Explanation
 
 ```
 cc-code explain [OPTIONS] [FILENAME] [OBJECT_NAME]
 
-  Explain code.
+Explain code.
 
 Options:
   --help  Show this message and exit.
 ```
 
-example1: Specify filename
+Example 1: Specify filename
+
 ```
 cc-code explain some_complex_scripts.py
 ```
 
-example2: Specify a particular function
+Example 2: Specify a particular function
+
 ```
 cc-code explain some_complex_scripts.py SomeClass::some_function
 ```
 
-example3: Use pipe
+Example 3: Use pipe
+
 ```
 cat some_complex_scripts.py | cc-code explain
 ```
 
 #### Fix Issues
+
 ```
 cc-code fix [OPTIONS] [FILENAME] [OBJECT_NAME]
 
-  Fix code.
+Fix code.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### Code Refactoring
+
 ```
 cc-code refactor [OPTIONS] [FILENAME] [OBJECT_NAME]
 
-  Refactor code.
+Refactor code.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### Code Review
+
 ```
 cc-code review [OPTIONS] [FILENAME] [OBJECT_NAME]
 
-  Review code.
+Review code.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### Code Translation
+
 ```
 cc-code translate [OPTIONS] [FILENAME] [OBJECT_NAME] LANGUAGE
 
-  Translate code from one language to another. Supported languages include c++, cpp,
-  c, rust, typescript, javascript, markdown, html.
+Translate code from one language to another. Supported languages include c++, cpp,
+c, rust, typescript, javascript, markdown, html.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### Select Code from Generated Results
 
-Used to select code snippets from the generated responses of the above commands
+Used to select code snippets from the generated responses of the above commands.
 
 ```
 cc-code select [OPTIONS] [INDEX]
 
-  Select code snippet from last output.
+Select code snippet from the last output.
 
-  Argument:     index: code snippet index
+Argument: index: code snippet index
 
 Options:
-  -c, --count  get the number of code snippets
+  -c, --count  Get the number of code snippets
   --help       Show this message and exit.
 ```
 
-`-c/--count` Get the number of candidate code blocks in the last response
+`-c/--count` Get the number of candidate code blocks in the last response.
+
+Example:
 
-example:
 ```
 >>> cc-code select -c
 2
 
 # Select the second code block from the last output
-# for macos
+# For macOS
 >>> cc-code select 1 | pbcopy
-# for linux
+# For Linux
 >>> cc-code select 1 | xclip -selection clipboard
 ```
 
 ### cc-db
 
 #### list: List all text collections
+
 ```
 cc-db list [OPTIONS] [NAME]
 
-  List all document databases
+List all document databases.
 
 Options:
-  -s, --short  List in short format
+  -s, --short  List in short format.
   --help       Show this message and exit.
 ```
 
 #### ingest: Digest documents
+
 ```
 cc-db ingest [OPTIONS] [FILES]...
 
-  Read documents and convert them into a searchable database.
+Read documents and convert them into a searchable database.
 
 Options:
   -n, --name TEXT     The name of the knowledge base.
-  -m, --comment TEXT  Add comment to info
+  -m, --comment TEXT  Add comment to info.
   --help              Show this message and exit.
 ```
 
-#### remove: Remove text collection
+#### remove: Remove document collection
+
 ```
 cc-db remove [OPTIONS] NAME
 
-  Remove database with the given name.
+Remove database with the given name.
 
 Options:
-  -d, --remove-documents  Remove documents if data
+  -d, --remove-documents  Remove documents if data.
   --help                  Show this message and exit.
 ```
 
 #### search: Search within a document collection
+
 ```
 cc-db search [OPTIONS] DB QUERY
 
 Options:
   -k, --topk INTEGER  Number of top results to return.
   --help              Show this message and exit.
 ```
 
 ### cc-service
-Used to manage local text-to-index services
+
+Used to manage local text-to-index services.
 
 #### start:
+
 ```
 cc-service start [OPTIONS]
 
 Options:
   --help  Show this message and exit.
 ```
 
+The process will take some time to load the model (~1min), determine if it has started with `cc-service status`.
+
 #### stop:
+
 ```
 cc-service stop [OPTIONS]
 
 Options:
   --help  Show this message and exit.
 ```
 
-#### status
+#### status:
+
 ```
 cc-service status [OPTIONS]
 
 Options:
   --help  Show this message and exit.
-```
+```
```

### Comparing `chat_cli_anything-0.1.3/chat_cli_anything/ask.py` & `chat_cli_anything-0.1.4/chat_cli_anything/ask.py`

 * *Files 0% similar despite different names*

```diff
@@ -687,15 +687,15 @@
 
 
 @db.command(name='search')
 @click.argument('db', type=str)
 @click.argument('query', type=str)
 @click.option('-k', '--topk', type=int, default=5, help='Number of top results to return.')
 def search(db: str, query: str, topk: int):
-    """"""
+    """Search in database."""
     from chat_cli_anything.db import load_vectorstore
     _db = db
     status, db = load_vectorstore(db)
     if status:
         check_and_start_service()
     else:
         click.secho(f"The '{_db}' does not exist.", fg='red')
```

### Comparing `chat_cli_anything-0.1.3/chat_cli_anything/config.py` & `chat_cli_anything-0.1.4/chat_cli_anything/config.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.3/chat_cli_anything/db.py` & `chat_cli_anything-0.1.4/chat_cli_anything/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,17 +204,15 @@
                                         kb_path=str(kb_path),
                                         file_path=file,
                                         modified_time=modified_datetime)
 
             session.add(new_index_info)
 
         set_doc_exists = 'document_set' in inspector.get_table_names()
-        print('here')
         if not (set_doc_exists and session.query(SetOfDocumentDB).filter(SetOfDocumentDB.name == name, SetOfDocumentDB.hash == hash_key).first()):
-            print('add item')
             session.add(SetOfDocumentDB(hash=hash_key, name=name))
 
     # update document set table 
     session.commit() 
     return True, 'Successfully created.'
```

### Comparing `chat_cli_anything-0.1.3/chat_cli_anything/embedding.py` & `chat_cli_anything-0.1.4/chat_cli_anything/embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def __init__(self, port: int) -> None:
         self.port = port
         super().__init__()
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         response = requests.post(
             f'http://localhost:{self.port}/embed_documents',
-            timeout=10 * len(texts),
+            timeout=10 * len(texts) + 10,
             json=[{'text': text} for text in texts]
         )
         return [r['embedding'] for r in response.json()]
 
     def embed_query(self, text: str) -> List[float]:
         response = requests.post(
             f'http://localhost:{self.port}/embedding',
```

### Comparing `chat_cli_anything-0.1.3/chat_cli_anything/loader.py` & `chat_cli_anything-0.1.4/chat_cli_anything/loader.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.3/chat_cli_anything/request.py` & `chat_cli_anything-0.1.4/chat_cli_anything/request.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.3/chat_cli_anything/rerank.py` & `chat_cli_anything-0.1.4/chat_cli_anything/rerank.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.3/chat_cli_anything/service.py` & `chat_cli_anything-0.1.4/chat_cli_anything/service.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.3/chat_cli_anything/util.py` & `chat_cli_anything-0.1.4/chat_cli_anything/util.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.3/pyproject.toml` & `chat_cli_anything-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chat-cli-anything"
-version = "0.1.3"
+version = "0.1.4"
 description = "Chat with anything on cli."
 authors = ["liuping <liuping@shukun.net>"]
 license = "Apache"
 readme = "README.md"
 keywords = ["chatgpt", "cli", "chat"]
 packages = [{ include = "chat_cli_anything" }]
 
@@ -25,14 +25,15 @@
 langchain-community = {version = "^0.0.29", optional = true}
 langchain = {version = "^0.1.13", optional = true}
 flagembedding = {version = "^1.2.8", optional = true}
 torch = {version = "^2.2.2", optional = true}
 langchain-openai = {version = "^0.1.1", optional = true}
 langchain-text-splitters = {version = "^0.0.1", optional = true}
 tiktoken = "^0.6.0"
+tqdm = "^4.66.2"
 
 [tool.poetry.group.dev.dependencies]
 openai = "^1.13.3"
 
 
 [tool.poetry.extras]
 all = ["flagembedding", "torch", "langchain",  "langchain-community", "langchain-openai", "langchain-text-splitters"]
```

### Comparing `chat_cli_anything-0.1.3/PKG-INFO` & `chat_cli_anything-0.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-cli-anything
-Version: 0.1.3
+Version: 0.1.4
 Summary: Chat with anything on cli.
 License: Apache
 Keywords: chatgpt,cli,chat
 Author: liuping
 Author-email: liuping@shukun.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -27,375 +27,429 @@
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pypdf (>=4.1.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0) ; extra == "all"
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Requires-Dist: xonsh (>=0.15.1,<0.16.0)
 Description-Content-Type: text/markdown
 
 ![chat-cli-anything](./logo.png)
 
 # Chat-Cli-Anything
 
-Interact with GPT-like services from the command line, supports local RAG, and pipe input.
+Interact with GPT-like services from the command line, supporting local RAG and pipe input.
+
+Why:
+① A significant portion of a developer's time is spent interacting with the system through the terminal. When encountering issues in the terminal, they expect to resolve them without having to switch to a search engine or another application.
+② By combining the language model's excellent text capabilities and text processing abilities, it helps us achieve code generation, explanation, and translation, as well as document Q&A, beyond simple searches.
 
 ## Tutorial
 
 1. Installation
 
 ```shell
 pip install "chat-cli-anything[all]"
 ```
 
-To simplify command length, set command aliases (optional)
+To simplify command length, you can set command aliases (optional):
 
 ```shell
+# put this in your ~/.bashrc or ~/.zshrc
 alias config="cc-config"
 alias code="cc-code"
 alias chat="cc-chat"
 alias db="cc-db"
 alias service="cc-service"
 ```
 
 2. Add LLM provider
 
 ```
 cc-config add "openai" "https://api.openai.com/v1"  --api-key "your-api-key"
 ```
 
-If command aliases are set
+If command aliases are already set:
 
 ```
 config add "openai" "https://api.openai.com/v1"  --api-key "your-api-key"
 ```
 
 3. Start Using
 
-*example1* Normal question
+**Example 1**: General question
 
 ```
 cc-ask "Who is the author of the science fiction novel 'Three Body'?"
 ```
 
-*example2* Using pipe
+```
+cc-ask "How to get the memory size occupied by a process in Linux?"
+```
+
+**Example 2**: Using pipe
 
 ```
 cat names_of_diseases.txt | cc-ask "What are the most common types of diseases among the names listed?"
 ```
 
-*example3* Interactive questioning
+**Example 3**: Interactive questioning
 
 ```
 cc-chat "What is the capital of France?"
 ```
 
-*example4* Local RAG
+**Example 4**: Local document Q&A
 
-step 1: Digest text to build a local database
+```
+cc-ask "Which school did the candidate graduate from?" -f resume.pdf
+```
+
+**Example 5**: Local document collection
+
+Step 1: Digest text to build a local database
 
 ```
-cc-db ingest "/path/to/西游记.txt" -n xiyouji
+# d2light code
+cc-db ingest "/path/to/detectron2-light" -n d2light
 ```
 
-step 2: Ask a question
+Step 2: Ask a question
 
 ```
 # for open question, '-a/--advance' option would be helpful
-cc-ask -d xiyouji "孙悟空一打白骨精的时候说了啥" -a
+cc-ask -d d2light "DETR implementation" -a
 ```
 
+**Example 6**: Code review
 
-## Commands
+```
+# Explain line by line
+cc-code review /path/to/your/code.py -l
+
+# If the code is lengthy, continue generating
+cc-code review /path/to/your/code.py -l -c
+```
+
+## Command Explanation
 
 ### cc-config
+
 Configure LLM provider
 
 #### 1. Add LLM provider
 
 ```
 cc-config add [OPTIONS] NAME BASE_URL
 
 Options:
   --model TEXT
   --api-key TEXT
   --proxy TEXT
   --help          Show this message and exit.
 ```
 
-example:
+Example:
 
 ```
 cc-config add "openai" "https://api.openai.com/v1"  --model "gpt-3.5-turbo-1106" --api-key "sk-xxxxxxxxxxx"
 ```
 
 #### 2. Test provider
+
 ```
 cc-config ping [OPTIONS] NAME
 
-  Switch to a different configuration and save the change.
+Switch to a different configuration and save the change.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### 3. List all providers
 
 ```
 cc-config list [OPTIONS]
 
-  List all configurations.
+List all configurations.
 
 Options:
   -s, --show-api-key
   --help              Show this message and exit.
 ```
-The default api-key is hidden, use `-s/--show-api-key` to display the key.
+
+The default api-key is hidden; use `-s/--show-api-key` to display the key.
 
 #### 4. Remove provider
+
 ```
 cc-config remove [OPTIONS] [NAME]
 
-  Remove a configuration.
+Remove a configuration.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### 5. Switch active provider
+
 ```
 ask.py cc-config switch [OPTIONS] NAME
 
-  Switch to a different configuration and save the change.
+Switch to a different configuration and save the change.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### 6. Load configuration file
+
 ```
 Import configurations.
 
 Options:
-  -o, --override  Whether override original config.
+  -o, --override  Whether to override the original config.
   --help          Show this message and exit.
 ```
 
 #### 7. Export configuration file
+
 ```
 ask.py cc-config dump [OPTIONS] PATH
 
-  Export current configurations.
+Export current configurations.
 
 Options:
-  -o, --override  Whether override existing file.
+  -o, --override  Whether to override the existing file.
   --help          Show this message and exit.
 ```
 
 ### cc-ask
 
 Perform a question-answering task
+
 ```
 cc-ask [OPTIONS] QUERY
 
-  Start a chat session with the given query.
+Start a chat session with the given query.
 
 Options:
   -d, --db TEXT        Name of database.
   -f, --filename TEXT  Name of file.
   -r, --rerank         Whether to rerank the results.
   -s, --show-chunks    Whether to show the related chunks retrieved from
-                       database.
-  -a, --advance        Whether to use advance RAG.
+                       the database.
+  -a, --advance        Whether to use advanced RAG.
   --help               Show this message and exit.
 ```
 
 ### cc-chat
+
 Interactive Q&A
+
 ```
 cc-chat [OPTIONS] [QUERY]
 
-  Interactive chat. Enter '/quit' to exit
+Interactive chat. Enter '/quit' to exit.
 
 Options:
-  -d, --db TEXT          name of database.
-  -f, --filename TEXT    Name of file.
+  -d, --db TEXT          Name of the database.
+  -f, --filename TEXT    Name of the file.
   -n, --not-interactive
   -s, --show-history
   -c, --clear
   --help                 Show this message and exit.
 ```
 
 ### cc-code
+
 Some common commands for code based on cc-ask.
 
 #### Code Explanation
 
 ```
 cc-code explain [OPTIONS] [FILENAME] [OBJECT_NAME]
 
-  Explain code.
+Explain code.
 
 Options:
   --help  Show this message and exit.
 ```
 
-example1: Specify filename
+Example 1: Specify filename
+
 ```
 cc-code explain some_complex_scripts.py
 ```
 
-example2: Specify a particular function
+Example 2: Specify a particular function
+
 ```
 cc-code explain some_complex_scripts.py SomeClass::some_function
 ```
 
-example3: Use pipe
+Example 3: Use pipe
+
 ```
 cat some_complex_scripts.py | cc-code explain
 ```
 
 #### Fix Issues
+
 ```
 cc-code fix [OPTIONS] [FILENAME] [OBJECT_NAME]
 
-  Fix code.
+Fix code.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### Code Refactoring
+
 ```
 cc-code refactor [OPTIONS] [FILENAME] [OBJECT_NAME]
 
-  Refactor code.
+Refactor code.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### Code Review
+
 ```
 cc-code review [OPTIONS] [FILENAME] [OBJECT_NAME]
 
-  Review code.
+Review code.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### Code Translation
+
 ```
 cc-code translate [OPTIONS] [FILENAME] [OBJECT_NAME] LANGUAGE
 
-  Translate code from one language to another. Supported languages include c++, cpp,
-  c, rust, typescript, javascript, markdown, html.
+Translate code from one language to another. Supported languages include c++, cpp,
+c, rust, typescript, javascript, markdown, html.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### Select Code from Generated Results
 
-Used to select code snippets from the generated responses of the above commands
+Used to select code snippets from the generated responses of the above commands.
 
 ```
 cc-code select [OPTIONS] [INDEX]
 
-  Select code snippet from last output.
+Select code snippet from the last output.
 
-  Argument:     index: code snippet index
+Argument: index: code snippet index
 
 Options:
-  -c, --count  get the number of code snippets
+  -c, --count  Get the number of code snippets
   --help       Show this message and exit.
 ```
 
-`-c/--count` Get the number of candidate code blocks in the last response
+`-c/--count` Get the number of candidate code blocks in the last response.
+
+Example:
 
-example:
 ```
 >>> cc-code select -c
 2
 
 # Select the second code block from the last output
-# for macos
+# For macOS
 >>> cc-code select 1 | pbcopy
-# for linux
+# For Linux
 >>> cc-code select 1 | xclip -selection clipboard
 ```
 
 ### cc-db
 
 #### list: List all text collections
+
 ```
 cc-db list [OPTIONS] [NAME]
 
-  List all document databases
+List all document databases.
 
 Options:
-  -s, --short  List in short format
+  -s, --short  List in short format.
   --help       Show this message and exit.
 ```
 
 #### ingest: Digest documents
+
 ```
 cc-db ingest [OPTIONS] [FILES]...
 
-  Read documents and convert them into a searchable database.
+Read documents and convert them into a searchable database.
 
 Options:
   -n, --name TEXT     The name of the knowledge base.
-  -m, --comment TEXT  Add comment to info
+  -m, --comment TEXT  Add comment to info.
   --help              Show this message and exit.
 ```
 
-#### remove: Remove text collection
+#### remove: Remove document collection
+
 ```
 cc-db remove [OPTIONS] NAME
 
-  Remove database with the given name.
+Remove database with the given name.
 
 Options:
-  -d, --remove-documents  Remove documents if data
+  -d, --remove-documents  Remove documents if data.
   --help                  Show this message and exit.
 ```
 
 #### search: Search within a document collection
+
 ```
 cc-db search [OPTIONS] DB QUERY
 
 Options:
   -k, --topk INTEGER  Number of top results to return.
   --help              Show this message and exit.
 ```
 
 ### cc-service
-Used to manage local text-to-index services
+
+Used to manage local text-to-index services.
 
 #### start:
+
 ```
 cc-service start [OPTIONS]
 
 Options:
   --help  Show this message and exit.
 ```
 
+The process will take some time to load the model (~1min), determine if it has started with `cc-service status`.
+
 #### stop:
+
 ```
 cc-service stop [OPTIONS]
 
 Options:
   --help  Show this message and exit.
 ```
 
-#### status
+#### status:
+
 ```
 cc-service status [OPTIONS]
 
 Options:
   --help  Show this message and exit.
 ```
-
```

