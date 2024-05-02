# Comparing `tmp/aitelegrambot-0.6.0.tar.gz` & `tmp/aitelegrambot-0.7.0.tar.gz`

## Comparing `aitelegrambot-0.6.0.tar` & `aitelegrambot-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/.env.example
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/Makefile
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/Makefile.venv
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/docs/README.md
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/docs/commands.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/docs/setup.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/src/aitelegrambot/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/src/aitelegrambot/__main__.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/src/aitelegrambot/bot.py
--rw-r--r--   0        0        0     8910 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/src/aitelegrambot/commandhandlers.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/src/aitelegrambot/constants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/.gitignore
--rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/LICENSE.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/.env.example
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/Makefile
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/Makefile.venv
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/docs/README.md
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/docs/commands.md
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/docs/setup.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/src/aitelegrambot/__init__.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/src/aitelegrambot/__main__.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/src/aitelegrambot/bot.py
+-rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/src/aitelegrambot/commandhandlers.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/src/aitelegrambot/constants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/.gitignore
+-rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/PKG-INFO
```

### Comparing `aitelegrambot-0.6.0/CHANGELOG.md` & `aitelegrambot-0.7.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -69,7 +69,11 @@
 - Fix bug
 
 ## 0.6.0
 
 - add help command.
 - Reply to the user even when streaming messages is disabled.
 - Fix bugs with pull and delete commands.
+
+## 0.7.0
+
+- add support for multiple administrators.
```

### Comparing `aitelegrambot-0.6.0/Makefile.venv` & `aitelegrambot-0.7.0/Makefile.venv`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.6.0/docs/commands.md` & `aitelegrambot-0.7.0/docs/commands.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 /help
 ```
 #### description
 
 Returns a list of all the commands.
 
 ## Administration Commands
-Commands only available for the administrator.
+Commands only available for the administrators.
 ### List model command
 #### invocation
 ```
 /list_models
 ```
 #### description
```

### Comparing `aitelegrambot-0.6.0/docs/setup.md` & `aitelegrambot-0.7.0/docs/setup.md`

 * *Files 7% similar despite different names*

```diff
@@ -44,22 +44,22 @@
 ADMIN_ID=adminuserid
 ENABLE_STREAMING_RESPONSE=disable
 MESSAGE_CHUNK_SIZE=5
 ```
 
 Here is a table detailing each option.
 
-| Option                      | Description                                                                                                | Examples                                         | Required                               | Runtime modifiable |
-|-----------------------------|------------------------------------------------------------------------------------------------------------|--------------------------------------------------|----------------------------------------|--------------------|
-| `TELEGRAM_BOT_TOKEN`        | Telegram bot token issued by Telegram's botfather                                                          | `9999999999:XXXXXXXXXXXXXXXXXXXXX_XXXXXXXXXXXXX` | Yes                                    | No                 |
-| `DEFAULT_MODEL`             | The default model to be used by the Telegram Bot (It can be changed during runtime by the admin)           | `tusharhero/rationalai`                          | No                                     | Yes                |
-| `OLLAMA_HOST`               | Host address of the `ollama` service.                                                                      | `localhost:11434`                                | No                                     | No                 |
-| `ADMIN_ID`                  | Telegram user id of the administrator, this userid will be able to change multiple options during runtime. | `9999999999`                                     | No (Admin commands won't be available) | No                 |
-| `ENABLE_STREAMING_RESPONSE` | Select whether, the bot will stream responses or not.                                                      | `enable` or `disable`                            | No (disabled by default)               | No                 |
-| `MESSAGE_CHUNK_SIZE`        | The number of words to be send at a time, when streaming responses.                                        | `5`, `6`, any integer.                           | No (`5` by default)                    | No                 |
+| Option                      | Description                                                                                                    | Examples                                                             | Required                               | Runtime modifiable |
+|-----------------------------|----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------|----------------------------------------|--------------------|
+| `TELEGRAM_BOT_TOKEN`        | Telegram bot token issued by Telegram's botfather                                                              | `9999999999:XXXXXXXXXXXXXXXXXXXXX_XXXXXXXXXXXXX`                     | Yes                                    | No                 |
+| `DEFAULT_MODEL`             | The default model to be used by the Telegram Bot (It can be changed during runtime by the admin)               | `tusharhero/rationalai`                                              | No                                     | Yes                |
+| `OLLAMA_HOST`               | Host address of the `ollama` service.                                                                          | `localhost:11434`                                                    | No                                     | No                 |
+| `ADMIN_ID`                  | Telegram user ids of the administrators, these userids will be able to change multiple options during runtime. | `9999999999` or `9999999999,9999999998`(for multiple administrators) | No (Admin commands won't be available) | No                 |
+| `ENABLE_STREAMING_RESPONSE` | Select whether, the bot will stream responses or not.                                                          | `enable` or `disable`                                                | No (disabled by default)               | No                 |
+| `MESSAGE_CHUNK_SIZE`        | The number of words to be send at a time, when streaming responses.                                            | `5`, `6`, any integer.                                               | No (`5` by default)                    | No                 |
 
 
 5. Run the bot.
 
 ```bash
 aitelegrambot
 ```
```

### Comparing `aitelegrambot-0.6.0/src/aitelegrambot/__main__.py` & `aitelegrambot-0.7.0/src/aitelegrambot/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         exit()
 
     # Run the bot.
     bot: TelegramBot = TelegramBot(
         ollama_host=os.environ.get("OLLAMA_HOST", "localhost:11434"),
         bot_token=os.environ["TELEGRAM_BOT_TOKEN"],
         default_model=os.environ.get("DEFAULT_MODEL", "tusharhero/rationalai"),
-        administrator_user_id=int(os.environ.get("ADMIN_ID", 0)),
+        administrator_user_ids=[
+            int(user_id) for user_id in os.environ.get("ADMIN_ID", 0).split(",")],
         enable_streaming_response=bool(
             os.environ.get("ENABLE_STREAMING_RESPONSE", "disable") == "enable"
         ),
         message_chunk_size=int(os.environ.get("MESSAGE_CHUNK_SIZE", 5)),
     )
 
     bot.run()
```

### Comparing `aitelegrambot-0.6.0/src/aitelegrambot/bot.py` & `aitelegrambot-0.7.0/src/aitelegrambot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,28 +39,28 @@
     """
 
     def __init__(
         self,
         ollama_host: str,
         bot_token: str,
         default_model: str,
-        administrator_user_id: int,
+        administrator_user_ids: list[int],
         enable_streaming_response: bool,
         message_chunk_size: int,
     ):
         """
         Initializes an instance of TelegramBot.
 
         Arguments:
         ==========
         ollama_host: Host address of the `ollama` service.
         bot_token: Bot token for telegram.
         default_model: The default model to load when the bot is
         initialized.
-        administrator_user_id: Telegram user id of the administrator.
+        administrator_user_ids: Telegram user ids of the administrators.
         enable_streaming_response: Enable streaming response option.
         message_chunk_size: The number of words to be send at a time.
         """
         ollama_state: OllamaState = OllamaState(
             Client(host=ollama_host), default_model, message_chunk_size
         )
         self.normal_command_handlers: CommandHandlers = NormalCommandHandlers(
@@ -69,15 +69,15 @@
         self.normal_command_handlers.inference = (
             self.normal_command_handlers.stream_inference
             if enable_streaming_response
             else self.normal_command_handlers.basic_inference
         )
 
         self.administrative_command_handlers: CommandHandlers = (
-            AdministrationCommandHandlers(ollama_state, administrator_user_id)
+            AdministrationCommandHandlers(ollama_state, administrator_user_ids)
         )
 
         self.application: Application = ApplicationBuilder().token(bot_token).build()
 
     def run(self):
         """
         Run the bot.
```

### Comparing `aitelegrambot-0.6.0/src/aitelegrambot/commandhandlers.py` & `aitelegrambot-0.7.0/src/aitelegrambot/commandhandlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,36 +179,36 @@
                 time.sleep(2)
         if not is_message_rounded:
             await message.edit_text(text="".join(message_stream), parse_mode="Markdown")
 
 
 class AdministrationCommandHandlers(CommandHandlers):
     """
-    Class for administrating Ollama by the Bot administrator.
+    Class for administrating Ollama by the Bot administrators.
     """
 
-    def __init__(self, ollama_state: OllamaState, administrator_user_id: str):
+    def __init__(self, ollama_state: OllamaState, administrator_user_ids: list[int]):
         """
         Arguments:
         ==========
         ollama_state: The Ollama State with Ollama client and model name.
-        administrator_user_id: Telegram user id of the administrator.
+        administrator_user_ids: Telegram user ids of the administrators.
         """
         super().__init__(ollama_state)
-        self.administrator_user_id: int = administrator_user_id
+        self.administrator_user_ids: list[int] = administrator_user_ids
 
     def is_admin(self, update: Update):
         """
-        Check if the current user is the administrator.
+        Check if the current user is an administrator.
 
         Arguments:
         ==========
         update: The update to be processed.
         """
-        return update.message.from_user.id == self.administrator_user_id
+        return (update.message.from_user.id in self.administrator_user_ids)
 
     async def list_models(
         self,
         update: Update,
         context: ContextTypes.DEFAULT_TYPE,
     ):
         """
```

### Comparing `aitelegrambot-0.6.0/src/aitelegrambot/constants.py` & `aitelegrambot-0.7.0/src/aitelegrambot/constants.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.6.0/LICENSE.md` & `aitelegrambot-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.6.0/pyproject.toml` & `aitelegrambot-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [tool.hatch.build.targets.wheel]
 packages = ["src/aitelegrambot"]
 [project]
 name = "aitelegrambot"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
   "ollama",
   "python-telegram-bot",
   "python-dotenv",
 ]
 authors = [
   {name = "tusharhero", email = "tusharhero@sdf.org"},
```

### Comparing `aitelegrambot-0.6.0/PKG-INFO` & `aitelegrambot-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aitelegrambot
-Version: 0.6.0
+Version: 0.7.0
 Summary: aitelegrambot is a Telegram bot that uses the Ollama backend to run the LLM rationalAI (by default).
 Author-email: tusharhero <tusharhero@sdf.org>, alokosx <alokosx@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: ollama
 Requires-Dist: python-dotenv
```

