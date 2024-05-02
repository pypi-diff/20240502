# Comparing `tmp/persona_ai-0.1.8.tar.gz` & `tmp/persona_ai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persona_ai-0.1.8.tar", max compression
+gzip compressed data, was "persona_ai-0.1.9.tar", max compression
```

## Comparing `persona_ai-0.1.8.tar` & `persona_ai-0.1.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    11250 2024-04-11 10:00:15.400629 persona_ai-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/code_runners/__init__.py
--rw-r--r--   0        0        0     1239 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/code_runners/base.py
--rw-r--r--   0        0        0     2363 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/code_runners/local.py
--rw-r--r--   0        0        0      153 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/constants.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/conversation_listeners/__init__.py
--rw-r--r--   0        0        0     6058 2024-04-13 08:46:20.890471 persona_ai-0.1.8/persona_ai/conversation_listeners/terminal_conversation_listener.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/conversations/__init__.py
--rw-r--r--   0        0        0     3214 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/conversations/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/__init__.py
--rw-r--r--   0        0        0     6372 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/conversations.py
--rw-r--r--   0        0        0      767 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/events.py
--rw-r--r--   0        0        0     1172 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/domain/repositories.py
--rw-r--r--   0        0        0       82 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/roles.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/schemas/__init__.py
--rw-r--r--   0        0        0      600 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/schemas/crud.py
--rw-r--r--   0        0        0     2759 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/tasks.py
--rw-r--r--   0        0        0      146 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/utils.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/infrastructure/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      758 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/infrastructure/repositories/base.py
--rw-r--r--   0        0        0     1967 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/infrastructure/repositories/in_memory.py
--rw-r--r--   0        0        0     2884 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/infrastructure/repositories/mongo.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/initializers/__init__.py
--rw-r--r--   0        0        0     4362 2024-04-11 10:13:24.751773 persona_ai-0.1.8/persona_ai/initializers/env_configurator.py
--rw-r--r--   0        0        0     1012 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/initializers/persona_configuration.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/models/__init__.py
--rw-r--r--   0        0        0      870 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/models/base.py
--rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/models/code_bison.py
--rw-r--r--   0        0        0    10057 2024-04-13 08:21:54.496495 persona_ai-0.1.8/persona_ai/models/gemini.py
--rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/models/text_bison.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/moderation/__init__.py
--rw-r--r--   0        0        0     2994 2024-04-13 08:48:32.646648 persona_ai-0.1.8/persona_ai/moderation/ai_moderator.py
--rw-r--r--   0        0        0     7345 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/moderation/base.py
--rw-r--r--   0        0        0     4478 2024-04-13 08:29:21.845098 persona_ai-0.1.8/persona_ai/moderation/history_moderator.py
--rw-r--r--   0        0        0     4759 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/moderation/history_moderator_fc.py
--rw-r--r--   0        0        0     5580 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/moderation/react_moderator.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/personas/__init__.py
--rw-r--r--   0        0        0     6678 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/personas/agent.py
--rw-r--r--   0        0        0     4221 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/personas/assistant.py
--rw-r--r--   0        0        0     6504 2024-04-11 10:53:55.133342 persona_ai-0.1.8/persona_ai/personas/base.py
--rw-r--r--   0        0        0     3805 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/personas/coder.py
--rw-r--r--   0        0        0    13267 2024-04-11 11:05:25.442988 persona_ai-0.1.8/persona_ai/personas/party.py
--rw-r--r--   0        0        0     3023 2024-04-11 14:30:55.936715 persona_ai-0.1.8/persona_ai/personas/technician.py
--rw-r--r--   0        0        0      760 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/personas/terminal.py
--rw-r--r--   0        0        0      860 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/agent.jinja2
--rw-r--r--   0        0        0      413 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/assistant.jinja2
--rw-r--r--   0        0        0     1009 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/coder.jinja2
--rw-r--r--   0        0        0     1194 2024-04-11 15:04:24.559375 persona_ai-0.1.8/persona_ai/prompt_templates/history_moderator.jinja2
--rw-r--r--   0        0        0     1062 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/history_moderator_fc.jinja2
--rw-r--r--   0        0        0     1776 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/react_json_moderator.jinja2
--rw-r--r--   0        0        0     1083 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/react_moderator.jinja2
--rw-r--r--   0        0        0      330 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/refiner.jinja2
--rw-r--r--   0        0        0      946 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2
--rw-r--r--   0        0        0      841 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2
--rw-r--r--   0        0        0      102 2024-04-11 14:33:38.412861 persona_ai-0.1.8/persona_ai/prompt_templates/technician.jinja2
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompts/__init__.py
--rw-r--r--   0        0        0      238 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/prompts/base.py
--rw-r--r--   0        0        0     2207 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/prompts/jinja.py
--rw-r--r--   0        0        0      588 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/prompts/text.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/refiners/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/refiners/request_refiner.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/task_manager/__init__.py
--rw-r--r--   0        0        0     2263 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/task_manager/base.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/tools/__init__.py
--rw-r--r--   0        0        0      469 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/tools/base.py
--rw-r--r--   0        0        0     1746 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/tools/functional.py
--rw-r--r--   0        0        0      730 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/tools/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/transport/__init__.py
--rw-r--r--   0        0        0     3477 2024-04-11 13:57:49.665513 persona_ai-0.1.8/persona_ai/transport/local/local_messagebus.py
--rw-r--r--   0        0        0     4022 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/transport/messagebus.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/transport/rabbitmq/__init__.py
--rw-r--r--   0        0        0    10002 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/utils/__init__.py
--rw-r--r--   0        0        0      723 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/utils/crypto.py
--rw-r--r--   0        0        0      911 2024-04-13 08:45:38.530414 persona_ai-0.1.8/persona_ai/utils/extractors.py
--rw-r--r--   0        0        0     1164 2024-04-13 09:10:47.190812 persona_ai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    12749 1970-01-01 00:00:00.000000 persona_ai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11250 2024-04-11 10:00:15.400629 persona_ai-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/code_runners/__init__.py
+-rw-r--r--   0        0        0     1239 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/code_runners/base.py
+-rw-r--r--   0        0        0     2363 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/code_runners/local.py
+-rw-r--r--   0        0        0      153 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/constants.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/conversation_listeners/__init__.py
+-rw-r--r--   0        0        0     6058 2024-04-13 08:46:20.890471 persona_ai-0.1.9/persona_ai/conversation_listeners/terminal_conversation_listener.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/conversations/__init__.py
+-rw-r--r--   0        0        0     3214 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/conversations/manager.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/domain/__init__.py
+-rw-r--r--   0        0        0     6372 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/domain/conversations.py
+-rw-r--r--   0        0        0      767 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/domain/events.py
+-rw-r--r--   0        0        0     1172 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/domain/repositories.py
+-rw-r--r--   0        0        0       82 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/domain/roles.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/domain/schemas/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/domain/schemas/crud.py
+-rw-r--r--   0        0        0     2759 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/domain/tasks.py
+-rw-r--r--   0        0        0      146 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/domain/utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/infrastructure/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      758 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/infrastructure/repositories/base.py
+-rw-r--r--   0        0        0     1967 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/infrastructure/repositories/in_memory.py
+-rw-r--r--   0        0        0     2884 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/infrastructure/repositories/mongo.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/initializers/__init__.py
+-rw-r--r--   0        0        0     4370 2024-04-13 09:19:31.924780 persona_ai-0.1.9/persona_ai/initializers/env_configurator.py
+-rw-r--r--   0        0        0     1012 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/initializers/persona_configuration.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/models/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/models/base.py
+-rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/models/code_bison.py
+-rw-r--r--   0        0        0    10057 2024-04-13 08:21:54.496495 persona_ai-0.1.9/persona_ai/models/gemini.py
+-rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/models/text_bison.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/moderation/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-13 08:48:32.646648 persona_ai-0.1.9/persona_ai/moderation/ai_moderator.py
+-rw-r--r--   0        0        0     7345 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/moderation/base.py
+-rw-r--r--   0        0        0     4478 2024-04-13 08:29:21.845098 persona_ai-0.1.9/persona_ai/moderation/history_moderator.py
+-rw-r--r--   0        0        0     4759 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/moderation/history_moderator_fc.py
+-rw-r--r--   0        0        0     5580 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/moderation/react_moderator.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/personas/__init__.py
+-rw-r--r--   0        0        0     6678 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/personas/agent.py
+-rw-r--r--   0        0        0     4221 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/personas/assistant.py
+-rw-r--r--   0        0        0     6504 2024-04-11 10:53:55.133342 persona_ai-0.1.9/persona_ai/personas/base.py
+-rw-r--r--   0        0        0     3805 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/personas/coder.py
+-rw-r--r--   0        0        0    13267 2024-04-11 11:05:25.442988 persona_ai-0.1.9/persona_ai/personas/party.py
+-rw-r--r--   0        0        0     3023 2024-04-11 14:30:55.936715 persona_ai-0.1.9/persona_ai/personas/technician.py
+-rw-r--r--   0        0        0      760 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/personas/terminal.py
+-rw-r--r--   0        0        0      860 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/prompt_templates/agent.jinja2
+-rw-r--r--   0        0        0      413 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/prompt_templates/assistant.jinja2
+-rw-r--r--   0        0        0     1009 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/prompt_templates/coder.jinja2
+-rw-r--r--   0        0        0     1194 2024-04-11 15:04:24.559375 persona_ai-0.1.9/persona_ai/prompt_templates/history_moderator.jinja2
+-rw-r--r--   0        0        0     1062 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/prompt_templates/history_moderator_fc.jinja2
+-rw-r--r--   0        0        0     1776 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/prompt_templates/react_json_moderator.jinja2
+-rw-r--r--   0        0        0     1083 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/prompt_templates/react_moderator.jinja2
+-rw-r--r--   0        0        0      330 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/prompt_templates/refiner.jinja2
+-rw-r--r--   0        0        0      946 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2
+-rw-r--r--   0        0        0      841 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2
+-rw-r--r--   0        0        0      102 2024-04-11 14:33:38.412861 persona_ai-0.1.9/persona_ai/prompt_templates/technician.jinja2
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/prompts/__init__.py
+-rw-r--r--   0        0        0      238 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/prompts/base.py
+-rw-r--r--   0        0        0     2207 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/prompts/jinja.py
+-rw-r--r--   0        0        0      588 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/prompts/text.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/refiners/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/refiners/request_refiner.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/task_manager/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/task_manager/base.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/tools/__init__.py
+-rw-r--r--   0        0        0      469 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/tools/base.py
+-rw-r--r--   0        0        0     1746 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/tools/functional.py
+-rw-r--r--   0        0        0      730 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/tools/manager.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/transport/__init__.py
+-rw-r--r--   0        0        0     3477 2024-04-11 13:57:49.665513 persona_ai-0.1.9/persona_ai/transport/local/local_messagebus.py
+-rw-r--r--   0        0        0     4022 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/transport/messagebus.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/transport/rabbitmq/__init__.py
+-rw-r--r--   0        0        0    10002 2024-04-11 10:00:15.400629 persona_ai-0.1.9/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/utils/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-08 06:52:52.049183 persona_ai-0.1.9/persona_ai/utils/crypto.py
+-rw-r--r--   0        0        0      911 2024-04-13 08:45:38.530414 persona_ai-0.1.9/persona_ai/utils/extractors.py
+-rw-r--r--   0        0        0     1164 2024-04-13 09:19:37.208799 persona_ai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    12749 1970-01-01 00:00:00.000000 persona_ai-0.1.9/PKG-INFO
```

### Comparing `persona_ai-0.1.8/README.md` & `persona_ai-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/code_runners/base.py` & `persona_ai-0.1.9/persona_ai/code_runners/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/code_runners/local.py` & `persona_ai-0.1.9/persona_ai/code_runners/local.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/conversation_listeners/terminal_conversation_listener.py` & `persona_ai-0.1.9/persona_ai/conversation_listeners/terminal_conversation_listener.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/conversations/manager.py` & `persona_ai-0.1.9/persona_ai/conversations/manager.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/domain/conversations.py` & `persona_ai-0.1.9/persona_ai/domain/conversations.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/domain/events.py` & `persona_ai-0.1.9/persona_ai/domain/events.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/domain/repositories.py` & `persona_ai-0.1.9/persona_ai/domain/repositories.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/domain/schemas/crud.py` & `persona_ai-0.1.9/persona_ai/domain/schemas/crud.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/domain/tasks.py` & `persona_ai-0.1.9/persona_ai/domain/tasks.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/infrastructure/repositories/base.py` & `persona_ai-0.1.9/persona_ai/infrastructure/repositories/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/infrastructure/repositories/in_memory.py` & `persona_ai-0.1.9/persona_ai/infrastructure/repositories/in_memory.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/infrastructure/repositories/mongo.py` & `persona_ai-0.1.9/persona_ai/infrastructure/repositories/mongo.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/initializers/env_configurator.py` & `persona_ai-0.1.9/persona_ai/initializers/env_configurator.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from persona_ai.transport.rabbitmq.rabbitmq_messagebus import RabbitMQMessageBus
 
 
 def configure_model(prefix: str):
     project_id = os.getenv("GOOGLE_CLOUD_PROJECT")
     default_location = os.getenv("GOOGLE_CLOUD_LOCATION", "us-central1")
 
-    model_name = os.getenv(f"{prefix}_MODEL_NAME", "gemini-pro")
+    model_name = os.getenv(f"{prefix}_MODEL_NAME", "gemini-1.0-pro-002")
     temperature = float(os.getenv(f"{prefix}_MODEL_TEMPERATURE", 0.0))
     max_output_tokens = int(os.getenv(f"{prefix}_MODEL_MAX_OUTPUT_TOKENS", 2048))
     location = os.getenv(f"{prefix}_MODEL_LOCATION", default_location)
 
     if "gemini" in model_name:
         return GeminiModel(
             model_name=model_name,
```

### Comparing `persona_ai-0.1.8/persona_ai/initializers/persona_configuration.py` & `persona_ai-0.1.9/persona_ai/initializers/persona_configuration.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/models/base.py` & `persona_ai-0.1.9/persona_ai/models/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/models/code_bison.py` & `persona_ai-0.1.9/persona_ai/models/code_bison.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/models/gemini.py` & `persona_ai-0.1.9/persona_ai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/models/text_bison.py` & `persona_ai-0.1.9/persona_ai/models/text_bison.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/moderation/ai_moderator.py` & `persona_ai-0.1.9/persona_ai/moderation/ai_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/moderation/base.py` & `persona_ai-0.1.9/persona_ai/moderation/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/moderation/history_moderator.py` & `persona_ai-0.1.9/persona_ai/moderation/history_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/moderation/history_moderator_fc.py` & `persona_ai-0.1.9/persona_ai/moderation/history_moderator_fc.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/moderation/react_moderator.py` & `persona_ai-0.1.9/persona_ai/moderation/react_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/personas/agent.py` & `persona_ai-0.1.9/persona_ai/personas/agent.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/personas/assistant.py` & `persona_ai-0.1.9/persona_ai/personas/assistant.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/personas/base.py` & `persona_ai-0.1.9/persona_ai/personas/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/personas/coder.py` & `persona_ai-0.1.9/persona_ai/personas/coder.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/personas/party.py` & `persona_ai-0.1.9/persona_ai/personas/party.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/personas/technician.py` & `persona_ai-0.1.9/persona_ai/personas/technician.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/personas/terminal.py` & `persona_ai-0.1.9/persona_ai/personas/terminal.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/prompt_templates/agent.jinja2` & `persona_ai-0.1.9/persona_ai/prompt_templates/agent.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/prompt_templates/coder.jinja2` & `persona_ai-0.1.9/persona_ai/prompt_templates/coder.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/prompt_templates/history_moderator.jinja2` & `persona_ai-0.1.9/persona_ai/prompt_templates/history_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/prompt_templates/history_moderator_fc.jinja2` & `persona_ai-0.1.9/persona_ai/prompt_templates/history_moderator_fc.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/prompt_templates/react_json_moderator.jinja2` & `persona_ai-0.1.9/persona_ai/prompt_templates/react_json_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/prompt_templates/react_moderator.jinja2` & `persona_ai-0.1.9/persona_ai/prompt_templates/react_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2` & `persona_ai-0.1.9/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2` & `persona_ai-0.1.9/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/prompts/jinja.py` & `persona_ai-0.1.9/persona_ai/prompts/jinja.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/prompts/text.py` & `persona_ai-0.1.9/persona_ai/prompts/text.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/refiners/request_refiner.py` & `persona_ai-0.1.9/persona_ai/refiners/request_refiner.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/task_manager/base.py` & `persona_ai-0.1.9/persona_ai/task_manager/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/tools/functional.py` & `persona_ai-0.1.9/persona_ai/tools/functional.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/tools/manager.py` & `persona_ai-0.1.9/persona_ai/tools/manager.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/transport/local/local_messagebus.py` & `persona_ai-0.1.9/persona_ai/transport/local/local_messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/transport/messagebus.py` & `persona_ai-0.1.9/persona_ai/transport/messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py` & `persona_ai-0.1.9/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/utils/crypto.py` & `persona_ai-0.1.9/persona_ai/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/persona_ai/utils/extractors.py` & `persona_ai-0.1.9/persona_ai/utils/extractors.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.8/pyproject.toml` & `persona_ai-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "persona_ai"
-version = "0.1.8"
+version = "0.1.9"
 description = "Persona is a groundbreaking distributed AI agent system utilizing Google Vertex AI's premier Large Language Models such as Gemini-pro, Text-Bison, and Code-Bison. Developed by Applica Software Guru, Persona is engineered for scalable, high-performance, and intelligent operations across various data sets and applications. It harnesses the power of Google's Vertex AI to deliver unmatched insights and automation capabilities, setting new standards in AI-driven analytics and decision-making processes"
 authors = ["Bruno Fortunato <bruno.fortunato@applica.guru>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `persona_ai-0.1.8/PKG-INFO` & `persona_ai-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persona_ai
-Version: 0.1.8
+Version: 0.1.9
 Summary: Persona is a groundbreaking distributed AI agent system utilizing Google Vertex AI's premier Large Language Models such as Gemini-pro, Text-Bison, and Code-Bison. Developed by Applica Software Guru, Persona is engineered for scalable, high-performance, and intelligent operations across various data sets and applications. It harnesses the power of Google's Vertex AI to deliver unmatched insights and automation capabilities, setting new standards in AI-driven analytics and decision-making processes
 License: MIT
 Author: Bruno Fortunato
 Author-email: bruno.fortunato@applica.guru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

