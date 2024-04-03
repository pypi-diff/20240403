# Comparing `tmp/discord_amethyst-1.0.1.tar.gz` & `tmp/discord_amethyst-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_amethyst-1.0.1.tar", max compression
+gzip compressed data, was "discord_amethyst-2.0.0.tar", max compression
```

## Comparing `discord_amethyst-1.0.1.tar` & `discord_amethyst-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     5199 2023-07-12 18:20:56.647785 discord_amethyst-1.0.1/README.md
--rw-r--r--   0        0        0      603 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      332 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/__init__.py
--rw-r--r--   0        0        0    23513 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/client.py
--rw-r--r--   0        0        0      606 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/error.py
--rw-r--r--   0        0        0     1369 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/util.py
--rw-r--r--   0        0        0      537 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/widget/__init__.py
--rw-r--r--   0        0        0     3570 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/widget/abc.py
--rw-r--r--   0        0        0     4886 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/widget/command.py
--rw-r--r--   0        0        0      287 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/widget/event/__init__.py
--rw-r--r--   0        0        0     3744 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/widget/event/handler.py
--rw-r--r--   0        0        0    38812 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/widget/event/library.py
--rw-r--r--   0        0        0     2628 2023-07-12 18:20:56.651785 discord_amethyst-1.0.1/src/amethyst/widget/schedule.py
--rw-r--r--   0        0        0     5784 1970-01-01 00:00:00.000000 discord_amethyst-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-03 15:17:00.330501 discord_amethyst-2.0.0/LICENCE
+-rw-r--r--   0        0        0     5117 2024-04-03 15:17:00.330501 discord_amethyst-2.0.0/README.md
+-rw-r--r--   0        0        0      679 2024-04-03 15:17:00.330501 discord_amethyst-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      707 2024-04-03 15:17:26.026056 discord_amethyst-2.0.0/src/amethyst/__init__.py
+-rw-r--r--   0        0        0    22823 2024-04-03 15:17:26.026056 discord_amethyst-2.0.0/src/amethyst/amethyst.py
+-rw-r--r--   0        0        0      705 2024-04-03 15:17:26.026056 discord_amethyst-2.0.0/src/amethyst/error.py
+-rw-r--r--   0        0        0     1950 2024-04-03 15:17:26.026056 discord_amethyst-2.0.0/src/amethyst/util.py
+-rw-r--r--   0        0        0        1 2024-04-03 15:17:26.030056 discord_amethyst-2.0.0/src/amethyst/widget/__init__.py
+-rw-r--r--   0        0        0     2388 2024-04-03 15:17:26.030056 discord_amethyst-2.0.0/src/amethyst/widget/command.py
+-rw-r--r--   0        0        0      200 2024-04-03 15:17:26.030056 discord_amethyst-2.0.0/src/amethyst/widget/event/__init__.py
+-rw-r--r--   0        0        0     3276 2024-04-03 15:17:26.030056 discord_amethyst-2.0.0/src/amethyst/widget/event/event.py
+-rw-r--r--   0        0        0    38702 2024-04-03 15:17:26.034056 discord_amethyst-2.0.0/src/amethyst/widget/event/library.py
+-rw-r--r--   0        0        0     2642 2024-04-03 15:17:26.030056 discord_amethyst-2.0.0/src/amethyst/widget/menu.py
+-rw-r--r--   0        0        0     2777 2024-04-03 15:17:26.030056 discord_amethyst-2.0.0/src/amethyst/widget/schedule.py
+-rw-r--r--   0        0        0     5933 1970-01-01 00:00:00.000000 discord_amethyst-2.0.0/PKG-INFO
```

### Comparing `discord_amethyst-1.0.1/README.md` & `discord_amethyst-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Discord Amethyst
 
-An opinionated extension for [discord.py](https://github.com/Rapptz/discord.py). Amethyst adds a handful of features that I found myself re-implementing or wanting for many of my Discord bots such as automatic app command synchronisation and job scheduling.
+An opinionated extension for [discord.py](https://github.com/Rapptz/discord.py), inspired by [JellyCommands](https://jellycommands.dev/). Amethyst adds a handful of features that I found myself re-implementing or wanting for many of my Discord bots such as automatic app command synchronisation and job scheduling.
 
 ## Widgets
 
-### Command
+### Command & Context Menus
 
-The amethyst command decorator is just a wrapper around discord.py's `app_commands.command` decorator. Please refer to the [discord.py documentation](https://discordpy.readthedocs.io/en/stable/interactions/api.html?highlight=app_commands%20command#discord.app_commands.command) for usage.
+The amethyst `command` and `context_menu` decorators are just a wrappers around discord.py's decorators. Please refer to the [discord.py documentation](https://discordpy.readthedocs.io/en/stable/interactions/api.html?highlight=app_commands%20command#discord.app_commands.command) for usage.
 
 ### Event
 
-Amethyst's event decorator is a type hinted wrapper around [discord.py's normal event decorator](https://discordpy.readthedocs.io/en/stable/api.html?highlight=client%20event#discord.Client.event). The primary difference is that you must specify which event you wish to subscribe to. The property `amethyst.events` is a module containing all of the [default discord.py events](https://discordpy.readthedocs.io/en/stable/api.html?highlight=client%20event#event-reference).
+Amethyst's event decorator is a type hinted wrapper around [discord.py's normal event decorator](https://discordpy.readthedocs.io/en/stable/api.html?highlight=client%20event#discord.Client.event). The primary difference is that you must specify which event you wish to subscribe to. The amethyst module exports all of the [default discord.py events](https://discordpy.readthedocs.io/en/stable/api.html?highlight=client%20event#event-reference) with the prefix `on_`.
 
 ```py
 import amethyst
 
-@amethyst.event(amethyst.events.on_ready)
+@amethyst.event(amethyst.on_ready)
 async def on_ready():
     print("Bot is ready!")
 ```
 
 ### Schedule
 
 Amethyst implements a [cron-like](https://en.wikipedia.org/wiki/Cron) asynchronous scheduler for calling functions on a set schedule, powered by [croniter](https://github.com/kiorky/croniter).
@@ -32,29 +32,29 @@
 @amethyst.schedule("0 8 * * *")
 async def every_morning():
     print("Good morning!")
 ```
 
 ## Dynamic Module Import
 
-Amethyst can dynamically load python modules, powered by [dynamicpy](https://github.com/NimajnebEC/dynamicpy#dynamicloader). When run, the client will automatically import and register any widgets found in the `.command`, `.commands`, `.plugin` and `.plugins` submodules. The submodules which are searched can be configured in the `AmethystClient`'s constructor.
+Amethyst can dynamically load python modules, powered by [dynamicpy](https://github.com/NimajnebEC/dynamicpy#dynamicloader). When run, the client will automatically import and register any widgets found in the `.command`, `.commands`, `.plugin` and `.plugins` submodules. The submodules which are searched can be configured in the `amethyst.Client` constructor.
 
 Lets say you have the following project structure:
 
 ```
 my-bot/
 ├── __init__.py
 ├── main.py
 └── commands/
     ├── __init__.py
     ├── foo.py
     └── bar.py
 ```
 
-If your instance of `AmethystClient` is instantiated in `main.py` then the `commands/` package will be recursively searched for widgets to register.
+If your instance of `amethyst.Client` is instantiated in `main.py` then the `commands/` package will be recursively searched for widgets to register.
 
 The searched modules can also be top-level, the only requirement is that they are at the same level as the module inside which the client was instantiated.
 
 ```
 my-bot.py
 plugins.py
 commands/
@@ -63,57 +63,55 @@
 └── bar.py
 ```
 
 In this example, the `commands.py` module and the `commands/` package will be searched.
 
 ## Plugin System
 
-Amethyst has a plugin system, powered by [dynamicpy](https://github.com/NimajnebEC/dynamicpy) and inspired by [discord.py Cogs](https://discordpy.readthedocs.io/en/stable/ext/commands/cogs.html). You can create a plugin by simply defining a class that extends `AmethystPlugin`. If this is found by the [Dynamic Module Importer](#dynamic-module-import) then it will be automatically registered to the client, otherwise you will have to use the `AmethystClient.register_plugin` method.
+Amethyst has a plugin system, powered by [dynamicpy](https://github.com/NimajnebEC/dynamicpy) and inspired by [discord.py Cogs](https://discordpy.readthedocs.io/en/stable/ext/commands/cogs.html). You can create a plugin by simply defining a class that extends `amethyst.Plugin`. If this is found by the [Dynamic Module Importer](#dynamic-module-import) then it will be automatically registered to the client, otherwise you will have to use the `Client.register_plugin` method.
 
 An example plugin may look like the following:
 
 ```py
 import amethyst
 
-class ExamplePlugin(amethyst.AmethystPlugin):
+class ExamplePlugin(amethyst.Plugin):
 
-    @amethyst.event(amethyst.events.on_ready)
+    @amethyst.event(amethyst.on_ready)
     async def on_ready(self):
         channel = self.client.get_channel(000000000000000000)
         await channel.send("Bot is ready!")
 ```
 
 ### Plugin Dependency Injection
 
-Amethyst plugins support [dynamicpy dependency injection](https://github.com/NimajnebEC/dynamicpy#dependencylibrary) for their constructors. You can add dependencies to the client using the `AmethystClient.add_dependency` method, which will then be injected into constructor parameters when the plugin is registered.
+Amethyst plugins support [dynamicpy dependency injection](https://github.com/NimajnebEC/dynamicpy#dependencylibrary) for their constructors. You can add dependencies to the client using the `Client.add_dependency` method, which will then be injected into constructor parameters when the plugin is registered.
 
 ```py
 import mysql.connector
 import amethyst
 
-client = amethyst.AmethystClient(...)
+client = amethyst.Client(...)
 database: mysql.connector.MySQLConnection = mysql.connector.connect(...)
 client.add_dependency(database)
 
-class ExamplePlugin(amethyst.AmethystPlugin):
+class ExamplePlugin(amethyst.Plugin):
 
     def __init__(self, database: mysql.connector.MySQLConnection) -> None:
         self.database = database
 
 ```
 
 ## Evironment Variables
 
 Amethyst uses [python-dotenv](https://pypi.org/project/python-dotenv/) to load `.env` files found at the project root. This can be used to configure certain aspects of the library.
 
-| Name                | Default | Description                                                                                     |
-| ------------------- | ------- | ----------------------------------------------------------------------------------------------- |
-| AMETHYST_BOT_TOKEN  | _None_  | If present, `token` can be omitted from the `AmethystClient.run` and this will be used instead. |
-| AMETHYST_AUTO_SYNC  | true    | If `true`, the client will synchronise app_commands if they are out of date with Discord.       |
-| AMETHYST_SYNC_GUILD | _None_  | If present, app_commands will only be synchronised to specified guild id.                       |
+| Name               | Default | Description                                                                                |
+| ------------------ | ------- | ------------------------------------------------------------------------------------------ |
+| AMETHYST_TOKEN     | _None_  | If present, `token` can be omitted from the `Client.run` and this will be used instead.    |
+| AMETHYST_AUTO_SYNC | true    | If present, the client will synchronise app_commands if they are out of date with Discord. |
+| AMETHYST_GUILD     | _None_  | If present, the client will ignore all events from any guild with a differnet id.          |
 
 ## Roadmap
 
-- [ ] Context Menus
 - [ ] Hybrid Commands
-- [ ] Plugins enable/disable after initialisation
 - [ ] Debug mode featuring automatic reload
```

### Comparing `discord_amethyst-1.0.1/pyproject.toml` & `discord_amethyst-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "discord-amethyst"
-version = "1.0.1"
+version = "2.0.0"
 description = "An opinionated extension for discord.py."
 authors = ["NimajnebEC <nimajnebec@users.noreply.github.com>"]
 packages = [{ include = "amethyst", from = "src" }]
+repository = "https://github.com/NimajnebEC/discord-amethyst"
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
-python-dotenv = "^1.0.0"
-discord-py = "^2.3.1"
-dynamicpy = "^1.1.0"
+lavender-logging = "^1.0.0"
+environ-import = "^0.1.0"
+discord-py = "^2.3.2"
+dynamicpy = "^1.2.2"
 croniter = "^1.4.1"
 python = "^3.11"
 
-
 [tool.poetry.group.dev.dependencies]
-flake8-length = "^0.3.1"
-flake8 = "^6.0.0"
 pytest = "^7.3.1"
-isort = "^5.12.0"
+ruff = "^0.1.14"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+line-length = 92
```

### Comparing `discord_amethyst-1.0.1/src/amethyst/client.py` & `discord_amethyst-2.0.0/src/amethyst/amethyst.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,583 +1,624 @@
+from __future__ import annotations
+
 import asyncio
 import contextlib
 import logging
-import os
-from datetime import datetime
-from typing import Any, Callable, Coroutine, Self, Type, TypeVar, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Concatenate,
+    Coroutine,
+    ParamSpec,
+    Self,
+    Type,
+    TypeAlias,
+    TypeVar,
+)
 
 import discord
 import dynamicpy
-from discord import app_commands
-from discord.abc import Snowflake
-from discord.utils import MISSING
-from dotenv import load_dotenv
+import environ
+import envnull
+import lavender
 
 from amethyst import error
-from amethyst.util import is_dict_subset
-from amethyst.widget import (
-    AmethystCommand,
-    AmethystEvent,
-    AmethystEventHandler,
-    AmethystPlugin,
-    AmethystSchedule,
-    DiscordPyEvent,
-    events,
-)
+from amethyst.util import classproperty, is_dict_subset, safesubclass
 
-__all__ = ("AmethystClient",)
+if TYPE_CHECKING:
+    from amethyst.widget.event import Event
 
-_environ_key_token = "AMETHYST_BOT_TOKEN"
-_environ_key_sync_guild = "AMETHSYT_SYNC_GUILD"
-_environ_key_auto_sync = "AMETHYST_AUTO_SYNC"
+__all__ = ("Client", "Plugin", "BaseWidget", "WidgetPlugin")
 
-_schedule_delay_cutoff = 30
+WidgetT = TypeVar("WidgetT", bound="BaseWidget[Any]")
+PluginT = TypeVar("PluginT", bound="Plugin")
+P = ParamSpec("P")
+T = TypeVar("T")
 
-_default_modules = [".command", ".commands", ".plugins", ".plugin"]
+PluginSelf: TypeAlias = "Self@Plugin"  # type: ignore
+CallbackT = TypeVar("CallbackT", bound=Callable[Concatenate[PluginSelf, ...], Any])
+Coro = Coroutine[Any, Any, T]
 
+_default_modules = [".command", ".commands", ".plugins", ".plugin"]
 _log = logging.getLogger(__name__)
 
-CoroT = TypeVar("CoroT", bound=Callable[..., Coroutine[Any, Any, Any]])
-T = TypeVar("T")
-
 
-def try_register(func: Callable[[T], None], widget: T) -> None:
-    """Calls the specified register method, suppressing any raised `WidgetAlreadyRegisteredError`.
+class Client(discord.Client):
+    """Represents a connection to Discord. This class extends discord.Client and is the primary home of amethyt's additions.
 
     Parameters
     ----------
-    func : `Callable[[T], None]`
-        The register method to wrap.
-    widget : `T`
-        The widget to register.
+    intents: `Intents`
+        The intents that you want to enable for the session. This is a way of
+        disabling and enabling certain gateway events from triggering and being sent.
+    search_modules : `list[str]`, optional
+        The modules to search for widgets and plugins in
+    max_messages: `int`, optional
+        The maximum number of messages to store in the internal message cache.
+        This defaults to ``1000``. Passing in ``None`` disables the message cache.
+    proxy: `str`, optional
+        Proxy URL.
+    proxy_auth: `aiohttp.BasicAuth`, optional
+        An object that represents proxy HTTP Basic Authorization.
+    shard_id: `int`, optional
+        Integer starting at ``0`` and less than `.shard_count`.
+    shard_count: `int`, optional
+        The total number of shards.
+    application_id: `int`
+        The client's application ID.
+    member_cache_flags: `MemberCacheFlags`
+        Allows for finer control over how the library caches members.
+        If not given, defaults to cache as much as possible with the
+        currently selected intents.
+    chunk_guilds_at_startup: `bool`
+        Indicates if `.on_ready` should be delayed to chunk all guilds
+        at start-up if necessary. This operation is incredibly slow for large
+        amounts of guilds. The default is ``True`` if `Intents.members`
+        is ``True``.
+    status: `.Status`, optional
+        A status to start your presence with upon logging on to Discord.
+    activity: `.BaseActivity`, optional
+        An activity to start your presence with upon logging on to Discord.
+    allowed_mentions: `AllowedMentions`, optional
+        Control how the client handles mentions by default on every message sent.
+    heartbeat_timeout: `float`
+        The maximum numbers of seconds before timing out and restarting the
+        WebSocket in the case of not receiving a HEARTBEAT_ACK. Useful if
+        processing the initial packets take too long to the point of disconnecting
+        you. The default timeout is 60 seconds.
+    guild_ready_timeout: `float`
+        The maximum number of seconds to wait for the GUILD_CREATE stream to end before
+        preparing the member cache and firing READY. The default timeout is 2 seconds.
+    assume_unsync_clock: `bool`
+        Whether to assume the system clock is unsynced. This applies to the ratelimit handling
+        code. If this is set to ``True``, the default, then the library uses the time to reset
+        a rate limit bucket given by Discord. If this is ``False`` then your system clock is
+        used to calculate how long to sleep for. If this is set to ``False`` it is recommended to
+        sync your system clock to Google's NTP server.
+    enable_debug_events: `bool`
+        Whether to enable events that are useful only for debugging gateway related information.
+
+        Right now this involves :func:`on_socket_raw_receive` and :func:`on_socket_raw_send`. If
+        this is ``False`` then those events will not be dispatched (due to performance considerations).
+        To enable these events, this must be set to ``True``. Defaults to ``False``.
+    http_trace: `aiohttp.TraceConfig`
+        The trace configuration to use for tracking HTTP requests the library does using ``aiohttp``.
+        This allows you to check requests the library is using. For more information, check the
+        [aiohttp documentation](https://docs.aiohttp.org/en/stable/client_advanced.html#client-tracing).
+    max_ratelimit_timeout: `float`, optional
+        The maximum number of seconds to wait when a non-global rate limit is encountered.
+        If a request requires sleeping for more than the seconds passed in, then
+        :exc:`~discord.RateLimited` will be raised. By default, there is no timeout limit.
+        In order to prevent misuse and unnecessary bans, the minimum value this can be
+        set to is ``30.0`` seconds.
     """
-    with contextlib.suppress(error.WidgetAlreadyRegisteredError):
-        return func(widget)
-
 
-class AmethystClient(discord.Client):
-    """Represents a connection to Discord. This class extends discord.Client and is the primary home of amethyt's additions."""
+    ##region Public Methods
 
     def __init__(
         self,
         intents: discord.Intents,
-        *,
-        search_modules: list[str] | None = None,
         **options: Any,
     ) -> None:
-        """Represents a connection to Discord. This class extends discord.Client and is the primary home of amethyt's additions.
-
-        Parameters
-        ----------
-        intents: `Intents`
-            The intents that you want to enable for the session. This is a way of
-            disabling and enabling certain gateway events from triggering and being sent.
-        search_modules : `list[str]`, optional
-            The modules to search for widgets and plugins in
-        max_messages: `int`, optional
-            The maximum number of messages to store in the internal message cache.
-            This defaults to ``1000``. Passing in ``None`` disables the message cache.
-        proxy: `str`, optional
-            Proxy URL.
-        proxy_auth: `aiohttp.BasicAuth`, optional
-            An object that represents proxy HTTP Basic Authorization.
-        shard_id: `int`, optional
-            Integer starting at ``0`` and less than `.shard_count`.
-        shard_count: `int`, optional
-            The total number of shards.
-        application_id: `int`
-            The client's application ID.
-        member_cache_flags: `MemberCacheFlags`
-            Allows for finer control over how the library caches members.
-            If not given, defaults to cache as much as possible with the
-            currently selected intents.
-        chunk_guilds_at_startup: `bool`
-            Indicates if `.on_ready` should be delayed to chunk all guilds
-            at start-up if necessary. This operation is incredibly slow for large
-            amounts of guilds. The default is ``True`` if `Intents.members`
-            is ``True``.
-        status: `.Status`, optional
-            A status to start your presence with upon logging on to Discord.
-        activity: `.BaseActivity`, optional
-            An activity to start your presence with upon logging on to Discord.
-        allowed_mentions: `AllowedMentions`, optional
-            Control how the client handles mentions by default on every message sent.
-        heartbeat_timeout: `float`
-            The maximum numbers of seconds before timing out and restarting the
-            WebSocket in the case of not receiving a HEARTBEAT_ACK. Useful if
-            processing the initial packets take too long to the point of disconnecting
-            you. The default timeout is 60 seconds.
-        guild_ready_timeout: `float`
-            The maximum number of seconds to wait for the GUILD_CREATE stream to end before
-            preparing the member cache and firing READY. The default timeout is 2 seconds.
-        assume_unsync_clock: `bool`
-            Whether to assume the system clock is unsynced. This applies to the ratelimit handling
-            code. If this is set to ``True``, the default, then the library uses the time to reset
-            a rate limit bucket given by Discord. If this is ``False`` then your system clock is
-            used to calculate how long to sleep for. If this is set to ``False`` it is recommended to
-            sync your system clock to Google's NTP server.
-        enable_debug_events: `bool`
-            Whether to enable events that are useful only for debugging gateway related information.
-
-            Right now this involves :func:`on_socket_raw_receive` and :func:`on_socket_raw_send`. If
-            this is ``False`` then those events will not be dispatched (due to performance considerations).
-            To enable these events, this must be set to ``True``. Defaults to ``False``.
-        http_trace: `aiohttp.TraceConfig`
-            The trace configuration to use for tracking HTTP requests the library does using ``aiohttp``.
-            This allows you to check requests the library is using. For more information, check the
-            [aiohttp documentation](https://docs.aiohttp.org/en/stable/client_advanced.html#client-tracing).
-        max_ratelimit_timeout: `float`, optional
-            The maximum number of seconds to wait when a non-global rate limit is encountered.
-            If a request requires sleeping for more than the seconds passed in, then
-            :exc:`~discord.RateLimited` will be raised. By default, there is no timeout limit.
-            In order to prevent misuse and unnecessary bans, the minimum value this can be
-            set to is ``30.0`` seconds.
-        """
         super().__init__(intents=intents, **options)
-        self._search_modules: list[str] | None = search_modules
-        self._home_package: str | None = self._get_home_package()
-        self._loader: dynamicpy.DynamicLoader = self._build_loader()
-        self._tree: app_commands.CommandTree[Self] = app_commands.CommandTree(self)
-        self._dependencies: dynamicpy.DependencyLibrary = dynamicpy.DependencyLibrary()
-        self._schedule_sleep_task: asyncio.Task | None = None
-        self._plugins: list[Type[AmethystPlugin]] = []
-        self._events: list[AmethystEventHandler] = []
-        self._schedules: list[AmethystSchedule] = []
-        self._commands: list[AmethystCommand] = []
+        self._instantiating_package = self._get_instantiating_package()
+        self._setup_hooks: list[Callable[..., Coro[None]]] = []
+        self._auto_sync = envnull.AMETHYST_AUTO_SYNC is not None
+        self._tree = discord.app_commands.CommandTree(self)
+        self._dependencies = dynamicpy.DependencyLibrary()
+        self._module_loader = self._build_module_loader()
+        self._plugins: dict[Type[Plugin], Plugin] = {}
+        self._tasks: list[Coro[Any]] | None = []
+        self._widgets: list[BaseWidget] = []
+
+        self._guild = None
+        if envnull.AMETHYST_GUILD is not None:
+            self._guild = int(envnull.AMETHYST_GUILD)
 
     @property
-    def home_package(self) -> str | None:
-        """The parent package of the module where this client was instantiated. Is `None` if it was a top-level module."""
-        return self._home_package
+    def allowed_guild(self) -> int | None:
+        """If present, the bot will ignore all events from guilds with a different id."""
+        return self._guild
 
     @property
-    def tree(self) -> app_commands.CommandTree:
+    def tree(self) -> discord.app_commands.CommandTree:
         """The command tree responsible for handling the application commands in this bot."""
         return self._tree
 
-    def add_dependency(self, dependency: Any) -> None:
-        """Add a dependency to the client's dependency library.
+    def has_plugin(self, plugin: Type[Plugin]) -> bool:
+        """Checks if the specified plugin has been registered with this client.
 
-        These dependencies are injected into plugin constructors.
+        Parameters
+        ----------
+        plugin : `Type[Plugin]`
+            The plugin to check if its been registered.
+
+        Returns
+        -------
+        bool
+            `True` if the plugin has been registered.
+        """
+        return plugin in self._plugins
+
+    def get_plugin(self, plugin: Type[PluginT]) -> PluginT:
+        """Gets the registered instance of the specified plugin.
 
         Parameters
         ----------
-        dependency : `Any`
-            The dependency to add the library.
+        plugin : `Type[PluginT]`
+            The plugin to get an instance of.
+
+        Returns
+        -------
+        `PluginT`
+            The registered instance of the specified plugin.
 
         Raises
         ------
-        `TypeError`
-            Raised when attempting to add a type to the library.
-        `DuplicateDependencyError`
-            Raised when another dependency with that type already exists in the library.
+        `KeyError`
+            Raised if no such plugin has been registered.
         """
-        self._dependencies.add(dependency)
+        if plugin in self._plugins:
+            return self._plugins[plugin]  # type: ignore
+        raise KeyError(f"Plugin {plugin.name} not registered.")
 
-    def register_command(self, command: AmethystCommand) -> None:
-        """Register an instance of `AmethystCommand` to the client.
+    def load_plugins(self, modules: list[str] = _default_modules) -> None:
+        """Load all plugins found in the specified modules and their submodules.
 
         Parameters
         ----------
-        `command` : `AmethystCommand`
-            The command to register.
+        modules : `list[str]`, optional
+            The list of modules to recursively search.
         """
-        # Ensure not already registered
-        if command in self._commands:
-            raise error.WidgetAlreadyRegisteredError(
-                f"Command {command.name} has already been registered."
-            )
-        _log.debug("Registering command '%s'", command.name)
-        self._tree.add_command(command)
-        self._commands.append(command)
+        _log.debug("Loading modules %s", modules)
+        for module in modules:
+            if self._instantiating_package is None and module.startswith("."):
+                module = module[1:]
+            with contextlib.suppress(ImportError):
+                self._module_loader.load_module(module, self._instantiating_package)
 
-    def register_plugin(self, plugin: Type[AmethystPlugin]) -> None:
-        """Register an `AmethystPlugin` to the client.
+    def register_plugin(self, plugin: Type[Plugin]) -> None:
+        """Register the specified plugin and all its widgets.
 
         Parameters
         ----------
-        plugin : `Type[AmethystPlugin]`
-            A type inheriting from `AmethystPlugin` to register to the client.
-        """
+        plugin : `Type[Plugin]`
+            The plugin to register.
 
-        # Ensure not already registered
+        Raises
+        ------
+        `DuplicatePluginError`
+            Raised if the plugin has already been registered.
+        `PluginDependencyError`
+            Raised if there was an error while injecting dependencies.
+        """
         if plugin in self._plugins:
-            raise error.WidgetAlreadyRegisteredError(
-                f"Plugin {plugin.name} has already been registered."
-            )
+            raise error.DuplicatePluginError(f"{plugin.name} has already been registered.")
         _log.debug("Registering plugin '%s'", plugin.name)
-        self._plugins.append(plugin)
 
+        # * Instantiate Plugin
         try:
             instance = plugin.__new__(plugin)
-            instance._client = self  # add client attribute
+            setattr(instance, "_client", self)
             self._dependencies.inject(instance.__init__)
-        except dynamicpy.DependencyNotFoundError as e:
-            raise error.RegisterPluginError(
-                f"Could not find a dependency when injecting into '{plugin.name}'"
-            ) from e
-        except dynamicpy.InjectDependenciesError as e:
-            raise error.RegisterPluginError(
+        except (dynamicpy.DependencyNotFoundError, dynamicpy.InjectDependenciesError) as e:
+            raise error.PluginDependencyError(
                 f"Error injecting dependencies into '{plugin.name}'"
             ) from e
 
-        self._loader.load_object(instance)
+        # * Load widgets
+        loader = dynamicpy.DynamicLoader()
+
+        @loader.widget_handler(BaseWidget)
+        def _(widget: BaseWidget):
+            if widget not in self._widgets:
+                widget.register(instance, self)
+                self._widgets.append(widget)
+
+        loader.load_object(instance)
+
+        # * Add to plugins list
+        self._plugins[plugin] = instance
 
-    def register_event(self, handler: AmethystEventHandler) -> None:
-        """Register an `AmethystEventHandler` to the client.
+    def add_dependency(self, dependency: Any) -> None:
+        """Add a dependency to the client's dependency library.
+
+        These dependencies are injected into plugin constructors.
 
         Parameters
         ----------
-        event : `AmethystEvent`
-            The instance `AmethystEventHandler` to register to the client.
+        dependency : `Any`
+            The dependency to add the library.
+
+        Raises
+        ------
+        `TypeError`
+            Raised when attempting to add a type to the library.
+        `DuplicateDependencyError`
+            Raised when another dependency with that type already exists in the library.
         """
+        self._dependencies.add(dependency)
 
-        # Ensure not already registered
-        if handler in self._events:
-            raise error.WidgetAlreadyRegisteredError(
-                f"Handler {handler.name} has already been registered."
-            )
-        self._events.append(handler)
-        event = handler.event
-        _log.debug(
-            "Registering handler '%s' for event '%s'",
-            handler.name,
-            event.name,
-        )
+    async def wait_for(
+        self,
+        event: "Event[P]",
+        /,
+        *,
+        check: Callable[P, bool] | None = None,
+        timeout: float | None = None,
+    ) -> None:
+        """
+        Waits for a WebSocket event to be dispatched.
 
-        # Setup invoker for default events
-        if isinstance(handler.event, DiscordPyEvent) and not hasattr(self, event.name):
-            setattr(
-                self,
-                event.name,
-                lambda *args, **kwargs: self.invoke_event(event, *args, **kwargs),
-            )
+        This could be used to wait for a user to reply to a message,
+        or to react to a message, or to edit a message in a self-contained
+        way.
+
+        The ``timeout`` parameter is passed onto :func:`asyncio.wait_for`. By default,
+        it does not timeout. Note that this does propagate the
+        :exc:`asyncio.TimeoutError` for you in case of timeout and is provided for
+        ease of use.
+
+        In case the event returns multiple arguments, a :class:`tuple` containing those
+        arguments is returned instead. Please check the
+        documentation for a list of events and their
+        parameters.
+
+        This function returns the **first event that meets the requirements**.
 
-    def register_schedule(self, schedule: AmethystSchedule) -> None:
-        """Register an `AmethystSchedule` to the client.
 
         Parameters
         ----------
-        schedule : `AmethystSchedule`
-            The instance `AmethystSchedule` to register to the client.
+        event : `Event[P]`
+            The event to wait for.
+        check : `Callable[P, bool] | None`, optional
+            A predicate to check what to wait for. The arguments must meet the
+            parameters of the event being waited for.
+        timeout : `float | None`, optional
+            The number of seconds to wait before timing out and raising `asyncio.TimeoutError`.
+        """
+        await super().wait_for(event.name, check=check, timeout=timeout)
+
+    def event(
+        self, event: "Event[P]"
+    ) -> Callable[[Callable[P, Coro[None]]], Callable[P, Coro[None]]]:
+        """A decorator that registers an event to listen to.
+
+        Parameters
+        ----------
+        event : `Event`
+            The event to listen to.
         """
 
-        # Ensure not already registered
-        if schedule in self._schedules:
-            raise error.WidgetAlreadyRegisteredError(
-                f"Schedule {schedule.name} has already been registered."
-            )
-        _log.debug("Registering schedule '%s'", schedule.name)
-        self._schedules.append(schedule)
+        def decorator(func: Callable[P, Coro[None]]) -> Callable[P, Coro[None]]:
+            from amethyst.widget.event import EventWidget
 
-        if self._schedule_sleep_task is None:
-            if self.is_ready():
-                # start loop
-                self.loop.create_task(self._schedule_loop())
-        elif (
-            not self._schedule_sleep_task.cancelled()
-            and not self._schedule_sleep_task.cancelling()
-        ):
-            # Cancel the sleep task to recalculate next_datetime
-            self._schedule_sleep_task.cancel()
-
-    @overload
-    def invoke_event(
-        self, event: AmethystEvent[Any, Coroutine], *args, **kwargs
-    ) -> Coroutine[Any, Any, None]:
-        ...
-
-    @overload
-    def invoke_event(self, event: AmethystEvent[Any, None], *args, **kwargs) -> None:
-        ...
+            EventWidget(func, event).register(None, self)  # type: ignore
+            return func
 
-    def invoke_event(self, event: AmethystEvent, *args, **kwargs) -> Coroutine | None:
-        """Invokes all the registered handlers of the specified event.
+        return decorator
+
+    def create_task(self, task: Coro[Any]) -> None:
+        """Creates an asynchronous task to be started once the event loop is set-up.
 
         Parameters
         ----------
-        event : `AmethystEvent`
-            The event to invoke the handlers of.
-
-        Returns
-        -------
-        `Coroutine | None`
-            When the event is a coroutine, a `Coroutine` will be returned. Otherwise `None`.
+        task : `Coro[Any]`
+            The coroutine to start.
         """
-        handlers = (e for e in self._events if e.event == event)
-        if event.is_coroutine:
-            return asyncio.gather(*(h.invoke(*args, **kwargs) for h in handlers))  # type: ignore
-        for handler in handlers:
-            handler.invoke(*args, **kwargs)
+        if self._tasks is None:
+            self.loop.create_task(task)
+        else:
+            self._tasks.append(task)
 
-    async def commands_in_sync(self, guild: Snowflake | None = None) -> bool:
-        """Checks if the the commands locally registered to this client are in sync with the commands on discord.
+    async def tree_changed(self, guild: discord.abc.Snowflake | None = None) -> bool:
+        """Checks if the local application command tree is different from the remote.
 
         Parameters
         ----------
-        guild : `Snowflake`, optional
-            The guild to check commands from. If left blank, checks global commands.
+        guild : `discord.abc.Snowflake | None`, optional
+            The guild to check the commands against. If not passed then global commands are checked instead.
 
         Returns
         -------
         `bool`
-            Returns true if the local commands match the remote commands.
+            `True` if the application commands do not match.
         """
-        local = {c.name: c.to_dict() for c in self.tree.get_commands(guild=guild)}
-        remote = {
-            c.name: {
-                "nsfw": c.nsfw,
-                "dm_permission": c.dm_permission,
-                "default_member_permissions": c.default_member_permissions,
-                **c.to_dict(),
+        remotes = await self.tree.fetch_commands(guild=guild)
+        locals = self.tree.get_commands(guild=guild)
+
+        if len(remotes) != len(locals):
+            return True
+
+        for local in locals:
+            subset = local.to_dict()
+            remote = discord.utils.get(
+                remotes,
+                name=local.name,
+                type=discord.AppCommandType(subset["type"]),
+            )
+
+            if remote is None:
+                return True
+
+            superset = {
+                "default_member_permissions": None
+                if remote.default_member_permissions is None
+                else remote.default_member_permissions.value,
+                "dm_permission": remote.dm_permission,
+                "nsfw": remote.nsfw,
+                **remote.to_dict(),
             }
-            for c in await self.tree.fetch_commands(guild=guild)
-        }
 
-        # Check for commands that only appear in one location
-        if len(set(local.keys()).symmetric_difference(remote.keys())) > 0:
-            return False
+            # USER and MESSAGE commands have an empty string for their description
+            # https://discord.com/developers/docs/interactions/application-commands#application-command-object-application-command-structure
+            if subset["type"] in (
+                discord.AppCommandType.message,
+                discord.AppCommandType.user,
+            ):
+                subset["description"] = ""
 
-        # Check for changes to existing commands
-        return is_dict_subset(remote, local)
+            if not is_dict_subset(superset, subset):
+                return True
 
-    def load(self, search_modules: list[str] | None = None) -> None:
-        """Recursively search the specified modules and register all widgets found.
+        return False
+
+    async def refresh_tree(self, guild: discord.abc.Snowflake | None = None) -> None:
+        """Synchronises the application command tree if it has changed.
 
         Parameters
         ----------
-        search_modules : `list[str]`, optional
-            The modules to search through, will use the modules specified in the constructor by default
+        guild : `discord.abc.Snowflake | None`, optional
+            The guild to refresh the commands to. If not passed then global commands are refreshed instead.
         """
-        self._load_modules(
-            search_modules or self._search_modules or _default_modules,
-            search_modules is None and self._search_modules is None,
-        )
+        if await self.tree_changed(guild):
+            _log.info("Synchronising application tree...")
+            await self.tree.sync(guild=guild)
+        else:
+            _log.debug("Skipping tree synchronisation - already up to date.")
 
-    async def start(self, token: str | None = None, *, reconnect: bool = True) -> None:
-        """A Shorthand coroutine for `load` + `login` + `connect`.
-
-        Also loads the .env file if it is found in the project directory.
+    def guild_allowed(self, check: discord.Guild | int | None) -> bool:
+        """Checks if the specified guild is allowed based on the `AMETHYST_GUILD` environment variable.
 
         Parameters
         ----------
-        token: `str`
-            The authentication token. Do not prefix this token with
-            anything as the library will do it for you.
-        reconnect: `bool`
-            If we should attempt reconnecting, either due to internet
-            failure or a specific failure on Discord's part. Certain
-            disconnects that lead to bad state will not be handled (such as
-            invalid sharding payloads or bad tokens).
-        """
-        load_dotenv()
-        self.load()
+        check : `discord.Guild | int | None`
+            The guild to check.
 
-        if token is None and _environ_key_token not in os.environ:
-            raise RuntimeError("Bot token was not supplied in parameters or eviron.")
-        token = token or os.environ[_environ_key_token]
+        Returns
+        -------
+        bool
+            `True` if guild is allowed.
+        """
+        if self.allowed_guild is None:
+            return True
 
-        await super().start(token, reconnect=reconnect)
+        if isinstance(check, discord.Guild):
+            return check.id == self.allowed_guild
+        if isinstance(check, int):
+            return check == self.allowed_guild
+        return False
 
     def run(
         self,
-        token: str | None = None,
         *,
         reconnect: bool = True,
-        log_handler: logging.Handler | None = MISSING,
-        log_formatter: logging.Formatter = MISSING,
-        log_level: int = MISSING,
-        root_logger: bool = False,
+        guild: int | None = -1,
+        token: str | None = None,
+        log_level: int = logging.INFO,
+        auto_sync: bool | None = None,
+        log_filters: dict[str, int] = {},
+        plugin_modules: list[str] = _default_modules,
     ) -> None:
         """A blocking call that abstracts away the event loop
         initialisation from you.
 
-        If you want more control over the event loop then this
-        function should not be used. Use `start` coroutine
-        or `connect` + `login`.
-
-        This function also sets up the logging library to make it easier
-        for beginners to know what is going on with the library. For more
-        advanced users, this can be disabled by passing ``None`` to
-        the ``log_handler`` parameter.
-
-        WARNING
-        -------
-        This function must be the last function to call due to the fact that it
-        is blocking. That means that registration of events or anything being
-        called after this function call will not execute until it returns.
-
-        Parameters
-        -----------
-        token: `str`
-            The authentication token. Do not prefix this token with
-            anything as the library will do it for you.
-        reconnect: `bool`
-            If we should attempt reconnecting, either due to internet
-            failure or a specific failure on Discord's part. Certain
-            disconnects that lead to bad state will not be handled (such as
-            invalid sharding payloads or bad tokens).
-        log_handler: `logging.Handler`, optional
-            The log handler to use for the library's logger. If this is ``None``
-            then the library will not set up anything logging related. Logging
-            will still work if ``None`` is passed, though it is your responsibility
-            to set it up.
-
-            The default log handler if not provided is `logging.StreamHandler`.
-
-        log_formatter: `logging.Formatter`
-            The formatter to use with the given log handler. If not provided then it
-            defaults to a colour based logging formatter (if available).
-
-        log_level: `int`
-            The default log level for the library's logger. This is only applied if the
-            ``log_handler`` parameter is not ``None``. Defaults to ``logging.INFO``.
-
-        root_logger: `bool`
-            Whether to set up the root logger rather than the library logger.
-            By default, only the library logger (``'discord'``) is set up. If this
-            is set to ``True`` then the root logger is set up as well.
+        This function also sets up [Lavender Logging](https://github.com/NimajnebEC/lavender-logging).
 
-            Defaults to ``False``.
-        """
-        super().run(
-            token,  # type: ignore
+        Parameters
+        ----------
+        token : `str | None`, optional
+            The authentication token. If not specified it will be taken from the `AMETHYST_TOKEN` environment variable.
+        reconnect : `bool`, optional
+           If we should attempt reconnecting, either due to internet failure or a specific failure on Discord's part. Certain
+           disconnects that lead to bad state will not be handled (such as invalid sharding payloads or bad tokens).
+        guild : `int | None`, optional
+            Overrides the `AMETHYST_GUILD` environment variable. If not `None` then the bot will only handle events from the specified guild.
+        guild : `bool | None`, optional
+            Overrides the `AMETHYST_AUTO_SYNC` environment variable. If `True` then the application command tree will be refreshed automatically.
+        log_level : `int`, optional
+            The default log level for Lavender's logger.
+        log_filters : `dict[str, int]`, optional
+            Initial logging filter patterns, by default no specific filters are specified.
+        plugin_modules : `list[str]`, optional
+            A list of modules to recursively search of plugins.
+        """
+        if guild != -1:
+            self._guild = guild
+        if auto_sync is not None:
+            self._auto_sync = auto_sync
+
+        lavender.setup(level=log_level, filter_config=log_filters)
+        self.load_plugins(plugin_modules)
+        return super().run(
+            token or environ.AMETHYST_TOKEN,
             reconnect=reconnect,
-            log_handler=log_handler,
-            log_formatter=log_formatter,
-            log_level=log_level,
-            root_logger=root_logger,
+            log_handler=None,
         )
 
-    def event(self, coro: CoroT) -> CoroT:
-        # override default event decorator to use new amethyst event system
-        """A decorator that registers an event handler to listen.
+    ##endregion
 
-        It is recommended to use the `amethyst.event` decorator instead of this as it supports type hints.
-        """
-        name: str = coro.__name__
-        if not hasattr(events, name):
-            raise TypeError(f"Could not find event '{name}'")
-
-        event = getattr(events, name)
-
-        if not isinstance(event, AmethystEvent):
-            raise TypeError(f"Could not find a valid event called '{name}'")
-
-        handler = AmethystEventHandler(event, coro)
-        self.register_event(handler)
-
-        return coro
+    ##region Events
 
     async def setup_hook(self) -> None:
-        # Synchronise commands if out of date
-        if os.getenv(_environ_key_auto_sync) != "false":
+        # ensure that all hooks are run before continuing
+        await asyncio.gather(*(h() for h in self._setup_hooks))
+
+        if self._auto_sync:
             guild = None
-            if _environ_key_sync_guild in os.environ:
-                guild = discord.Object(os.environ[_environ_key_sync_guild])
+            if self._guild is not None:
+                guild = discord.Object(self._guild)
                 self.tree.copy_global_to(guild=guild)
+            await self.refresh_tree(guild)
 
-            if not await self.commands_in_sync(guild):
-                _log.info("Synchronising Commands...")
-                await self.tree.sync(guild=guild)
-
-        # Invoke subscribed handlers
-        await self.invoke_event(events.on_setup_hook)
+        # Run pending tasks
+        if self._tasks is not None:
+            for task in self._tasks:
+                self.loop.create_task(task)
+            self._tasks = None
 
-    async def on_ready(self):
-        """override on_ready event."""
+    async def on_ready(self) -> None:
         if self.user is None:
             raise AttributeError("Expected client to be logged in.")
         name = self.user.global_name or f"{self.user.name}#{self.user.discriminator}"
         _log.info(
             "Client connected as '%s' with %sms ping.",
             name,
             round(self.latency * 1000),
         )
 
-        # Start schedule loop
-        if self._schedule_sleep_task is None and len(self._schedules) > 0:
-            self.loop.create_task(self._schedule_loop())
-
-        # Invoke subscribed handlers
-        await self.invoke_event(events.on_ready)
-
-    async def _schedule_loop(self):
-        """Is responsible for calling schedules"""
-        while not self.is_closed():
-            schedule_map = {s: s.next_occurrence() for s in self._schedules}
-            next_datetime = min(schedule_map.values())
-
-            while True:
-                delay = (next_datetime - datetime.now()).total_seconds()
-                final = delay <= _schedule_delay_cutoff
-
-                if not final:
-                    delay /= 2
-
-                # Sleep until next point
-                self._schedule_sleep_task = asyncio.Task(asyncio.sleep(delay))
-                try:
-                    await self._schedule_sleep_task
-                except asyncio.CancelledError:
-                    break  # Break to recalculate next_datetime
-
-                # Invoke schedules
-                if final:
-                    schedules = [s for s, d in schedule_map.items() if d == next_datetime]
-                    _log.debug("Invoking schedules %s", schedules)
-                    asyncio.gather(*(s.invoke() for s in schedules))
-                    await asyncio.sleep(1)  # sleep until the end of the second
-                    break  # Break and recalculate for next schedule
+    ##endregion
 
-    def _build_loader(self) -> dynamicpy.DynamicLoader:
-        """Builds a DynamicLoader for finding widgets to add to the client."""
+    ##region Private Methods
+
+    def _build_module_loader(self) -> dynamicpy.DynamicLoader:
+        """Build the `DynamicLoader` used for finding plugins in modules."""
         loader = dynamicpy.DynamicLoader()
 
-        loader.register_type_handler(
-            lambda _, v: try_register(self.register_command, v), AmethystCommand
-        )
-        loader.register_type_handler(
-            lambda _, v: try_register(self.register_event, v), AmethystEventHandler
-        )
-        loader.register_type_handler(
-            lambda _, v: try_register(self.register_schedule, v), AmethystSchedule
-        )
-        loader.register_handler(
-            lambda _, v: try_register(self.register_plugin, v),
-            lambda _, v: isinstance(v, type)
-            and v is not AmethystPlugin
-            and issubclass(v, AmethystPlugin),
-        )
+        @loader.handler()
+        def _(_, value: Any):
+            if (
+                value is not Plugin
+                and safesubclass(value, Plugin)
+                and not issubclass(value, WidgetPlugin)
+            ):
+                with contextlib.suppress(error.DuplicatePluginError):
+                    self.register_plugin(value)
 
         return loader
 
-    def _load_modules(self, search_modules: list[str], allow_missing: bool = False) -> None:
-        """Loads the modules specified in `search_modules` using the client's DynamicLoader."""
-        _log.debug("Loading modules %s", search_modules)
-        for module in search_modules:
-            if self.home_package is None and module.startswith("."):
-                module = module[1:]
-            try:
-                self._loader.load_module(module, self.home_package)
-            except ImportError:
-                if not allow_missing:
-                    raise
+    def _get_instantiating_package(self) -> str | None:
+        """Return the package the application was instantiated from."""
 
-    def _get_home_package(self) -> str | None:
-        """Return the home package of the application."""
         try:
             module = dynamicpy.get_foreign_module()
 
             if dynamicpy.is_package(module):
                 package = module
             else:
                 package = dynamicpy.get_module_parent(module)
 
-            _log.debug("Home package located as '%s'", package)
+            _log.debug("Instantiating package located as '%s'", package)
             return package
         except dynamicpy.NoParentError:
             _log.debug("Instantiating module is top-level.")
             return None
         except ImportError as e:
-            _log.error("Error locating home package: %s", e)
-            raise error.ModuleLocateError("Error locating home package") from e
+            raise error.ModuleLocateError("Error locating instantiating package") from e
+
+    ##endregion
+
+
+class Plugin:
+    """The base class for all Amethyst plugins to inherit from."""
+
+    def __init__(self) -> None:
+        """The client will attempt to bind constructor parameters to dependencies when registered."""
+
+    @property
+    def client(self) -> Client:
+        """The instance of `Client` this plugin has been registered to."""
+        return getattr(self, "_client") if hasattr(self, "_client") else None  # type: ignore
+
+    @classproperty
+    def name(cls):
+        """The name of this plugin."""
+        return cls.__qualname__
+
+
+class BaseWidget(dynamicpy.BaseWidget[CallbackT]):
+    """The base class for all Amethyst widgets to inherit from."""
+
+    def __init__(self, callback: CallbackT) -> None:
+        super().__init__(callback)
+
+    def register(self, plugin: Plugin, client: Client) -> None:
+        """Register the widget with the provided `Client`.
+
+        Parameters
+        ----------
+        plugin: `Plugin`
+            The plugin this widget belongs to.
+        client : `Client`
+            The client to register the widget with.
+        """
+        raise NotImplementedError(f"{self.type} must implement 'register'")
+
+    @classproperty
+    def type(cls) -> str:
+        """The name of the type of widget."""
+        return cls.__qualname__
+
+    @property
+    def name(self) -> str:
+        """The name of this widget instance."""
+        return self.callback.__qualname__
+
+
+class _WidgetPluginMeta(type):
+    """Metaclass for injecting plugin registration into widgets."""
+
+    def __new__(mcls, name, bases, namespace):
+        cls = super().__new__(mcls, name, bases, namespace)
+        loader = dynamicpy.DynamicLoader()
+        loader.register_handler(cls._inject, lambda _, v: safesubclass(v, BaseWidget))
+        loader.load_object(cls)
+        return cls
+
+    def _inject(cls, _, widget) -> None:
+        """Inject the plugin's registration method into the widget's registration method."""
+
+        def proxy(widget, plugin: Plugin, client: Client) -> None:
+            if not client.has_plugin(cls):
+                # todo: protect against circular widget dependencies
+                client.register_plugin(cls)
+            widget_plugin = client.get_plugin(cls)  # type: ignore
+            cls.register(widget_plugin, widget, plugin)  # type: ignore
+
+        setattr(widget, "register", proxy)
+
+
+class WidgetPlugin(Plugin, metaclass=_WidgetPluginMeta):
+    """Base class for wiget plugins, allowing for the creation of more complex widgets."""
+
+    def register(self, widget: BaseWidget, plugin: Plugin):
+        """Register the provided widget with the client.
+
+        Parameters
+        ----------
+        widget : `BaseWidget`
+            The widget to be registered.
+        plugin : `Plugin`
+            The plugin this widget belongs to.
+        """
+        raise NotImplementedError(f"{self.name} must implement 'register'")
```

### Comparing `discord_amethyst-1.0.1/src/amethyst/error.py` & `discord_amethyst-2.0.0/src/amethyst/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 __all__ = (
-    "AmethystError",
-    "ModuleLocateError",
+    "PluginDependencyError",
+    "DuplicatePluginError",
     "RegisterPluginError",
-    "WidgetAlreadyRegisteredError",
+    "ModuleLocateError",
+    "AmethystError",
 )
 
 
 class AmethystError(Exception):
     """Base exception class for the amethyst module."""
 
 
 class ModuleLocateError(AmethystError):
     """Exception raised when there is an error locating a module."""
 
 
 class RegisterPluginError(AmethystError):
-    """Exception raised when there is an error registering a plugin."""
+    """Exceptions raised when registering a plugin fails."""
+
+
+class DuplicatePluginError(RegisterPluginError):
+    """Exception raised when attempting to register a plugin that is already registered."""
 
 
-class WidgetAlreadyRegisteredError(AmethystError):
-    """Exception raised when attempting to register a widget that has already been registered to this client."""
+class PluginDependencyError(RegisterPluginError):
+    """Exception raised when binding dependencies fails."""
```

### Comparing `discord_amethyst-1.0.1/src/amethyst/widget/event/handler.py` & `discord_amethyst-2.0.0/src/amethyst/widget/event/event.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,115 @@
 from __future__ import annotations
 
-import inspect
-from typing import Any, Callable, Coroutine, Generic, ParamSpec, TypeVar
+import logging
+from typing import (
+    Any,
+    Callable,
+    Concatenate,
+    Coroutine,
+    Generic,
+    ParamSpec,
+    TypeVar,
+)
 
-from amethyst.widget.abc import AmethystPlugin, Callback, CallbackWidget
+import discord
+
+from amethyst.amethyst import BaseWidget, Client, Plugin, PluginSelf
+
+__all__ = ("Event", "EventWidget", "event")
 
-PluginT = TypeVar("PluginT", bound=AmethystPlugin)
-NoneT = TypeVar("NoneT", bound=None | Coroutine[Any, Any, None])
 P = ParamSpec("P")
 T = TypeVar("T")
 
-HandlerCallback = Callback[PluginT, P, NoneT]
+Coro = Coroutine[Any, Any, None]
+Callback = Callable[Concatenate[PluginSelf, P], Coro]
 
-__all__ = ("AmethystEvent", "DiscordPyEvent", "AmethystEventHandler", "event")
+_log = logging.getLogger(__name__)
 
 
-class AmethystEvent(Generic[P, NoneT]):
+class Event(Generic[P]):
     """Represents a subscribable event and the callback signature.
 
     Events can be defined by simply making an instance of this class and typing it with the callback parameters.
 
     Example:
     ```
     on_message: AmethystEvent[[discord.Message], Coroutine] = AmethystEvent("on_message")
     ```
     """
 
-    def __init__(self, name: str, is_coroutine: bool = False) -> None:
-        """Represents a subscribable event and the callback signature.
-
-        Parameters
-        ----------
-        name: `str`
-            The name of this event.
-        is_coroutine : `bool`, optional
-            Wether this event will be called asynchronously, by default False
-        """
-        self._is_coroutine: bool = is_coroutine
+    def __init__(
+        self,
+        name: str,
+        guild: Callable[P, discord.Guild | int | None] | None = None,
+    ) -> None:
+        self._guild = guild or (lambda *_: None)
         self._name = name
 
     @property
     def name(self) -> str:
         """The name of the event."""
         return self._name
 
-    @property
-    def is_coroutine(self) -> bool:
-        """Wether the event is a coroutine."""
-        return self._is_coroutine
-
-
-class DiscordPyEvent(AmethystEvent[P, Coroutine]):
-    """Represents a normal Discord.py event and its parameters."""
-
-    def __init__(self, name: str) -> None:
-        super().__init__(name, True)
+    def get_guild(self, *args) -> discord.Guild | int | None:
+        return self._guild(*args)  # type: ignore
 
 
-class AmethystEventHandler(CallbackWidget[PluginT, P, NoneT]):
-    """Represents a event handler, consisting of a callback function and the `AmethystEvent` that its subscribed to.
+class EventWidget(BaseWidget[Callback[P]]):
+    """Represents a event widget, consisting of a callback function and the `AmethystEvent` that its subscribed to.
 
     These are not usually created manually, instead they are created using the `amethyst.event` decorator.
     """
 
-    def __init__(
-        self,
-        event: AmethystEvent[P, NoneT],
-        callback: Callback[PluginT, P, NoneT],
-        name: str | None = None,
-    ) -> None:
-        """Represents a event handler, consisting of a callback function and the `AmethystEvent` that its subscribed to.
-
-        These are not usually created manually, instead they are created using the `amethyst.event` decorator.
-
-        Parameters
-        ----------
-        event: `AmethystEvent[P, NoneT]`
-            The event to subscribe to.
-        callback : `Callable[Concatenate[PluginT, P], NoneT] | Callable[P, NoneT]`
-            The callback function that will be invoked for this event.
-        name: `str`, optional
-            The name of this event handler widget, by default None
-        """
-        super().__init__(callback, name)
+    def __init__(self, callback: Callback[P], event: Event[P]) -> None:
+        super().__init__(callback)
         self._event = event
 
     @property
-    def event(self) -> AmethystEvent[P, NoneT]:
+    def event(self) -> Event[P]:
         """The event this handler is subscribed to."""
         return self._event
 
-
-def event(
-    event: AmethystEvent[P, NoneT],
-) -> Callable[
-    [HandlerCallback[PluginT, P, NoneT]], AmethystEventHandler[PluginT, P, NoneT]
-]:
-    """Decorator to designate a regular function to be called when the specified event is invoked.
-
-    Parameters
-    ----------
-    event: `AmethystEvent`
-        The event to subscribe to.
-    """
-
-    def decorator(
-        func: HandlerCallback[PluginT, P, NoneT]
-    ) -> AmethystEventHandler[PluginT, P, NoneT]:
-        if event._is_coroutine != inspect.iscoroutinefunction(func):
-            raise TypeError(
-                f"Function must {'' if event._is_coroutine else 'not '}be a coroutine."
-            )
-
-        return AmethystEventHandler(event, func)
-
-    return decorator
+    def register(self, plugin: Plugin | None, client: Client) -> None:
+        _log.debug(
+            "Registering event handler '%s' for '%s'",
+            self.name,
+            self.event.name,
+        )
+
+        if self.event.name == "setup_hook":
+            if plugin is None:
+                client._setup_hooks.append(self.callback)
+            else:
+                client._setup_hooks.append(lambda: self.callback(plugin))  # type: ignore
+            return
+
+        async def wrapper(*args) -> None:
+            try:
+                await self.callback(*args)  # type: ignore
+            except Exception:
+                _log.error("Error handling '%s': ", self.name, exc_info=True)
+
+        def handler(*args) -> bool:
+            guild = self.event.get_guild(*args)
+            if guild is None or client.guild_allowed(guild):
+                if plugin is not None:  # To support anonymous events using Client.event
+                    args = (plugin, *args)
+
+                client.create_task(wrapper(*args))
+            else:
+                _log.debug(
+                    f"Skipping invokation of event '{self.name}' as guild '{guild}' is not allowed."
+                )
+            return False
+
+        client.create_task(client.wait_for(self.event, check=handler))  # type: ignore
+
+
+event = EventWidget.decorate
+"""Decorator to designate a regular function to be called when the specified event is invoked.
+
+Parameters
+----------
+event: `Event`
+    The event to subscribe to.
+"""
```

### Comparing `discord_amethyst-1.0.1/src/amethyst/widget/event/library.py` & `discord_amethyst-2.0.0/src/amethyst/widget/event/library.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 from typing import List, Sequence
 
 import discord
 from discord import app_commands
 
-from amethyst.widget.event.handler import DiscordPyEvent
+from amethyst.widget.event.event import Event
 
 __all__ = (
     "on_app_command_completion",
     "on_audit_log_entry_create",
     "on_automod_action",
     "on_automod_rule_create",
     "on_automod_rule_delete",
@@ -83,286 +83,285 @@
     "on_thread_member_join",
     "on_thread_member_remove",
     "on_thread_remove",
     "on_thread_update",
     "on_user_update",
     "on_voice_state_update",
     "on_webhooks_update",
+    "on_setup_hook",
 )
 
-on_raw_app_command_permissions_update: DiscordPyEvent[
+on_raw_app_command_permissions_update: Event[
     discord.RawAppCommandPermissionsUpdateEvent
-] = DiscordPyEvent("on_raw_app_command_permissions_update")
+] = Event("raw_app_command_permissions_update", lambda x: x.guild)
 """Called when application command permissions are updated.
 
 Parameters
 ----------
 payload: RawAppCommandPermissionsUpdateEvent
     The raw event payload data.
 """
 
-on_app_command_completion: DiscordPyEvent[
+on_app_command_completion: Event[
     [discord.Interaction, app_commands.Command | app_commands.ContextMenu]
-] = DiscordPyEvent("on_app_command_completion")
+] = Event("app_command_completion", lambda x, _: x.guild)
 """Called when a app_commands.Command or app_commands.ContextMenu has successfully completed without error.
 
 Parameters
 ----------
 interaction: Interaction
     The interaction of the command.
 command: Union[app_commands.Command, app_commands.ContextMenu]
     The command that completed successfully
 """
 
-on_automod_rule_create: DiscordPyEvent[discord.AutoModRule] = DiscordPyEvent(
-    "on_automod_rule_create"
+on_automod_rule_create: Event[discord.AutoModRule] = Event(
+    "on_automod_rule_create", lambda x: x.guild
 )
 """Called when a AutoModRule is created. You must have manage_guild to receive this.
 
 This requires Intents.auto_moderation_configuration to be enabled.
 
 Parameters
 ----------
 rule: AutoModRule
     The rule that was created.
 """
 
-on_automod_rule_update: DiscordPyEvent[discord.AutoModRule] = DiscordPyEvent(
-    "on_automod_rule_update"
+on_automod_rule_update: Event[discord.AutoModRule] = Event(
+    "on_automod_rule_update", lambda x: x.guild
 )
 """Called when a AutoModRule is updated. You must have manage_guild to receive this.
 
 This requires Intents.auto_moderation_configuration to be enabled.
 
 Parameters
 ----------
 rule: AutoModRule
     The rule that was updated.
 """
 
-on_automod_rule_delete: DiscordPyEvent[discord.AutoModRule] = DiscordPyEvent(
-    "on_automod_rule_delete"
+on_automod_rule_delete: Event[discord.AutoModRule] = Event(
+    "on_automod_rule_delete", lambda x: x.guild
 )
 """Called when a AutoModRule is deleted. You must have manage_guild to receive this.
 
 This requires Intents.auto_moderation_configuration to be enabled.
 
 Parameters
 ----------
 rule: AutoModRule
     The rule that was deleted.
 """
 
-on_automod_action: DiscordPyEvent[discord.AutoModAction] = DiscordPyEvent(
-    "on_automod_action"
-)
+on_automod_action: Event[discord.AutoModAction] = Event("automod_action", lambda x: x.guild)
 """Called when a AutoModAction is created/performed. You must have manage_guild to receive this.
 
 This requires Intents.auto_moderation_execution to be enabled.
 
 Parameters
 ----------
 execution: AutoModAction
     The rule execution that was performed.
 """
 
-on_guild_channel_delete: DiscordPyEvent[discord.abc.GuildChannel] = DiscordPyEvent(
-    "on_guild_channel_delete"
+on_guild_channel_delete: Event[discord.abc.GuildChannel] = Event(
+    "on_guild_channel_delete", lambda x: x.guild
 )
 """Called whenever a guild channel is deleted.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 channel: abc.GuildChannel
     The guild channel that got deleted.
 """
 
-on_guild_channel_create: DiscordPyEvent[discord.abc.GuildChannel] = DiscordPyEvent(
-    "on_guild_channel_create"
+on_guild_channel_create: Event[discord.abc.GuildChannel] = Event(
+    "on_guild_channel_create", lambda x: x.guild
 )
 """Called whenever a guild channel is created.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 channel: abc.GuildChannel
     The guild channel that got created.
 """
 
-on_guild_channel_update: DiscordPyEvent[
+on_guild_channel_update: Event[
     [discord.abc.GuildChannel, discord.abc.GuildChannel]
-] = DiscordPyEvent("on_guild_channel_update")
+] = Event("guild_channel_update", lambda x, _: x.guild)
 """Called whenever a guild channel is updated. e.g. changed name, topic, permissions.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 before: abc.GuildChannel
     The updated guild channel's old info.
 after: abc.GuildChannel
     The updated guild channel's new info.
 """
 
-on_guild_channel_pins_update: DiscordPyEvent[
+on_guild_channel_pins_update: Event[
     [discord.abc.GuildChannel | discord.Thread, datetime.datetime]
-] = DiscordPyEvent("on_guild_channel_pins_update")
+] = Event("guild_channel_pins_update", lambda x, _: x.guild)
 """Called whenever a message is pinned or unpinned from a guild channel.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 channel: Union[abc.GuildChannel, Thread]
     The guild channel that had its pins updated.
 last_pin: Optional[datetime.datetime]
     The latest message that was pinned as an aware datetime in UTC. Could be None.
 """
 
-on_private_channel_update: DiscordPyEvent[
-    discord.GroupChannel, discord.GroupChannel
-] = DiscordPyEvent("on_private_channel_update")
+on_private_channel_update: Event[discord.GroupChannel, discord.GroupChannel] = Event(
+    "private_channel_update"
+)
 """Called whenever a private group DM is updated. e.g. changed name or topic.
 
 This requires Intents.messages to be enabled.
 
 Parameters
 ----------
 before: GroupChannel
     The updated group channel's old info.
 after: GroupChannel
     The updated group channel's new info.
 """
 
-on_private_channel_pins_update: DiscordPyEvent[
+on_private_channel_pins_update: Event[
     [discord.abc.PrivateChannel, datetime.datetime | None]
-] = DiscordPyEvent("on_private_channel_pins_update")
+] = Event("private_channel_pins_update")
 """Called whenever a message is pinned or unpinned from a private channel.
 
 Parameters
 ----------
 channel: abc.PrivateChannel
     The private channel that had its pins updated.
 last_pin: Optional[datetime.datetime]
     The latest message that was pinned as an aware datetime in UTC. Could be None.
 """
 
 
-on_raw_typing: DiscordPyEvent[discord.RawTypingEvent] = DiscordPyEvent("on_raw_typing")
+on_raw_typing: Event[discord.RawTypingEvent] = Event("raw_typing", lambda x: x.guild_id)
 """Called when someone begins typing a message. Unlike on_typing() this is called regardless of the channel and user being in the internal cache.
 
 This requires Intents.typing to be enabled.
 
 Parameters
 ----------
 payload: RawTypingEvent
     The raw event payload data.
 """
 
-on_connect: DiscordPyEvent[[]] = DiscordPyEvent("on_connect")
+on_connect: Event[[]] = Event("connect")
 """Called when the client has successfully connected to Discord. This is not the same as the client being fully prepared, see on_ready() for that.
 
 The warnings on on_ready() also apply.
 """
 
-on_disconnect: DiscordPyEvent[[]] = DiscordPyEvent("on_disconnect")
+on_disconnect: Event[[]] = Event("disconnect")
 """Called when the client has disconnected from Discord, or a connection attempt to Discord has failed.
 This could happen either through the internet being disconnected, explicit calls to close, or Discord terminating the connection one way or the other.
 
 This function can be called many times without a corresponding on_connect() call.
 """
 
-on_socket_event_type: DiscordPyEvent[str] = DiscordPyEvent("on_socket_event_type")
+on_socket_event_type: Event[str] = Event("socket_event_type")
 """Called whenever a websocket event is received from the WebSocket.
 
 This is mainly useful for logging how many events you are receiving from the Discord gateway.
 
 Parameters
 ----------
 event_type: str
     The event type from Discord that is received, e.g. 'READY'.
 """
 
-on_socket_raw_receive: DiscordPyEvent[str] = DiscordPyEvent("on_socket_raw_receive")
+on_socket_raw_receive: Event[str] = Event("socket_raw_receive")
 """Called whenever a message is completely received from the WebSocket, before it's processed and parsed.
 This event is always dispatched when a complete message is received and the passed data is not parsed in any way.
 
 This is only really useful for grabbing the WebSocket stream and debugging purposes.
 
 This requires setting the enable_debug_events setting in the Client.
 
 Parameters
 ----------
 msg: str
     The message passed in from the WebSocket library.
 """
 
-on_socket_raw_send: DiscordPyEvent[bytes | str] = DiscordPyEvent("on_socket_raw_send")
+on_socket_raw_send: Event[bytes | str] = Event("socket_raw_send")
 """Called whenever a send operation is done on the WebSocket before the message is sent. The passed parameter is the message that is being sent to the WebSocket.
 
 This is only really useful for grabbing the WebSocket stream and debugging purposes.
 
 This requires setting the enable_debug_events setting in the Client.
 
 Parameters
 ----------
 payload: Union[bytes, str]
     The message that is about to be passed on to the WebSocket library. It can be bytes to denote a binary message or str to denote a regular text message.
 """
 
-on_ready: DiscordPyEvent[[]] = DiscordPyEvent("on_ready")
+on_ready: Event[[]] = Event("ready")
 """Called when the client is done preparing the data received from Discord. Usually after login is successful and the Client.guilds and co. are filled up.
 
 WARNING
 -------
 This function is not guaranteed to be the first event called. Likewise, this function is not guaranteed to only be called once.
 This library implements reconnection logic and thus will end up calling this event whenever a RESUME request fails.
 """
 
-on_setup_hook: DiscordPyEvent[[]] = DiscordPyEvent("on_setup_hook")
+on_setup_hook: Event[[]] = Event("setup_hook")
 """
 Called after the bot is logged in but before it has connected to the Websocket. Can be used to perform asynchronous setup.
 
 This is only called once, in login(), and will be called before any events are dispatched, making it a better solution than doing such setup in the on_ready() event.
 
 WARNING
 -------
 Since this is called before the websocket connection is made therefore anything that waits for the websocket will deadlock,
 this includes things like wait_for() and wait_until_ready().
 """
 
-on_resumed: DiscordPyEvent[[]] = DiscordPyEvent("on_resumed")
+on_resumed: Event[[]] = Event("resumed")
 """Called when the client has resumed a session."""
 
-on_guild_available: DiscordPyEvent[discord.Guild] = DiscordPyEvent("on_guild_available")
+on_guild_available: Event[discord.Guild] = Event("guild_available", lambda x: x)
 """Called when a guild becomes available. The guild must have existed in the Client.guilds cache.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 guild: Guild
     The Guild that has changed availability.
 """
 
-on_guild_join: DiscordPyEvent[discord.Guild] = DiscordPyEvent("on_guild_join")
+on_guild_join: Event[discord.Guild] = Event("guild_join", lambda x: x)
 """Called when a Guild is either created by the Client or when the Client joins a guild.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 guild: Guild
     The guild that was joined.
 """
 
-on_guild_remove: DiscordPyEvent[discord.Guild] = DiscordPyEvent("on_guild_remove")
+on_guild_remove: Event[discord.Guild] = Event("guild_remove", lambda x: x)
 """Called when a Guild is removed from the Client.
 
 This happens through, but not limited to, these circumstances:
 - The client got banned.
 - The client got kicked.
 - The client left the guild.
 - The client or the guild owner deleted the guild.
@@ -373,16 +372,16 @@
 
 Parameters
 ----------
 guild: Guild
     The guild that got removed.
 """
 
-on_guild_update: DiscordPyEvent[discord.Guild, discord.Guild] = DiscordPyEvent(
-    "on_guild_update"
+on_guild_update: Event[discord.Guild, discord.Guild] = Event(
+    "on_guild_update", lambda x, _: x
 )
 """Called when a Guild updates, for example:
 - Changed name
 - Changed AFK channel
 - Changed AFK timeout
 - etc
 
@@ -392,50 +391,50 @@
 ----------
 before: Guild
     The guild prior to being updated.
 after: Guild
     The guild after being updated.
 """
 
-on_guild_emojis_update: DiscordPyEvent[
+on_guild_emojis_update: Event[
     discord.Guild, Sequence[discord.Emoji], Sequence[discord.Emoji]
-] = DiscordPyEvent("on_guild_emojis_update")
+] = Event("guild_emojis_update", lambda *s: next(x for xs in s for x in xs).guild)
 """Called when a Guild adds or removes Emoji.
 
 This requires Intents.emojis_and_stickers to be enabled.
 
 Parameters
 ----------
 guild: Guild
     The guild that got their emojis updated.
 before: Sequence[Emoji]
     A list of emojis before the update.
 after: Sequence[Emoji]
     A list of emojis after the update.
 """
 
-on_guild_stickers_update: DiscordPyEvent[
+on_guild_stickers_update: Event[
     [discord.Guild, Sequence[discord.GuildSticker], Sequence[discord.GuildSticker]]
-] = DiscordPyEvent("on_guild_stickers_update")
+] = Event("guild_stickers_update", lambda *s: next(x for xs in s for x in xs).guild)
 """Called when a Guild updates its stickers.
 
 This requires Intents.emojis_and_stickers to be enabled.
 
 Parameters
 ----------
 guild: Guild
     The guild that got their stickers updated.
 before: Sequence[GuildSticker]
     A list of stickers before the update.
 after: Sequence[GuildSticker]
     A list of stickers after the update.
 """
 
-on_audit_log_entry_create: DiscordPyEvent[discord.AuditLogEntry] = DiscordPyEvent(
-    "on_audit_log_entry_create"
+on_audit_log_entry_create: Event[discord.AuditLogEntry] = Event(
+    "on_audit_log_entry_create", lambda x: x.guild
 )
 """Called when a Guild gets a new audit log entry. You must have view_audit_log to receive this.
 
 This requires Intents.moderation to be enabled.
 
 WARNING
 -------
@@ -447,107 +446,107 @@
 
 Parameters
 ----------
 entry: AuditLogEntry
     The audit log entry that was created.
 """
 
-on_invite_create: DiscordPyEvent[discord.Invite] = DiscordPyEvent("on_invite_create")
+on_invite_create: Event[discord.Invite] = Event("invite_create", lambda x: x.guild)
 """Called when an Invite is created. You must have manage_channels to receive this.
 
 There is a rare possibility that the Invite.guild and Invite.channel attributes will be of Object rather than the respective models.
 
 This requires Intents.invites to be enabled.
 
 Parameters
 ----------
 invite: Invite
     The invite that was created.
 """
 
-on_invite_delete: DiscordPyEvent[discord.Invite] = DiscordPyEvent("on_invite_delete")
+on_invite_delete: Event[discord.Invite] = Event("invite_delete", lambda x: x.guild)
 """Called when an Invite is deleted. You must have manage_channels to receive this.
 
 There is a rare possibility that the Invite.guild and Invite.channel attributes will be of Object rather than the respective models.
 Outside of those two attributes, the only other attribute guaranteed to be filled by the Discord gateway for this event is Invite.code.
 
 This requires Intents.invites to be enabled.
 
 Parameters
 ----------
 invite: Invite
     The invite that was deleted.
 """
 
-on_integration_create: DiscordPyEvent[discord.Integration] = DiscordPyEvent(
-    "on_integration_create"
+on_integration_create: Event[discord.Integration] = Event(
+    "on_integration_create", lambda x: x.guild
 )
 """Called when an integration is created.
 
 This requires Intents.integrations to be enabled.
 
 Parameters
 ----------
 integration: Integration
     The integration that was created.
 """
 
-on_integration_update: DiscordPyEvent[discord.Integration] = DiscordPyEvent(
-    "on_integration_update"
+on_integration_update: Event[discord.Integration] = Event(
+    "on_integration_update", lambda x: x.guild
 )
 """Called when an integration is updated.
 
 This requires Intents.integrations to be enabled.
 
 Parameters
 ----------
 integration: Integration
     The integration that was updated.
 """
 
-on_guild_integrations_update: DiscordPyEvent[discord.Guild] = DiscordPyEvent(
-    "on_guild_integrations_update"
+on_guild_integrations_update: Event[discord.Guild] = Event(
+    "on_guild_integrations_update", lambda x: x
 )
 """Called whenever an integration is created, modified, or removed from a guild.
 
 This requires Intents.integrations to be enabled.
 
 Parameters
 ----------
 guild: Guild
     The guild that had its integrations updated.
 """
 
-on_webhooks_update: DiscordPyEvent[discord.abc.GuildChannel] = DiscordPyEvent(
-    "on_webhooks_update"
+on_webhooks_update: Event[discord.abc.GuildChannel] = Event(
+    "on_webhooks_update", lambda x: x.guild
 )
 """Called whenever a webhook is created, modified, or removed from a guild channel.
 
 This requires Intents.webhooks to be enabled.
 
 Parameters
 ----------
 channel: abc.GuildChannel
     The channel that had its webhooks updated.
 """
 
-on_raw_integration_delete: DiscordPyEvent[
-    discord.RawIntegrationDeleteEvent
-] = DiscordPyEvent("on_raw_integration_delete")
+on_raw_integration_delete: Event[discord.RawIntegrationDeleteEvent] = Event(
+    "on_raw_integration_delete", lambda x: x.guild_id
+)
 """Called when an integration is deleted.
 
 This requires Intents.integrations to be enabled.
 
 Parameters
 ----------
 payload: RawIntegrationDeleteEvent
     The raw event payload data.
 """
 
-on_interaction: DiscordPyEvent[discord.Interaction] = DiscordPyEvent("on_interaction")
+on_interaction: Event[discord.Interaction] = Event("interaction", lambda x: x.guild)
 """Called when an interaction happened.
 
 This currently happens due to slash command invocations or components being used.
 
 WARNING
 -------
 This is a low-level function that is not generally meant to be used.
@@ -555,55 +554,55 @@
 
 Parameters
 ----------
 interaction: Interaction
     The interaction data.
 """
 
-on_member_join: DiscordPyEvent[discord.Member] = DiscordPyEvent("on_member_join")
+on_member_join: Event[discord.Member] = Event("member_join", lambda x: x.guild)
 """Called when a Member joins a Guild.
 
 This requires Intents.members to be enabled.
 
 Parameters
 ----------
 member: Member
     The member who joined.
 """
 
-on_member_remove: DiscordPyEvent[discord.Member] = DiscordPyEvent("on_member_remove")
+on_member_remove: Event[discord.Member] = Event("member_remove", lambda x: x.guild)
 """Called when a Member leaves a Guild.
 
 If the guild or member could not be found in the internal cache, this event will not be called. You may use on_raw_member_remove() instead.
 
 This requires Intents.members to be enabled.
 
 Parameters
 ----------
 member: Member
     The member who left.
 """
 
-on_raw_member_remove: DiscordPyEvent[discord.RawMemberRemoveEvent] = DiscordPyEvent(
-    "on_raw_member_remove"
+on_raw_member_remove: Event[discord.RawMemberRemoveEvent] = Event(
+    "on_raw_member_remove", lambda x: x.guild_id
 )
 """Called when a Member leaves a Guild.
 
 Unlike on_member_remove(), this is called regardless of the guild or member being in the internal cache.
 
 This requires Intents.members to be enabled.
 
 Parameters
 ----------
 payload: RawMemberRemoveEvent
     The raw event payload data.
 """
 
-on_member_update: DiscordPyEvent[discord.Member, discord.Member] = DiscordPyEvent(
-    "on_member_update"
+on_member_update: Event[discord.Member, discord.Member] = Event(
+    "on_member_update", lambda x, _: x.guild
 )
 """Called when a Member updates their profile.
 
 This is called when one or more of the following things change:
 
 - nickname
 - roles
@@ -620,17 +619,15 @@
 ----------
 before: Member
     The updated member's old info.
 after: Member
     The updated member's updated info.
 """
 
-on_user_update: DiscordPyEvent[discord.User, discord.User] = DiscordPyEvent(
-    "on_user_update"
-)
+on_user_update: Event[discord.User, discord.User] = Event("user_update")
 """Called when a User updates their profile.
 
 This is called when one or more of the following things change:
 
 - avatar
 - username
 - discriminator
@@ -641,46 +638,44 @@
 ----------
 before: User
     The updated user's old info.
 after: User
     The updated user's updated info.
 """
 
-on_member_ban: DiscordPyEvent[
-    discord.Guild, discord.User | discord.Member
-] = DiscordPyEvent("on_member_ban")
+on_member_ban: Event[discord.Guild, discord.User | discord.Member] = Event(
+    "on_member_ban", lambda x, _: x
+)
 """Called when a user gets banned from a Guild.
 
 This requires Intents.moderation to be enabled.
 
 Parameters
 ----------
 guild: Guild
     The guild the user got banned from.
 user: User | Member
     The user that got banned. Can be either User or Member depending on whether the user was in the guild or not at the time of removal.
 """
 
-on_member_unban: DiscordPyEvent[discord.Guild, discord.User] = DiscordPyEvent(
-    "on_member_unban"
-)
+on_member_unban: Event[discord.Guild, discord.User] = Event("member_unban", lambda x, _: x)
 """Called when a User gets unbanned from a Guild.
 
 This requires Intents.moderation to be enabled.
 
 Parameters
 ----------
 guild: Guild
     The guild the user got unbanned from.
 user: User
     The user that got unbanned.
 """
 
-on_presence_update: DiscordPyEvent[discord.Member, discord.Member] = DiscordPyEvent(
-    "on_presence_update"
+on_presence_update: Event[discord.Member, discord.Member] = Event(
+    "on_presence_update", lambda x, _: x.guild
 )
 """Called when a Member updates their presence.
 
 This is called when one or more of the following things change:
 - status
 - activity
 
@@ -690,15 +685,15 @@
 ----------
 before: Member
     The updated member's old info.
 after: Member
     The updated member's updated info.
 """
 
-on_message: DiscordPyEvent[discord.Message] = DiscordPyEvent("on_message")
+on_message: Event[discord.Message] = Event("message", lambda x: x.guild)
 """Called when a Message is created and sent.
 
 This requires Intents.messages to be enabled.
 
 WARNING
 -------
 Your bot's own messages and private messages are sent through this event.
@@ -707,16 +702,16 @@
 
 Parameters
 ----------
 message: Message
     The current message.
 """
 
-on_message_edit: DiscordPyEvent[discord.Message, discord.Message] = DiscordPyEvent(
-    "on_message_edit"
+on_message_edit: Event[discord.Message, discord.Message] = Event(
+    "on_message_edit", lambda x, _: x.guild
 )
 """Called when a Message receives an update event.
 If the message is not found in the internal message cache, then these events will not be called.
 Messages might not be in the cache if the message is too old or the client is participating in high traffic guilds.
 
 If this occurs, increase the max_messages parameter or use the on_raw_message_edit() event instead.
 
@@ -733,30 +728,30 @@
 ----------
 before: Message
     The previous version of the message.
 after: Message
     The current version of the message.
 """
 
-on_message_delete: DiscordPyEvent[discord.Message] = DiscordPyEvent("on_message_delete")
+on_message_delete: Event[discord.Message] = Event("message_delete", lambda x: x.guild)
 """Called when a message is deleted. If the message is not found in the internal message cache, then this event will not be called.
 Messages might not be in the cache if the message is too old or the client is participating in high traffic guilds.
 
 If this occurs, increase the max_messages parameter or use the on_raw_message_delete() event instead.
 
 This requires Intents.messages to be enabled.
 
 Parameters
 ----------
 message: Message
     The deleted message.
 """
 
-on_bulk_message_delete: DiscordPyEvent[List[discord.Message]] = DiscordPyEvent(
-    "on_bulk_message_delete"
+on_bulk_message_delete: Event[List[discord.Message]] = Event(
+    "on_bulk_message_delete", lambda x: x[0].guild
 )
 """Called when messages are bulk deleted.
 If none of the messages deleted are found in the internal message cache, then this event will not be called.
 If individual messages were not found in the internal message cache, this event will still be called, but the messages not found will not be included in the messages list.
 Messages might not be in the cache if the message is too old or the client is participating in high traffic guilds.
 
 If this occurs, increase the max_messages parameter or use the on_raw_bulk_message_delete() event instead.
@@ -765,16 +760,16 @@
 
 Parameters
 ----------
 messages: List[Message]
     The messages that have been deleted.
 """
 
-on_raw_message_edit: DiscordPyEvent[discord.RawMessageUpdateEvent] = DiscordPyEvent(
-    "on_raw_message_edit"
+on_raw_message_edit: Event[discord.RawMessageUpdateEvent] = Event(
+    "on_raw_message_edit", lambda x: x.guild_id
 )
 """Called when a message is edited. Unlike on_message_edit(), this is called regardless of the state of the internal message cache.
 
 If the message is found in the message cache, it can be accessed via RawMessageUpdateEvent.cached_message.
 The cached message represents the message before it has been edited.
 For example, if the content of a message is modified and triggers the on_raw_message_edit() coroutine,
 the RawMessageUpdateEvent.cached_message will return a Message object that represents the message before the content was modified.
@@ -789,47 +784,47 @@
 
 Parameters
 ----------
 payload: RawMessageUpdateEvent
     The raw event payload data.
 """
 
-on_raw_message_delete: DiscordPyEvent[discord.RawMessageDeleteEvent] = DiscordPyEvent(
-    "on_raw_message_delete"
+on_raw_message_delete: Event[discord.RawMessageDeleteEvent] = Event(
+    "on_raw_message_delete", lambda x: x.guild_id
 )
 """Called when a message is deleted. Unlike on_message_delete(), this is called regardless of the message being in the internal message cache or not.
 
 If the message is found in the message cache, it can be accessed via RawMessageDeleteEvent.cached_message.
 
 This requires Intents.messages to be enabled.
 
 Parameters
 ----------
 payload: RawMessageDeleteEvent
     The raw event payload data.
 """
 
-on_raw_bulk_message_delete: DiscordPyEvent[
-    discord.RawBulkMessageDeleteEvent
-] = DiscordPyEvent("on_raw_bulk_message_delete")
+on_raw_bulk_message_delete: Event[discord.RawBulkMessageDeleteEvent] = Event(
+    "on_raw_bulk_message_delete", lambda x: x.guild_id
+)
 """Called when a bulk delete is triggered. Unlike on_bulk_message_delete(), this is called regardless of the messages being in the internal message cache or not.
 
 If the messages are found in the message cache, they can be accessed via RawBulkMessageDeleteEvent.cached_messages.
 
 This requires Intents.messages to be enabled.
 
 Parameters
 ----------
 payload: RawBulkMessageDeleteEvent
     The raw event payload data.
 """
 
-on_reaction_add: DiscordPyEvent[
-    discord.Reaction, discord.Member | discord.User
-] = DiscordPyEvent("on_reaction_add")
+on_reaction_add: Event[discord.Reaction, discord.Member | discord.User] = Event(
+    "reaction_add", lambda x, _: x.message.guild
+)
 """Called when a message has a reaction added to it. Similar to on_message_edit(), if the message is not found in the internal message cache,
 then this event will not be called. Consider using on_raw_reaction_add() instead.
 
 To get the Message being reacted, access it via Reaction.message.
 
 This requires Intents.reactions to be enabled.
 
@@ -840,17 +835,17 @@
 ----------
 reaction: Reaction
     The current state of the reaction.
 user: Member | User
     The user who added the reaction.
 """
 
-on_reaction_remove: DiscordPyEvent[
-    discord.Reaction, discord.Member | discord.User
-] = DiscordPyEvent("on_reaction_remove")
+on_reaction_remove: Event[discord.Reaction, discord.Member | discord.User] = Event(
+    "reaction_remove", lambda x, _: x.message.guild
+)
 """Called when a message has a reaction removed from it. Similar to on_message_edit,
 if the message is not found in the internal message cache, then this event will not be called.
 
 To get the message being reacted, access it via Reaction.message.
 
 This requires both Intents.reactions and Intents.members to be enabled.
 
@@ -860,168 +855,168 @@
 ----------
 reaction: Reaction
     The current state of the reaction.
 user: Member | User
     The user whose reaction was removed.
 """
 
-on_reaction_clear: DiscordPyEvent[discord.Message, List[discord.Reaction]] = DiscordPyEvent(
-    "on_reaction_clear"
+on_reaction_clear: Event[discord.Message, List[discord.Reaction]] = Event(
+    "on_reaction_clear", lambda x, _: x.guild
 )
 """Called when a message has all its reactions removed from it.
 Similar to on_message_edit(), if the message is not found in the internal message cache,then this event will not be called. Consider using on_raw_reaction_clear() instead.
 
 This requires Intents.reactions to be enabled.
 
 Parameters
 ----------
 message: Message
     The message that had its reactions cleared.
 reactions: List[Reaction]
     The reactions that were removed.
 """
 
-on_reaction_clear_emoji: DiscordPyEvent[discord.Reaction] = DiscordPyEvent(
-    "on_reaction_clear_emoji"
+on_reaction_clear_emoji: Event[discord.Reaction] = Event(
+    "on_reaction_clear_emoji", lambda x: x.message.guild
 )
 """Called when a message has a specific reaction removed from it.
 Similar to on_message_edit(), if the message is not found in the internal message cache,then this event will not be called. Consider using on_raw_reaction_clear_emoji() instead.
 
 This requires Intents.reactions to be enabled.
 
 New in version 1.3.
 
 Parameters
 ----------
 reaction: Reaction
     The reaction that got cleared.
 """
 
-on_raw_reaction_add: DiscordPyEvent[discord.RawReactionActionEvent] = DiscordPyEvent(
-    "on_raw_reaction_add"
+on_raw_reaction_add: Event[discord.RawReactionActionEvent] = Event(
+    "on_raw_reaction_add", lambda x: x.guild_id
 )
 """Called when a message has a reaction added. Unlike on_reaction_add(), this is called regardless of the state of the internal message cache.
 
 This requires Intents.reactions to be enabled.
 
 Parameters
 ----------
 payload: RawReactionActionEvent
     The raw event payload data.
 """
 
-on_raw_reaction_remove: DiscordPyEvent[discord.RawReactionActionEvent] = DiscordPyEvent(
-    "on_raw_reaction_remove"
+on_raw_reaction_remove: Event[discord.RawReactionActionEvent] = Event(
+    "on_raw_reaction_remove", lambda x: x.guild_id
 )
 """Called when a message has a reaction removed. Unlike on_reaction_remove(), this is called regardless of the state of the internal message cache.
 
 This requires Intents.reactions to be enabled.
 
 Parameters
 ----------
 payload: RawReactionActionEvent
     The raw event payload data.
 """
 
-on_raw_reaction_clear: DiscordPyEvent[discord.RawReactionClearEvent] = DiscordPyEvent(
-    "on_raw_reaction_clear"
+on_raw_reaction_clear: Event[discord.RawReactionClearEvent] = Event(
+    "on_raw_reaction_clear", lambda x: x.guild_id
 )
 """Called when a message has all its reactions removed. Unlike on_reaction_clear(), this is called regardless of the state of the internal message cache.
 
 This requires Intents.reactions to be enabled.
 
 Parameters
 ----------
 payload: RawReactionClearEvent
     The raw event payload data.
 """
 
-on_raw_reaction_clear_emoji: DiscordPyEvent[
-    discord.RawReactionClearEmojiEvent
-] = DiscordPyEvent("on_raw_reaction_clear_emoji")
+on_raw_reaction_clear_emoji: Event[discord.RawReactionClearEmojiEvent] = Event(
+    "raw_reaction_clear_emoji", lambda x: x.guild_id
+)
 """Called when a message has a specific reaction removed from it. Unlike on_reaction_clear_emoji(), this is called regardless of the state of the internal message cache.
 
 This requires Intents.reactions to be enabled.
 
 Parameters
 ----------
 payload: RawReactionClearEmojiEvent
     The raw event payload data.
 """
 
-on_guild_role_create: DiscordPyEvent[discord.Role] = DiscordPyEvent("on_guild_role_create")
+on_guild_role_create: Event[discord.Role] = Event("guild_role_create", lambda x: x.guild)
 """Called when a Guild creates a new Role.
 
 To get the guild it belongs to, use Role.guild.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 role: Role
     The role that was created.
 """
 
-on_guild_role_delete: DiscordPyEvent[discord.Role] = DiscordPyEvent("on_guild_role_delete")
+on_guild_role_delete: Event[discord.Role] = Event("guild_role_delete", lambda x: x.guild)
 """Called when a Guild deletes a Role.
 
 To get the guild it belongs to, use Role.guild.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 role: Role
     The role that was deleted.
 """
 
-on_guild_role_update: DiscordPyEvent[discord.Role, discord.Role] = DiscordPyEvent(
-    "on_guild_role_update"
+on_guild_role_update: Event[discord.Role, discord.Role] = Event(
+    "on_guild_role_update", lambda x, _: x.guild
 )
 """Called when a Role is changed guild-wide.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 before: Role
     The updated role's old info.
 after: Role
     The updated role's updated info.
 """
 
-on_scheduled_event_create: DiscordPyEvent[discord.ScheduledEvent] = DiscordPyEvent(
-    "on_scheduled_event_create"
+on_scheduled_event_create: Event[discord.ScheduledEvent] = Event(
+    "on_scheduled_event_create", lambda x: x.guild
 )
 """Called when a ScheduledEvent is created.
 
 This requires Intents.guild_scheduled_events to be enabled.
 
 Parameters
 ----------
 event: ScheduledEvent
     The scheduled event that was created.
 """
 
-on_scheduled_event_delete: DiscordPyEvent[discord.ScheduledEvent] = DiscordPyEvent(
-    "on_scheduled_event_delete"
+on_scheduled_event_delete: Event[discord.ScheduledEvent] = Event(
+    "on_scheduled_event_delete", lambda x: x.guild
 )
 """Called when a ScheduledEvent is deleted.
 
 This requires Intents.guild_scheduled_events to be enabled.
 
 Parameters
 ----------
 event: ScheduledEvent
     The scheduled event that was deleted.
 """
 
-on_scheduled_event_update: DiscordPyEvent[
-    discord.ScheduledEvent, discord.ScheduledEvent
-] = DiscordPyEvent("on_scheduled_event_update")
+on_scheduled_event_update: Event[discord.ScheduledEvent, discord.ScheduledEvent] = Event(
+    "scheduled_event_update", lambda x, _: x.guild
+)
 """Called when a ScheduledEvent is updated.
 
 This requires Intents.guild_scheduled_events to be enabled.
 
 The following, but not limited to, examples illustrate when this event is called:
 - The scheduled start/end times are changed.
 - The channel is changed.
@@ -1033,111 +1028,111 @@
 ----------
 before: ScheduledEvent
     The scheduled event before the update.
 after: ScheduledEvent
     The scheduled event after the update.
 """
 
-on_scheduled_event_user_add: DiscordPyEvent[
-    discord.ScheduledEvent, discord.User
-] = DiscordPyEvent("on_scheduled_event_user_add")
+on_scheduled_event_user_add: Event[discord.ScheduledEvent, discord.User] = Event(
+    "scheduled_event_user_add", lambda x, _: x.guild
+)
 """Called when a user is added to a ScheduledEvent.
 
 This requires Intents.guild_scheduled_events to be enabled.
 
 Parameters
 ----------
 event: ScheduledEvent
     The scheduled event that the user was added to.
 user: User
     The user that was added.
 """
 
-on_scheduled_event_user_remove: DiscordPyEvent[
-    discord.ScheduledEvent, discord.User
-] = DiscordPyEvent("on_scheduled_event_user_remove")
+on_scheduled_event_user_remove: Event[discord.ScheduledEvent, discord.User] = Event(
+    "scheduled_event_user_remove", lambda x, _: x.guild
+)
 """Called when a user is removed from a ScheduledEvent.
 
 This requires Intents.guild_scheduled_events to be enabled.
 
 Parameters
 ----------
 event: ScheduledEvent
     The scheduled event that the user was removed from.
 user: User
     The user that was removed.
 """
 
-on_stage_instance_create: DiscordPyEvent[discord.StageInstance] = DiscordPyEvent(
-    "on_stage_instance_create"
+on_stage_instance_create: Event[discord.StageInstance] = Event(
+    "on_stage_instance_create", lambda x: x.guild
 )
 """Called when a StageInstance is created for a StageChannel.
 
 Parameters
 ----------
 stage_instance: StageInstance
     The stage instance that was created.
 """
 
-on_stage_instance_delete: DiscordPyEvent[discord.StageInstance] = DiscordPyEvent(
-    "on_stage_instance_delete"
+on_stage_instance_delete: Event[discord.StageInstance] = Event(
+    "on_stage_instance_delete", lambda x: x.guild
 )
 """Called when a StageInstance is deleted for a StageChannel.
 
 Parameters
 ----------
 stage_instance: StageInstance
     The stage instance that was deleted.
 """
 
-on_stage_instance_update: DiscordPyEvent[
-    discord.StageInstance, discord.StageInstance
-] = DiscordPyEvent("on_stage_instance_update")
+on_stage_instance_update: Event[discord.StageInstance, discord.StageInstance] = Event(
+    "stage_instance_update", lambda x, _: x.guild
+)
 """Called when a StageInstance is updated.
 
 The following, but not limited to, examples illustrate when this event is called:
 - The topic is changed.
 - The privacy level is changed.
 
 Parameters
 ----------
 before: StageInstance
     The stage instance before the update.
 after: StageInstance
     The stage instance after the update.
 """
 
-on_thread_create: DiscordPyEvent[discord.Thread] = DiscordPyEvent("on_thread_create")
+on_thread_create: Event[discord.Thread] = Event("thread_create", lambda x: x.guild)
 """Called whenever a thread is created.
 
 Note that you can get the guild from Thread.guild.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 thread: Thread
     The thread that was created.
 """
 
-on_thread_join: DiscordPyEvent[discord.Thread] = DiscordPyEvent("on_thread_join")
+on_thread_join: Event[discord.Thread] = Event("thread_join", lambda x: x.guild)
 """Called whenever a thread is joined.
 
 Note that you can get the guild from Thread.guild.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 thread: Thread
     The thread that was joined.
 """
 
-on_thread_update: DiscordPyEvent[discord.Thread, discord.Thread] = DiscordPyEvent(
-    "on_thread_update"
+on_thread_update: Event[discord.Thread, discord.Thread] = Event(
+    "on_thread_update", lambda x, _: x.guild
 )
 """Called whenever a thread is updated.
 
 If the thread could not be found in the internal cache, this event will not be called.
 Threads will not be in the cache if they are archived.
 If you need this information, use on_raw_thread_update() instead.
 
@@ -1147,15 +1142,15 @@
 ----------
 before: Thread
     The updated thread's old info.
 after: Thread
     The updated thread's new info.
 """
 
-on_thread_remove: DiscordPyEvent[discord.Thread] = DiscordPyEvent("on_thread_remove")
+on_thread_remove: Event[discord.Thread] = Event("thread_remove", lambda x: x.guild)
 """Called whenever a thread is removed. This is different from a thread being deleted.
 
 Note that you can get the guild from Thread.guild.
 
 This requires Intents.guilds to be enabled.
 
 Due to technical limitations, this event might not be called as soon as one expects.
@@ -1163,101 +1158,101 @@
 
 Parameters
 ----------
 thread: Thread
     The thread that was removed.
 """
 
-on_thread_delete: DiscordPyEvent[discord.Thread] = DiscordPyEvent("on_thread_delete")
+on_thread_delete: Event[discord.Thread] = Event("thread_delete", lambda x: x.guild)
 """Called whenever a thread is deleted. If the thread could not be found in the internal cache, this event will not be called.
 Threads will not be in the cache if they are archived.
 If you need this information, use on_raw_thread_delete() instead.
 
 Note that you can get the guild from Thread.guild.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 thread: Thread
     The thread that was deleted.
 """
 
-on_raw_thread_update: DiscordPyEvent[discord.RawThreadUpdateEvent] = DiscordPyEvent(
-    "on_raw_thread_update"
+on_raw_thread_update: Event[discord.RawThreadUpdateEvent] = Event(
+    "on_raw_thread_update", lambda x: x.guild_id
 )
 """Called whenever a thread is updated. Unlike on_thread_update(), this is called regardless of the thread being in the internal thread cache or not.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 payload: RawThreadUpdateEvent
     The raw event payload data.
 """
 
-on_raw_thread_delete: DiscordPyEvent[discord.RawThreadDeleteEvent] = DiscordPyEvent(
-    "on_raw_thread_delete"
+on_raw_thread_delete: Event[discord.RawThreadDeleteEvent] = Event(
+    "on_raw_thread_delete", lambda x: x.guild_id
 )
 """Called whenever a thread is deleted. Unlike on_thread_delete(), this is called regardless of the thread being in the internal thread cache or not.
 
 This requires Intents.guilds to be enabled.
 
 Parameters
 ----------
 payload: RawThreadDeleteEvent
     The raw event payload data.
 """
 
-on_thread_member_join: DiscordPyEvent[discord.ThreadMember] = DiscordPyEvent(
-    "on_thread_member_join"
+on_thread_member_join: Event[discord.ThreadMember] = Event(
+    "on_thread_member_join", lambda x: x.thread.guild
 )
 """Called when a ThreadMember joins a Thread.
 
 You can get the thread a member belongs to by accessing ThreadMember.thread.
 
 This requires Intents.members to be enabled.
 
 Parameters
 ----------
 member: ThreadMember
     The member who joined.
 """
 
-on_thread_member_remove: DiscordPyEvent[discord.ThreadMember] = DiscordPyEvent(
-    "on_thread_member_remove"
+on_thread_member_remove: Event[discord.ThreadMember] = Event(
+    "on_thread_member_remove", lambda x: x.thread.guild
 )
 """Called when a ThreadMember leaves a Thread.
 
 You can get the thread a member belongs to by accessing ThreadMember.thread.
 
 This requires Intents.members to be enabled.
 
 Parameters
 ----------
 member: ThreadMember
     The member who left.
 """
 
-on_raw_thread_member_remove: DiscordPyEvent[
-    discord.RawThreadMembersUpdate
-] = DiscordPyEvent("on_raw_thread_member_remove")
+on_raw_thread_member_remove: Event[discord.RawThreadMembersUpdate] = Event(
+    "on_raw_thread_member_remove", lambda x: x.guild_id
+)
 """Called when a ThreadMember leaves a Thread. Unlike on_thread_member_remove(), this is called regardless of the member being in the internal thread's members cache or not.
 
 This requires Intents.members to be enabled.
 
 Parameters
 ----------
 payload: RawThreadMembersUpdate
     The raw event payload data.
 """
 
-on_voice_state_update: DiscordPyEvent[
+on_voice_state_update: Event[
     discord.Member, discord.VoiceState, discord.VoiceState
-] = DiscordPyEvent("on_voice_state_update")
+] = Event("voice_state_update", lambda x, *_: x.guild)
 """Called when a Member changes their VoiceState.
 
 The following, but not limited to, examples illustrate when this event is called:
 
 - A member joins a voice or stage channel.
 - A member leaves a voice or stage channel.
 - A member is muted or deafened by their own accord.
```

### Comparing `discord_amethyst-1.0.1/PKG-INFO` & `discord_amethyst-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: discord-amethyst
-Version: 1.0.1
+Version: 2.0.0
 Summary: An opinionated extension for discord.py.
+Home-page: https://github.com/NimajnebEC/discord-amethyst
 License: MIT
 Author: NimajnebEC
 Author-email: nimajnebec@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: croniter (>=1.4.1,<2.0.0)
-Requires-Dist: discord-py (>=2.3.1,<3.0.0)
-Requires-Dist: dynamicpy (>=1.1.0,<2.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: discord-py (>=2.3.2,<3.0.0)
+Requires-Dist: dynamicpy (>=1.2.2,<2.0.0)
+Requires-Dist: environ-import (>=0.1.0,<0.2.0)
+Requires-Dist: lavender-logging (>=1.0.0,<2.0.0)
+Project-URL: Repository, https://github.com/NimajnebEC/discord-amethyst
 Description-Content-Type: text/markdown
 
 # Discord Amethyst
 
-An opinionated extension for [discord.py](https://github.com/Rapptz/discord.py). Amethyst adds a handful of features that I found myself re-implementing or wanting for many of my Discord bots such as automatic app command synchronisation and job scheduling.
+An opinionated extension for [discord.py](https://github.com/Rapptz/discord.py), inspired by [JellyCommands](https://jellycommands.dev/). Amethyst adds a handful of features that I found myself re-implementing or wanting for many of my Discord bots such as automatic app command synchronisation and job scheduling.
 
 ## Widgets
 
-### Command
+### Command & Context Menus
 
-The amethyst command decorator is just a wrapper around discord.py's `app_commands.command` decorator. Please refer to the [discord.py documentation](https://discordpy.readthedocs.io/en/stable/interactions/api.html?highlight=app_commands%20command#discord.app_commands.command) for usage.
+The amethyst `command` and `context_menu` decorators are just a wrappers around discord.py's decorators. Please refer to the [discord.py documentation](https://discordpy.readthedocs.io/en/stable/interactions/api.html?highlight=app_commands%20command#discord.app_commands.command) for usage.
 
 ### Event
 
-Amethyst's event decorator is a type hinted wrapper around [discord.py's normal event decorator](https://discordpy.readthedocs.io/en/stable/api.html?highlight=client%20event#discord.Client.event). The primary difference is that you must specify which event you wish to subscribe to. The property `amethyst.events` is a module containing all of the [default discord.py events](https://discordpy.readthedocs.io/en/stable/api.html?highlight=client%20event#event-reference).
+Amethyst's event decorator is a type hinted wrapper around [discord.py's normal event decorator](https://discordpy.readthedocs.io/en/stable/api.html?highlight=client%20event#discord.Client.event). The primary difference is that you must specify which event you wish to subscribe to. The amethyst module exports all of the [default discord.py events](https://discordpy.readthedocs.io/en/stable/api.html?highlight=client%20event#event-reference) with the prefix `on_`.
 
 ```py
 import amethyst
 
-@amethyst.event(amethyst.events.on_ready)
+@amethyst.event(amethyst.on_ready)
 async def on_ready():
     print("Bot is ready!")
 ```
 
 ### Schedule
 
 Amethyst implements a [cron-like](https://en.wikipedia.org/wiki/Cron) asynchronous scheduler for calling functions on a set schedule, powered by [croniter](https://github.com/kiorky/croniter).
@@ -49,29 +53,29 @@
 @amethyst.schedule("0 8 * * *")
 async def every_morning():
     print("Good morning!")
 ```
 
 ## Dynamic Module Import
 
-Amethyst can dynamically load python modules, powered by [dynamicpy](https://github.com/NimajnebEC/dynamicpy#dynamicloader). When run, the client will automatically import and register any widgets found in the `.command`, `.commands`, `.plugin` and `.plugins` submodules. The submodules which are searched can be configured in the `AmethystClient`'s constructor.
+Amethyst can dynamically load python modules, powered by [dynamicpy](https://github.com/NimajnebEC/dynamicpy#dynamicloader). When run, the client will automatically import and register any widgets found in the `.command`, `.commands`, `.plugin` and `.plugins` submodules. The submodules which are searched can be configured in the `amethyst.Client` constructor.
 
 Lets say you have the following project structure:
 
 ```
 my-bot/
 ├── __init__.py
 ├── main.py
 └── commands/
     ├── __init__.py
     ├── foo.py
     └── bar.py
 ```
 
-If your instance of `AmethystClient` is instantiated in `main.py` then the `commands/` package will be recursively searched for widgets to register.
+If your instance of `amethyst.Client` is instantiated in `main.py` then the `commands/` package will be recursively searched for widgets to register.
 
 The searched modules can also be top-level, the only requirement is that they are at the same level as the module inside which the client was instantiated.
 
 ```
 my-bot.py
 plugins.py
 commands/
@@ -80,58 +84,56 @@
 └── bar.py
 ```
 
 In this example, the `commands.py` module and the `commands/` package will be searched.
 
 ## Plugin System
 
-Amethyst has a plugin system, powered by [dynamicpy](https://github.com/NimajnebEC/dynamicpy) and inspired by [discord.py Cogs](https://discordpy.readthedocs.io/en/stable/ext/commands/cogs.html). You can create a plugin by simply defining a class that extends `AmethystPlugin`. If this is found by the [Dynamic Module Importer](#dynamic-module-import) then it will be automatically registered to the client, otherwise you will have to use the `AmethystClient.register_plugin` method.
+Amethyst has a plugin system, powered by [dynamicpy](https://github.com/NimajnebEC/dynamicpy) and inspired by [discord.py Cogs](https://discordpy.readthedocs.io/en/stable/ext/commands/cogs.html). You can create a plugin by simply defining a class that extends `amethyst.Plugin`. If this is found by the [Dynamic Module Importer](#dynamic-module-import) then it will be automatically registered to the client, otherwise you will have to use the `Client.register_plugin` method.
 
 An example plugin may look like the following:
 
 ```py
 import amethyst
 
-class ExamplePlugin(amethyst.AmethystPlugin):
+class ExamplePlugin(amethyst.Plugin):
 
-    @amethyst.event(amethyst.events.on_ready)
+    @amethyst.event(amethyst.on_ready)
     async def on_ready(self):
         channel = self.client.get_channel(000000000000000000)
         await channel.send("Bot is ready!")
 ```
 
 ### Plugin Dependency Injection
 
-Amethyst plugins support [dynamicpy dependency injection](https://github.com/NimajnebEC/dynamicpy#dependencylibrary) for their constructors. You can add dependencies to the client using the `AmethystClient.add_dependency` method, which will then be injected into constructor parameters when the plugin is registered.
+Amethyst plugins support [dynamicpy dependency injection](https://github.com/NimajnebEC/dynamicpy#dependencylibrary) for their constructors. You can add dependencies to the client using the `Client.add_dependency` method, which will then be injected into constructor parameters when the plugin is registered.
 
 ```py
 import mysql.connector
 import amethyst
 
-client = amethyst.AmethystClient(...)
+client = amethyst.Client(...)
 database: mysql.connector.MySQLConnection = mysql.connector.connect(...)
 client.add_dependency(database)
 
-class ExamplePlugin(amethyst.AmethystPlugin):
+class ExamplePlugin(amethyst.Plugin):
 
     def __init__(self, database: mysql.connector.MySQLConnection) -> None:
         self.database = database
 
 ```
 
 ## Evironment Variables
 
 Amethyst uses [python-dotenv](https://pypi.org/project/python-dotenv/) to load `.env` files found at the project root. This can be used to configure certain aspects of the library.
 
-| Name                | Default | Description                                                                                     |
-| ------------------- | ------- | ----------------------------------------------------------------------------------------------- |
-| AMETHYST_BOT_TOKEN  | _None_  | If present, `token` can be omitted from the `AmethystClient.run` and this will be used instead. |
-| AMETHYST_AUTO_SYNC  | true    | If `true`, the client will synchronise app_commands if they are out of date with Discord.       |
-| AMETHYST_SYNC_GUILD | _None_  | If present, app_commands will only be synchronised to specified guild id.                       |
+| Name               | Default | Description                                                                                |
+| ------------------ | ------- | ------------------------------------------------------------------------------------------ |
+| AMETHYST_TOKEN     | _None_  | If present, `token` can be omitted from the `Client.run` and this will be used instead.    |
+| AMETHYST_AUTO_SYNC | true    | If present, the client will synchronise app_commands if they are out of date with Discord. |
+| AMETHYST_GUILD     | _None_  | If present, the client will ignore all events from any guild with a differnet id.          |
 
 ## Roadmap
 
-- [ ] Context Menus
 - [ ] Hybrid Commands
-- [ ] Plugins enable/disable after initialisation
 - [ ] Debug mode featuring automatic reload
```

