# Comparing `tmp/chat_cli_anything-0.1.2.tar.gz` & `tmp/chat_cli_anything-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_cli_anything-0.1.2.tar", max compression
+gzip compressed data, was "chat_cli_anything-0.1.3.tar", max compression
```

## Comparing `chat_cli_anything-0.1.2.tar` & `chat_cli_anything-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-13 16:33:27.236056 chat_cli_anything-0.1.2/LICENSE
--rw-r--r--   0        0        0     6606 2024-04-01 16:02:39.532632 chat_cli_anything-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-20 12:50:07.078680 chat_cli_anything-0.1.2/chat_cli_anything/__init__.py
--rw-r--r--   0        0        0    25938 2024-04-01 14:46:58.548301 chat_cli_anything-0.1.2/chat_cli_anything/ask.py
--rw-r--r--   0        0        0     6609 2024-03-31 17:13:11.207888 chat_cli_anything-0.1.2/chat_cli_anything/config.py
--rw-r--r--   0        0        0     7928 2024-04-01 11:30:03.539469 chat_cli_anything-0.1.2/chat_cli_anything/db.py
--rw-r--r--   0        0        0     1616 2024-04-01 13:09:38.160887 chat_cli_anything-0.1.2/chat_cli_anything/embedding.py
--rw-r--r--   0        0        0     2675 2024-03-31 17:13:11.207713 chat_cli_anything-0.1.2/chat_cli_anything/loader.py
--rw-r--r--   0        0        0     2712 2024-03-13 05:19:41.646954 chat_cli_anything-0.1.2/chat_cli_anything/request.py
--rw-r--r--   0        0        0      729 2024-03-31 17:35:50.217211 chat_cli_anything-0.1.2/chat_cli_anything/rerank.py
--rw-r--r--   0        0        0     1868 2024-04-01 08:49:00.737620 chat_cli_anything-0.1.2/chat_cli_anything/service.py
--rw-r--r--   0        0        0     1041 2024-03-14 09:10:51.056908 chat_cli_anything-0.1.2/chat_cli_anything/util.py
--rw-r--r--   0        0        0     1448 2024-04-01 16:10:12.818895 chat_cli_anything-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8109 1970-01-01 00:00:00.000000 chat_cli_anything-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-13 16:33:27.236056 chat_cli_anything-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6607 2024-04-02 02:18:28.290235 chat_cli_anything-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 12:50:07.078680 chat_cli_anything-0.1.3/chat_cli_anything/__init__.py
+-rw-r--r--   0        0        0    28955 2024-04-03 08:40:52.276963 chat_cli_anything-0.1.3/chat_cli_anything/ask.py
+-rw-r--r--   0        0        0     6896 2024-04-03 05:20:02.168901 chat_cli_anything-0.1.3/chat_cli_anything/config.py
+-rw-r--r--   0        0        0     7928 2024-04-03 05:20:24.146595 chat_cli_anything-0.1.3/chat_cli_anything/db.py
+-rw-r--r--   0        0        0     1616 2024-04-01 13:09:38.160887 chat_cli_anything-0.1.3/chat_cli_anything/embedding.py
+-rw-r--r--   0        0        0     2798 2024-04-03 06:48:40.337190 chat_cli_anything-0.1.3/chat_cli_anything/loader.py
+-rw-r--r--   0        0        0     2714 2024-04-03 07:17:55.368638 chat_cli_anything-0.1.3/chat_cli_anything/request.py
+-rw-r--r--   0        0        0      729 2024-03-31 17:35:50.217211 chat_cli_anything-0.1.3/chat_cli_anything/rerank.py
+-rw-r--r--   0        0        0     1868 2024-04-01 08:49:00.737620 chat_cli_anything-0.1.3/chat_cli_anything/service.py
+-rw-r--r--   0        0        0     1050 2024-04-02 06:30:30.360008 chat_cli_anything-0.1.3/chat_cli_anything/util.py
+-rw-r--r--   0        0        0     1448 2024-04-03 07:05:53.661098 chat_cli_anything-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8110 1970-01-01 00:00:00.000000 chat_cli_anything-0.1.3/PKG-INFO
```

### Comparing `chat_cli_anything-0.1.2/LICENSE` & `chat_cli_anything-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.2/README.md` & `chat_cli_anything-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 step 2: Ask a question
 
 ```
 # for open question, '-a/--advance' option would be helpful
 cc-ask -d xiyouji "孙悟空一打白骨精的时候说了啥" -a
 ```
 
+
 ## Commands
 
 ### cc-config
 Configure LLM provider
 
 #### 1. Add LLM provider
```

### Comparing `chat_cli_anything-0.1.2/chat_cli_anything/ask.py` & `chat_cli_anything-0.1.3/chat_cli_anything/ask.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,18 +74,20 @@
         self.config = Config().config
         self.history_file = cache_path / '.history.json'
 
         if self.history_file.exists():
             with open(self.history_file, 'r') as file:
                 self.history = json.load(file)
                 self.diag_history = self.history.get('history', [])
-                self.last_output = self.history.get('last_output', [])
+                self.last_output = self.history.get('last_output', '')
+                self.last_query = self.history.get('last_query', '')
         else:
             self.diag_history = []
             self.last_output = '' 
+            self.last_query = '' 
 
         self.pipeline_input = self._read_from_pipeline_input()
         self.active_config = self.config['providers'][self.config['active']]
         self.client = build_client(
             self.active_config['base_url'],
             self.active_config['api_key'],
             self.active_config['proxy'],
@@ -132,20 +134,39 @@
             prompt = self._build_prompt_for_rag(content)
 
         if as_system:
             self.diag_history.insert(0, {'role': 'system', 'content': prompt})
         else:
             self.diag_history.append({'role': 'user', 'content': prompt})
 
+    def load_file(self, filename: str):
+        from loader import SUPPORTED_FILES, load_file
+        ext = os.path.splitext(filename)
+        if ext[1] and ext[1] in SUPPORTED_FILES: 
+            pages = load_file(filename)
+            content = ''.join(page.page_content for page in pages)
+        else:
+            click.secho(click.style('Not supported file extension. ' + f' currrent supported format: {",".join(SUPPORTED_FILES)}', fg='orange') + 'It will be loaded as plain text')
+            with open(filename, 'r', encoding='utf-8') as f:
+                content = f.read()
+        return content
 
-    def chat(self, query: str, filename: str, db: Any, not_interactive: bool=False):
+    def chat(self,
+             query: str,
+             filename: str,
+             db: Any,
+             not_interactive: bool=False):
         """Start a chat session with the given query."""
+        content = None
         if filename:
-            with open(filename, 'r', encoding='utf-8') as f:
-                content = f.read()
+            if not os.path.exists(filename):
+                click.secho(f'Could not find {filename}.', fg='red')
+                return
+            content = self.load_file(filename)
+
         elif self.pipeline_input:
             content = self.pipeline_input
 
         if content or (db is not None):
             self.clear_chat_history()
 
         if content: 
@@ -162,14 +183,19 @@
 
                 if db:
                     docs = _get_relevant_docs(query, db)
                     docs_str = _build_prompt_from_docs(docs)
                     # update system prompt
                     self._build_prompt(docs_str, as_system=False)
 
+                # add last query and output into history
+                if not_interactive and self.last_output:
+                    self.diag_history.append({'role': 'user', 'content': self.last_query})
+                    self.diag_history.append({'role': 'assistant', 'content': self.last_output})
+
                 responses = stream_predict(
                     self.client,
                     self.active_config['model'],
                     query=query,
                     history=deepcopy(self.diag_history)
                 )
 
@@ -177,17 +203,16 @@
                 click.secho('Assistant:', fg='blue')
 
                 with Live(Markdown(full_response), refresh_per_second=20) as live:
                     for response in responses:
                         if response.choices[0].delta.content is not None:
                             partial_response = response.choices[0].delta.content
                             full_response += partial_response
-                            if response.choices[0].finish_reason == 'stop':
-                                self.last_output = full_response
                             live.update(Markdown(full_response))
+                self.last_output = full_response
                 self.diag_history.append({'role': 'user', 'content': query})
                 self.diag_history.append({'role': 'assistant', 'content': full_response})
 
                 if interactive:
                     click.secho("\nUser: ", fg='cyan', nl=False)
                     # click.prompt could not throw keyboard interruption
                     query = input("")
@@ -198,15 +223,16 @@
                 break
 
         # when in interactive chat mode, output will be cleared
         if interactive:
             self.diag_history = []
         # write history back
         with open(self.history_file, 'w') as f:
-            json.dump({'history': self.diag_history, 'last_output': self.last_output},
+            # diag_history + last_output = all diag
+            json.dump({'history': self.diag_history[:-2], 'last_query': query, 'last_output': self.last_output},
                        f, ensure_ascii=False, indent=4)
 
     def show_chat_history(self):
         """Show chat history."""
         for item in self.diag_history:
             click.secho(f"{item['role']}: ".capitalize(), fg='cyan' if item['role'] == 'user' else 'blue', nl=False)
             click.secho(f"{item['content']}")
@@ -228,16 +254,18 @@
             show_chunks: Optional[bool]=False,
             advance:bool=False):
         """Single round query."""
 
         self.clear_chat_history()
 
         if filename:
-            with open(filename, 'r', encoding='utf-8') as f:
-                content = f.read()
+            if not os.path.exists(filename):
+                click.secho(f'Could not find {filename}.', fg='red')
+                return
+            content = self.load_file(filename)
             self._build_prompt(content, type)
         elif db:
             if advance:
                 # HyDE
                 query = predict(self.client,
                                 self.active_config['model'], 
                                 f"Please write a passage to answer the question?\n {query}".format(query=query),
@@ -267,68 +295,93 @@
             for response in responses:
                 if response.choices[0].delta.content is not None:
                     partial_response = response.choices[0].delta.content
                     full_response += partial_response
                     live.update(Markdown(full_response))
         self.last_output = full_response
         with open(self.history_file, 'w') as f:
-            json.dump({'history': [], 'last_output': self.last_output}, f, ensure_ascii=False, indent=4)
+            json.dump({'history': [], 'last_query': query, 'last_output': self.last_output}, 
+                      f, ensure_ascii=False, indent=4)
 
     def fk(self, query: str):
         """Similar to `thefuck` fix output."""
         # TODO
         ...
 
-    def refactor(self, filename: str, object_name: str):
+    def refactor(self, filename: str, object_name: str, continue_generate: bool):
         """Refactor code."""
         if object_name:
-            prompt = f"""重构代码中的 `{object_name}` 代码, 你首先应该把目标代码提取出来, 然后再进行重构, 直接输出重构后的代码"""
+            prompt = f"""重构上面代码中的 `{object_name}` 代码, 你首先应该把目标代码提取出来, 然后再进行重构, 直接输出重构后的代码"""
+        else:
+            prompt = f"""重构上面的代码"""
+
+        if continue_generate:
+            prompt = "请继续输出"
+            self.chat(prompt, filename, db=None, not_interactive=True)
         else:
-            prompt = f"""重构代码"""
-        self.ask(prompt, 'code', filename)
+            self.ask(prompt, 'code', filename)
 
-    def explain(self, filename: str, object_name: str, line_by_line: bool=False):
+    def explain(self, filename: str, object_name: str, line_by_line: bool, continue_generate: bool):
         """"""
         if object_name:
-            prompt = f"""解释 {object_name} 的函数, 你首先应该把目标代码提取出来, 然后再进行解释"""
+            prompt = f"""从上面给出代码中, 解释 {object_name} 的函数, 你首先应该把目标代码提取出来, 然后再进行解释"""
             if line_by_line:
                 prompt += '逐行给出解释。'
         else:
-            prompt = f"""解释给出的代码, 对于复杂难懂的地方给出说明"""
+            prompt = f"""解释上面给出的代码, 对于复杂难懂的地方给出说明"""
             if line_by_line:
-                prompt = f"""解释给出的代码, 逐行给出解释"""
+                prompt = f"""解释上面给出的代码, 逐行给出解释"""
             else:
-                prompt = f"""解释给出的代码, 对于复杂难懂的地方给出说明"""
-        self.ask(prompt, 'code', filename)
+                prompt = f"""解释上面给出的代码, 对于复杂难懂的地方给出说明"""
+
+        if continue_generate:
+            prompt = "请继续输出"
+            self.chat(prompt, filename, db=None, not_interactive=True)
+        else:
+            self.ask(prompt, 'code', filename)
 
-    def translate(self, filename: str, object_name: str, target_language: str):
+    def translate(self, filename: str, object_name: str, target_language: str, continue_generate: bool):
         """Translate code from one language to another language"""
         if object_name:
             prompt = f"""把 `{object_name}` 转化为 {target_language} 语言实现, 你首先应该把目标代码提取出来, 然后再进行翻译, 直接输出翻译后的代码"""
         else:
-            prompt = f"""把代码转化为 {target_language} 语言实现"""
-        self.ask(prompt, 'code', filename)
+            prompt = f"""把上面给出的代码转化为 {target_language} 语言实现"""
 
-    def review(self, filename: str, object_name: str):
+        if continue_generate:
+            prompt = "请继续输出"
+            self.chat(prompt, filename, db=None, not_interactive=True)
+        else:
+            self.ask(prompt, 'code', filename)
+
+    def review(self, filename: str, object_name: str, continue_generate: bool):
         """Do code review"""
         instruction = """对需要优化的代码实现，变量命名, 代码分格, 代码注释等给出 comment."""
         if object_name:
             prompt = f"""对 `{object_name}` 实现进行 code review, 你首先应该把目标代码提取出来, 然后再""" + instruction
         else:
             prompt = f"""对上面的代码进行code review, """ + instruction
-        self.ask(prompt, 'code', filename)
 
-    def fix(self, filename: str, object_name: str):
+        if continue_generate:
+            prompt = "请继续输出"
+            self.chat(prompt, filename, db=None, not_interactive=True)
+        else:
+            self.ask(prompt, 'code', filename)
+
+    def fix(self, filename: str, object_name: str, continue_generate: bool):
         """Fix given function name"""
         if object_name:
             prompt = f"""修复 `{object_name}` 中可能的错误, 你首先应该把目标代码提取出来, 然后再进行修复, 直接输出修复后的代码"""
         else:
-            prompt = f"""修复中可能的错误"""
+            prompt = f"""修复上面代码其中可能的错误"""
 
-        self.ask(prompt, 'code', filename)
+        if continue_generate:
+            prompt = "请继续输出"
+            self.chat(prompt, filename, db=None, not_interactive=True)
+        else:
+            self.ask(prompt, 'code', filename)
 
     def select_code_snippet(self, index: str, count: bool):
         """"""
         blocks = parse_markdown_codeblock(self.last_output)
         if count:
             click.echo(len(blocks))
             return
@@ -364,15 +417,16 @@
 @click.group(name='cc-service')
 def service():
     """Manage service"""
     pass
 
 
 filename = click.argument('filename', required=False, default='')
-object_name = click.argument('object_name', required=False, default='')
+object_name = click.option('-o', '--object-name', required=False, default='')
+continue_generate = click.option('-c', '--continue-generate', is_flag=True)
 
 
 @config.command()
 @click.argument('name', default=None)
 @click.argument('base-url', default=None)
 @click.option('--model', default='Empty')
 @click.option('--api-key', default='Empty', envvar="OPENAI_API_KEY")
@@ -388,29 +442,28 @@
     config = Config()
     config.add(name, base_url, api_key, model, proxy)
     click.echo(f"Configuration '{name}' added successfully.")
 
 
 @config.command()
 @click.argument('name')
-def remove(name: str):
+@click.option('-a', '--all', is_flag=True, help='Remove all providers')
+def remove(name: str, all: bool):
     """Remove a configuration."""
     config = Config()
-    if name:
-        config.remove(name)
+    config.remove(name, all)
 
 
 @config.command()
 @click.argument('name', required=False, default='')
 @click.option('-s', '--show-api-key', is_flag=True)
 def list(name: str, show_api_key: bool):
     """List configurations. The active provider will be marked with '*'."""
     config = Config()
-    if name:
-        config.list(api_key=show_api_key)  # Set api_key to True or False based on your preference
+    config.list(name, api_key=show_api_key)  # Set api_key to True or False based on your preference
 
 
 @config.command()
 @click.argument('name', required=True)
 def switch(name: str):
     """Switch to a different configuration and save the change."""
     config = Config()
@@ -500,60 +553,69 @@
     if not filename and sys.stdin.isatty():
         click.secho('Please provide a filename or input from pipe.', fg='red')
         sys.exit(1)
 
 @code.command()
 @filename
 @object_name
-def refactor(filename: str, object_name: str):
+@continue_generate
+def refactor(filename: str, object_name: str, continue_generate: bool):
     """Refactor code."""
     check_has_context(filename)
     interface = Interface()
-    interface.refactor(filename, object_name)
+    interface.refactor(filename, object_name, continue_generate)
 
 
 @code.command()
+@click.argument('language')
 @filename
 @object_name
-@click.argument('language')
-def translate(filename: str, object_name: str, language: str):
+@continue_generate
+def translate(filename: str, object_name: str, language: str, continue_generate: bool):
     """Translate code from one language to another. Supported languages 
     c++, cpp, c, rust, typescript, javascript, markdown, html.
     """
     check_has_context(filename)
     interface = Interface()
-    interface.translate(filename, object_name, language)
+    interface.translate(filename, object_name, language, continue_generate)
+
 
 @code.command()
 @filename
 @object_name
-def fix(filename: str, object_name: str):
+@continue_generate
+def fix(filename: str, object_name: str, continue_generate: bool):
     """Fix code."""
     check_has_context(filename)
     interface = Interface()
-    interface.fix(filename, object_name)
+    interface.fix(filename, object_name, continue_generate)
+
 
 @code.command()
 @filename
 @object_name
-def review(filename: str, object_name: str):
+@continue_generate
+def review(filename: str, object_name: str, continue_generate: bool):
     """Review code."""
     check_has_context(filename)
     interface = Interface()
-    interface.review(filename, object_name)
+    interface.review(filename, object_name, continue_generate)
+
 
 @code.command()
 @filename
 @object_name
 @click.option('-l', '--line', is_flag=True, help='Line by line.')
-def explain(filename: str, object_name: str, line: bool):
+@continue_generate
+def explain(filename: str, object_name: str, line: bool, continue_generate: bool):
     """Explain code."""
     check_has_context(filename)
     interface = Interface()
-    interface.explain(filename, object_name, line_by_line=line)
+    interface.explain(filename, object_name, line_by_line=line, continue_generate=continue_generate)
+
 
 @code.command()
 @click.argument('index', required=False, default='')
 @click.option('-c', '--count', is_flag=True, help='get number of code snippets')
 def select(index: str, count: bool):
     """Select code snippet from last output.
 
@@ -682,15 +744,15 @@
         import subprocess
         cmds = "{} -m chat_cli_anything.service {}".format(sys.executable, port)
         # cmds = "{} -m cli-chat.chat_cli_anything.service {}".format(sys.executable, port)
         cmds = shlex.split(cmds)
         _ = subprocess.Popen(cmds, start_new_session=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         config['local_service_port'] = port
         config.save()
-    click.secho(f'{SERVICE_NAME} is running background.')
+        click.secho(f'{SERVICE_NAME} is running background.')
 
 
 def show_service():
     from chat_cli_anything.service import SERVICE_NAME
     config = Config()
     port = config.config.get('local_service_port', Config.DEFAULT_PORT)
     if _check_port_is_accessible(port) and _is_excepted_service_type(port, SERVICE_NAME):
@@ -732,14 +794,22 @@
 def stop():
     stop_service()
 
 @service.command(name='status')
 def status():
     show_service()
 
+@cli.command(name='cc-info')
+def info():
+    # list db path
+    from chat_cli_anything.db import DB_PATH
+    click.secho('db path: {}'.format(DB_PATH))
+    # list config path
+    click.secho('config path: {}'.format(Config.CONFIG_PATH))
+
 def main():
     cli.add_command(config)
     cli.add_command(code)
     cli.add_command(db)
     cli.add_command(service)
     cli()
```

### Comparing `chat_cli_anything-0.1.2/chat_cli_anything/config.py` & `chat_cli_anything-0.1.3/chat_cli_anything/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,30 +31,36 @@
     Here will set multiple sources, 
     current: 
     other:
 
     it will save in a json file.
     """
     DEFAULT_PORT = 8789
+    CONFIG_PATH = cache_path / '.config.json'
+
     def __init__(self):
         self.config: Dict[str, Any] = {}
-        self.config_file = cache_path / '.config.json'
 
         # Load existing config if available
-        if self.config_file.exists():
-            with open(self.config_file, 'r') as file:
+        if self.CONFIG_PATH.exists():
+            with open(self.CONFIG_PATH, 'r') as file:
                 self.config = json.load(file)
 
-    def remove(self, name: str):
+    def remove(self, name: str, all: bool=False):
         """Clean providers in config given name."""
-        if name in self.config['providers']:
-            del self.config['providers'][name]
-            if self.config['active'] == name:
-                self.config['active'] = None
-            self._dump_config()
+        if all:
+            self.config['providers'] = {}
+        else:
+            if name in self.config['providers']:
+                del self.config['providers'][name]
+                if self.config['active'] == name:
+                    self.config['active'] = None
+            else:
+                click.secho(f"'{name}' not found in config.", fg='red')
+        self._dump_config()
         click.echo(f"'{name}' was removed successfully.")
 
     def add(self, name: str, base_url: str, 
             api_key: str='Empty', model: str='Empty',
             proxy: Optional[str]=None):
         """Add provider in local config file. If name already in config files, the original
         configuration will be overrride.
@@ -74,24 +80,26 @@
         self.config['providers'] = providers
 
         if not self._has_active_provider():
             self.config['active'] = name
 
         self._dump_config()
 
-    def list(self, api_key: bool=False):
+    def list(self, provider_name: str='', api_key: bool=False):
         """List all providers in a formatted table."""
         # Prepare the data for the table
         data = []
-        click.echo(f'Configuration in {str(self.config_file)}')
+        click.echo(f'Configuration in {str(self.CONFIG_PATH)}')
         click.echo('Name start with "*" indicating current active provider.')
         if 'providers' not in self.config:
             click.echo('No provider has been add.')
             return
         for name, details in self.config['providers'].items():
+            if provider_name and name != provider_name:
+                continue
             api_key_str = details['api_key'] if api_key else "Hidden"
             if name == self.config['active']:
                 name = '*' + name
             data.append([name, details['base_url'], api_key_str,
                          details['model'], details['proxy']])
 
         # Use tabulate to format the data into a table
@@ -136,15 +144,15 @@
             self.config = config
             click.echo('Configuration loaded and override original configuration.')
         else:
             # merge configuration
             for k, v in self.config.get('providers', {}).items():
                 self.config[k] = v
             click.echo('Configuration loaded and merged to original configuration.')
-        with open(self.config_file, 'w') as file:
+        with open(self.CONFIG_PATH, 'w') as file:
             json.dump(self.config, file, indent=4)
 
     def _has_active_provider(self):
         """Check whether there is a """
         if ('active' not in self.config or
              not self.config['active'] or
              self.config['active'] not in self.config['providers']):
@@ -172,15 +180,15 @@
         """Set local service port"""
         self.config['local_service_port'] = port
 
     def save(self):
         self._dump_config() 
 
     def _dump_config(self):
-        with open(self.config_file, 'w') as file:
+        with open(self.CONFIG_PATH, 'w') as file:
             json.dump(self.config, file, indent=4)
     
     def __setitem__(self, __name: str, __value: Any) -> None:
         self.config[__name] = __value
 
     def __contains__(self, __key: object) -> bool:
         return self.config.__contains__(__key)
```

### Comparing `chat_cli_anything-0.1.2/chat_cli_anything/db.py` & `chat_cli_anything-0.1.3/chat_cli_anything/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 from chat_cli_anything.embedding import LocalEmbeddings
 
 logger = getLogger(__name__)
 logger.setLevel(logging.INFO)
 logger.addHandler(logging.StreamHandler())
 
 
-db_path = cache_path / 'db' 
-if not db_path.exists():
-    db_path.mkdir()
+DB_PATH = cache_path / 'db' 
+if not DB_PATH.exists():
+    DB_PATH.mkdir()
 
-engine = create_engine(f"sqlite:///{str(db_path/ 'info.db')}")#, echo=True)
+engine = create_engine(f"sqlite:///{str(DB_PATH/ 'info.db')}")#, echo=True)
 
 Base = declarative_base()
 
 
 class DocumentInfoDB(Base):
     """"""
     __tablename__ = 'document_info'
@@ -190,15 +190,15 @@
     session.add(document_set)
 
     for doc, (hash_key, file) in zip(docs, hash_files_processed.items()):
 
         if not session.query(DocumentInfoDB).filter(DocumentInfoDB.hash == hash_key).first():
             logger.info(f'{hash_key}, {file}')
             faiss_index = FAISS.from_documents(doc, embedding_model)
-            kb_path = db_path / (os.path.basename(hash_key).split('.')[0] + '.db')
+            kb_path = DB_PATH / (os.path.basename(hash_key).split('.')[0] + '.db')
             faiss_index.save_local(str(kb_path)) # TODO
             
             # update document info table
             modified_time = os.path.getmtime(file)
             modified_datetime = datetime.fromtimestamp(modified_time)
             new_index_info = DocumentInfoDB(hash=hash_key,
                                         kb_path=str(kb_path),
```

### Comparing `chat_cli_anything-0.1.2/chat_cli_anything/embedding.py` & `chat_cli_anything-0.1.3/chat_cli_anything/embedding.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.2/chat_cli_anything/loader.py` & `chat_cli_anything-0.1.3/chat_cli_anything/loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,25 +9,43 @@
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 
 
 from chat_cli_anything.util import cache_path, calculate_hash
 from typing import Union, List, Tuple, Dict
 
 
-__SUPPORTED_FILES__ = [
+SUPPORTED_FILES = [
     # documents
     '.txt', '.md', '.pdf', '.docx', '.doc',
     # programming language
     '.py', '.c', '.cpp', '.java', '.js', '.ts',
     '.go', '.rs', '.php', '.html', '.css', '.json',
     '.yaml', '.yml'
 ]
 
 FileHash = Dict[str, str]
 
+def load_file(input: str, chunk_size: int=400, chunk_overlap: int=100):
+    ext = os.path.splitext(input)[1]
+    if ext not in SUPPORTED_FILES:
+        return
+    if ext == '.pdf':
+        loader = PyPDFLoader(input)
+    elif ext in ['.docx', '.doc']:
+        loader = UnstructuredWordDocumentLoader(input)
+    else:
+        loader = TextLoader(input)
+    pages = loader.load()
+    # from_tiktoken_encoder enables use to split on tokens rather than characters
+    recursive_text_splitter = RecursiveCharacterTextSplitter.from_tiktoken_encoder(
+        chunk_size=chunk_size, 
+        chunk_overlap=chunk_overlap,
+    )
+    pages = recursive_text_splitter.split_documents(pages)
+    return pages
 
 def parse_files(
     input: str,
     do_cache: bool=True,
     recursive: bool=True,
     verbose: bool=True,
 ) -> Union[Tuple[List[List[Document]], Dict[str, str]], None]:
@@ -36,43 +54,30 @@
     all_files_processed = {}
 
     all_pages: List[List[Document]] = []
     if os.path.isdir(input):
         for item in os.listdir(input):
             sub_item = os.path.join(input, item)
             if os.path.isfile(sub_item):
-                if os.path.splitext(sub_item)[-1] in __SUPPORTED_FILES__:
+                if os.path.splitext(sub_item)[-1] in SUPPORTED_FILES:
                     pages, _files_processed = parse_files(sub_item, do_cache=do_cache)
                     all_pages.extend(pages)
                     all_files_processed.update(_files_processed)
             else:
                 if recursive:
                     pages, _files_processed = parse_files(sub_item, do_cache=do_cache, recursive=recursive)
                     all_pages.extend(pages)
                     all_files_processed.update(_files_processed)
 
     elif os.path.exists(input):
-        ext = os.path.splitext(input)[1]
-        if ext not in __SUPPORTED_FILES__:
-            click.secho(f'File type {ext} not supported', fg='red')
-            return
-        if verbose:
-            click.secho(f'found "{input}"', fg='green')
-        if ext == '.pdf':
-            loader = PyPDFLoader(input)
-        elif ext in ['.docx', '.doc']:
-            loader = UnstructuredWordDocumentLoader(input)
+        pages = load_file(input)
+        if pages:
+            if verbose:
+                click.secho(f'found "{input}"', fg='green')
+            all_pages.append(pages)
+            all_files_processed[calculate_hash(input)] = os.path.abspath(input)
         else:
-            loader = TextLoader(input)
-        pages = loader.load()
-        # from_tiktoken_encoder enables use to split on tokens rather than characters
-        recursive_text_splitter = RecursiveCharacterTextSplitter.from_tiktoken_encoder(
-            chunk_size=400, 
-            chunk_overlap=100,
-        )
-        pages = recursive_text_splitter.split_documents(pages)
-        all_pages.append(pages)
-        all_files_processed[calculate_hash(input)] = os.path.abspath(input)
-
+            click.secho(f'File type not supported', fg='red')
+            return
     else:
         click.secho(f'File {input} not found', fg='red')
     return all_pages, all_files_processed
```

### Comparing `chat_cli_anything-0.1.2/chat_cli_anything/request.py` & `chat_cli_anything-0.1.3/chat_cli_anything/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     return client
 
 
 def predict(client: OpenAI,
             model: str,
             query: str,
             history: Optional[List[Dict[str, str]]] = None, 
-            max_tokens: int = 4096,
+            max_tokens: int = 16384,
             temperature: float = 0.95,
             top_p: float = 1.0):
     """"""
     history = history or []
 
     if query:
         history.append({"role": "user", "content": query})
@@ -58,15 +58,15 @@
 
 
 def stream_predict(
         client: OpenAI,
         model: str,
         query: str,
         history: Optional[List[Dict[str, str]]] = None, 
-        max_tokens: int = 4096,
+        max_tokens: int = 16384,
         temperature: float = 0.95,
         top_p: float = 1.0):
     history = history or []
 
     history.append({"role": "user", "content": query})
     print(history)
```

### Comparing `chat_cli_anything-0.1.2/chat_cli_anything/rerank.py` & `chat_cli_anything-0.1.3/chat_cli_anything/rerank.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.2/chat_cli_anything/service.py` & `chat_cli_anything-0.1.3/chat_cli_anything/service.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.2/chat_cli_anything/util.py` & `chat_cli_anything-0.1.3/chat_cli_anything/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import List
 from pathlib import Path
 import hashlib
 
 
-cache_path = Path.home() / '.cache' / 'cli-chat'
+cache_path = Path.home() / '.cache' / 'cli-chat-anything'
 if not cache_path.exists():
     cache_path.mkdir(parents=True)
 
 
 LANGUAGES = [
     'python', 'javascript', 'typescript', 'cpp',
     'c', 'java', 'php', 'ruby', 'go', 'rust',
```

### Comparing `chat_cli_anything-0.1.2/pyproject.toml` & `chat_cli_anything-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chat-cli-anything"
-version = "0.1.2"
+version = "0.1.3"
 description = "Chat with anything on cli."
 authors = ["liuping <liuping@shukun.net>"]
 license = "Apache"
 readme = "README.md"
 keywords = ["chatgpt", "cli", "chat"]
 packages = [{ include = "chat_cli_anything" }]
```

### Comparing `chat_cli_anything-0.1.2/PKG-INFO` & `chat_cli_anything-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-cli-anything
-Version: 0.1.2
+Version: 0.1.3
 Summary: Chat with anything on cli.
 License: Apache
 Keywords: chatgpt,cli,chat
 Author: liuping
 Author-email: liuping@shukun.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -102,14 +102,15 @@
 step 2: Ask a question
 
 ```
 # for open question, '-a/--advance' option would be helpful
 cc-ask -d xiyouji "孙悟空一打白骨精的时候说了啥" -a
 ```
 
+
 ## Commands
 
 ### cc-config
 Configure LLM provider
 
 #### 1. Add LLM provider
```

