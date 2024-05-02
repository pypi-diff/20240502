# Comparing `tmp/g4f-0.3.0.7.tar.gz` & `tmp/g4f-0.3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.0.7.tar", last modified: Sun Apr 28 20:50:03 2024, max compression
+gzip compressed data, was "g4f-0.3.0.8.tar", last modified: Thu May  2 21:54:17 2024, max compression
```

## Comparing `g4f-0.3.0.7.tar` & `g4f-0.3.0.8.tar`

### file list

```diff
@@ -1,247 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.210319 g4f-0.3.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-28 20:49:59.000000 g4f-0.3.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-28 20:49:59.000000 g4f-0.3.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55397 2024-04-28 20:50:03.210319 g4f-0.3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    52201 2024-04-28 20:49:59.000000 g4f-0.3.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.170319 g4f-0.3.0.7/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.178319 g4f-0.3.0.7/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Reka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.178319 g4f-0.3.0.7/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.186319 g4f-0.3.0.7/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.186319 g4f-0.3.0.7/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.186319 g4f-0.3.0.7/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    33742 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/openai/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/openai/proofofwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.166319 g4f-0.3.0.7/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.198319 g4f-0.3.0.7/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22896 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.198319 g4f-0.3.0.7/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.198319 g4f-0.3.0.7/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    47420 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.198319 g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.202319 g4f-0.3.0.7/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.202319 g4f-0.3.0.7/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.202319 g4f-0.3.0.7/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.202319 g4f-0.3.0.7/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.202319 g4f-0.3.0.7/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.206319 g4f-0.3.0.7/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55397 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 20:50:03.210319 g4f-0.3.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-28 20:49:59.000000 g4f-0.3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.091830 g4f-0.3.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-02 21:54:13.000000 g4f-0.3.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 21:54:13.000000 g4f-0.3.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55611 2024-05-02 21:54:17.091830 g4f-0.3.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    52415 2024-05-02 21:54:13.000000 g4f-0.3.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.059831 g4f-0.3.0.8/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.067830 g4f-0.3.0.8/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Reka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.067830 g4f-0.3.0.8/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.071830 g4f-0.3.0.8/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.071830 g4f-0.3.0.8/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33742 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/openai/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/openai/proofofwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.055830 g4f-0.3.0.8/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22896 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.083830 g4f-0.3.0.8/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.083830 g4f-0.3.0.8/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    47420 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.083830 g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55611 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:54:17.091830 g4f-0.3.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-02 21:54:13.000000 g4f-0.3.0.8/setup.py
```

### Comparing `g4f-0.3.0.7/LICENSE` & `g4f-0.3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/PKG-INFO` & `g4f-0.3.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.7
+Version: 0.3.0.8
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -492,25 +492,23 @@
 | Meta AI | `g4f.Provider.MetaAI` | ✔️ | ❌ | [meta.ai](https://www.meta.ai) |
 | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
 | Reka | `g4f.Provider.Reka` | ❌ | ✔️ | [chat.reka.ai](https://chat.reka.ai/) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e-3| ✔️ | [you.com](https://you.com) |
 
 ```python
+import requests
 from g4f.client import Client
-from g4f.Provider.GeminiPro import GeminiPro
 
-client = Client(
-    api_key="...",
-    provider=GeminiPro
-)
+client = Client()
+image = requests.get("https://change_me.jpg", stream=True).raw
 response = client.chat.completions.create(
-    model="gemini-pro-vision",
-    messages=[{"role": "user", "content": "What are on this image?"}],
-    image=open("docs/waterfall.jpeg", "rb")
+    "",
+    messages=[{"role": "user", "content": "what is in this picture?"}],
+    image=image
 )
 print(response.choices[0].message.content)
 ```
 
 ## 🔗 Powered by gpt4free
 
 <table>
@@ -935,47 +933,49 @@
 <a href="https://github.com/hlohaus" target="_blank"><img src="https://avatars.githubusercontent.com/u/983577?v=4&s=45" width="45" title="hlohaus"></a>
 <a href="https://github.com/bagusindrayana" target="_blank"><img src="https://avatars.githubusercontent.com/u/36830534?v=4&s=45" width="45" title="bagusindrayana"></a>
 <a href="https://github.com/sudouser777" target="_blank"><img src="https://avatars.githubusercontent.com/u/22415463?v=4&s=45" width="45" title="sudouser777"></a>
 <a href="https://github.com/thatlukinhasguy1" target="_blank"><img src="https://avatars.githubusercontent.com/u/139662282?v=4&s=45" width="45" title="thatlukinhasguy1"></a>
 <a href="https://github.com/Commenter123321" target="_blank"><img src="https://avatars.githubusercontent.com/u/36051603?v=4&s=45" width="45" title="Commenter123321"></a>
 <a href="https://github.com/DanielShemesh" target="_blank"><img src="https://avatars.githubusercontent.com/u/20585236?v=4&s=45" width="45" title="DanielShemesh"></a>
 <a href="https://github.com/Luneye" target="_blank"><img src="https://avatars.githubusercontent.com/u/73485421?v=4&s=45" width="45" title="Luneye"></a>
-<a href="https://github.com/enganese" target="_blank"><img src="https://avatars.githubusercontent.com/u/69082498?v=4&s=45" width="45" title="enganese"></a>
 <a href="https://github.com/ezerinz" target="_blank"><img src="https://avatars.githubusercontent.com/u/100193740?v=4&s=45" width="45" title="ezerinz"></a>
+<a href="https://github.com/enganese" target="_blank"><img src="https://avatars.githubusercontent.com/u/69082498?v=4&s=45" width="45" title="enganese"></a>
 <a href="https://github.com/Lin-jun-xiang" target="_blank"><img src="https://avatars.githubusercontent.com/u/63782903?v=4&s=45" width="45" title="Lin-jun-xiang"></a>
 <a href="https://github.com/nullstreak" target="_blank"><img src="https://avatars.githubusercontent.com/u/139914347?v=4&s=45" width="45" title="nullstreak"></a>
 <a href="https://github.com/valerii-chirkov" target="_blank"><img src="https://avatars.githubusercontent.com/u/81074936?v=4&s=45" width="45" title="valerii-chirkov"></a>
 <a href="https://github.com/MIDORIBIN" target="_blank"><img src="https://avatars.githubusercontent.com/u/25425217?v=4&s=45" width="45" title="MIDORIBIN"></a>
 <a href="https://github.com/repollo" target="_blank"><img src="https://avatars.githubusercontent.com/u/2671466?v=4&s=45" width="45" title="repollo"></a>
 <a href="https://github.com/hpsj" target="_blank"><img src="https://avatars.githubusercontent.com/u/54535414?v=4&s=45" width="45" title="hpsj"></a>
 <a href="https://github.com/taiyi747" target="_blank"><img src="https://avatars.githubusercontent.com/u/63543716?v=4&s=45" width="45" title="taiyi747"></a>
-<a href="https://github.com/ostix360" target="_blank"><img src="https://avatars.githubusercontent.com/u/55257054?v=4&s=45" width="45" title="ostix360"></a>
-<a href="https://github.com/WdR-Tech" target="_blank"><img src="https://avatars.githubusercontent.com/u/143020293?v=4&s=45" width="45" title="WdR-Tech"></a>
-<a href="https://github.com/HexyeDEV" target="_blank"><img src="https://avatars.githubusercontent.com/u/65314629?v=4&s=45" width="45" title="HexyeDEV"></a>
 <a href="https://github.com/9fo" target="_blank"><img src="https://avatars.githubusercontent.com/u/71867245?v=4&s=45" width="45" title="9fo"></a>
-<a href="https://github.com/eltociear" target="_blank"><img src="https://avatars.githubusercontent.com/u/22633385?v=4&s=45" width="45" title="eltociear"></a>
-<a href="https://github.com/ramonvc" target="_blank"><img src="https://avatars.githubusercontent.com/u/13617054?v=4&s=45" width="45" title="ramonvc"></a>
-<a href="https://github.com/naa7" target="_blank"><img src="https://avatars.githubusercontent.com/u/44613678?v=4&s=45" width="45" title="naa7"></a>
-<a href="https://github.com/zeng-rr" target="_blank"><img src="https://avatars.githubusercontent.com/u/47846202?v=4&s=45" width="45" title="zeng-rr"></a>
-<a href="https://github.com/editor-syntax" target="_blank"><img src="https://avatars.githubusercontent.com/u/109844019?v=4&s=45" width="45" title="editor-syntax"></a>
+<a href="https://github.com/HexyeDEV" target="_blank"><img src="https://avatars.githubusercontent.com/u/65314629?v=4&s=45" width="45" title="HexyeDEV"></a>
+<a href="https://github.com/WdR-Tech" target="_blank"><img src="https://avatars.githubusercontent.com/u/143020293?v=4&s=45" width="45" title="WdR-Tech"></a>
+<a href="https://github.com/ostix360" target="_blank"><img src="https://avatars.githubusercontent.com/u/55257054?v=4&s=45" width="45" title="ostix360"></a>
 <a href="https://github.com/devAdityaa" target="_blank"><img src="https://avatars.githubusercontent.com/u/77636021?v=4&s=45" width="45" title="devAdityaa"></a>
+<a href="https://github.com/editor-syntax" target="_blank"><img src="https://avatars.githubusercontent.com/u/109844019?v=4&s=45" width="45" title="editor-syntax"></a>
+<a href="https://github.com/zeng-rr" target="_blank"><img src="https://avatars.githubusercontent.com/u/47846202?v=4&s=45" width="45" title="zeng-rr"></a>
+<a href="https://github.com/naa7" target="_blank"><img src="https://avatars.githubusercontent.com/u/44613678?v=4&s=45" width="45" title="naa7"></a>
+<a href="https://github.com/ramonvc" target="_blank"><img src="https://avatars.githubusercontent.com/u/13617054?v=4&s=45" width="45" title="ramonvc"></a>
+<a href="https://github.com/eltociear" target="_blank"><img src="https://avatars.githubusercontent.com/u/22633385?v=4&s=45" width="45" title="eltociear"></a>
 <a href="https://github.com/kggn" target="_blank"><img src="https://avatars.githubusercontent.com/u/95663228?v=4&s=45" width="45" title="kggn"></a>
 <a href="https://github.com/xiangsx" target="_blank"><img src="https://avatars.githubusercontent.com/u/29322721?v=4&s=45" width="45" title="xiangsx"></a>
 <a href="https://github.com/ggindinson" target="_blank"><img src="https://avatars.githubusercontent.com/u/97807772?v=4&s=45" width="45" title="ggindinson"></a>
 <span></span>
 <img src="https://avatars.githubusercontent.com/u/71154407?s=45&v=4" width="45" title="ading2210">
 <img src="https://avatars.githubusercontent.com/u/12299238?s=45&v=4" width="45" title="xqdoo00o">
 <img src="https://avatars.githubusercontent.com/u/97126670?s=45&v=4" width="45" title="nathanrchn">
 <img src="https://avatars.githubusercontent.com/u/81407603?v=4&s=45" width="45" title="dsdanielpark">
+<img src="https://avatars.githubusercontent.com/u/55200481?v=4&s=45" width="45" title="missuo">
 
 - The [`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
 - The [`har_file.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
 - The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
 - The [`Gemini.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
 - The [`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm)
+- The [`proofofwork.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/proofofwork.py) has input from [missuo/FreeGPT35](https://github.com/missuo/FreeGPT35)
 
 *Having input implies that the AI's code generation utilized it as one of many sources.*
 
 ## ©️ Copyright
 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.7 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.8 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -387,20 +387,19 @@
 | `g4f.Provider.GeminiPro` | â | gemini-1.5-pro | [ai.google.dev](https://
 ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | âï¸ | â | [meta.ai]
 (https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
 3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Reka |
 `g4f.Provider.Reka` | â | âï¸ | [chat.reka.ai](https://chat.reka.ai/) | |
 Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b |
 [replicate.com](https://replicate.com) | | You.com | `g4f.Provider.You` | dall-
-e-3| âï¸ | [you.com](https://you.com) | ```python from g4f.client import
-Client from g4f.Provider.GeminiPro import GeminiPro client = Client
-( api_key="...", provider=GeminiPro ) response = client.chat.completions.create
-( model="gemini-pro-vision", messages=[{"role": "user", "content": "What are on
-this image?"}], image=open("docs/waterfall.jpeg", "rb") ) print
-(response.choices[0].message.content) ``` ## ð Powered by gpt4free
+e-3| âï¸ | [you.com](https://you.com) | ```python import requests from
+g4f.client import Client client = Client() image = requests.get("https://
+change_me.jpg", stream=True).raw response = client.chat.completions.create( "",
+messages=[{"role": "user", "content": "what is in this picture?"}], image=image
+) print(response.choices[0].message.content) ``` ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
@@ -427,64 +426,67 @@
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_3_5_7_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_8_3_0_5_3_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_4_1_5_4_6_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_6_6_2_2_8_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_0_5_1_6_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_0_5_8_5_2_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_3_4_8_5_4_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_9_0_8_2_4_9_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_0_1_9_3_7_4_0_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_9_0_8_2_4_9_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_7_8_2_9_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_9_1_4_3_4_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_8_1_0_7_4_9_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_5_4_2_5_2_1_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_6_7_1_4_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_4_5_3_5_4_1_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_5_4_3_7_1_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_5_2_5_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_4_3_0_2_0_2_9_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_5_3_1_4_6_2_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_1_8_6_7_2_4_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_6_3_3_3_8_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_6_1_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_4_6_1_3_6_7_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_7_8_4_6_2_0_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_9_8_4_4_0_1_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_5_3_1_4_6_2_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_4_3_0_2_0_2_9_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_5_2_5_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_7_6_3_6_0_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_9_8_4_4_0_1_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_7_8_4_6_2_0_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_4_6_1_3_6_7_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_6_1_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_6_3_3_3_8_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_5_6_6_3_2_2_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_9_3_2_2_7_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_7_8_0_7_7_7_2_?_v_=_4_&_s_=_4_5_][https://
 avatars.githubusercontent.com/u/71154407?s=45&v=4][https://
 avatars.githubusercontent.com/u/12299238?s=45&v=4][https://
 avatars.githubusercontent.com/u/97126670?s=45&v=4][https://
-avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](https://
+avatars.githubusercontent.com/u/81407603?v=4&s=45][https://
+avatars.githubusercontent.com/u/55200481?v=4&s=45]- The [`Vercel.py`](https://
 github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code
 from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by
 [@ading2210](https://github.com/ading2210) - The [`har_file.py`](https://
 github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input
 from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API) -
 The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/
 Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://
 github.com/nathanrchn/perplexityai) - The [`Gemini.py`](https://github.com/
 xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from
 [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API) - The
 [`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/
 MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-
-ai-api) by [@Strvm](https://github.com/Strvm) *Having input implies that the
-AI's code generation utilized it as one of many sources.* ## Â©ï¸ Copyright
-This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/
-gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This program is
-free software: you can redistribute it and/or modify it under the terms of the
-GNU General Public License as published by the Free Software Foundation, either
-version 3 of the License, or (at your option) any later version. This program
-is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
-without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE. See the GNU General Public License for more details. You
-should have received a copy of the GNU General Public License along with this
-program. If not, see
+ai-api) by [@Strvm](https://github.com/Strvm) - The [`proofofwork.py`](https://
+github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/proofofwork.py) has
+input from [missuo/FreeGPT35](https://github.com/missuo/FreeGPT35) *Having
+input implies that the AI's code generation utilized it as one of many
+sources.* ## Â©ï¸ Copyright This program is licensed under the [GNU GPL v3]
+(https://www.gnu.org/licenses/gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C)
+2023 xtekky This program is free software: you can redistribute it and/or
+modify it under the terms of the GNU General Public License as published by the
+Free Software Foundation, either version 3 of the License, or (at your option)
+any later version. This program is distributed in the hope that it will be
+useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
+License for more details. You should have received a copy of the GNU General
+Public License along with this program. If not, see
 www.gnu.org/licenses/>. ``` ## â­ Star History _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]## ð
 License
 [https://upload.wikimedia.org/wikipedia/ [https://img.shields.io/badge/License-
    commons/thumb/9/93/GPLv3_Logo.svg/    GNU_GPL_v3.0-red.svg]
        1200px-GPLv3_Logo.svg.png]        This project is licensed under
                                          _G_N_U___G_P_L___v_3_._0.
                                                              (_ð___¼_ _B_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `g4f-0.3.0.7/README.md` & `g4f-0.3.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -414,25 +414,23 @@
 | Meta AI | `g4f.Provider.MetaAI` | ✔️ | ❌ | [meta.ai](https://www.meta.ai) |
 | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
 | Reka | `g4f.Provider.Reka` | ❌ | ✔️ | [chat.reka.ai](https://chat.reka.ai/) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e-3| ✔️ | [you.com](https://you.com) |
 
 ```python
+import requests
 from g4f.client import Client
-from g4f.Provider.GeminiPro import GeminiPro
 
-client = Client(
-    api_key="...",
-    provider=GeminiPro
-)
+client = Client()
+image = requests.get("https://change_me.jpg", stream=True).raw
 response = client.chat.completions.create(
-    model="gemini-pro-vision",
-    messages=[{"role": "user", "content": "What are on this image?"}],
-    image=open("docs/waterfall.jpeg", "rb")
+    "",
+    messages=[{"role": "user", "content": "what is in this picture?"}],
+    image=image
 )
 print(response.choices[0].message.content)
 ```
 
 ## 🔗 Powered by gpt4free
 
 <table>
@@ -857,47 +855,49 @@
 <a href="https://github.com/hlohaus" target="_blank"><img src="https://avatars.githubusercontent.com/u/983577?v=4&s=45" width="45" title="hlohaus"></a>
 <a href="https://github.com/bagusindrayana" target="_blank"><img src="https://avatars.githubusercontent.com/u/36830534?v=4&s=45" width="45" title="bagusindrayana"></a>
 <a href="https://github.com/sudouser777" target="_blank"><img src="https://avatars.githubusercontent.com/u/22415463?v=4&s=45" width="45" title="sudouser777"></a>
 <a href="https://github.com/thatlukinhasguy1" target="_blank"><img src="https://avatars.githubusercontent.com/u/139662282?v=4&s=45" width="45" title="thatlukinhasguy1"></a>
 <a href="https://github.com/Commenter123321" target="_blank"><img src="https://avatars.githubusercontent.com/u/36051603?v=4&s=45" width="45" title="Commenter123321"></a>
 <a href="https://github.com/DanielShemesh" target="_blank"><img src="https://avatars.githubusercontent.com/u/20585236?v=4&s=45" width="45" title="DanielShemesh"></a>
 <a href="https://github.com/Luneye" target="_blank"><img src="https://avatars.githubusercontent.com/u/73485421?v=4&s=45" width="45" title="Luneye"></a>
-<a href="https://github.com/enganese" target="_blank"><img src="https://avatars.githubusercontent.com/u/69082498?v=4&s=45" width="45" title="enganese"></a>
 <a href="https://github.com/ezerinz" target="_blank"><img src="https://avatars.githubusercontent.com/u/100193740?v=4&s=45" width="45" title="ezerinz"></a>
+<a href="https://github.com/enganese" target="_blank"><img src="https://avatars.githubusercontent.com/u/69082498?v=4&s=45" width="45" title="enganese"></a>
 <a href="https://github.com/Lin-jun-xiang" target="_blank"><img src="https://avatars.githubusercontent.com/u/63782903?v=4&s=45" width="45" title="Lin-jun-xiang"></a>
 <a href="https://github.com/nullstreak" target="_blank"><img src="https://avatars.githubusercontent.com/u/139914347?v=4&s=45" width="45" title="nullstreak"></a>
 <a href="https://github.com/valerii-chirkov" target="_blank"><img src="https://avatars.githubusercontent.com/u/81074936?v=4&s=45" width="45" title="valerii-chirkov"></a>
 <a href="https://github.com/MIDORIBIN" target="_blank"><img src="https://avatars.githubusercontent.com/u/25425217?v=4&s=45" width="45" title="MIDORIBIN"></a>
 <a href="https://github.com/repollo" target="_blank"><img src="https://avatars.githubusercontent.com/u/2671466?v=4&s=45" width="45" title="repollo"></a>
 <a href="https://github.com/hpsj" target="_blank"><img src="https://avatars.githubusercontent.com/u/54535414?v=4&s=45" width="45" title="hpsj"></a>
 <a href="https://github.com/taiyi747" target="_blank"><img src="https://avatars.githubusercontent.com/u/63543716?v=4&s=45" width="45" title="taiyi747"></a>
-<a href="https://github.com/ostix360" target="_blank"><img src="https://avatars.githubusercontent.com/u/55257054?v=4&s=45" width="45" title="ostix360"></a>
-<a href="https://github.com/WdR-Tech" target="_blank"><img src="https://avatars.githubusercontent.com/u/143020293?v=4&s=45" width="45" title="WdR-Tech"></a>
-<a href="https://github.com/HexyeDEV" target="_blank"><img src="https://avatars.githubusercontent.com/u/65314629?v=4&s=45" width="45" title="HexyeDEV"></a>
 <a href="https://github.com/9fo" target="_blank"><img src="https://avatars.githubusercontent.com/u/71867245?v=4&s=45" width="45" title="9fo"></a>
-<a href="https://github.com/eltociear" target="_blank"><img src="https://avatars.githubusercontent.com/u/22633385?v=4&s=45" width="45" title="eltociear"></a>
-<a href="https://github.com/ramonvc" target="_blank"><img src="https://avatars.githubusercontent.com/u/13617054?v=4&s=45" width="45" title="ramonvc"></a>
-<a href="https://github.com/naa7" target="_blank"><img src="https://avatars.githubusercontent.com/u/44613678?v=4&s=45" width="45" title="naa7"></a>
-<a href="https://github.com/zeng-rr" target="_blank"><img src="https://avatars.githubusercontent.com/u/47846202?v=4&s=45" width="45" title="zeng-rr"></a>
-<a href="https://github.com/editor-syntax" target="_blank"><img src="https://avatars.githubusercontent.com/u/109844019?v=4&s=45" width="45" title="editor-syntax"></a>
+<a href="https://github.com/HexyeDEV" target="_blank"><img src="https://avatars.githubusercontent.com/u/65314629?v=4&s=45" width="45" title="HexyeDEV"></a>
+<a href="https://github.com/WdR-Tech" target="_blank"><img src="https://avatars.githubusercontent.com/u/143020293?v=4&s=45" width="45" title="WdR-Tech"></a>
+<a href="https://github.com/ostix360" target="_blank"><img src="https://avatars.githubusercontent.com/u/55257054?v=4&s=45" width="45" title="ostix360"></a>
 <a href="https://github.com/devAdityaa" target="_blank"><img src="https://avatars.githubusercontent.com/u/77636021?v=4&s=45" width="45" title="devAdityaa"></a>
+<a href="https://github.com/editor-syntax" target="_blank"><img src="https://avatars.githubusercontent.com/u/109844019?v=4&s=45" width="45" title="editor-syntax"></a>
+<a href="https://github.com/zeng-rr" target="_blank"><img src="https://avatars.githubusercontent.com/u/47846202?v=4&s=45" width="45" title="zeng-rr"></a>
+<a href="https://github.com/naa7" target="_blank"><img src="https://avatars.githubusercontent.com/u/44613678?v=4&s=45" width="45" title="naa7"></a>
+<a href="https://github.com/ramonvc" target="_blank"><img src="https://avatars.githubusercontent.com/u/13617054?v=4&s=45" width="45" title="ramonvc"></a>
+<a href="https://github.com/eltociear" target="_blank"><img src="https://avatars.githubusercontent.com/u/22633385?v=4&s=45" width="45" title="eltociear"></a>
 <a href="https://github.com/kggn" target="_blank"><img src="https://avatars.githubusercontent.com/u/95663228?v=4&s=45" width="45" title="kggn"></a>
 <a href="https://github.com/xiangsx" target="_blank"><img src="https://avatars.githubusercontent.com/u/29322721?v=4&s=45" width="45" title="xiangsx"></a>
 <a href="https://github.com/ggindinson" target="_blank"><img src="https://avatars.githubusercontent.com/u/97807772?v=4&s=45" width="45" title="ggindinson"></a>
 <span></span>
 <img src="https://avatars.githubusercontent.com/u/71154407?s=45&v=4" width="45" title="ading2210">
 <img src="https://avatars.githubusercontent.com/u/12299238?s=45&v=4" width="45" title="xqdoo00o">
 <img src="https://avatars.githubusercontent.com/u/97126670?s=45&v=4" width="45" title="nathanrchn">
 <img src="https://avatars.githubusercontent.com/u/81407603?v=4&s=45" width="45" title="dsdanielpark">
+<img src="https://avatars.githubusercontent.com/u/55200481?v=4&s=45" width="45" title="missuo">
 
 - The [`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
 - The [`har_file.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
 - The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
 - The [`Gemini.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
 - The [`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm)
+- The [`proofofwork.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/proofofwork.py) has input from [missuo/FreeGPT35](https://github.com/missuo/FreeGPT35)
 
 *Having input implies that the AI's code generation utilized it as one of many sources.*
 
 ## ©️ Copyright
 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
```

#### html2text {}

```diff
@@ -345,20 +345,19 @@
 | `g4f.Provider.GeminiPro` | â | gemini-1.5-pro | [ai.google.dev](https://
 ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | âï¸ | â | [meta.ai]
 (https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
 3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Reka |
 `g4f.Provider.Reka` | â | âï¸ | [chat.reka.ai](https://chat.reka.ai/) | |
 Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b |
 [replicate.com](https://replicate.com) | | You.com | `g4f.Provider.You` | dall-
-e-3| âï¸ | [you.com](https://you.com) | ```python from g4f.client import
-Client from g4f.Provider.GeminiPro import GeminiPro client = Client
-( api_key="...", provider=GeminiPro ) response = client.chat.completions.create
-( model="gemini-pro-vision", messages=[{"role": "user", "content": "What are on
-this image?"}], image=open("docs/waterfall.jpeg", "rb") ) print
-(response.choices[0].message.content) ``` ## ð Powered by gpt4free
+e-3| âï¸ | [you.com](https://you.com) | ```python import requests from
+g4f.client import Client client = Client() image = requests.get("https://
+change_me.jpg", stream=True).raw response = client.chat.completions.create( "",
+messages=[{"role": "user", "content": "what is in this picture?"}], image=image
+) print(response.choices[0].message.content) ``` ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
@@ -385,64 +384,67 @@
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_3_5_7_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_8_3_0_5_3_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_4_1_5_4_6_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_6_6_2_2_8_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_0_5_1_6_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_0_5_8_5_2_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_3_4_8_5_4_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_9_0_8_2_4_9_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_0_1_9_3_7_4_0_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_9_0_8_2_4_9_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_7_8_2_9_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_9_1_4_3_4_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_8_1_0_7_4_9_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_5_4_2_5_2_1_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_6_7_1_4_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_4_5_3_5_4_1_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_5_4_3_7_1_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_5_2_5_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_4_3_0_2_0_2_9_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_5_3_1_4_6_2_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_1_8_6_7_2_4_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_6_3_3_3_8_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_6_1_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_4_6_1_3_6_7_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_7_8_4_6_2_0_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_9_8_4_4_0_1_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_5_3_1_4_6_2_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_4_3_0_2_0_2_9_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_5_2_5_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_7_6_3_6_0_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_9_8_4_4_0_1_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_7_8_4_6_2_0_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_4_6_1_3_6_7_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_6_1_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_6_3_3_3_8_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_5_6_6_3_2_2_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_9_3_2_2_7_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_7_8_0_7_7_7_2_?_v_=_4_&_s_=_4_5_][https://
 avatars.githubusercontent.com/u/71154407?s=45&v=4][https://
 avatars.githubusercontent.com/u/12299238?s=45&v=4][https://
 avatars.githubusercontent.com/u/97126670?s=45&v=4][https://
-avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](https://
+avatars.githubusercontent.com/u/81407603?v=4&s=45][https://
+avatars.githubusercontent.com/u/55200481?v=4&s=45]- The [`Vercel.py`](https://
 github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code
 from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by
 [@ading2210](https://github.com/ading2210) - The [`har_file.py`](https://
 github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input
 from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API) -
 The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/
 Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://
 github.com/nathanrchn/perplexityai) - The [`Gemini.py`](https://github.com/
 xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from
 [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API) - The
 [`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/
 MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-
-ai-api) by [@Strvm](https://github.com/Strvm) *Having input implies that the
-AI's code generation utilized it as one of many sources.* ## Â©ï¸ Copyright
-This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/
-gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This program is
-free software: you can redistribute it and/or modify it under the terms of the
-GNU General Public License as published by the Free Software Foundation, either
-version 3 of the License, or (at your option) any later version. This program
-is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
-without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE. See the GNU General Public License for more details. You
-should have received a copy of the GNU General Public License along with this
-program. If not, see
+ai-api) by [@Strvm](https://github.com/Strvm) - The [`proofofwork.py`](https://
+github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/proofofwork.py) has
+input from [missuo/FreeGPT35](https://github.com/missuo/FreeGPT35) *Having
+input implies that the AI's code generation utilized it as one of many
+sources.* ## Â©ï¸ Copyright This program is licensed under the [GNU GPL v3]
+(https://www.gnu.org/licenses/gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C)
+2023 xtekky This program is free software: you can redistribute it and/or
+modify it under the terms of the GNU General Public License as published by the
+Free Software Foundation, either version 3 of the License, or (at your option)
+any later version. This program is distributed in the hope that it will be
+useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
+License for more details. You should have received a copy of the GNU General
+Public License along with this program. If not, see
 www.gnu.org/licenses/>. ``` ## â­ Star History _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]## ð
 License
 [https://upload.wikimedia.org/wikipedia/ [https://img.shields.io/badge/License-
    commons/thumb/9/93/GPLv3_Logo.svg/    GNU_GPL_v3.0-red.svg]
        1200px-GPLv3_Logo.svg.png]        This project is licensed under
                                          _G_N_U___G_P_L___v_3_._0.
                                                              (_ð___¼_ _B_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `g4f-0.3.0.7/g4f/Provider/Aichatos.py` & `g4f-0.3.0.8/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Aura.py` & `g4f-0.3.0.8/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Bing.py` & `g4f-0.3.0.8/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/BingCreateImages.py` & `g4f-0.3.0.8/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Blackbox.py` & `g4f-0.3.0.8/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/ChatForAi.py` & `g4f-0.3.0.8/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.0.8/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/ChatgptAi.py` & `g4f-0.3.0.8/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/ChatgptFree.py` & `g4f-0.3.0.8/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/ChatgptNext.py` & `g4f-0.3.0.8/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/ChatgptX.py` & `g4f-0.3.0.8/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Cnote.py` & `g4f-0.3.0.8/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Cohere.py` & `g4f-0.3.0.8/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/DeepInfra.py` & `g4f-0.3.0.8/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.0.8/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.0.8/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Ecosia.py` & `g4f-0.3.0.8/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Feedough.py` & `g4f-0.3.0.8/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/FlowGpt.py` & `g4f-0.3.0.8/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.0.8/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/FreeGpt.py` & `g4f-0.3.0.8/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/GeminiPro.py` & `g4f-0.3.0.8/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/GeminiProChat.py` & `g4f-0.3.0.8/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/GigaChat.py` & `g4f-0.3.0.8/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/GptTalkRu.py` & `g4f-0.3.0.8/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/HuggingChat.py` & `g4f-0.3.0.8/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/HuggingFace.py` & `g4f-0.3.0.8/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Koala.py` & `g4f-0.3.0.8/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Liaobots.py` & `g4f-0.3.0.8/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Llama.py` & `g4f-0.3.0.8/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Local.py` & `g4f-0.3.0.8/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/MetaAI.py` & `g4f-0.3.0.8/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.0.8/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.0.8/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Pi.py` & `g4f-0.3.0.8/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Reka.py` & `g4f-0.3.0.8/g4f/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Replicate.py` & `g4f-0.3.0.8/g4f/Provider/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/ReplicateImage.py` & `g4f-0.3.0.8/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/Vercel.py` & `g4f-0.3.0.8/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.0.8/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/You.py` & `g4f-0.3.0.8/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/__init__.py` & `g4f-0.3.0.8/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/bing/conversation.py` & `g4f-0.3.0.8/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/bing/create_images.py` & `g4f-0.3.0.8/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/bing/upload_image.py` & `g4f-0.3.0.8/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/V50.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.0.8/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.0.8/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.0.8/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.0.8/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.0.8/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.0.8/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.0.8/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.0.8/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.0.8/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.0.8/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.0.8/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.0.8/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.0.8/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.0.8/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.0.8/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.0.8/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.0.8/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.0.8/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.0.8/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.0.8/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.0.8/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.0.8/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.0.8/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.0.8/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.0.8/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.0.8/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/npm/package-lock.json` & `g4f-0.3.0.8/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/openai/crypt.py` & `g4f-0.3.0.8/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/openai/har_file.py` & `g4f-0.3.0.8/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/openai/proofofwork.py` & `g4f-0.3.0.8/g4f/Provider/openai/proofofwork.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.0.8/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/selenium/Bard.py` & `g4f-0.3.0.8/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.0.8/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.0.8/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/selenium/Phind.py` & `g4f-0.3.0.8/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.0.8/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.0.8/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.0.8/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.0.8/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.0.8/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/Provider/you/har_file.py` & `g4f-0.3.0.8/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/__init__.py` & `g4f-0.3.0.8/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/api/__init__.py` & `g4f-0.3.0.8/g4f/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,80 +15,93 @@
 from pydantic import BaseModel
 from typing import Union, Optional
 
 import g4f
 import g4f.debug
 from g4f.client import AsyncClient
 from g4f.typing import Messages
+from g4f.cookies import read_cookie_files
 
-def create_app(g4f_api_key:str = None):
+def create_app():
     app = FastAPI()
-    api = Api(app, g4f_api_key=g4f_api_key)
+    api = Api(app)
     api.register_routes()
     api.register_authorization()
     api.register_validation_exception_handler()
+    if not AppConfig.ignore_cookie_files:
+        read_cookie_files()
     return app
 
-class ChatCompletionsConfig(BaseModel):
+def create_app_debug():
+    g4f.debug.logging = True
+    return create_app()
+
+class ChatCompletionsForm(BaseModel):
     messages: Messages
     model: str
     provider: Optional[str] = None
     stream: bool = False
     temperature: Optional[float] = None
     max_tokens: Optional[int] = None
     stop: Union[list[str], str, None] = None
     api_key: Optional[str] = None
     web_search: Optional[bool] = None
     proxy: Optional[str] = None
 
-list_ignored_providers: list[str] = None
-
-def set_list_ignored_providers(ignored: list[str]):
-    global list_ignored_providers
-    list_ignored_providers = ignored
+class AppConfig():
+    list_ignored_providers: Optional[list[str]] = None
+    g4f_api_key: Optional[str] = None
+    ignore_cookie_files: bool = False
+
+    @classmethod
+    def set_list_ignored_providers(cls, ignored: list[str]):
+        cls.list_ignored_providers = ignored
+
+    @classmethod
+    def set_g4f_api_key(cls, key: str = None):
+        cls.g4f_api_key = key
+
+    @classmethod
+    def set_ignore_cookie_files(cls, value: bool):
+        cls.ignore_cookie_files = value
 
 class Api:
-    def __init__(self, app: FastAPI, g4f_api_key=None) -> None:
+    def __init__(self, app: FastAPI) -> None:
         self.app = app
         self.client = AsyncClient()
-        self.g4f_api_key = g4f_api_key
         self.get_g4f_api_key = APIKeyHeader(name="g4f-api-key")
 
     def register_authorization(self):
         @self.app.middleware("http")
         async def authorization(request: Request, call_next):
-            if self.g4f_api_key and request.url.path in ["/v1/chat/completions", "/v1/completions"]:
+            if AppConfig.g4f_api_key and request.url.path in ["/v1/chat/completions", "/v1/completions"]:
                 try:
                     user_g4f_api_key = await self.get_g4f_api_key(request)
                 except HTTPException as e:
                     if e.status_code == 403:
                         return JSONResponse(
                             status_code=HTTP_401_UNAUTHORIZED,
                             content=jsonable_encoder({"detail": "G4F API key required"}),
                         )
-                if not secrets.compare_digest(self.g4f_api_key, user_g4f_api_key):
+                if not secrets.compare_digest(AppConfig.g4f_api_key, user_g4f_api_key):
                     return JSONResponse(
-                    status_code=HTTP_403_FORBIDDEN,
-                    content=jsonable_encoder({"detail": "Invalid G4F API key"}),
-                )
-            
-            response = await call_next(request)
-            return response
+                        status_code=HTTP_403_FORBIDDEN,
+                        content=jsonable_encoder({"detail": "Invalid G4F API key"}),
+                    )
+            return await call_next(request)
 
     def register_validation_exception_handler(self):
         @self.app.exception_handler(RequestValidationError)
         async def validation_exception_handler(request: Request, exc: RequestValidationError):
             details = exc.errors()
-            modified_details = []
-            for error in details:
-                modified_details.append({
-                    "loc": error["loc"],
-                    "message": error["msg"],
-                    "type": error["type"],
-                })
+            modified_details = [{
+                "loc": error["loc"],
+                "message": error["msg"],
+                "type": error["type"],
+            } for error in details]
             return JSONResponse(
                 status_code=HTTP_422_UNPROCESSABLE_ENTITY,
                 content=jsonable_encoder({"detail": modified_details}),
             )
 
     def register_routes(self):
         @self.app.get("/")
@@ -99,18 +112,18 @@
         async def read_root_v1():
             return HTMLResponse('g4f API: Go to '
                                 '<a href="/v1/chat/completions">chat/completions</a> '
                                 'or <a href="/v1/models">models</a>.')
 
         @self.app.get("/v1/models")
         async def models():
-            model_list = dict(
-                (model, g4f.models.ModelUtils.convert[model])
+            model_list = {
+                model: g4f.models.ModelUtils.convert[model]
                 for model in g4f.Model.__all__()
-            )
+            }
             model_list = [{
                 'id': model_id,
                 'object': 'model',
                 'created': 0,
                 'owned_by': model.base_provider
             } for model_id, model in model_list.items()]
             return JSONResponse(model_list)
@@ -125,26 +138,26 @@
                     'created': 0,
                     'owned_by': model_info.base_provider
                 })
             except:
                 return JSONResponse({"error": "The model does not exist."})
 
         @self.app.post("/v1/chat/completions")
-        async def chat_completions(config: ChatCompletionsConfig, request: Request = None, provider: str = None):
+        async def chat_completions(config: ChatCompletionsForm, request: Request = None, provider: str = None):
             try:
                 config.provider = provider if config.provider is None else config.provider
                 if config.api_key is None and request is not None:
                     auth_header = request.headers.get("Authorization")
                     if auth_header is not None:
                         auth_header = auth_header.split(None, 1)[-1]
                         if auth_header and auth_header != "Bearer":
                             config.api_key = auth_header
                 response = self.client.chat.completions.create(
                     **config.dict(exclude_none=True),
-                    ignored=list_ignored_providers
+                    ignored=AppConfig.list_ignored_providers
                 )
             except Exception as e:
                 logging.exception(e)
                 return Response(content=format_exception(e, config), status_code=500, media_type="application/json")
 
             if not config.stream:
                 return JSONResponse((await response).to_json())
@@ -162,32 +175,36 @@
 
             return StreamingResponse(streaming(), media_type="text/event-stream")
 
         @self.app.post("/v1/completions")
         async def completions():
             return Response(content=json.dumps({'info': 'Not working yet.'}, indent=4), media_type="application/json")
 
-def format_exception(e: Exception, config: ChatCompletionsConfig) -> str:
+def format_exception(e: Exception, config: ChatCompletionsForm) -> str:
     last_provider = g4f.get_last_provider(True)
     return json.dumps({
         "error": {"message": f"{e.__class__.__name__}: {e}"},
         "model": last_provider.get("model") if last_provider else config.model,
         "provider": last_provider.get("name") if last_provider else config.provider
     })
 
 def run_api(
     host: str = '0.0.0.0',
     port: int = 1337,
     bind: str = None,
     debug: bool = False,
     workers: int = None,
-    use_colors: bool = None,
-    g4f_api_key: str = None
+    use_colors: bool = None
 ) -> None:
     print(f'Starting server... [g4f v-{g4f.version.utils.current_version}]' + (" (debug)" if debug else ""))
     if use_colors is None:
         use_colors = debug
     if bind is not None:
         host, port = bind.split(":")
-    if debug:
-        g4f.debug.logging = True
-    uvicorn.run(create_app(g4f_api_key), host=host, port=int(port), workers=workers, use_colors=use_colors)
+    uvicorn.run(
+        f"g4f.api:{'create_app_debug' if debug else 'create_app'}",
+        host=host, port=int(port),
+        workers=workers,
+        use_colors=use_colors,
+        factory=True,
+        reload=debug
+    )
```

### Comparing `g4f-0.3.0.7/g4f/api/_logging.py` & `g4f-0.3.0.8/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/cli.py` & `g4f-0.3.0.8/g4f/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from __future__ import annotations
 
 import argparse
 
 from g4f import Provider
 from g4f.gui.run import gui_parser, run_gui_args
-from g4f.cookies import read_cookie_files
-from g4f import debug
 
 def main():
     parser = argparse.ArgumentParser(description="Run gpt4free")
     subparsers = parser.add_subparsers(dest="mode", help="Mode to run the g4f in.")
     api_parser = subparsers.add_parser("api")
     api_parser.add_argument("--bind", default="0.0.0.0:1337", help="The bind string.")
     api_parser.add_argument("--debug", action="store_true", help="Enable verbose logging.")
     api_parser.add_argument("--workers", type=int, default=None, help="Number of workers.")
     api_parser.add_argument("--disable-colors", action="store_true", help="Don't use colors.")
     api_parser.add_argument("--ignore-cookie-files", action="store_true", help="Don't read .har and cookie files.")
-    api_parser.add_argument("--g4f-api-key", type=str, default=None, help="Sets an authentication key for your API.")
-    api_parser.add_argument("--ignored-providers", nargs="+", choices=[provider for provider in Provider.__map__],
-                            default=[], help="List of providers to ignore when processing request.")
+    api_parser.add_argument("--g4f-api-key", type=str, default=None, help="Sets an authentication key for your API. (incompatible with --debug and --workers)")
+    api_parser.add_argument("--ignored-providers", nargs="+", choices=[provider.__name__ for provider in Provider.__providers__ if provider.working],
+                            default=[], help="List of providers to ignore when processing request. (incompatible with --debug and --workers)")
     subparsers.add_parser("gui", parents=[gui_parser()], add_help=False)
 
     args = parser.parse_args()
     if args.mode == "api":
         run_api_args(args)
     elif args.mode == "gui":
         run_gui_args(args)
     else:
         parser.print_help()
         exit(1)
 
 def run_api_args(args):
-    if args.debug:
-        debug.logging = True
-    if not args.ignore_cookie_files:
-        read_cookie_files()
-    import g4f.api
-    g4f.api.set_list_ignored_providers(
+    from g4f.api import AppConfig, run_api
+
+    AppConfig.set_ignore_cookie_files(
+        args.ignore_cookie_files
+    )
+    AppConfig.set_list_ignored_providers(
         args.ignored_providers
     )
-    g4f.api.run_api(
+    AppConfig.set_g4f_api_key(
+        args.g4f_api_key
+    )
+    run_api(
         bind=args.bind,
         debug=args.debug,
         workers=args.workers,
-        g4f_api_key=args.g4f_api_key,
         use_colors=not args.disable_colors
     )
 
 if __name__ == "__main__":
     main()
```

### Comparing `g4f-0.3.0.7/g4f/client/async_client.py` & `g4f-0.3.0.8/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/client/client.py` & `g4f-0.3.0.8/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/client/helper.py` & `g4f-0.3.0.8/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/client/image_models.py` & `g4f-0.3.0.8/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/client/service.py` & `g4f-0.3.0.8/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/client/stubs.py` & `g4f-0.3.0.8/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/client/types.py` & `g4f-0.3.0.8/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/cookies.py` & `g4f-0.3.0.8/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/errors.py` & `g4f-0.3.0.8/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/__init__.py` & `g4f-0.3.0.8/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/index.html` & `g4f-0.3.0.8/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/css/style.css` & `g4f-0.3.0.8/g4f/gui/client/static/css/style.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.0.8/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.0.8/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.0.8/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.0.8/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.0.8/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/img/user.png` & `g4f-0.3.0.8/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.0.8/g4f/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.0.8/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.0.8/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/js/icons.js` & `g4f-0.3.0.8/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/server/android_gallery.py` & `g4f-0.3.0.8/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/server/api.py` & `g4f-0.3.0.8/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/server/backend.py` & `g4f-0.3.0.8/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/server/config.py` & `g4f-0.3.0.8/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/server/internet.py` & `g4f-0.3.0.8/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/server/js_api.py` & `g4f-0.3.0.8/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/server/website.py` & `g4f-0.3.0.8/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/gui/webview.py` & `g4f-0.3.0.8/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/image.py` & `g4f-0.3.0.8/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/local/__init__.py` & `g4f-0.3.0.8/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/locals/models.py` & `g4f-0.3.0.8/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/locals/provider.py` & `g4f-0.3.0.8/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/models.py` & `g4f-0.3.0.8/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/providers/base_provider.py` & `g4f-0.3.0.8/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/providers/create_images.py` & `g4f-0.3.0.8/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/providers/helper.py` & `g4f-0.3.0.8/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/providers/retry_provider.py` & `g4f-0.3.0.8/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/providers/types.py` & `g4f-0.3.0.8/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/requests/__init__.py` & `g4f-0.3.0.8/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/requests/aiohttp.py` & `g4f-0.3.0.8/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/requests/curl_cffi.py` & `g4f-0.3.0.8/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/requests/defaults.py` & `g4f-0.3.0.8/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/requests/raise_for_status.py` & `g4f-0.3.0.8/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/stubs.py` & `g4f-0.3.0.8/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/typing.py` & `g4f-0.3.0.8/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/version.py` & `g4f-0.3.0.8/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f/webdriver.py` & `g4f-0.3.0.8/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f.egg-info/PKG-INFO` & `g4f-0.3.0.8/g4f.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.7
+Version: 0.3.0.8
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -492,25 +492,23 @@
 | Meta AI | `g4f.Provider.MetaAI` | ✔️ | ❌ | [meta.ai](https://www.meta.ai) |
 | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
 | Reka | `g4f.Provider.Reka` | ❌ | ✔️ | [chat.reka.ai](https://chat.reka.ai/) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e-3| ✔️ | [you.com](https://you.com) |
 
 ```python
+import requests
 from g4f.client import Client
-from g4f.Provider.GeminiPro import GeminiPro
 
-client = Client(
-    api_key="...",
-    provider=GeminiPro
-)
+client = Client()
+image = requests.get("https://change_me.jpg", stream=True).raw
 response = client.chat.completions.create(
-    model="gemini-pro-vision",
-    messages=[{"role": "user", "content": "What are on this image?"}],
-    image=open("docs/waterfall.jpeg", "rb")
+    "",
+    messages=[{"role": "user", "content": "what is in this picture?"}],
+    image=image
 )
 print(response.choices[0].message.content)
 ```
 
 ## 🔗 Powered by gpt4free
 
 <table>
@@ -935,47 +933,49 @@
 <a href="https://github.com/hlohaus" target="_blank"><img src="https://avatars.githubusercontent.com/u/983577?v=4&s=45" width="45" title="hlohaus"></a>
 <a href="https://github.com/bagusindrayana" target="_blank"><img src="https://avatars.githubusercontent.com/u/36830534?v=4&s=45" width="45" title="bagusindrayana"></a>
 <a href="https://github.com/sudouser777" target="_blank"><img src="https://avatars.githubusercontent.com/u/22415463?v=4&s=45" width="45" title="sudouser777"></a>
 <a href="https://github.com/thatlukinhasguy1" target="_blank"><img src="https://avatars.githubusercontent.com/u/139662282?v=4&s=45" width="45" title="thatlukinhasguy1"></a>
 <a href="https://github.com/Commenter123321" target="_blank"><img src="https://avatars.githubusercontent.com/u/36051603?v=4&s=45" width="45" title="Commenter123321"></a>
 <a href="https://github.com/DanielShemesh" target="_blank"><img src="https://avatars.githubusercontent.com/u/20585236?v=4&s=45" width="45" title="DanielShemesh"></a>
 <a href="https://github.com/Luneye" target="_blank"><img src="https://avatars.githubusercontent.com/u/73485421?v=4&s=45" width="45" title="Luneye"></a>
-<a href="https://github.com/enganese" target="_blank"><img src="https://avatars.githubusercontent.com/u/69082498?v=4&s=45" width="45" title="enganese"></a>
 <a href="https://github.com/ezerinz" target="_blank"><img src="https://avatars.githubusercontent.com/u/100193740?v=4&s=45" width="45" title="ezerinz"></a>
+<a href="https://github.com/enganese" target="_blank"><img src="https://avatars.githubusercontent.com/u/69082498?v=4&s=45" width="45" title="enganese"></a>
 <a href="https://github.com/Lin-jun-xiang" target="_blank"><img src="https://avatars.githubusercontent.com/u/63782903?v=4&s=45" width="45" title="Lin-jun-xiang"></a>
 <a href="https://github.com/nullstreak" target="_blank"><img src="https://avatars.githubusercontent.com/u/139914347?v=4&s=45" width="45" title="nullstreak"></a>
 <a href="https://github.com/valerii-chirkov" target="_blank"><img src="https://avatars.githubusercontent.com/u/81074936?v=4&s=45" width="45" title="valerii-chirkov"></a>
 <a href="https://github.com/MIDORIBIN" target="_blank"><img src="https://avatars.githubusercontent.com/u/25425217?v=4&s=45" width="45" title="MIDORIBIN"></a>
 <a href="https://github.com/repollo" target="_blank"><img src="https://avatars.githubusercontent.com/u/2671466?v=4&s=45" width="45" title="repollo"></a>
 <a href="https://github.com/hpsj" target="_blank"><img src="https://avatars.githubusercontent.com/u/54535414?v=4&s=45" width="45" title="hpsj"></a>
 <a href="https://github.com/taiyi747" target="_blank"><img src="https://avatars.githubusercontent.com/u/63543716?v=4&s=45" width="45" title="taiyi747"></a>
-<a href="https://github.com/ostix360" target="_blank"><img src="https://avatars.githubusercontent.com/u/55257054?v=4&s=45" width="45" title="ostix360"></a>
-<a href="https://github.com/WdR-Tech" target="_blank"><img src="https://avatars.githubusercontent.com/u/143020293?v=4&s=45" width="45" title="WdR-Tech"></a>
-<a href="https://github.com/HexyeDEV" target="_blank"><img src="https://avatars.githubusercontent.com/u/65314629?v=4&s=45" width="45" title="HexyeDEV"></a>
 <a href="https://github.com/9fo" target="_blank"><img src="https://avatars.githubusercontent.com/u/71867245?v=4&s=45" width="45" title="9fo"></a>
-<a href="https://github.com/eltociear" target="_blank"><img src="https://avatars.githubusercontent.com/u/22633385?v=4&s=45" width="45" title="eltociear"></a>
-<a href="https://github.com/ramonvc" target="_blank"><img src="https://avatars.githubusercontent.com/u/13617054?v=4&s=45" width="45" title="ramonvc"></a>
-<a href="https://github.com/naa7" target="_blank"><img src="https://avatars.githubusercontent.com/u/44613678?v=4&s=45" width="45" title="naa7"></a>
-<a href="https://github.com/zeng-rr" target="_blank"><img src="https://avatars.githubusercontent.com/u/47846202?v=4&s=45" width="45" title="zeng-rr"></a>
-<a href="https://github.com/editor-syntax" target="_blank"><img src="https://avatars.githubusercontent.com/u/109844019?v=4&s=45" width="45" title="editor-syntax"></a>
+<a href="https://github.com/HexyeDEV" target="_blank"><img src="https://avatars.githubusercontent.com/u/65314629?v=4&s=45" width="45" title="HexyeDEV"></a>
+<a href="https://github.com/WdR-Tech" target="_blank"><img src="https://avatars.githubusercontent.com/u/143020293?v=4&s=45" width="45" title="WdR-Tech"></a>
+<a href="https://github.com/ostix360" target="_blank"><img src="https://avatars.githubusercontent.com/u/55257054?v=4&s=45" width="45" title="ostix360"></a>
 <a href="https://github.com/devAdityaa" target="_blank"><img src="https://avatars.githubusercontent.com/u/77636021?v=4&s=45" width="45" title="devAdityaa"></a>
+<a href="https://github.com/editor-syntax" target="_blank"><img src="https://avatars.githubusercontent.com/u/109844019?v=4&s=45" width="45" title="editor-syntax"></a>
+<a href="https://github.com/zeng-rr" target="_blank"><img src="https://avatars.githubusercontent.com/u/47846202?v=4&s=45" width="45" title="zeng-rr"></a>
+<a href="https://github.com/naa7" target="_blank"><img src="https://avatars.githubusercontent.com/u/44613678?v=4&s=45" width="45" title="naa7"></a>
+<a href="https://github.com/ramonvc" target="_blank"><img src="https://avatars.githubusercontent.com/u/13617054?v=4&s=45" width="45" title="ramonvc"></a>
+<a href="https://github.com/eltociear" target="_blank"><img src="https://avatars.githubusercontent.com/u/22633385?v=4&s=45" width="45" title="eltociear"></a>
 <a href="https://github.com/kggn" target="_blank"><img src="https://avatars.githubusercontent.com/u/95663228?v=4&s=45" width="45" title="kggn"></a>
 <a href="https://github.com/xiangsx" target="_blank"><img src="https://avatars.githubusercontent.com/u/29322721?v=4&s=45" width="45" title="xiangsx"></a>
 <a href="https://github.com/ggindinson" target="_blank"><img src="https://avatars.githubusercontent.com/u/97807772?v=4&s=45" width="45" title="ggindinson"></a>
 <span></span>
 <img src="https://avatars.githubusercontent.com/u/71154407?s=45&v=4" width="45" title="ading2210">
 <img src="https://avatars.githubusercontent.com/u/12299238?s=45&v=4" width="45" title="xqdoo00o">
 <img src="https://avatars.githubusercontent.com/u/97126670?s=45&v=4" width="45" title="nathanrchn">
 <img src="https://avatars.githubusercontent.com/u/81407603?v=4&s=45" width="45" title="dsdanielpark">
+<img src="https://avatars.githubusercontent.com/u/55200481?v=4&s=45" width="45" title="missuo">
 
 - The [`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
 - The [`har_file.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
 - The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
 - The [`Gemini.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
 - The [`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm)
+- The [`proofofwork.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/proofofwork.py) has input from [missuo/FreeGPT35](https://github.com/missuo/FreeGPT35)
 
 *Having input implies that the AI's code generation utilized it as one of many sources.*
 
 ## ©️ Copyright
 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.7 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.8 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -387,20 +387,19 @@
 | `g4f.Provider.GeminiPro` | â | gemini-1.5-pro | [ai.google.dev](https://
 ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | âï¸ | â | [meta.ai]
 (https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
 3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Reka |
 `g4f.Provider.Reka` | â | âï¸ | [chat.reka.ai](https://chat.reka.ai/) | |
 Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b |
 [replicate.com](https://replicate.com) | | You.com | `g4f.Provider.You` | dall-
-e-3| âï¸ | [you.com](https://you.com) | ```python from g4f.client import
-Client from g4f.Provider.GeminiPro import GeminiPro client = Client
-( api_key="...", provider=GeminiPro ) response = client.chat.completions.create
-( model="gemini-pro-vision", messages=[{"role": "user", "content": "What are on
-this image?"}], image=open("docs/waterfall.jpeg", "rb") ) print
-(response.choices[0].message.content) ``` ## ð Powered by gpt4free
+e-3| âï¸ | [you.com](https://you.com) | ```python import requests from
+g4f.client import Client client = Client() image = requests.get("https://
+change_me.jpg", stream=True).raw response = client.chat.completions.create( "",
+messages=[{"role": "user", "content": "what is in this picture?"}], image=image
+) print(response.choices[0].message.content) ``` ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
@@ -427,64 +426,67 @@
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_3_5_7_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_8_3_0_5_3_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_4_1_5_4_6_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_6_6_2_2_8_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_0_5_1_6_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_0_5_8_5_2_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_3_4_8_5_4_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_9_0_8_2_4_9_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_0_1_9_3_7_4_0_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_9_0_8_2_4_9_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_7_8_2_9_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_9_1_4_3_4_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_8_1_0_7_4_9_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_5_4_2_5_2_1_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_6_7_1_4_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_4_5_3_5_4_1_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_5_4_3_7_1_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_5_2_5_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_4_3_0_2_0_2_9_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_5_3_1_4_6_2_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_1_8_6_7_2_4_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_6_3_3_3_8_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_6_1_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_4_6_1_3_6_7_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_7_8_4_6_2_0_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_9_8_4_4_0_1_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_5_3_1_4_6_2_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_4_3_0_2_0_2_9_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_5_2_5_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_7_6_3_6_0_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_9_8_4_4_0_1_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_7_8_4_6_2_0_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_4_6_1_3_6_7_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_6_1_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_6_3_3_3_8_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_5_6_6_3_2_2_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_9_3_2_2_7_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_7_8_0_7_7_7_2_?_v_=_4_&_s_=_4_5_][https://
 avatars.githubusercontent.com/u/71154407?s=45&v=4][https://
 avatars.githubusercontent.com/u/12299238?s=45&v=4][https://
 avatars.githubusercontent.com/u/97126670?s=45&v=4][https://
-avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](https://
+avatars.githubusercontent.com/u/81407603?v=4&s=45][https://
+avatars.githubusercontent.com/u/55200481?v=4&s=45]- The [`Vercel.py`](https://
 github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code
 from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by
 [@ading2210](https://github.com/ading2210) - The [`har_file.py`](https://
 github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input
 from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API) -
 The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/
 Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://
 github.com/nathanrchn/perplexityai) - The [`Gemini.py`](https://github.com/
 xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from
 [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API) - The
 [`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/
 MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-
-ai-api) by [@Strvm](https://github.com/Strvm) *Having input implies that the
-AI's code generation utilized it as one of many sources.* ## Â©ï¸ Copyright
-This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/
-gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This program is
-free software: you can redistribute it and/or modify it under the terms of the
-GNU General Public License as published by the Free Software Foundation, either
-version 3 of the License, or (at your option) any later version. This program
-is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
-without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE. See the GNU General Public License for more details. You
-should have received a copy of the GNU General Public License along with this
-program. If not, see
+ai-api) by [@Strvm](https://github.com/Strvm) - The [`proofofwork.py`](https://
+github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/proofofwork.py) has
+input from [missuo/FreeGPT35](https://github.com/missuo/FreeGPT35) *Having
+input implies that the AI's code generation utilized it as one of many
+sources.* ## Â©ï¸ Copyright This program is licensed under the [GNU GPL v3]
+(https://www.gnu.org/licenses/gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C)
+2023 xtekky This program is free software: you can redistribute it and/or
+modify it under the terms of the GNU General Public License as published by the
+Free Software Foundation, either version 3 of the License, or (at your option)
+any later version. This program is distributed in the hope that it will be
+useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
+License for more details. You should have received a copy of the GNU General
+Public License along with this program. If not, see
 www.gnu.org/licenses/>. ``` ## â­ Star History _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]## ð
 License
 [https://upload.wikimedia.org/wikipedia/ [https://img.shields.io/badge/License-
    commons/thumb/9/93/GPLv3_Logo.svg/    GNU_GPL_v3.0-red.svg]
        1200px-GPLv3_Logo.svg.png]        This project is licensed under
                                          _G_N_U___G_P_L___v_3_._0.
                                                              (_ð___¼_ _B_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `g4f-0.3.0.7/g4f.egg-info/SOURCES.txt` & `g4f-0.3.0.8/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/g4f.egg-info/requires.txt` & `g4f-0.3.0.8/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.7/setup.py` & `g4f-0.3.0.8/setup.py`

 * *Files identical despite different names*

