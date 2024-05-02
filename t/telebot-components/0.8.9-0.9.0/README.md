# Comparing `tmp/telebot_components-0.8.9.tar.gz` & `tmp/telebot_components-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_components-0.8.9.tar", max compression
+gzip compressed data, was "telebot_components-0.9.0.tar", max compression
```

## Comparing `telebot_components-0.8.9.tar` & `telebot_components-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0    35148 2023-07-12 07:22:41.880527 telebot_components-0.8.9/LICENSE
--rw-r--r--   0        0        0     2266 2023-07-12 07:22:41.880527 telebot_components-0.8.9/README.md
--rw-r--r--   0        0        0     1619 2023-07-12 07:23:10.805042 telebot_components-0.8.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/__init__.py
--rw-r--r--   0        0        0    13083 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/broadcast/__init__.py
--rw-r--r--   0        0        0     2835 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/broadcast/message_senders.py
--rw-r--r--   0        0        0      159 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/broadcast/subscriber.py
--rw-r--r--   0        0        0        0 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/constants/__init__.py
--rw-r--r--   0        0        0    15212 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/constants/emoji.py
--rw-r--r--   0        0        0      168 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/constants/times.py
--rw-r--r--   0        0        0    54512 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/feedback/__init__.py
--rw-r--r--   0        0        0     2075 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/feedback/anti_spam.py
--rw-r--r--   0        0        0        0 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/feedback/integration/__init__.py
--rw-r--r--   0        0        0     8321 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/feedback/integration/aux_feedback_handler.py
--rw-r--r--   0        0        0     3983 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/feedback/integration/interface.py
--rw-r--r--   0        0        0    34435 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/feedback/integration/trello.py
--rw-r--r--   0        0        0      237 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/feedback/trello_integration.py
--rw-r--r--   0        0        0      493 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/feedback/types.py
--rw-r--r--   0        0        0        0 2023-07-12 07:22:41.880527 telebot_components-0.8.9/telebot_components/form/__init__.py
--rw-r--r--   0        0        0    31714 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/form/field.py
--rw-r--r--   0        0        0    18987 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/form/form.py
--rw-r--r--   0        0        0    20318 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/form/handler.py
--rw-r--r--   0        0        0        0 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/form/helpers/__init__.py
--rw-r--r--   0        0        0     7572 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/form/helpers/calendar_keyboard.py
--rw-r--r--   0        0        0        0 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/menu/__init__.py
--rw-r--r--   0        0        0    13686 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/menu/menu.py
--rw-r--r--   0        0        0        0 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/py.typed
--rw-r--r--   0        0        0        0 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/redis_utils/__init__.py
--rw-r--r--   0        0        0    11405 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/redis_utils/emulation.py
--rw-r--r--   0        0        0     6564 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/redis_utils/interface.py
--rw-r--r--   0        0        0        0 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/stores/__init__.py
--rw-r--r--   0        0        0     1825 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/stores/banned_users.py
--rw-r--r--   0        0        0     8229 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/stores/category.py
--rw-r--r--   0        0        0     9342 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/stores/forum_topics.py
--rw-r--r--   0        0        0     9845 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/stores/generic.py
--rw-r--r--   0        0        0     8298 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/stores/language.py
--rw-r--r--   0        0        0      397 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/stores/types.py
--rw-r--r--   0        0        0     3914 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/stores/user_group.py
--rw-r--r--   0        0        0      614 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/stores/utils.py
--rw-r--r--   0        0        0     8172 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/utils/__init__.py
--rw-r--r--   0        0        0     5185 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/utils/airtable.py
--rw-r--r--   0        0        0     2564 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/utils/alerts.py
--rw-r--r--   0        0        0     1257 2023-07-12 07:22:41.884527 telebot_components-0.8.9/telebot_components/utils/strings.py
--rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 telebot_components-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-09-27 11:53:15.296269 telebot_components-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2265 2023-09-27 11:53:15.300269 telebot_components-0.9.0/README.md
+-rw-r--r--   0        0        0     1662 2023-09-27 11:53:38.216381 telebot_components-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-27 11:53:15.300269 telebot_components-0.9.0/telebot_components/__init__.py
+-rw-r--r--   0        0        0    13083 2023-09-27 11:53:15.300269 telebot_components-0.9.0/telebot_components/broadcast/__init__.py
+-rw-r--r--   0        0        0     2835 2023-09-27 11:53:15.300269 telebot_components-0.9.0/telebot_components/broadcast/message_senders.py
+-rw-r--r--   0        0        0      159 2023-09-27 11:53:15.300269 telebot_components-0.9.0/telebot_components/broadcast/subscriber.py
+-rw-r--r--   0        0        0        0 2023-09-27 11:53:15.300269 telebot_components-0.9.0/telebot_components/constants/__init__.py
+-rw-r--r--   0        0        0    15212 2023-09-27 11:53:15.300269 telebot_components-0.9.0/telebot_components/constants/emoji.py
+-rw-r--r--   0        0        0      168 2023-09-27 11:53:15.300269 telebot_components-0.9.0/telebot_components/constants/times.py
+-rw-r--r--   0        0        0    56127 2023-09-27 11:53:15.300269 telebot_components-0.9.0/telebot_components/feedback/__init__.py
+-rw-r--r--   0        0        0     2075 2023-09-27 11:53:15.300269 telebot_components-0.9.0/telebot_components/feedback/anti_spam.py
+-rw-r--r--   0        0        0        0 2023-09-27 11:53:15.300269 telebot_components-0.9.0/telebot_components/feedback/integration/__init__.py
+-rw-r--r--   0        0        0     8339 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/feedback/integration/aux_feedback_handler.py
+-rw-r--r--   0        0        0     3983 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/feedback/integration/interface.py
+-rw-r--r--   0        0        0    34435 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/feedback/integration/trello.py
+-rw-r--r--   0        0        0      237 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/feedback/trello_integration.py
+-rw-r--r--   0        0        0      493 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/feedback/types.py
+-rw-r--r--   0        0        0        0 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/form/__init__.py
+-rw-r--r--   0        0        0    31710 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/form/field.py
+-rw-r--r--   0        0        0    18987 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/form/form.py
+-rw-r--r--   0        0        0    20370 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/form/handler.py
+-rw-r--r--   0        0        0        0 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/form/helpers/__init__.py
+-rw-r--r--   0        0        0     7572 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/form/helpers/calendar_keyboard.py
+-rw-r--r--   0        0        0      112 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/menu/__init__.py
+-rw-r--r--   0        0        0    19894 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/menu/menu.py
+-rw-r--r--   0        0        0        0 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/py.typed
+-rw-r--r--   0        0        0        0 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/redis_utils/__init__.py
+-rw-r--r--   0        0        0    16019 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/redis_utils/emulation.py
+-rw-r--r--   0        0        0     6850 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/redis_utils/interface.py
+-rw-r--r--   0        0        0        0 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/stores/__init__.py
+-rw-r--r--   0        0        0     1825 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/stores/banned_users.py
+-rw-r--r--   0        0        0     8229 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/stores/category.py
+-rw-r--r--   0        0        0     9342 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/stores/forum_topics.py
+-rw-r--r--   0        0        0    10381 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/stores/generic.py
+-rw-r--r--   0        0        0     8492 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/stores/language.py
+-rw-r--r--   0        0        0      397 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/stores/types.py
+-rw-r--r--   0        0        0     3914 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/stores/user_group.py
+-rw-r--r--   0        0        0      614 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/stores/utils.py
+-rw-r--r--   0        0        0     8172 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/utils/__init__.py
+-rw-r--r--   0        0        0     5185 2023-09-27 11:53:15.304269 telebot_components-0.9.0/telebot_components/utils/airtable.py
+-rw-r--r--   0        0        0     2835 2023-09-27 11:53:15.308269 telebot_components-0.9.0/telebot_components/utils/alerts.py
+-rw-r--r--   0        0        0     6680 2023-09-27 11:53:15.308269 telebot_components-0.9.0/telebot_components/utils/secrets.py
+-rw-r--r--   0        0        0     1257 2023-09-27 11:53:15.308269 telebot_components-0.9.0/telebot_components/utils/strings.py
+-rw-r--r--   0        0        0     3505 1970-01-01 00:00:00.000000 telebot_components-0.9.0/PKG-INFO
```

### Comparing `telebot_components-0.8.9/LICENSE` & `telebot_components-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/README.md` & `telebot_components-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 1. Clone repository
    ```bash
    git clone git@github.com:bots-against-war/telebot-components.git baw
    cd ./baw
    ```
 
-2. The project requires Poerty 1.5.1 (see [installation instruction](https://python-poetry.org/docs/master#installing-with-the-official-installer))).
+2. The project requires Poerty 1.5.1 (see [installation instruction](https://python-poetry.org/docs/master#installing-with-the-official-installer)).
    For example, to install `1.5.1` on Unix, run
    ```bash
    curl -sSL https://install.python-poetry.org | python3 - --version 1.5.1
    ```
 
 3. Then, to install the library with all dependencies, run from project root
    ```bash
```

### Comparing `telebot_components-0.8.9/pyproject.toml` & `telebot_components-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telebot-components"
-version = "0.8.9"
+version = "0.9.0"
 description = "Framework/toolkit for building Telegram bots with telebot and redis"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot-components"
 packages = [{include = "telebot_components"}]
 
@@ -16,26 +16,28 @@
 enable = false
 vcs = "git"
 dirty = true
 style="semver"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-telebot-against-war = "^0.6.7"
+telebot-against-war = "^0.6.11"
 redis = "^4.3.1"
 py-trello = "^0.18.0"
 markdownify = "^0.11.2"
 pytest-mock = "^3.7.0"
 "ruamel.yaml" = "^0.17.21"
 pyairtable = "^1.5.0"
 Pillow = "^9.2.0"
 markdown = "^3.4.1"
 beautifulsoup4 = "^4.11.1"
 tenacity = "^8.1.0"
 async-lru = "^2.0.2"
+cryptography = "^41.0.2"
+toml = "^0.10.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-aiohttp = "1.0.4"
 pytest-asyncio = "^0.18.3"
 python-dotenv = "^0.20.0"
 aioresponses = "0.7.3"
```

### Comparing `telebot_components-0.8.9/telebot_components/broadcast/__init__.py` & `telebot_components-0.9.0/telebot_components/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/broadcast/message_senders.py` & `telebot_components-0.9.0/telebot_components/broadcast/message_senders.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/constants/emoji.py` & `telebot_components-0.9.0/telebot_components/constants/emoji.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/feedback/__init__.py` & `telebot_components-0.9.0/telebot_components/feedback/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -258,22 +258,14 @@
         self.validate_service_messages()
 
         if admin_chat_response_actions is None:
             self.admin_chat_response_actions = []
         else:
             self.admin_chat_response_actions = admin_chat_response_actions
 
-        if self.banned_users_store is not None:
-            self.admin_chat_response_actions.append(
-                AdminChatAction(
-                    command="/ban",
-                    callback=self._ban_admin_chat_action,
-                    delete_everything_related_to_user_after=True,
-                )
-            )
         self.admin_chat_response_action_by_command = {aca.command: aca for aca in self.admin_chat_response_actions}
 
         # === stores used by the handler ===
 
         # forwarded message in admin chat -> origin chat id (user id)
         self.origin_chat_id_store = KeyValueStore[int](
             name="origin-chat-for-msg",
@@ -377,14 +369,38 @@
             if message is None:
                 continue
             if self.language_store is None:
                 vaildate_singlelang_text(message)
             else:
                 self.language_store.validate_multilang(message)
 
+    async def _delete_user_related_messages(
+        self, bot: AsyncTeleBot, origin_chat_id: int, initiator_message_id: int
+    ) -> None:
+        if self.config.forum_topic_per_user:
+            user_topic_message_thread_id = await self.message_thread_id_by_user_id_store.load(origin_chat_id)
+            if user_topic_message_thread_id is not None:
+                self.logger.info("Found forum topic for user, deleting it")
+                await bot.delete_forum_topic(self.admin_chat_id, message_thread_id=user_topic_message_thread_id)
+                await self.message_thread_id_by_user_id_store.drop(origin_chat_id)
+                self.logger.info("User forum topic deleted")
+                return
+
+        user_related_message_ids = await self.user_related_messages_store.all(origin_chat_id)
+        user_related_message_ids.add(initiator_message_id)
+        for message_id in user_related_message_ids:
+            try:
+                await bot.delete_message(self.admin_chat_id, message_id)
+                await self.origin_chat_id_store.drop(message_id)
+                await asyncio.sleep(0.5)
+            except Exception:
+                pass
+        await self.user_related_messages_store.drop(origin_chat_id)
+        await self.message_log_store.drop(origin_chat_id)
+
     async def _ban_admin_chat_action(
         self, admin_message: tg.Message, forwarded_message: tg.Message, origin_chat_id: int
     ):
         if self.banned_users_store is not None:
             await self.banned_users_store.ban_user(origin_chat_id)
 
     async def save_message_from_user(
@@ -952,31 +968,26 @@
                 if origin_chat_id is None:
                     return
 
                 if message.text is not None and message.text.startswith("/"):
                     # admin chat commands
                     if message.text in self.admin_chat_response_action_by_command:
                         if forwarded_msg is None:
-                            raise RuntimeError(
-                                "Admin chat response actions are not supported in per-user forum topics, "
-                                "please try replying to a user's message directly."
-                            )
+                            raise RuntimeError("To execute command, please reply to a user's message directly.")
                         admin_chat_action = self.admin_chat_response_action_by_command[message.text]
                         await admin_chat_action.callback(message, forwarded_msg, origin_chat_id)
                         if admin_chat_action.delete_everything_related_to_user_after:
-                            user_related_message_ids = await self.user_related_messages_store.all(origin_chat_id)
-                            user_related_message_ids.add(message.id)
-                            for message_id in user_related_message_ids:
-                                try:
-                                    await bot.delete_message(self.admin_chat_id, message_id)
-                                    await self.origin_chat_id_store.drop(message_id)
-                                except Exception:
-                                    pass
-                            await self.user_related_messages_store.drop(origin_chat_id)
-                            await self.message_log_store.drop(origin_chat_id)
+                            await self._delete_user_related_messages(
+                                bot=bot, origin_chat_id=origin_chat_id, initiator_message_id=message.id
+                            )
+                    elif message.text.strip() == "/ban" and self.banned_users_store is not None:
+                        await self.banned_users_store.ban_user(user_id=origin_chat_id)
+                        await self._delete_user_related_messages(
+                            bot=bot, origin_chat_id=origin_chat_id, initiator_message_id=message.id
+                        )
                     elif message.text_content.startswith("/log"):
                         try:
                             page_str = extract_arguments(message.text_content) or "1"
                             page = int(page_str)
                             if page > 0:
                                 page -= 1  # one based to zero based
                         except Exception:
@@ -1037,18 +1048,20 @@
                                 f"⬆️ Log page {page + 1} / {total_pages}"
                                 + (f"\nNext: <code>/log {page + 2}</code>" if page + 1 < total_pages else "")
                             ),
                             parse_mode="HTML",
                         )
                     else:
                         available_commands = list(self.admin_chat_response_action_by_command.keys()) + ["/log"]
+                        if self.banned_users_store is not None:
+                            available_commands.append("/ban")
                         await bot.reply_to(
                             message,
-                            f"Invalid admin chat command: {message.text}; available commands are: "
-                            + ", ".join(available_commands),
+                            f"Invalid admin chat command: {message.text!r}; available commands are: "
+                            + ", ".join(repr(cmd) for cmd in available_commands),
                         )
                 else:
                     # actual response to the user
                     try:
                         copied_message_id = await bot.copy_message(
                             chat_id=origin_chat_id, from_chat_id=self.admin_chat_id, message_id=message.id
                         )
@@ -1073,15 +1086,15 @@
                                 origin_chat_id=origin_chat_id, sent_message_id=int(copied_message_id.message_id)
                             ),
                         )
 
                     if self.config.hashtags_in_admin_chat:
                         await self._remove_unanswered_hashtag(bot, forwarded_msg_id)
                     has_attachments = message.content_type != "text"
-                    await asyncio.gather(
+                    maybe_exceptions = await asyncio.gather(
                         *[
                             integration.handle_user_message_replied_elsewhere(
                                 UserMessageRepliedEvent(
                                     bot=bot,
                                     origin_chat_id=origin_chat_id,
                                     reply_text=(
                                         (message.html_text if not has_attachments else message.html_caption) or ""
@@ -1089,16 +1102,29 @@
                                     reply_has_attachments=has_attachments,
                                     reply_author=message.from_user.first_name,
                                     reply_link=telegram_message_url(self.admin_chat_id, message.id),
                                     main_admin_chat_message_id=forwarded_msg_id,
                                 )
                             )
                             for integration in self.integrations
-                        ]
+                        ],
+                        return_exceptions=True,
                     )
+                    for maybe_exception, integration in zip(maybe_exceptions, self.integrations):
+                        if maybe_exception is None:
+                            continue
+                        elif isinstance(maybe_exception, Exception):
+                            self.logger.error(
+                                f"Error notifying integration {integration.name()!r}, ignoring: {maybe_exception!r}"
+                            )
+                        else:
+                            self.logger.warning(
+                                f"Unexpected value returned from notifying integration {integration.name()!r}, "
+                                + f"ignoring: {maybe_exception!r}"
+                            )
             except Exception as e:
                 await bot.reply_to(message, f"Something went wrong! {e}")
                 self.logger.exception("Unexpected error while replying to forwarded msg")
 
 
 def _join_hashtags(hashtags: list[str]) -> str:
     return " ".join(["#" + h for h in hashtags])
```

### Comparing `telebot_components-0.8.9/telebot_components/feedback/anti_spam.py` & `telebot_components-0.9.0/telebot_components/feedback/anti_spam.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/feedback/integration/aux_feedback_handler.py` & `telebot_components-0.9.0/telebot_components/feedback/integration/aux_feedback_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             return
         # the terminology is reversed here, because for integration's POV, aux chat is main and vice versa
         aux_admin_chat_message_id = event.main_admin_chat_message_id
         main_admin_chat_message_id = await self.aux.main_by_aux_admin_chat_message_id_store.load(
             aux_admin_chat_message_id
         )
         if main_admin_chat_message_id is None:
-            self.logger.error("Message in aux admin chat has no saved main admin chat message id")
+            self.logger.info("Message in aux admin chat has no saved main admin chat message id, ignoring")
             return
         await self.aux.message_replied_callback(
             UserMessageRepliedFromIntegrationEvent(
                 bot=event.bot,
                 origin_chat_id=event.origin_chat_id,
                 reply_text=event.reply_text,
                 reply_has_attachments=event.reply_has_attachments,
@@ -152,15 +152,15 @@
             )
 
     async def handle_user_message_replied_elsewhere(self, event: UserMessageRepliedEvent) -> None:
         aux_admin_chat_message_id = await self.aux_by_main_admin_chat_message_id_store.load(
             event.main_admin_chat_message_id
         )
         if aux_admin_chat_message_id is None:
-            self.logger.error("Message in the main admin chat has no saved aux admin chat message id")
+            self.logger.info("Message in the main admin chat has no saved aux admin chat message id, ignoring")
             return
         # from aux feedback handler's POV, aux admin chat msg id is main
         event.main_admin_chat_message_id = aux_admin_chat_message_id
 
         if not isinstance(event, UserMessageRepliedFromIntegrationEvent):
             event = UserMessageRepliedFromIntegrationEvent(
                 bot=event.bot,
```

### Comparing `telebot_components-0.8.9/telebot_components/feedback/integration/interface.py` & `telebot_components-0.9.0/telebot_components/feedback/integration/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/feedback/integration/trello.py` & `telebot_components-0.9.0/telebot_components/feedback/integration/trello.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/form/field.py` & `telebot_components-0.9.0/telebot_components/form/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
         parsed_enum = self.parse_enum(message.text_content)
         if parsed_enum is None:
             raise BadFieldValueError(self.invalid_enum_value_error_msg)
         else:
             return parsed_enum
 
     def value_to_str(self, value: Enum, lang: MaybeLanguage) -> str:
-        if not is_any_text(value.value):
+        if is_any_text(value.value):
             return any_text_to_str(value.value, lang)
         else:
             return str(value.value)
 
 
 EnumField = SingleSelectField  # backward compatibility
```

### Comparing `telebot_components-0.8.9/telebot_components/form/form.py` & `telebot_components-0.9.0/telebot_components/form/form.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/form/handler.py` & `telebot_components-0.9.0/telebot_components/form/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,17 @@
     def can_skip_field_msg(self, language: MaybeLanguage) -> str:
         return any_text_to_str(self.can_skip_field_template, language).format(self.skip_cmd)
 
     def keep_existing_field_value_msg(self, value_dump: str, language: MaybeLanguage) -> Optional[str]:
         if self.keep_existing_field_value_template is None:
             return None
         else:
-            return any_text_to_str(self.keep_existing_field_value_template, language).format(value_dump, self.keep_cmd)
+            return any_text_to_str(self.keep_existing_field_value_template, language).format(
+                telegram_html_escape(value_dump), self.keep_cmd
+            )
 
     def form_starting_msg(self, language: MaybeLanguage) -> str:
         return any_text_to_str(self.form_starting_template, language).format(", ".join(self.cancel_cmds))
 
     def unsupported_cmd_error_msg(self, language: MaybeLanguage) -> str:
         return any_text_to_str(self.unsupported_cmd_error_template, language).format(", ".join(self.available_cmds))
```

### Comparing `telebot_components-0.8.9/telebot_components/form/helpers/calendar_keyboard.py` & `telebot_components-0.9.0/telebot_components/form/helpers/calendar_keyboard.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/redis_utils/interface.py` & `telebot_components-0.9.0/telebot_components/redis_utils/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # type defs copied from redis
 
 
 class RedisInterface(ABC):
     """Abstract interface for the parts of redis.asyncio.Redis class we're using;
     please update when utilizing new methods.
 
-    Note that Redis must not decode responses and return plain bytes
-    (i.e. do NOT specify decode_responses=True option).
+    Note that this is an interface for Redis configured to not decode responses and return plain bytes
+    (i.e. it must not specify decode_responses=True option).
 
     When using real Redis instance in place of RedisInterface, mypy may complain, but we have to ignore it
     """
 
     @abstractmethod
     def pipeline(self, transaction: bool = True, shard_hint: Optional[str] = None) -> "RedisPipelineInterface":
         """
@@ -169,14 +169,23 @@
 
     @abstractmethod
     async def hvals(self, name: str) -> list[bytes]:
         """Return the list of values within hash ``name``"""
         ...
 
     @abstractmethod
+    async def hgetall(self, name: str) -> dict[bytes, bytes]:
+        """
+        Return a Python dict of the hash's name/value pairs
+
+        For more information see https://redis.io/commands/hgetall
+        """
+        ...
+
+    @abstractmethod
     async def hdel(self, name: str, *keys: str) -> int:
         """Delete ``keys`` from hash ``name``"""
         ...
 
 
 RedisCmdReturn = Union[bytes, list[bytes], None, int]
```

### Comparing `telebot_components-0.8.9/telebot_components/stores/banned_users.py` & `telebot_components-0.9.0/telebot_components/stores/banned_users.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/stores/category.py` & `telebot_components-0.9.0/telebot_components/stores/category.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/stores/forum_topics.py` & `telebot_components-0.9.0/telebot_components/stores/forum_topics.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/stores/generic.py` & `telebot_components-0.9.0/telebot_components/stores/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import secrets
 from dataclasses import dataclass
 from datetime import timedelta
 from hashlib import md5
 from typing import Callable, ClassVar, Generic, Optional, Protocol, TypeVar, cast
 
 import tenacity
 
@@ -40,21 +41,26 @@
     redis: RedisInterface
     expiration_time: Optional[timedelta] = MONTH
     dumper: Callable[[T], str] = json.dumps
     loader: Callable[[str], T] = json.loads
 
     _prefix_registry: ClassVar[set[str]] = set()
 
+    RANDOMIZE_PREFIXES: ClassVar[bool] = False
+
     def __post_init__(self):
         self.logger = logging.getLogger(f"{__name__}[{self.prefix}-{self.name}]")
         # adding prefix hash to allow stores with nested prefixes
         # e.g. stores with prefixes 'a' and 'ab' could cause a collision but
         # we transform them to 'a-0cc17' and 'ab-187ef' and voila
         plain_prefix = f"{self.prefix}-{self.name}"
         prefix_hash = md5(plain_prefix.encode("utf-8")).hexdigest()[:5]
+        if self.RANDOMIZE_PREFIXES:
+            # option for testing that allows creating unlimited number of independent copies for every store
+            prefix_hash += "-RANDOM" + secrets.token_hex(nbytes=8)
         self._full_prefix = f"{plain_prefix}-{prefix_hash}-"
         if self._full_prefix in self._prefix_registry:
             raise ValueError(
                 f"Attempt to create {self.__class__.__name__} with prefix {self._full_prefix!r} already in use"
             )
         else:
             self._prefix_registry.add(self._full_prefix)
@@ -261,9 +267,14 @@
 
     @redis_retry()
     async def list_values(self, key: str_able) -> list[ValueT]:
         value_dumps = await self.redis.hvals(self._full_key(key))
         return [self.loader(dump.decode("utf-8")) for dump in value_dumps]
 
     @redis_retry()
+    async def load(self, key: str_able) -> dict[str, ValueT]:
+        raw = await self.redis.hgetall(self._full_key(key))
+        return {raw_key.decode("utf-8"): self.loader(raw_value.decode("utf-8")) for raw_key, raw_value in raw.items()}
+
+    @redis_retry()
     async def remove_subkey(self, key: str_able, subkey: str_able) -> bool:
         return await self.redis.hdel(self._full_key(key), str(subkey)) == 1
```

### Comparing `telebot_components-0.8.9/telebot_components/stores/language.py` & `telebot_components-0.9.0/telebot_components/stores/language.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,16 +120,19 @@
         self.default_language = default_language
         self.language_callback_data = CallbackData("code", prefix="lang")
         self.menu_config = menu_config
 
     def validate_multilang(self, ml_text: Any):
         validate_multilang_text(ml_text, self.languages)
 
+    async def get_selected_user_language(self, user: types.User) -> Optional[Language]:
+        return await self.user_language_store.load(user.id)
+
     async def get_user_language(self, user: types.User) -> Language:
-        stored_lang = await self.user_language_store.load(user.id)
+        stored_lang = await self.get_selected_user_language(user)
         if stored_lang is not None:
             return stored_lang
         if user.language_code is None:
             return self.default_language
         try:
             user_interface_language = Language(user.language_code.lower())
             if user_interface_language in self.languages:
@@ -140,40 +143,43 @@
 
     async def set_user_language(self, user: types.User, lang: Language) -> bool:
         if lang not in self.languages:
             raise ValueError(f"Can't set user language to unsupported value {lang!r}")
         return await self.user_language_store.save(user.id, lang)
 
     def setup(self, bot: AsyncTeleBot, on_language_change: Optional[OnOptionSelected[Language]] = None):
-        @bot.callback_query_handler(callback_data=self.language_callback_data)
+        @bot.callback_query_handler(callback_data=self.language_callback_data, auto_answer=True)
         async def language_selected(call: types.CallbackQuery):
             user = call.from_user
             try:
                 data = self.language_callback_data.parse(call.data)
                 language = Language(data["code"])
             except Exception:
                 await callback_query_processing_error(bot, call, f"corrupted callback query '{call.data}'", self.logger)
                 return
 
             if language not in self.languages:
                 await callback_query_processing_error(bot, call, f"language '{language}' is not supported", self.logger)
                 return
 
-            language_saved = await self.set_user_language(user, language)
-            if not language_saved:
+            previous_language = await self.get_user_language(user)
+
+            if not await self.set_user_language(user, language):
                 await callback_query_processing_error(bot, call, "unable to save selected language", self.logger)
                 return
+
+            if language == previous_language:
+                return  # language not changed, nothing to do
+
             try:
-                await bot.answer_callback_query(call.id)
                 await bot.edit_message_reply_markup(
                     user.id, call.message.id, reply_markup=self.markup_for_selected_language(language)
                 )
             except Exception:
-                # exception may be raised when user clicks on the same button and markup is not changed
-                pass
+                self.logger.exception("Error editing message reply markup")
             if on_language_change is not None:
                 try:
                     await on_language_change(bot, call.message, call.from_user, language)
                 except Exception:
                     self.logger.exception("Error in on_language_change callback")
 
     def markup_for_selected_language(self, selected_language: Language):
```

### Comparing `telebot_components-0.8.9/telebot_components/stores/user_group.py` & `telebot_components-0.9.0/telebot_components/stores/user_group.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/stores/utils.py` & `telebot_components-0.9.0/telebot_components/stores/utils.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/utils/__init__.py` & `telebot_components-0.9.0/telebot_components/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 def from_yaml_unsafe(dump: str) -> Any:
     return yaml.load(dump)
 
 
 def telegram_html_escape(string: str) -> str:
     """See https://core.telegram.org/bots/api#html-style"""
-    return string.replace("<", "&lt;").replace(">", "&gt;").replace("&", "&amp;")
+    return string.replace("&", "&amp;").replace("<", "&lt;").replace(">", "&gt;")
 
 
 def html_link(href: str, text: str) -> str:
     text = telegram_html_escape(text)
     return f'<a href="{href}">{text}</a>'
```

### Comparing `telebot_components-0.8.9/telebot_components/utils/airtable.py` & `telebot_components-0.9.0/telebot_components/utils/airtable.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/telebot_components/utils/alerts.py` & `telebot_components-0.9.0/telebot_components/utils/alerts.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,62 +3,72 @@
 import re
 from datetime import datetime
 from io import StringIO
 from typing import Optional
 
 from telebot import AsyncTeleBot
 
+from telebot_components.utils import telegram_html_escape
+
 
 class TelegramAlertsHandler(logging.Handler):
     """Sentry-like logging integration: report all error level logs to a dedicated alert Telegram channel"""
 
     def __init__(self, bot: AsyncTeleBot, channel_id: int, app_name: Optional[str]) -> None:
         super().__init__(level=logging.ERROR)
         self.app_name = app_name
-        self.message_prefix = (self.app_name + "\n") if self.app_name else ""
+        self.header = telegram_html_escape(self.app_name) if self.app_name else ""
         self.bot = bot
         self.channel_id = channel_id
         self._tasks: set[asyncio.Task] = set()
         self.formatter = logging.Formatter(fmt="%(name)s: %(message)s\n%(pathname)s:%(lineno)d")
 
     NOT_LETTERS_RE = re.compile(r"\W+")
 
     async def _send_error_message(self, message: str):
         try:
             await self.bot.send_message(
-                self.channel_id, self.message_prefix + "\n<pre>" + message + "</pre>", parse_mode="HTML"
+                self.channel_id,
+                self.header + "\n<pre>" + telegram_html_escape(message) + "</pre>",
+                parse_mode="HTML",
+                auto_split_message=False,
             )
         except Exception:
             try:
                 body = StringIO(initial_value=message)
-                filename_raw = self.message_prefix + message.splitlines()[-1]
+                filename_raw = message.splitlines()[-1]
                 filename = self.NOT_LETTERS_RE.sub("-", filename_raw)
                 filename = filename[:40]
                 filename = f"{filename}-{datetime.now().isoformat(timespec='seconds')}.txt"
-                await self.bot.send_document(self.channel_id, body, visible_file_name=filename)
+                await self.bot.send_document(
+                    self.channel_id,
+                    document=body,
+                    caption=self.header or None,
+                    visible_file_name=filename,
+                )
             except Exception as e:
                 print(f"Error sending alert to Telegram channel: {e!r}")
                 try:
                     await self.bot.send_message(
                         self.channel_id,
-                        self.message_prefix + "⚠️ Failed to send alert, see application logs",
+                        self.header + "\n\n⚠️ Failed to send alert, see application logs",
                     )
                 except Exception:
                     pass
 
     def emit(self, record: logging.LogRecord) -> None:
         try:
             task = asyncio.get_running_loop().create_task(self._send_error_message(self.format(record)))
             self._tasks.add(task)
             task.add_done_callback(self._tasks.discard)
         except Exception as e:
             print(f"{self.__class__.__name__}: Unable to emit message, {e!r}")
 
 
-def configure_alerts(token: str, alerts_channel_id: int, app_name: Optional[str]):
+def configure_alerts(token: str, alerts_channel_id: int, app_name: Optional[str] = None):
     logging.getLogger().addHandler(
         TelegramAlertsHandler(
             bot=AsyncTeleBot(token),
             channel_id=alerts_channel_id,
             app_name=app_name,
         )
     )
```

### Comparing `telebot_components-0.8.9/telebot_components/utils/strings.py` & `telebot_components-0.9.0/telebot_components/utils/strings.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.9/PKG-INFO` & `telebot_components-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: telebot-components
-Version: 0.8.9
+Version: 0.9.0
 Summary: Framework/toolkit for building Telegram bots with telebot and redis
 Home-page: https://github.com/bots-against-war/telebot-components
 License: GPLv3
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: async-lru (>=2.0.2,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: cryptography (>=41.0.2,<42.0.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: markdownify (>=0.11.2,<0.12.0)
 Requires-Dist: py-trello (>=0.18.0,<0.19.0)
 Requires-Dist: pyairtable (>=1.5.0,<2.0.0)
 Requires-Dist: pytest-mock (>=3.7.0,<4.0.0)
 Requires-Dist: redis (>=4.3.1,<5.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
-Requires-Dist: telebot-against-war (>=0.6.7,<0.7.0)
+Requires-Dist: telebot-against-war (>=0.6.11,<0.7.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/bots-against-war/telebot-components
 Description-Content-Type: text/markdown
 
 # telebot-components
 
 Framework / toolkit for building bots with [telebot](https://github.com/bots-against-war/telebot).
 
@@ -36,15 +38,15 @@
 
 1. Clone repository
    ```bash
    git clone git@github.com:bots-against-war/telebot-components.git baw
    cd ./baw
    ```
 
-2. The project requires Poerty 1.5.1 (see [installation instruction](https://python-poetry.org/docs/master#installing-with-the-official-installer))).
+2. The project requires Poerty 1.5.1 (see [installation instruction](https://python-poetry.org/docs/master#installing-with-the-official-installer)).
    For example, to install `1.5.1` on Unix, run
    ```bash
    curl -sSL https://install.python-poetry.org | python3 - --version 1.5.1
    ```
 
 3. Then, to install the library with all dependencies, run from project root
    ```bash
```

