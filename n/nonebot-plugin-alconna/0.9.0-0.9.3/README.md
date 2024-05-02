# Comparing `tmp/nonebot-plugin-alconna-0.9.0.tar.gz` & `tmp/nonebot_plugin_alconna-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.9.0.tar", last modified: Mon Jul  3 13:04:57 2023, max compression
+gzip compressed data, was "nonebot_plugin_alconna-0.9.3.tar", last modified: Sat Jul 22 16:21:36 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.9.0.tar` & `nonebot_plugin_alconna-0.9.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.9.0/LICENSE
--rw-r--r--   0        0        0     1551 2023-07-03 12:34:25.733263 nonebot-plugin-alconna-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     8878 2023-07-03 13:02:02.807832 nonebot-plugin-alconna-0.9.0/README.md
--rw-r--r--   0        0        0     1959 2023-07-03 12:27:47.197059 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0     6364 2023-06-29 04:17:15.903159 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      523 2023-05-31 10:32:51.256024 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0     1052 2023-05-31 10:32:51.263057 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0     1661 2023-05-31 10:32:51.272058 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     2120 2023-05-31 10:32:51.280029 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      519 2023-05-31 10:32:51.286108 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0     1163 2023-05-31 10:32:51.293032 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0      761 2023-05-31 10:32:51.300025 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/minecraft.py
--rw-r--r--   0        0        0     3129 2023-05-31 10:32:51.308024 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0     1088 2023-05-31 10:32:51.314025 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     3151 2023-05-31 10:32:51.321077 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     2496 2023-05-31 10:32:51.327029 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     3251 2023-05-31 10:32:51.334314 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0     3224 2023-06-22 16:21:04.989803 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0      579 2023-05-31 10:32:51.160062 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/argv.py
--rw-r--r--   0        0        0      405 2023-05-31 10:32:51.165611 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0      182 2023-05-31 10:31:14.855148 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/i18n/.config.json
--rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/i18n/en-US.json
--rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0     3638 2023-07-03 12:51:09.077940 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1323 2023-07-03 13:01:00.887691 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/matcher.pyi
--rw-r--r--   0        0        0     1478 2023-05-31 10:32:51.204511 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     3830 2023-05-31 10:32:51.214457 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     8779 2023-06-28 10:23:05.446107 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0     2528 2023-07-03 13:01:00.957077 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     8945 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-22 16:20:40.818321 nonebot_plugin_alconna-0.9.3/LICENSE
+-rw-r--r--   0        0        0     8559 2023-07-22 16:20:40.818321 nonebot_plugin_alconna-0.9.3/README.md
+-rw-r--r--   0        0        0     2000 2023-07-22 16:21:36.399263 nonebot_plugin_alconna-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2053 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0     6269 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      507 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1026 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1614 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2063 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      502 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1137 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      741 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3045 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1063 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3066 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2423 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3205 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3214 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      560 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      245 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      101 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      293 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      254 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     3399 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1570 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1416 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     3992 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     9028 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     2466 2023-07-22 16:20:40.822322 nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     9189 1970-01-01 00:00:00.000000 nonebot_plugin_alconna-0.9.3/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.9.0/pyproject.toml` & `nonebot_plugin_alconna-0.9.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,107 @@
 [project]
 name = "nonebot-plugin-alconna"
-version = "0.9.0"
 description = "Alconna Adapter for Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
-    "arclet-alconna<2.0.0, >=1.7.10",
+    "arclet-alconna<2.0.0, >=1.7.13",
     "arclet-alconna-tools<0.7.0, >=0.6.3",
+    "nepattern<0.6.0, >=0.5.10",
 ]
+dynamic = []
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "command",
     "argparse",
     "cli",
     "alconna",
     "nonebot",
 ]
+version = "0.9.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
-repository = "https://github.com/ArcletProject/nonebot-plugin-alconna"
+homepage = "https://github.com/nonebot/plugin-alconna"
+repository = "https://github.com/nonebot/plugin-alconna"
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "nonebot2[fastapi,httpx,websockets]>=2.0.0",
     "fix-future-annotations>=0.5.0",
     "nonebot-adapter-onebot>=2.2.3",
     "nonebot-adapter-feishu>=2.0.0b8",
     "nonebot-adapter-console>=0.3.2",
     "nonebot-adapter-ding>=2.0.0a16",
     "nonebot-adapter-mirai2>=0.0.22",
     "nonebot-adapter-minecraft>=0.1.1",
     "nonebot-adapter-ntchat>=0.3.5",
     "nonebot-adapter-qqguild>=0.2.3",
     "nonebot-adapter-telegram>=0.1.0b10",
+    "isort ~=5.10",
+    "black ~=23.1",
+    "loguru>=0.7.0",
+    "ruff ~=0.0.275",
+    "nonemoji ~=0.1",
+    "pre-commit ~=3.1",
 ]
 
 [tool.pdm.build]
 includes = [
     "src/nonebot_plugin_alconna",
 ]
 
+[tool.pdm.version]
+source = "file"
+path = "src/nonebot_plugin_alconna/__init__.py"
+
 [tool.black]
 line-length = 88
 target-version = [
     "py38",
     "py39",
     "py310",
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [tool.isort]
 profile = "black"
 line_length = 88
-length_sort = false
+length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
-src_paths = [
-    "nonebot",
-    "tests",
-]
 extra_standard_library = [
     "typing_extensions",
 ]
+
+[tool.ruff]
+select = [
+    "E",
+    "W",
+    "F",
+    "UP",
+    "C",
+    "T",
+    "PYI",
+    "PT",
+    "Q",
+]
+ignore = [
+    "C901",
+    "T201",
+    "E731",
+]
+line-length = 88
+target-version = "py38"
```

### Comparing `nonebot-plugin-alconna-0.9.0/README.md` & `nonebot_plugin_alconna-0.9.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-<p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
-</p>
-
-<div align="center">
-
-# NoneBot Plugin Alconna
-
-_✨ Alconna Usage For NoneBot2 ✨_
-
-</div>
-
-<p align="center">
-  <a href="https://raw.githubusercontent.com/ArcletProject/nonebot-plugin-alconna/master/LICENSE">
-    <img src="https://img.shields.io/github/license/ArcletProject/nonebot-plugin-alconna.svg" alt="license">
-  </a>
-  <a href="https://pypi.python.org/pypi/nonebot-plugin-alconna">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-alconna.svg" alt="pypi">
-  </a>
-  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-</p>
-
-该插件提供了 [Alconna](https://github.com/ArcletProject/Alconna) 的 [Nonebot2](https://github.com/nonebot/nonebot2) 适配版本与工具
-
-## 特性
-
-- 完整的 Alconna 特性支持
-- 基本的 rule, matcher 与 依赖注入
-- 自动回复命令帮助信息 (help, shortcut, completion) 选项
-- 现有全部协议的 Segment 标注
-- match_value, match_path 等检查函数
-- 补全会话支持
-
-## 讨论
-
-QQ 交流群: [链接](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
-
-
-## 使用方法
-
-Nonebot文档: [📖这里](https://nonebot.dev/docs/advanced/matcher#alconna)
-详细介绍: [📦这里](/docs.md)
-
-### 消息解析
-
-```python
-from nonebot.adapters.onebot.v12 import Message, MessageSegment
-from arclet.alconna import Alconna, Option, Args
-
-msg = Message("Hello! --foo 123")
-img = MessageSegment.image("1.png")
-print(msg)
-
-alc = Alconna("Hello!", Option("--foo", Args["foo", int]))
-res = alc.parse(msg)
-assert res.matched
-assert res.query("foo.foo") == 123
-assert not alc.parse(Message(["Hello!", img])).matched
-```
-
-### MessageSegment 标注
-
-特定适配器:
-
-```python
-from nonebot_plugin_alconna.adapters.onebot12 import Mention
-from nonebot.adapters.onebot.v12 import Message
-from arclet.alconna import Alconna, Args
-
-msg = Message(["Hello!", Mention("123")])
-print(msg)  # Hello![mention:user_id=123]
-
-alc = Alconna("Hello!", Args["target", Mention])
-res = alc.parse(msg)
-assert res.matched
-assert res.query("target").data['user_id'] == '123'
-```
-
-通用标注:
-
-```python
-from nonebot.adapters.onebot.v12 import Message as Ob12Msg, MessageSegment as Ob12MS
-from nonebot.adapters.onebot.v11 import Message as Ob11Msg, MessageSegment as Ob11MS
-from nonebot_plugin_alconna.adapters import At
-from arclet.alconna import Alconna, Args
-
-msg1 = Ob12Msg(["Hello!", Ob12MS.mention("123")]) # Hello![mention:user_id=123]
-msg2 = Ob11Msg(["Hello!", Ob11MS.at(123)]) # Hello![CQ:at,qq=123]
-
-
-alc = Alconna("Hello!", Args["target", At])
-res1 = alc.parse(msg1)
-assert res1.matched
-target = res1.query("target")
-assert isinstance(target, At)
-assert target.target == '123'
-
-res2 = alc.parse(msg2)
-assert res2.matched
-target = res2.query("target")
-assert isinstance(target, At)
-assert target.target == '123'
-```
-
-### Matcher 与 依赖注入
-```python
-...
-from nonebot import require
-require("nonebot_plugin_alconna")
-...
-
-from nonebot_plugin_alconna import (
-    on_alconna, 
-    Match,
-    Query,
-    AlconnaMatch, 
-    AlconnaQuery,
-    AlcMatches,
-    AlcResult
-)
-from arclet.alconna import Alconna, Args, Option
-
-test = on_alconna(
-    Alconna(
-        "test",
-        Option("foo", Args["bar", int]),
-        Option("baz", Args["qux", bool, False])
-    ),
-    auto_send_output=True
-)
-
-
-@test.handle()
-async def handle_test1(result: AlcResult):
-    await test.send(f"matched: {result.matched}")
-    await test.send(f"maybe output: {result.output}")
-
-@test.handle()
-async def handle_test2(result: AlcMatches):
-    await test.send(f"head result: {result.header_result}")
-    await test.send(f"args: {result.all_matched_args}")
-
-@test.handle()
-async def handle_test3(bar: Match[int] = AlconnaMatch("bar")):
-    if bar.available:    
-        await test.send(f"foo={bar.result}")
-
-@test.handle()
-async def handle_test4(qux: Query[bool] = AlconnaQuery("baz.qux", False)):
-    if qux.available:
-        await test.send(f"baz.qux={qux.result}")
-```
-
-### 条件控制
-
-```python
-...
-from nonebot import require
-require("nonebot_plugin_alconna")
-...
-
-from arclet.alconna import Alconna, Subcommand, Option, Args
-from nonebot_plugin_alconna import assign, on_alconna, AlconnaResult, CommandResult, Check
-
-pip = Alconna(
-    "pip",
-    Subcommand(
-        "install", 
-        Args["pak", str],
-        Option("--upgrade"),
-        Option("--force-reinstall")
-    ),
-    Subcommand(
-        "list",
-        Option("--out-dated")
-    )
-)
-
-pip_cmd = on_alconna(pip)
-
-@pip_cmd.handle([Check(assign("install.pak", "pip"))])
-async def update(arp: CommandResult = AlconnaResult()):
-    ...
-
-@pip_cmd.handle([Check(assign("list"))])
-async def list_(arp: CommandResult = AlconnaResult()):
-    ...
-
-@pip_cmd.handle([Check(assign("install"))])
-async def install(arp: CommandResult = AlconnaResult()):
-    ...
-```
-
-
-### Duplication
-
-```python
-...
-from nonebot import require
-require("nonebot_plugin_alconna")
-...
-
-from nonebot_plugin_alconna import (
-    on_alconna, 
-    AlconnaDuplication
-)
-from arclet.alconna import Alconna, Args, Duplication, Option, OptionStub
-
-test = on_alconna(
-    Alconna(
-        "test",
-        Option("foo", Args["bar", int]),
-        Option("baz", Args["qux", bool, False])
-    ),
-    auto_send_output=True
-)
-
-class MyResult(Duplication):
-    bar: int
-    qux: bool
-    foo: OptionStub
-
-@test.handle()
-async def handle_test1(result: MyResult = AlconnaDuplication(MyResult)):
-    await test.send(f"matched: bar={result.bar}, qux={result.qux}")
-    await test.send(f"options: foo={result.foo.origin}")
-
-```
-
-## 配置
-
-目前配置项有：
-
-- ALCONNA_AUTO_SEND_OUTPUT : 是否全局启用输出信息自动发送
-- ALCONNA_USE_COMMAND_START : 是否将 COMMAND_START 作为全局命令前缀
-- ALCONNA_AUTO_COMPLETION: 是否全局启用补全会话功能
-
-## 参数解释
-
-```python
-def on_alconna(
-    command: Alconna | str,
-    skip_for_unmatch: bool = True,
-    auto_send_output: bool = False,
-    output_converter: Callable[[OutputType, str], Message | Awaitable[Message]] | None = None,
-    aliases: set[str | tuple[str, ...]] | None = None,
-    comp_config: CompConfig | None = None,
-    **kwargs,
-) -> type[Matcher]:
-```
-
-- `command`: Alconna 命令
-- `skip_for_unmatch`: 是否在命令不匹配时跳过该响应
-- `auto_send_output`: 是否自动发送输出信息并跳过响应
-- `output_converter`: 输出信息字符串转换为 Message 方法
-- `aliases`: 命令别名, 作用类似于 `on_command`
-- `comp_config`: 补全会话配置, 不传入则不启用补全会话
-
-## 提供了 MessageSegment标注 的协议:
-
-| 协议名称                                                                | 路径                                   |
-|---------------------------------------------------------------------|--------------------------------------|
-| [OneBot 协议](https://onebot.dev/)                                    | adapters.onebot11, adapters.onebot12 |
-| [Telegram](https://core.telegram.org/bots/api)                      | adapters.telegram                    |
-| [飞书](https://open.feishu.cn/document/home/index)                    | adapters.feishu                      |
-| [GitHub](https://docs.github.com/en/developers/apps)                | adapters.github                      |
-| [QQ 频道](https://bot.q.qq.com/wiki/)                                 | adapters.qqguild                     |
-| [钉钉](https://open.dingtalk.com/document/)                           | adapters.ding                        |
-| [Console](https://github.com/nonebot/adapter-console)               | adapters.console                     |
-| [开黑啦](https://developer.kookapp.cn/)                                | adapters.kook                        |
-| [Mirai](https://docs.mirai.mamoe.net/mirai-api-http/)               | adapters.mirai                       |
-| [Ntchat](https://github.com/JustUndertaker/adapter-ntchat)          | adapters.ntchat                      |
-| [MineCraft](https://github.com/17TheWord/nonebot-adapter-minecraft) | adapters.minecraft                   |
-| [BiliBili Live](https://github.com/wwweww/adapter-bilibili)         | adapters.bilibili                    |
-
-
-### 便捷装饰器
-
-`funcommand` 装饰器用于将一个接受任意参数，返回 `str` 或 `Message` 或 `MessageSegment` 的函数转换为命令响应器。
-
-```python
-from nonebot_plugin_alconna import funcommand
-
-@funcommand()
-async def echo(msg: str):
-    return msg
-```
-
-## 体验
-
-[demo bot](./src/test/plugins/demo.py)
+<p align="center">
+  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+</p>
+
+<div align="center">
+
+# NoneBot Plugin Alconna
+
+_✨ Alconna Usage For NoneBot2 ✨_
+
+</div>
+
+<p align="center">
+  <a href="https://raw.githubusercontent.com/nonebot/plugin-alconna/master/LICENSE">
+    <img src="https://img.shields.io/github/license/nonebot/plugin-alconna.svg" alt="license">
+  </a>
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-alconna">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-alconna.svg" alt="pypi">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+</p>
+
+该插件提供了 [Alconna](https://github.com/ArcletProject/Alconna) 的 [Nonebot2](https://github.com/nonebot/nonebot2) 适配版本与工具
+
+## 特性
+
+- 完整的 Alconna 特性支持
+- 基本的 rule, matcher 与 依赖注入
+- 自动回复命令帮助信息 (help, shortcut, completion) 选项
+- 现有全部协议的 Segment 标注
+- match_value, match_path 等检查函数
+- 补全会话支持
+
+## 讨论
+
+QQ 交流群: [链接](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
+
+
+## 使用方法
+
+Nonebot文档: [📖这里](https://nonebot.dev/docs/advanced/matcher#alconna)
+详细介绍: [📦这里](/docs.md)
+
+### 消息解析
+
+```python
+from nonebot.adapters.onebot.v12 import Message, MessageSegment
+from arclet.alconna import Alconna, Option, Args
+
+msg = Message("Hello! --foo 123")
+img = MessageSegment.image("1.png")
+print(msg)
+
+alc = Alconna("Hello!", Option("--foo", Args["foo", int]))
+res = alc.parse(msg)
+assert res.matched
+assert res.query("foo.foo") == 123
+assert not alc.parse(Message(["Hello!", img])).matched
+```
+
+### MessageSegment 标注
+
+特定适配器:
+
+```python
+from nonebot_plugin_alconna.adapters.onebot12 import Mention
+from nonebot.adapters.onebot.v12 import Message
+from arclet.alconna import Alconna, Args
+
+msg = Message(["Hello!", Mention("123")])
+print(msg)  # Hello![mention:user_id=123]
+
+alc = Alconna("Hello!", Args["target", Mention])
+res = alc.parse(msg)
+assert res.matched
+assert res.query("target").data['user_id'] == '123'
+```
+
+通用标注:
+
+```python
+from nonebot.adapters.onebot.v12 import Message as Ob12Msg, MessageSegment as Ob12MS
+from nonebot.adapters.onebot.v11 import Message as Ob11Msg, MessageSegment as Ob11MS
+from nonebot_plugin_alconna.adapters import At
+from arclet.alconna import Alconna, Args
+
+msg1 = Ob12Msg(["Hello!", Ob12MS.mention("123")]) # Hello![mention:user_id=123]
+msg2 = Ob11Msg(["Hello!", Ob11MS.at(123)]) # Hello![CQ:at,qq=123]
+
+
+alc = Alconna("Hello!", Args["target", At])
+res1 = alc.parse(msg1)
+assert res1.matched
+target = res1.query("target")
+assert isinstance(target, At)
+assert target.target == '123'
+
+res2 = alc.parse(msg2)
+assert res2.matched
+target = res2.query("target")
+assert isinstance(target, At)
+assert target.target == '123'
+```
+
+### Matcher 与 依赖注入
+```python
+...
+from nonebot import require
+require("nonebot_plugin_alconna")
+...
+
+from nonebot_plugin_alconna import (
+    on_alconna, 
+    Match,
+    Query,
+    AlconnaMatch, 
+    AlconnaQuery,
+    AlcMatches,
+    AlcResult
+)
+from arclet.alconna import Alconna, Args, Option
+
+test = on_alconna(
+    Alconna(
+        "test",
+        Option("foo", Args["bar", int]),
+        Option("baz", Args["qux", bool, False])
+    ),
+    auto_send_output=True
+)
+
+
+@test.handle()
+async def handle_test1(result: AlcResult):
+    await test.send(f"matched: {result.matched}")
+    await test.send(f"maybe output: {result.output}")
+
+@test.handle()
+async def handle_test2(result: AlcMatches):
+    await test.send(f"head result: {result.header_result}")
+    await test.send(f"args: {result.all_matched_args}")
+
+@test.handle()
+async def handle_test3(bar: Match[int] = AlconnaMatch("bar")):
+    if bar.available:    
+        await test.send(f"foo={bar.result}")
+
+@test.handle()
+async def handle_test4(qux: Query[bool] = AlconnaQuery("baz.qux", False)):
+    if qux.available:
+        await test.send(f"baz.qux={qux.result}")
+```
+
+### 条件控制
+
+```python
+...
+from nonebot import require
+require("nonebot_plugin_alconna")
+...
+
+from arclet.alconna import Alconna, Subcommand, Option, Args
+from nonebot_plugin_alconna import assign, on_alconna, AlconnaResult, CommandResult, Check
+
+pip = Alconna(
+    "pip",
+    Subcommand(
+        "install", 
+        Args["pak", str],
+        Option("--upgrade"),
+        Option("--force-reinstall")
+    ),
+    Subcommand(
+        "list",
+        Option("--out-dated")
+    )
+)
+
+pip_cmd = on_alconna(pip)
+
+@pip_cmd.handle([Check(assign("install.pak", "pip"))])
+async def update(arp: CommandResult = AlconnaResult()):
+    ...
+
+@pip_cmd.handle([Check(assign("list"))])
+async def list_(arp: CommandResult = AlconnaResult()):
+    ...
+
+@pip_cmd.handle([Check(assign("install"))])
+async def install(arp: CommandResult = AlconnaResult()):
+    ...
+```
+
+
+### Duplication
+
+```python
+...
+from nonebot import require
+require("nonebot_plugin_alconna")
+...
+
+from nonebot_plugin_alconna import (
+    on_alconna, 
+    AlconnaDuplication
+)
+from arclet.alconna import Alconna, Args, Duplication, Option, OptionStub
+
+test = on_alconna(
+    Alconna(
+        "test",
+        Option("foo", Args["bar", int]),
+        Option("baz", Args["qux", bool, False])
+    ),
+    auto_send_output=True
+)
+
+class MyResult(Duplication):
+    bar: int
+    qux: bool
+    foo: OptionStub
+
+@test.handle()
+async def handle_test1(result: MyResult = AlconnaDuplication(MyResult)):
+    await test.send(f"matched: bar={result.bar}, qux={result.qux}")
+    await test.send(f"options: foo={result.foo.origin}")
+
+```
+
+## 配置
+
+目前配置项有：
+
+- ALCONNA_AUTO_SEND_OUTPUT : 是否全局启用输出信息自动发送
+- ALCONNA_USE_COMMAND_START : 是否将 COMMAND_START 作为全局命令前缀
+- ALCONNA_AUTO_COMPLETION: 是否全局启用补全会话功能
+
+## 参数解释
+
+```python
+def on_alconna(
+    command: Alconna | str,
+    skip_for_unmatch: bool = True,
+    auto_send_output: bool = False,
+    output_converter: Callable[[OutputType, str], Message | Awaitable[Message]] | None = None,
+    aliases: set[str | tuple[str, ...]] | None = None,
+    comp_config: CompConfig | None = None,
+    **kwargs,
+) -> type[Matcher]:
+```
+
+- `command`: Alconna 命令
+- `skip_for_unmatch`: 是否在命令不匹配时跳过该响应
+- `auto_send_output`: 是否自动发送输出信息并跳过响应
+- `output_converter`: 输出信息字符串转换为 Message 方法
+- `aliases`: 命令别名, 作用类似于 `on_command`
+- `comp_config`: 补全会话配置, 不传入则不启用补全会话
+
+## 提供了 MessageSegment标注 的协议:
+
+| 协议名称                                                                | 路径                                   |
+|---------------------------------------------------------------------|--------------------------------------|
+| [OneBot 协议](https://onebot.dev/)                                    | adapters.onebot11, adapters.onebot12 |
+| [Telegram](https://core.telegram.org/bots/api)                      | adapters.telegram                    |
+| [飞书](https://open.feishu.cn/document/home/index)                    | adapters.feishu                      |
+| [GitHub](https://docs.github.com/en/developers/apps)                | adapters.github                      |
+| [QQ 频道](https://bot.q.qq.com/wiki/)                                 | adapters.qqguild                     |
+| [钉钉](https://open.dingtalk.com/document/)                           | adapters.ding                        |
+| [Console](https://github.com/nonebot/adapter-console)               | adapters.console                     |
+| [开黑啦](https://developer.kookapp.cn/)                                | adapters.kook                        |
+| [Mirai](https://docs.mirai.mamoe.net/mirai-api-http/)               | adapters.mirai                       |
+| [Ntchat](https://github.com/JustUndertaker/adapter-ntchat)          | adapters.ntchat                      |
+| [MineCraft](https://github.com/17TheWord/nonebot-adapter-minecraft) | adapters.minecraft                   |
+| [BiliBili Live](https://github.com/wwweww/adapter-bilibili)         | adapters.bilibili                    |
+
+
+### 便捷装饰器
+
+`funcommand` 装饰器用于将一个接受任意参数，返回 `str` 或 `Message` 或 `MessageSegment` 的函数转换为命令响应器。
+
+```python
+from nonebot_plugin_alconna import funcommand
+
+@funcommand()
+async def echo(msg: str):
+    return msg
+```
+
+## 体验
+
+[demo bot](./src/test/plugins/demo.py)
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/__init__.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-from nonebot import __version__ as nonebot_version
-from nonebot.plugin import PluginMetadata
-
-from .argv import MessageArgv as MessageArgv
-from .consts import ALCONNA_RESULT as ALCONNA_RESULT
-from .matcher import on_alconna as on_alconna
-from .matcher import funcommand as funcommand
-from .model import CommandResult as CommandResult
-from .model import Match as Match
-from .model import Query as Query
-from .params import AlcMatches as AlcMatches
-from .params import AlcResult as AlcResult
-from .params import AlconnaDuplication as AlconnaDuplication
-from .params import AlconnaMatch as AlconnaMatch
-from .params import AlconnaMatches as AlconnaMatches
-from .params import AlconnaQuery as AlconnaQuery
-from .params import AlconnaResult as AlconnaResult
-from .params import Check as Check
-from .params import assign as assign
-from .params import match_path as match_path
-from .params import match_value as match_value
-from .rule import alconna as alconna
-from .rule import set_output_converter as set_output_converter
-from .config import Config
-
-__version__ = "0.9.0"
-
-_meta_source = {
-    "name": "Alconna 插件",
-    "description": "提供 [Alconna](https://github.com/ArcletProject/Alconna) 的 Nonebot2 适配版本与工具",
-    "usage": "matcher = on_alconna(...)",
-    "homepage": "https://github.com/ArcletProject/Alconna",
-    "type": "library",
-    "supported_adapters": None,
-    "config": Config,
-    "extra": {
-        "author": "RF-Tar-Railt",
-        "priority": 1,
-        "version": __version__,
-    }
-}
-
-
-if not nonebot_version.split(".")[-1].isdigit():
-    _meta_source["extra"]["homepage"] = _meta_source.pop("homepage")
-    _meta_source["extra"]["type"] = _meta_source.pop("type")
-    _meta_source["extra"]["config"] = _meta_source.pop("config")
-    _meta_source["extra"]["supported_adapters"] = _meta_source.pop("supported_adapters")
-
-
-__plugin_meta__ = PluginMetadata(**_meta_source)
+from nonebot.plugin import PluginMetadata
+from nonebot import __version__ as nonebot_version
+
+from .config import Config
+from .model import Match as Match
+from .model import Query as Query
+from .params import Check as Check
+from .params import assign as assign
+from .rule import alconna as alconna
+from .params import AlcResult as AlcResult
+from .argv import MessageArgv as MessageArgv
+from .params import AlcMatches as AlcMatches
+from .params import match_path as match_path
+from .matcher import funcommand as funcommand
+from .matcher import on_alconna as on_alconna
+from .params import match_value as match_value
+from .params import AlconnaMatch as AlconnaMatch
+from .params import AlconnaQuery as AlconnaQuery
+from .model import CommandResult as CommandResult
+from .params import AlcExecResult as AlcExecResult
+from .params import AlconnaResult as AlconnaResult
+from .consts import ALCONNA_RESULT as ALCONNA_RESULT
+from .params import AlconnaMatches as AlconnaMatches
+from .params import AlconnaExecResult as AlconnaExecResult
+from .params import AlconnaDuplication as AlconnaDuplication
+from .consts import ALCONNA_EXEC_RESULT as ALCONNA_EXEC_RESULT
+from .rule import set_output_converter as set_output_converter
+
+__version__ = "0.9.3"
+
+_meta_source = {
+    "name": "Alconna 插件",
+    "description": "提供 ArcletProject/Alconna 的 Nonebot2 适配版本与工具",
+    "usage": "matcher = on_alconna(...)",
+    "homepage": "https://github.com/nonebot/plugin-alconna",
+    "type": "library",
+    "supported_adapters": None,
+    "config": Config,
+    "extra": {
+        "author": "RF-Tar-Railt",
+        "priority": 1,
+        "version": __version__,
+    },
+}
+
+
+if not nonebot_version.split(".")[-1].isdigit():
+    _meta_source["extra"]["homepage"] = _meta_source.pop("homepage")
+    _meta_source["extra"]["type"] = _meta_source.pop("type")
+    _meta_source["extra"]["config"] = _meta_source.pop("config")
+    _meta_source["extra"]["supported_adapters"] = _meta_source.pop("supported_adapters")
+
+
+__plugin_meta__ = PluginMetadata(**_meta_source)
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/__init__.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,214 +1,240 @@
-"""通用标注, 无法用于创建 MS对象"""
-from dataclasses import dataclass, field
-import re
-from typing import Optional
-
-from nepattern import create_local_patterns
-from nonebot.internal.adapter.message import MessageSegment
-from nonebot_plugin_alconna.typings import gen_unit
-
-Text = str
-
-
-@dataclass
-class Segment:
-    """基类标注"""
-    origin: MessageSegment
-
-
-@dataclass
-class At(Segment):
-    """At对象, 表示一类提醒某用户的元素"""
-    target: str
-
-@dataclass
-class Emoji(Segment):
-    """Emoji对象, 表示一类表情元素"""
-    id: str
-    name: Optional[str] = field(default=None)
-
-
-@dataclass
-class Media(Segment):
-    url: Optional[str] = field(default=None)
-    id: Optional[str] = field(default=None)
-
-@dataclass
-class Image(Media):
-    """Image对象, 表示一类图片元素"""
-
-@dataclass
-class Audio(Media):
-    """Audio对象, 表示一类音频元素"""
-
-@dataclass
-class Voice(Media):
-    """Voice对象, 表示一类语音元素"""
-
-@dataclass
-class Video(Media):
-    """Video对象, 表示一类视频元素"""
-
-@dataclass
-class File(Segment):
-    """File对象, 表示一类文件元素"""
-    id: str
-    name: Optional[str] = field(default=None)
-
-_Segment = gen_unit(
-    Segment,
-    {
-        "*": lambda seg: Segment(seg),
-    }
-)
-
-def _handle_kmarkdown_met(seg: MessageSegment):
-    content = seg.data["content"]
-    if not content.startswith("(met)"):
-        return None
-    if (end := content.find("(met)", 5)) == -1:
-        return None
-    return content[5: end] not in ("here", "all") and At(seg, content[5: end])
-
-_At = gen_unit(
-    At,
-    {
-        "at": lambda seg: At(seg, str(seg.data.get("qq", seg.data.get("user_id")))),
-        "mention": lambda seg: At(seg, seg.data.get("user_id", seg.data.get("text"))),
-        "mention_user": lambda seg: At(seg, str(seg.data["user_id"])),
-        "At": lambda seg: At(seg, str(seg, seg.data["target"])),
-        "kmarkdown": _handle_kmarkdown_met
-    }
-)
-"""
-at: ob11, feishu
-mention: ob12, tg
-mention_user: qqguild
-At: mirai
-kmarkdown: kook
-"""
-
-def _handle_kmarkdown_emj(seg: MessageSegment):
-    content = seg.data["content"]
-    if content.startswith("(emj)"):
-        mat = re.search(r"\(emj\)(?P<name>[^()\[\]]+)\(emj\)\[(?P<id>[^\[\]]+)\]", content)
-        return mat and Emoji(seg, mat["id"], mat["name"])
-    if content.startswith(":"):
-        mat = re.search(r":(?P<name>[^:]+):", content)
-        return mat and Emoji(seg, mat["name"], mat["name"])
-
-_Emoji = gen_unit(
-    Emoji,
-    {
-        "emoji": lambda seg: Emoji(seg, str(seg.data.get("id", seg.data.get("name")))),
-        "Face": lambda seg: Emoji(seg, str(seg.data["faceId"]), seg.data["name"]),
-        "face": lambda seg: str(Emoji(seg, seg.data["id"])),
-        "custom_emoji": lambda seg: Emoji(seg, seg.data["custom_emoji_id"], seg.data["text"]),
-        "kmarkdown": _handle_kmarkdown_emj
-    }
-)
-
-
-
-def _handle_image(seg: MessageSegment):
-    if "file_id" in seg.data:  # ob12
-        return Image(seg, id=seg.data["file_id"])
-    if "image_key" in seg.data:  # feishu
-        return Image(seg, url=seg.data["image_key"])
-    if "file_key" in seg.data:  # kook
-        return Image(seg, url=seg.data["file_key"])
-    if "url" in seg.data:  # ob11, qqguild
-        return Image(seg, url=seg.data["url"])
-    if "msgData" in seg.data:  # minecraft
-        return Image(seg, url=seg.data["msgData"])
-    if "file_path" in seg.data:  # ntchat
-        return Image(seg, id=seg.data["file_path"])
-    if "picURL" in seg.data:  # ding
-        return Image(seg, url=seg.data["picURL"])
-
-
-
-_Image = gen_unit(
-    Image,
-    {
-        "image": _handle_image,
-        "photo": lambda seg: Image(seg, id=seg.data["file_id"]),
-        "Image": lambda seg: Image(seg, seg.data["url"], seg.data["imageId"]),
-    }
-)
-
-
-def _handle_video(seg: MessageSegment):
-    if "file_id" in seg.data:  # ob12, telegram
-        return Video(seg, id=seg.data["file_id"])
-    if "file" in seg.data:  # ob11
-        return Video(seg, url=seg.data["file"])
-    if "file_key" in seg.data:  # kook
-        return Video(seg, url=seg.data["file_key"])
-    if "msgData" in seg.data:  # minecraft
-        return Video(seg, url=seg.data["msgData"])
-    if "file_path" in seg.data:  # ntchat
-        return Video(seg, id=seg.data["file_path"])
-
-
-_Video = gen_unit(
-    Video,
-    {
-        "video": lambda seg: Video(seg, seg.data["url"], seg.data["videoId"]),
-        "animation": lambda seg: Video(seg, id=seg.data["file_id"]),
-    }
-)
-
-
-def _handle_voice(seg: MessageSegment):
-    if "file_id" in seg.data:  # ob12, telegram
-        return Voice(seg, id=seg.data["file_id"])
-    if "file_key" in seg.data:  # kook
-        return Voice(seg, url=seg.data["file_key"])
-    if "file_path" in seg.data:  # ntchat
-        return Voice(seg, id=seg.data["file_path"])
-
-_Voice = gen_unit(
-    Voice,
-    {
-        "voice": _handle_voice,
-        "record": lambda seg: Voice(seg, seg.data["url"]),
-        "Voice": lambda seg: Voice(seg, seg.data["url"], seg.data["voiceId"]),
-    }
-)
-
-def _handle_audio(seg: MessageSegment):
-    if "file_id" in seg.data:  # ob12, telegram
-        return Audio(seg, id=seg.data["file_id"])
-    if "file_key" in seg.data:  # kook, feishu
-        return Audio(seg, url=seg.data["file_key"])
-    if "file_path" in seg.data:  # ntchat
-        return Audio(seg, id=seg.data["file_path"])
-
-_Audio = gen_unit(
-    Audio,
-    {
-        "audio": _handle_audio,
-    }
-)
-
-
-def _handle_file(seg: MessageSegment):
-    if "file_id" in seg.data:  # ob12
-        return File(seg, id=seg.data["file_id"])
-    if "file_key" in seg.data:  # feishu, kook
-        return File(seg, id=seg.data["file_key"], name=seg.data.get("file_name", seg.data.get("title")))
-    if "file_path" in seg.data:  # ntchat
-        return File(seg, id=seg.data["file_path"])
-
-_File = gen_unit(
-    File,
-    {
-        "file": _handle_file,
-        "document": lambda seg: File(seg, seg.data["file_id"], seg.data["file_name"]),
-        "File": lambda seg: File(seg, seg.data["id"], seg.data["name"]),
-    }
-)
-
-env = create_local_patterns("nonebot")
-env.sets([_At, _Image, _Video, _Voice, _Audio, _File, _Segment])
+"""通用标注, 无法用于创建 MS对象"""
+import re
+from typing import Optional
+from dataclasses import field, dataclass
+
+from nepattern import create_local_patterns
+from nonebot.internal.adapter.message import MessageSegment
+
+from nonebot_plugin_alconna.typings import gen_unit
+
+Text = str
+
+
+@dataclass
+class Segment:
+    """基类标注"""
+
+    origin: MessageSegment
+
+
+@dataclass
+class At(Segment):
+    """At对象, 表示一类提醒某用户的元素"""
+
+    target: str
+
+
+@dataclass
+class Emoji(Segment):
+    """Emoji对象, 表示一类表情元素"""
+
+    id: str
+    name: Optional[str] = field(default=None)
+
+
+@dataclass
+class Media(Segment):
+    url: Optional[str] = field(default=None)
+    id: Optional[str] = field(default=None)
+
+
+@dataclass
+class Image(Media):
+    """Image对象, 表示一类图片元素"""
+
+
+@dataclass
+class Audio(Media):
+    """Audio对象, 表示一类音频元素"""
+
+
+@dataclass
+class Voice(Media):
+    """Voice对象, 表示一类语音元素"""
+
+
+@dataclass
+class Video(Media):
+    """Video对象, 表示一类视频元素"""
+
+
+@dataclass
+class File(Segment):
+    """File对象, 表示一类文件元素"""
+
+    id: str
+    name: Optional[str] = field(default=None)
+
+
+_Segment = gen_unit(
+    Segment,
+    {
+        "*": lambda seg: Segment(seg),
+    },
+)
+
+
+def _handle_kmarkdown_met(seg: MessageSegment):
+    content = seg.data["content"]
+    if not content.startswith("(met)"):
+        return None
+    if (end := content.find("(met)", 5)) == -1:
+        return None
+    return content[5:end] not in ("here", "all") and At(seg, content[5:end])
+
+
+_At = gen_unit(
+    At,
+    {
+        "at": lambda seg: At(seg, str(seg.data.get("qq", seg.data.get("user_id")))),
+        "mention": lambda seg: At(seg, seg.data.get("user_id", seg.data.get("text"))),
+        "mention_user": lambda seg: At(seg, str(seg.data["user_id"])),
+        "At": lambda seg: At(seg, str(seg, seg.data["target"])),
+        "kmarkdown": _handle_kmarkdown_met,
+    },
+)
+"""
+at: ob11, feishu
+mention: ob12, tg
+mention_user: qqguild
+At: mirai
+kmarkdown: kook
+"""
+
+
+def _handle_kmarkdown_emj(seg: MessageSegment):
+    content = seg.data["content"]
+    if content.startswith("(emj)"):
+        mat = re.search(
+            r"\(emj\)(?P<name>[^()\[\]]+)\(emj\)\[(?P<id>[^\[\]]+)\]", content
+        )
+        return mat and Emoji(seg, mat["id"], mat["name"])
+    if content.startswith(":"):
+        mat = re.search(r":(?P<name>[^:]+):", content)
+        return mat and Emoji(seg, mat["name"], mat["name"])
+
+
+_Emoji = gen_unit(
+    Emoji,
+    {
+        "emoji": lambda seg: Emoji(seg, str(seg.data.get("id", seg.data.get("name")))),
+        "Face": lambda seg: Emoji(seg, str(seg.data["faceId"]), seg.data["name"]),
+        "face": lambda seg: str(Emoji(seg, seg.data["id"])),
+        "custom_emoji": lambda seg: Emoji(
+            seg, seg.data["custom_emoji_id"], seg.data["text"]
+        ),
+        "kmarkdown": _handle_kmarkdown_emj,
+    },
+)
+
+
+def _handle_image(seg: MessageSegment):
+    if "file_id" in seg.data:  # ob12
+        return Image(seg, id=seg.data["file_id"])
+    if "image_key" in seg.data:  # feishu
+        return Image(seg, url=seg.data["image_key"])
+    if "file_key" in seg.data:  # kook
+        return Image(seg, url=seg.data["file_key"])
+    if "url" in seg.data:  # ob11, qqguild
+        return Image(seg, url=seg.data["url"])
+    if "msgData" in seg.data:  # minecraft
+        return Image(seg, url=seg.data["msgData"])
+    if "file_path" in seg.data:  # ntchat
+        return Image(seg, id=seg.data["file_path"])
+    if "picURL" in seg.data:  # ding
+        return Image(seg, url=seg.data["picURL"])
+
+
+_Image = gen_unit(
+    Image,
+    {
+        "image": _handle_image,
+        "photo": lambda seg: Image(seg, id=seg.data["file_id"]),
+        "Image": lambda seg: Image(seg, seg.data["url"], seg.data["imageId"]),
+    },
+)
+
+
+def _handle_video(seg: MessageSegment):
+    if "file_id" in seg.data:  # ob12, telegram
+        return Video(seg, id=seg.data["file_id"])
+    if "file" in seg.data:  # ob11
+        return Video(seg, url=seg.data["file"])
+    if "file_key" in seg.data:  # kook
+        return Video(seg, url=seg.data["file_key"])
+    if "msgData" in seg.data:  # minecraft
+        return Video(seg, url=seg.data["msgData"])
+    if "file_path" in seg.data:  # ntchat
+        return Video(seg, id=seg.data["file_path"])
+
+
+_Video = gen_unit(
+    Video,
+    {
+        "video": lambda seg: Video(seg, seg.data["url"], seg.data["videoId"]),
+        "animation": lambda seg: Video(seg, id=seg.data["file_id"]),
+    },
+)
+
+
+def _handle_voice(seg: MessageSegment):
+    if "file_id" in seg.data:  # ob12, telegram
+        return Voice(seg, id=seg.data["file_id"])
+    if "file_key" in seg.data:  # kook
+        return Voice(seg, url=seg.data["file_key"])
+    if "file_path" in seg.data:  # ntchat
+        return Voice(seg, id=seg.data["file_path"])
+
+
+_Voice = gen_unit(
+    Voice,
+    {
+        "voice": _handle_voice,
+        "record": lambda seg: Voice(seg, seg.data["url"]),
+        "Voice": lambda seg: Voice(seg, seg.data["url"], seg.data["voiceId"]),
+    },
+)
+
+
+def _handle_audio(seg: MessageSegment):
+    if "file_id" in seg.data:  # ob12, telegram
+        return Audio(seg, id=seg.data["file_id"])
+    if "file_key" in seg.data:  # kook, feishu
+        return Audio(seg, url=seg.data["file_key"])
+    if "file_path" in seg.data:  # ntchat
+        return Audio(seg, id=seg.data["file_path"])
+
+
+_Audio = gen_unit(
+    Audio,
+    {
+        "audio": _handle_audio,
+    },
+)
+
+
+def _handle_file(seg: MessageSegment):
+    if "file_id" in seg.data:  # ob12
+        return File(seg, id=seg.data["file_id"])
+    if "file_key" in seg.data:  # feishu, kook
+        return File(
+            seg,
+            id=seg.data["file_key"],
+            name=seg.data.get("file_name", seg.data.get("title")),
+        )
+    if "file_path" in seg.data:  # ntchat
+        return File(seg, id=seg.data["file_path"])
+
+
+_File = gen_unit(
+    File,
+    {
+        "file": _handle_file,
+        "document": lambda seg: File(seg, seg.data["file_id"], seg.data["file_name"]),
+        "File": lambda seg: File(seg, seg.data["id"], seg.data["name"]),
+    },
+)
+
+env = create_local_patterns("nonebot")
+env.sets([_At, _Image, _Video, _Voice, _Audio, _File, _Segment])
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/console.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/console.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from arclet.alconna import argv_config, set_default_argv_type
-from nonebot.adapters.console.message import BaseMessage
-from nonebot.adapters.console.message import Emoji as _Emoji
-from nonebot.adapters.console.message import Markdown as _Markdown
-from nonebot.adapters.console.message import Markup as _Markup
-from nonebot.adapters.console.message import Message, MessageSegment
-from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot_plugin_alconna.typings import SegmentPattern
-
-
-class ConsoleMessageArgv(MessageArgv):
-    ...
-
-
-set_default_argv_type(ConsoleMessageArgv)
-argv_config(
-    ConsoleMessageArgv,
-    filter_out=[],
-    checker=lambda x: isinstance(x, BaseMessage),
-    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
-    converter=lambda x: Message(x)
-)
-
-Emoji = SegmentPattern("emoji", _Emoji, MessageSegment.emoji)
-Markup = SegmentPattern("markup", _Markup, MessageSegment.markup)
-Markdown = SegmentPattern("markdown", _Markdown, MessageSegment.markdown)
-
-Text = str
+from nonebot.adapters.console.message import Message
+from nonebot.adapters.console.message import Emoji as _Emoji
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.console.message import Markup as _Markup
+from nonebot.adapters.console.message import Markdown as _Markdown
+from nonebot.adapters.console.message import BaseMessage, MessageSegment
+
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
+
+
+class ConsoleMessageArgv(MessageArgv):
+    ...
+
+
+set_default_argv_type(ConsoleMessageArgv)
+argv_config(
+    ConsoleMessageArgv,
+    filter_out=[],
+    checker=lambda x: isinstance(x, BaseMessage),
+    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
+    converter=lambda x: Message(x),
+)
+
+Emoji = SegmentPattern("emoji", _Emoji, MessageSegment.emoji)
+Markup = SegmentPattern("markup", _Markup, MessageSegment.markup)
+Markdown = SegmentPattern("markdown", _Markdown, MessageSegment.markdown)
+
+Text = str
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/ding.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/mirai.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,87 @@
-from arclet.alconna import argv_config, set_default_argv_type
-from nonebot.adapters.ding.message import BaseMessage, Message, MessageSegment
-from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot_plugin_alconna.typings import SegmentPattern
-
-
-class DingMessageArgv(MessageArgv):
-    ...
-
-
-set_default_argv_type(DingMessageArgv)
-argv_config(
-    DingMessageArgv,
-    filter_out=[],
-    checker=lambda x: isinstance(x, BaseMessage),
-    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
-    converter=lambda x: Message(x)
-)
-
-Text = str
-AtAll = SegmentPattern(
-    "at", MessageSegment, MessageSegment.atAll, lambda x: "isAtAll" in x.data
-)
-AtMobiles = SegmentPattern(
-    "at", MessageSegment, MessageSegment.atMobiles, lambda x: "atMobiles" in x.data
-)
-AtDingtalkIds = SegmentPattern(
-    "at",
-    MessageSegment,
-    MessageSegment.atDingtalkIds,
-    lambda x: "atDingtalkIds" in x.data,
-)
-Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
-Extension = SegmentPattern("extension", MessageSegment, MessageSegment.extension)
-Markdown = SegmentPattern("markdown", MessageSegment, MessageSegment.markdown)
-ActionCardSingleBtn = SegmentPattern(
-    "actionCard",
-    MessageSegment,
-    MessageSegment.actionCardSingleBtn,
-    lambda x: "singleTitle" in x.data,
-)
-ActionCardMultiBtns = SegmentPattern(
-    "actionCard",
-    MessageSegment,
-    MessageSegment.actionCardMultiBtns,
-    lambda x: "btns" in x.data,
-)
-FeedCard = SegmentPattern("feedCard", MessageSegment, MessageSegment.feedCard)
-Raw = SegmentPattern("raw", MessageSegment, MessageSegment.raw)
+from nepattern.main import INTEGER
+from arclet.alconna import argv_config, set_default_argv_type
+from nepattern import URL, BasePattern, PatternModel, UnionPattern
+from nonebot.adapters.mirai2.message import BaseMessage, MessageChain, MessageSegment
+
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
+
+
+class MiraiMessageArgv(MessageArgv):
+    ...
+
+
+set_default_argv_type(MiraiMessageArgv)
+argv_config(
+    MiraiMessageArgv,
+    filter_out=[],
+    checker=lambda x: isinstance(x, BaseMessage),
+    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
+    converter=lambda x: MessageChain(x),
+)
+
+Source = SegmentPattern("Source", MessageSegment, MessageSegment.source)
+Quote = SegmentPattern("Quote", MessageSegment, MessageSegment.quote)
+Plain = str
+At = SegmentPattern("At", MessageSegment, MessageSegment.at)
+AtAll = SegmentPattern("AtAll", MessageSegment, MessageSegment.at_all)
+Face = SegmentPattern("Face", MessageSegment, MessageSegment.face)
+Image = SegmentPattern("Image", MessageSegment, MessageSegment.image)
+FlashImage = SegmentPattern("FlashImage", MessageSegment, MessageSegment.flash_image)
+Voice = SegmentPattern("Voice", MessageSegment, MessageSegment.voice)
+Xml = SegmentPattern("Xml", MessageSegment, MessageSegment.xml)
+Json = SegmentPattern("Json", MessageSegment, MessageSegment.json)
+App = SegmentPattern("App", MessageSegment, MessageSegment.app)
+Dice = SegmentPattern("Dice", MessageSegment, MessageSegment.Dice)
+Poke = SegmentPattern("Poke", MessageSegment, MessageSegment.poke)
+MarketFace = SegmentPattern("MarketFace", MessageSegment, MessageSegment.market_face)
+MusicShare = SegmentPattern("MusicShare", MessageSegment, MessageSegment.music_share)
+Forward = SegmentPattern("Forward", MessageSegment, MessageSegment.forward)
+File = SegmentPattern("File", MessageSegment, MessageSegment.file)
+MiraiCode = SegmentPattern("MiraiCode", MessageSegment, MessageSegment.mirai_code)
+
+
+ImgOrUrl = (
+    UnionPattern(
+        [
+            BasePattern(
+                model=PatternModel.TYPE_CONVERT,
+                origin=str,
+                converter=lambda _, x: x.data["url"],
+                alias="img",
+                accepts=[Image],
+            ),
+            URL,
+        ]
+    )
+    @ "img_url"
+)
+"""
+内置类型, 允许传入图片元素(Image)或者链接(URL)，返回链接
+"""
+
+AtID = (
+    UnionPattern(
+        [
+            BasePattern(
+                model=PatternModel.TYPE_CONVERT,
+                origin=int,
+                alias="At",
+                accepts=[At],
+                converter=lambda _, x: int(x.data["target"]),
+            ),
+            BasePattern(
+                r"@(\d+)",
+                model=PatternModel.REGEX_CONVERT,
+                origin=int,
+                alias="@xxx",
+                accepts=[str],
+            ),
+            INTEGER,
+        ]
+    )
+    @ "at_id"
+)
+"""
+内置类型，允许传入提醒元素(At)或者'@xxxx'式样的字符串或者数字, 返回数字
+"""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/feishu.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/feishu.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-from arclet.alconna import argv_config, set_default_argv_type
-from nepattern import BasePattern, PatternModel, UnionPattern
-from nepattern.main import INTEGER
-from nonebot.adapters.feishu.message import BaseMessage, Message, MessageSegment
-from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot_plugin_alconna.typings import SegmentPattern
-
-
-class FeishuMessageArgv(MessageArgv):
-    ...
-
-
-set_default_argv_type(FeishuMessageArgv)
-argv_config(
-    FeishuMessageArgv,
-    filter_out=[],
-    checker=lambda x: isinstance(x, BaseMessage),
-    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
-    converter=lambda x: Message(x)
-)
-
-Text = str
-At = SegmentPattern("at", MessageSegment, MessageSegment.at)
-Post = SegmentPattern("post", MessageSegment, MessageSegment.post)
-Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
-Interactive = SegmentPattern("interactive", MessageSegment, MessageSegment.interactive)
-ShareChat = SegmentPattern("share_chat", MessageSegment, MessageSegment.share_chat)
-ShareUser = SegmentPattern("share_user", MessageSegment, MessageSegment.share_user)
-Audio = SegmentPattern("audio", MessageSegment, MessageSegment.audio)
-Media = SegmentPattern("media", MessageSegment, MessageSegment.media)
-File = SegmentPattern("File", MessageSegment, MessageSegment.file)
-Sticker = SegmentPattern("sticker", MessageSegment, MessageSegment.sticker)
-
-
-AtID = (
-    UnionPattern(
-        [
-            BasePattern(
-                model=PatternModel.TYPE_CONVERT,
-                origin=int,
-                alias="At",
-                accepts=[At],
-                converter=lambda _, x: int(x.data['user_id']),
-            ),
-            BasePattern(
-                r"@(\d+)",
-                model=PatternModel.REGEX_CONVERT,
-                origin=int,
-                alias="@xxx",
-                accepts=[str],
-            ),
-            INTEGER,
-        ]
-    )
-    @ "at_id"
-)
-"""
-内置类型，允许传入提醒元素(At)或者'@xxxx'式样的字符串或者数字, 返回数字
-"""
+from nepattern.main import INTEGER
+from arclet.alconna import argv_config, set_default_argv_type
+from nepattern import BasePattern, PatternModel, UnionPattern
+from nonebot.adapters.feishu.message import Message, BaseMessage, MessageSegment
+
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
+
+
+class FeishuMessageArgv(MessageArgv):
+    ...
+
+
+set_default_argv_type(FeishuMessageArgv)
+argv_config(
+    FeishuMessageArgv,
+    filter_out=[],
+    checker=lambda x: isinstance(x, BaseMessage),
+    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
+    converter=lambda x: Message(x),
+)
+
+Text = str
+At = SegmentPattern("at", MessageSegment, MessageSegment.at)
+Post = SegmentPattern("post", MessageSegment, MessageSegment.post)
+Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
+Interactive = SegmentPattern("interactive", MessageSegment, MessageSegment.interactive)
+ShareChat = SegmentPattern("share_chat", MessageSegment, MessageSegment.share_chat)
+ShareUser = SegmentPattern("share_user", MessageSegment, MessageSegment.share_user)
+Audio = SegmentPattern("audio", MessageSegment, MessageSegment.audio)
+Media = SegmentPattern("media", MessageSegment, MessageSegment.media)
+File = SegmentPattern("File", MessageSegment, MessageSegment.file)
+Sticker = SegmentPattern("sticker", MessageSegment, MessageSegment.sticker)
+
+
+AtID = (
+    UnionPattern(
+        [
+            BasePattern(
+                model=PatternModel.TYPE_CONVERT,
+                origin=int,
+                alias="At",
+                accepts=[At],
+                converter=lambda _, x: int(x.data["user_id"]),
+            ),
+            BasePattern(
+                r"@(\d+)",
+                model=PatternModel.REGEX_CONVERT,
+                origin=int,
+                alias="@xxx",
+                accepts=[str],
+            ),
+            INTEGER,
+        ]
+    )
+    @ "at_id"
+)
+"""
+内置类型，允许传入提醒元素(At)或者'@xxxx'式样的字符串或者数字, 返回数字
+"""
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/kook.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/kook.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from arclet.alconna import argv_config, set_default_argv_type
-from nonebot.adapters.kaiheila.message import BaseMessage, Message, MessageSegment
-from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot_plugin_alconna.typings import SegmentPattern
-
-
-class KookMessageArgv(MessageArgv):
-    ...
-
-
-set_default_argv_type(KookMessageArgv)
-argv_config(
-    KookMessageArgv,
-    filter_out=[],
-    checker=lambda x: isinstance(x, BaseMessage),
-    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
-    converter=lambda x: Message(x)
-)
-
-Text = str
-At = SegmentPattern("at", MessageSegment, MessageSegment.at)
-Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
-Video = SegmentPattern("video", MessageSegment, MessageSegment.video)
-File = SegmentPattern("file", MessageSegment, MessageSegment.file)
-Audio = SegmentPattern("audio", MessageSegment, MessageSegment.audio)
-KMarkdown = SegmentPattern("kmarkdown", MessageSegment, MessageSegment.kmarkdown)
-Card = SegmentPattern("card", MessageSegment, MessageSegment.card)
-Quote = SegmentPattern("quote", MessageSegment, MessageSegment.quote)
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.kaiheila.message import Message, BaseMessage, MessageSegment
+
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
+
+
+class KookMessageArgv(MessageArgv):
+    ...
+
+
+set_default_argv_type(KookMessageArgv)
+argv_config(
+    KookMessageArgv,
+    filter_out=[],
+    checker=lambda x: isinstance(x, BaseMessage),
+    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
+    converter=lambda x: Message(x),
+)
+
+Text = str
+At = SegmentPattern("at", MessageSegment, MessageSegment.at)
+Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
+Video = SegmentPattern("video", MessageSegment, MessageSegment.video)
+File = SegmentPattern("file", MessageSegment, MessageSegment.file)
+Audio = SegmentPattern("audio", MessageSegment, MessageSegment.audio)
+KMarkdown = SegmentPattern("kmarkdown", MessageSegment, MessageSegment.kmarkdown)
+Card = SegmentPattern("card", MessageSegment, MessageSegment.card)
+Quote = SegmentPattern("quote", MessageSegment, MessageSegment.quote)
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/minecraft.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/minecraft.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from arclet.alconna import argv_config, set_default_argv_type
-from nonebot.adapters.minecraft.message import BaseMessage, Message, MessageSegment
-from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot_plugin_alconna.typings import SegmentPattern
-
-
-class MinecraftMessageArgv(MessageArgv):
-    ...
-
-
-set_default_argv_type(MinecraftMessageArgv)
-argv_config(
-    MinecraftMessageArgv,
-    filter_out=[],
-    checker=lambda x: isinstance(x, BaseMessage),
-    to_text=lambda x: x if x.__class__ is str else str(x) if x.type == "text" else None,
-    converter=lambda x: Message(x)
-)
-
-Text = str
-Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
-Video = SegmentPattern("video", MessageSegment, MessageSegment.video)
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.minecraft.message import Message, BaseMessage, MessageSegment
+
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
+
+
+class MinecraftMessageArgv(MessageArgv):
+    ...
+
+
+set_default_argv_type(MinecraftMessageArgv)
+argv_config(
+    MinecraftMessageArgv,
+    filter_out=[],
+    checker=lambda x: isinstance(x, BaseMessage),
+    to_text=lambda x: x if x.__class__ is str else str(x) if x.type == "text" else None,
+    converter=lambda x: Message(x),
+)
+
+Text = str
+Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
+Video = SegmentPattern("video", MessageSegment, MessageSegment.video)
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/mirai.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/onebot11.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,88 @@
-from arclet.alconna import argv_config, set_default_argv_type
-from nepattern import URL, BasePattern, PatternModel, UnionPattern
-from nepattern.main import INTEGER
-from nonebot.adapters.mirai2.message import BaseMessage, MessageChain, MessageSegment
-from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot_plugin_alconna.typings import SegmentPattern
-
-
-class MiraiMessageArgv(MessageArgv):
-    ...
-
-
-set_default_argv_type(MiraiMessageArgv)
-argv_config(
-    MiraiMessageArgv,
-    filter_out=[],
-    checker=lambda x: isinstance(x, BaseMessage),
-    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
-    converter=lambda x: MessageChain(x)
-)
-
-Source = SegmentPattern("Source", MessageSegment, MessageSegment.source)
-Quote = SegmentPattern("Quote", MessageSegment, MessageSegment.quote)
-Plain = str
-At = SegmentPattern("At", MessageSegment, MessageSegment.at)
-AtAll = SegmentPattern("AtAll", MessageSegment, MessageSegment.at_all)
-Face = SegmentPattern("Face", MessageSegment, MessageSegment.face)
-Image = SegmentPattern("Image", MessageSegment, MessageSegment.image)
-FlashImage = SegmentPattern("FlashImage", MessageSegment, MessageSegment.flash_image)
-Voice = SegmentPattern("Voice", MessageSegment, MessageSegment.voice)
-Xml = SegmentPattern("Xml", MessageSegment, MessageSegment.xml)
-Json = SegmentPattern("Json", MessageSegment, MessageSegment.json)
-App = SegmentPattern("App", MessageSegment, MessageSegment.app)
-Dice = SegmentPattern("Dice", MessageSegment, MessageSegment.Dice)
-Poke = SegmentPattern("Poke", MessageSegment, MessageSegment.poke)
-MarketFace = SegmentPattern("MarketFace", MessageSegment, MessageSegment.market_face)
-MusicShare = SegmentPattern("MusicShare", MessageSegment, MessageSegment.music_share)
-Forward = SegmentPattern("Forward", MessageSegment, MessageSegment.forward)
-File = SegmentPattern("File", MessageSegment, MessageSegment.file)
-MiraiCode = SegmentPattern("MiraiCode", MessageSegment, MessageSegment.mirai_code)
-
-
-ImgOrUrl = (
-    UnionPattern(
-        [
-            BasePattern(
-                model=PatternModel.TYPE_CONVERT,
-                origin=str,
-                converter=lambda _, x: x.data['url'],
-                alias="img",
-                accepts=[Image],
-            ),
-            URL,
-        ]
-    )
-    @ "img_url"
-)
-"""
-内置类型, 允许传入图片元素(Image)或者链接(URL)，返回链接
-"""
-
-AtID = (
-    UnionPattern(
-        [
-            BasePattern(
-                model=PatternModel.TYPE_CONVERT,
-                origin=int,
-                alias="At",
-                accepts=[At],
-                converter=lambda _, x: int(x.data['target']),
-            ),
-            BasePattern(
-                r"@(\d+)",
-                model=PatternModel.REGEX_CONVERT,
-                origin=int,
-                alias="@xxx",
-                accepts=[str],
-            ),
-            INTEGER,
-        ]
-    )
-    @ "at_id"
-)
-"""
-内置类型，允许传入提醒元素(At)或者'@xxxx'式样的字符串或者数字, 返回数字
-"""
+from nepattern.main import INTEGER
+from arclet.alconna import argv_config, set_default_argv_type
+from nepattern import URL, BasePattern, PatternModel, UnionPattern
+from nonebot.adapters.onebot.v11.message import Message, BaseMessage, MessageSegment
+
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
+
+
+class Ob11MessageArgv(MessageArgv):
+    ...
+
+
+set_default_argv_type(Ob11MessageArgv)
+argv_config(
+    Ob11MessageArgv,
+    filter_out=[],
+    checker=lambda x: isinstance(x, BaseMessage),
+    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
+    converter=lambda x: Message(x),
+)
+
+Anonymous = SegmentPattern("anonymous", MessageSegment, MessageSegment.anonymous)
+Text = str
+At = SegmentPattern("at", MessageSegment, MessageSegment.at)
+Contact = SegmentPattern("contact", MessageSegment, MessageSegment.contact)
+Dice = SegmentPattern("dice", MessageSegment, MessageSegment.dice)
+Face = SegmentPattern("face", MessageSegment, MessageSegment.face)
+Forward = SegmentPattern("forward", MessageSegment, MessageSegment.forward)
+Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
+Json = SegmentPattern("json", MessageSegment, MessageSegment.json)
+Location = SegmentPattern("location", MessageSegment, MessageSegment.location)
+Music = SegmentPattern("music", MessageSegment, MessageSegment.music)
+Node = SegmentPattern("node", MessageSegment, MessageSegment.node)
+Poke = SegmentPattern("poke", MessageSegment, MessageSegment.poke)
+Record = SegmentPattern("record", MessageSegment, MessageSegment.record)
+Reply = SegmentPattern("reply", MessageSegment, MessageSegment.reply)
+RPS = SegmentPattern("rps", MessageSegment, MessageSegment.rps)
+Shake = SegmentPattern("shake", MessageSegment, MessageSegment.shake)
+Share = SegmentPattern("share", MessageSegment, MessageSegment.share)
+Video = SegmentPattern("video", MessageSegment, MessageSegment.video)
+Xml = SegmentPattern("xml", MessageSegment, MessageSegment.xml)
+
+
+ImgOrUrl = (
+    UnionPattern(
+        [
+            BasePattern(
+                model=PatternModel.TYPE_CONVERT,
+                origin=str,
+                converter=lambda _, x: x.data["url"],
+                alias="img",
+                accepts=[Image],
+            ),
+            URL,
+        ]
+    )
+    @ "img_url"
+)
+"""
+内置类型, 允许传入图片元素(Image)或者链接(URL)，返回链接
+"""
+
+AtID = (
+    UnionPattern(
+        [
+            BasePattern(
+                model=PatternModel.TYPE_CONVERT,
+                origin=int,
+                alias="At",
+                accepts=[At],
+                converter=lambda _, x: int(x.data["qq"]),
+            ),
+            BasePattern(
+                r"@(\d+)",
+                model=PatternModel.REGEX_CONVERT,
+                origin=int,
+                alias="@xxx",
+                accepts=[str],
+            ),
+            INTEGER,
+        ]
+    )
+    @ "at_id"
+)
+"""
+内置类型，允许传入提醒元素(At)或者'@xxxx'式样的字符串或者数字, 返回数字
+"""
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/ntchat.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/ntchat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from arclet.alconna import argv_config, set_default_argv_type
-from nonebot.adapters.ntchat.message import BaseMessage, Message, MessageSegment
-from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot_plugin_alconna.typings import SegmentPattern
-
-
-class WXMessageArgv(MessageArgv):
-    ...
-
-
-set_default_argv_type(WXMessageArgv)
-argv_config(
-    WXMessageArgv,
-    filter_out=[],
-    checker=lambda x: isinstance(x, BaseMessage),
-    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
-    converter=lambda x: Message(x)
-)
-
-Text = str
-RoomAtMsg = SegmentPattern("room_at_msg", MessageSegment, MessageSegment.room_at_msg)
-Card = SegmentPattern("card", MessageSegment, MessageSegment.card)
-Link = SegmentPattern("link", MessageSegment, MessageSegment.link)
-Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
-File = SegmentPattern("file", MessageSegment, MessageSegment.file)
-Video = SegmentPattern("video", MessageSegment, MessageSegment.video)
-XML = SegmentPattern("xml", MessageSegment, MessageSegment.xml)
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.ntchat.message import Message, BaseMessage, MessageSegment
+
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
+
+
+class WXMessageArgv(MessageArgv):
+    ...
+
+
+set_default_argv_type(WXMessageArgv)
+argv_config(
+    WXMessageArgv,
+    filter_out=[],
+    checker=lambda x: isinstance(x, BaseMessage),
+    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
+    converter=lambda x: Message(x),
+)
+
+Text = str
+RoomAtMsg = SegmentPattern("room_at_msg", MessageSegment, MessageSegment.room_at_msg)
+Card = SegmentPattern("card", MessageSegment, MessageSegment.card)
+Link = SegmentPattern("link", MessageSegment, MessageSegment.link)
+Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
+File = SegmentPattern("file", MessageSegment, MessageSegment.file)
+Video = SegmentPattern("video", MessageSegment, MessageSegment.video)
+XML = SegmentPattern("xml", MessageSegment, MessageSegment.xml)
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/onebot11.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/onebot12.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,76 @@
-from arclet.alconna import argv_config, set_default_argv_type
-from nepattern import URL, BasePattern, PatternModel, UnionPattern
-from nepattern.main import INTEGER
-from nonebot.adapters.onebot.v11.message import BaseMessage, Message, MessageSegment
-from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot_plugin_alconna.typings import SegmentPattern
-
-
-class Ob11MessageArgv(MessageArgv):
-    ...
-
-
-set_default_argv_type(Ob11MessageArgv)
-argv_config(
-    Ob11MessageArgv,
-    filter_out=[],
-    checker=lambda x: isinstance(x, BaseMessage),
-    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
-    converter=lambda x: Message(x)
-)
-
-Anonymous = SegmentPattern("anonymous", MessageSegment, MessageSegment.anonymous)
-Text = str
-At = SegmentPattern("at", MessageSegment, MessageSegment.at)
-Contact = SegmentPattern("contact", MessageSegment, MessageSegment.contact)
-Dice = SegmentPattern("dice", MessageSegment, MessageSegment.dice)
-Face = SegmentPattern("face", MessageSegment, MessageSegment.face)
-Forward = SegmentPattern("forward", MessageSegment, MessageSegment.forward)
-Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
-Json = SegmentPattern("json", MessageSegment, MessageSegment.json)
-Location = SegmentPattern("location", MessageSegment, MessageSegment.location)
-Music = SegmentPattern("music", MessageSegment, MessageSegment.music)
-Node = SegmentPattern("node", MessageSegment, MessageSegment.node)
-Poke = SegmentPattern("poke", MessageSegment, MessageSegment.poke)
-Record = SegmentPattern("record", MessageSegment, MessageSegment.record)
-Reply = SegmentPattern("reply", MessageSegment, MessageSegment.reply)
-RPS = SegmentPattern("rps", MessageSegment, MessageSegment.rps)
-Shake = SegmentPattern("shake", MessageSegment, MessageSegment.shake)
-Share = SegmentPattern("share", MessageSegment, MessageSegment.share)
-Video = SegmentPattern("video", MessageSegment, MessageSegment.video)
-Xml = SegmentPattern("xml", MessageSegment, MessageSegment.xml)
-
-
-ImgOrUrl = (
-    UnionPattern(
-        [
-            BasePattern(
-                model=PatternModel.TYPE_CONVERT,
-                origin=str,
-                converter=lambda _, x: x.data['url'],
-                alias="img",
-                accepts=[Image],
-            ),
-            URL,
-        ]
-    )
-    @ "img_url"
-)
-"""
-内置类型, 允许传入图片元素(Image)或者链接(URL)，返回链接
-"""
-
-AtID = (
-    UnionPattern(
-        [
-            BasePattern(
-                model=PatternModel.TYPE_CONVERT,
-                origin=int,
-                alias="At",
-                accepts=[At],
-                converter=lambda _, x: int(x.data['qq']),
-            ),
-            BasePattern(
-                r"@(\d+)",
-                model=PatternModel.REGEX_CONVERT,
-                origin=int,
-                alias="@xxx",
-                accepts=[str],
-            ),
-            INTEGER,
-        ]
-    )
-    @ "at_id"
-)
-"""
-内置类型，允许传入提醒元素(At)或者'@xxxx'式样的字符串或者数字, 返回数字
-"""
+from nepattern.main import URL, INTEGER
+from arclet.alconna import argv_config, set_default_argv_type
+from nepattern import BasePattern, PatternModel, UnionPattern
+from nonebot.adapters.onebot.v12.message import Message, BaseMessage, MessageSegment
+
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
+
+
+class Ob12MessageArgv(MessageArgv):
+    ...
+
+
+set_default_argv_type(Ob12MessageArgv)
+argv_config(
+    Ob12MessageArgv,
+    filter_out=[],
+    checker=lambda x: isinstance(x, BaseMessage),
+    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
+    converter=lambda x: Message(x),
+)
+Text = str
+Mention = SegmentPattern("mention", MessageSegment, MessageSegment.mention)
+MentionAll = SegmentPattern("mention_all", MessageSegment, MessageSegment.mention_all)
+Image = SegmentPattern("image", MessageSegment, MessageSegment.image)
+Audio = SegmentPattern("audio", MessageSegment, MessageSegment.audio)
+Voice = SegmentPattern("voice", MessageSegment, MessageSegment.voice)
+File = SegmentPattern("file", MessageSegment, MessageSegment.file)
+Video = SegmentPattern("video", MessageSegment, MessageSegment.video)
+Location = SegmentPattern("location", MessageSegment, MessageSegment.location)
+Reply = SegmentPattern("reply", MessageSegment, MessageSegment.reply)
+
+ImgOrUrl = (
+    UnionPattern(
+        [
+            BasePattern(
+                model=PatternModel.TYPE_CONVERT,
+                origin=str,
+                converter=lambda _, x: x.data["url"],
+                alias="img",
+                accepts=[Image],
+            ),
+            URL,
+        ]
+    )
+    @ "img_url"
+)
+"""
+内置类型, 允许传入图片元素(Image)或者链接(URL)，返回链接
+"""
+
+MentionID = (
+    UnionPattern(
+        [
+            BasePattern(
+                model=PatternModel.TYPE_CONVERT,
+                origin=int,
+                alias="Mention",
+                accepts=[Mention],
+                converter=lambda _, x: int(x.data["user_id"]),
+            ),
+            BasePattern(
+                r"@(\d+)",
+                model=PatternModel.REGEX_CONVERT,
+                origin=int,
+                alias="@xxx",
+                accepts=[str],
+            ),
+            INTEGER,
+        ]
+    )
+    @ "mention_id"
+)
+"""
+内置类型，允许传入提醒元素(Mention)或者'@xxxx'式样的字符串或者数字, 返回数字
+"""
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/qqguild.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/qqguild.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,94 @@
-from arclet.alconna import argv_config, set_default_argv_type
-from nepattern import BasePattern, PatternModel, UnionPattern
-from nepattern.main import INTEGER, URL
-from nonebot.adapters.qqguild.message import Ark as _Ark
-from nonebot.adapters.qqguild.message import Attachment as _Attachment
-from nonebot.adapters.qqguild.message import BaseMessage
-from nonebot.adapters.qqguild.message import Embed as _Embed
-from nonebot.adapters.qqguild.message import Emoji as _Emoji
-from nonebot.adapters.qqguild.message import LocalImage as _LocalImage
-from nonebot.adapters.qqguild.message import MentionChannel as _MentionChannel
-from nonebot.adapters.qqguild.message import MentionEveryone as _MentionEveryone
-from nonebot.adapters.qqguild.message import MentionUser as _MentionUser
-from nonebot.adapters.qqguild.message import Message, MessageSegment
-from nonebot.adapters.qqguild.message import Reference as _Reference
-from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot_plugin_alconna.typings import SegmentPattern
-
-
-class QQGuildMessageArgv(MessageArgv):
-    ...
-
-
-set_default_argv_type(QQGuildMessageArgv)
-argv_config(
-    QQGuildMessageArgv,
-    filter_out=[],
-    checker=lambda x: isinstance(x, BaseMessage),
-    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
-    converter=lambda x: Message(x)
-)
-
-
-Text = str
-Ark = SegmentPattern("ark", _Ark, MessageSegment.ark)
-Embed = SegmentPattern("embed", _Embed, MessageSegment.embed)
-Emoji = SegmentPattern("emoji", _Emoji, MessageSegment.emoji)
-Image = SegmentPattern("attachment", _Attachment, MessageSegment.image)
-FileImage = SegmentPattern("file_image", _LocalImage, MessageSegment.file_image)
-MentionUser = SegmentPattern("mention_user", _MentionUser, MessageSegment.mention_user)
-MentionChannel = SegmentPattern(
-    "mention_channel", _MentionChannel, MessageSegment.mention_channel
-)
-MentionEveryone = SegmentPattern(
-    "mention_everyone", _MentionEveryone, MessageSegment.mention_everyone
-)
-Reference = SegmentPattern("reference", _Reference, MessageSegment.reference)
-
-
-ImgOrUrl = (
-    UnionPattern(
-        [
-            BasePattern(
-                model=PatternModel.TYPE_CONVERT,
-                origin=str,
-                converter=lambda _, x: x.data['url'],
-                alias="img",
-                accepts=[Image],
-            ),
-            URL,
-        ]
-    )
-    @ "img_url"
-)
-"""
-内置类型, 允许传入图片元素(Image)或者链接(URL)，返回链接
-"""
-
-MentionID = (
-    UnionPattern(
-        [
-            BasePattern(
-                model=PatternModel.TYPE_CONVERT,
-                origin=int,
-                alias="MentionUser",
-                accepts=[MentionUser],
-                converter=lambda _, x: int(x.data["user_id"]),
-            ),
-            BasePattern(
-                r"@(\d+)",
-                model=PatternModel.REGEX_CONVERT,
-                origin=int,
-                alias="@xxx",
-                accepts=[str],
-            ),
-            INTEGER,
-        ]
-    )
-    @ "mention_id"
-)
-"""
-内置类型，允许传入提醒元素(Mention)或者'@xxxx'式样的字符串或者数字, 返回数字
-"""
+from nepattern.main import URL, INTEGER
+from nonebot.adapters.qqguild.message import Message
+from nonebot.adapters.qqguild.message import Ark as _Ark
+from nonebot.adapters.qqguild.message import BaseMessage
+from nonebot.adapters.qqguild.message import MessageSegment
+from nonebot.adapters.qqguild.message import Embed as _Embed
+from nonebot.adapters.qqguild.message import Emoji as _Emoji
+from arclet.alconna import argv_config, set_default_argv_type
+from nepattern import BasePattern, PatternModel, UnionPattern
+from nonebot.adapters.qqguild.message import Reference as _Reference
+from nonebot.adapters.qqguild.message import Attachment as _Attachment
+from nonebot.adapters.qqguild.message import LocalImage as _LocalImage
+from nonebot.adapters.qqguild.message import MentionUser as _MentionUser
+from nonebot.adapters.qqguild.message import MentionChannel as _MentionChannel
+from nonebot.adapters.qqguild.message import MentionEveryone as _MentionEveryone
+
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
+
+
+class QQGuildMessageArgv(MessageArgv):
+    ...
+
+
+set_default_argv_type(QQGuildMessageArgv)
+argv_config(
+    QQGuildMessageArgv,
+    filter_out=[],
+    checker=lambda x: isinstance(x, BaseMessage),
+    to_text=lambda x: x if x.__class__ is str else str(x) if x.is_text() else None,
+    converter=lambda x: Message(x),
+)
+
+
+Text = str
+Ark = SegmentPattern("ark", _Ark, MessageSegment.ark)
+Embed = SegmentPattern("embed", _Embed, MessageSegment.embed)
+Emoji = SegmentPattern("emoji", _Emoji, MessageSegment.emoji)
+Image = SegmentPattern("attachment", _Attachment, MessageSegment.image)
+FileImage = SegmentPattern("file_image", _LocalImage, MessageSegment.file_image)
+MentionUser = SegmentPattern("mention_user", _MentionUser, MessageSegment.mention_user)
+MentionChannel = SegmentPattern(
+    "mention_channel", _MentionChannel, MessageSegment.mention_channel
+)
+MentionEveryone = SegmentPattern(
+    "mention_everyone", _MentionEveryone, MessageSegment.mention_everyone
+)
+Reference = SegmentPattern("reference", _Reference, MessageSegment.reference)
+
+
+ImgOrUrl = (
+    UnionPattern(
+        [
+            BasePattern(
+                model=PatternModel.TYPE_CONVERT,
+                origin=str,
+                converter=lambda _, x: x.data["url"],
+                alias="img",
+                accepts=[Image],
+            ),
+            URL,
+        ]
+    )
+    @ "img_url"
+)
+"""
+内置类型, 允许传入图片元素(Image)或者链接(URL)，返回链接
+"""
+
+MentionID = (
+    UnionPattern(
+        [
+            BasePattern(
+                model=PatternModel.TYPE_CONVERT,
+                origin=int,
+                alias="MentionUser",
+                accepts=[MentionUser],
+                converter=lambda _, x: int(x.data["user_id"]),
+            ),
+            BasePattern(
+                r"@(\d+)",
+                model=PatternModel.REGEX_CONVERT,
+                origin=int,
+                alias="@xxx",
+                accepts=[str],
+            ),
+            INTEGER,
+        ]
+    )
+    @ "mention_id"
+)
+"""
+内置类型，允许传入提醒元素(Mention)或者'@xxxx'式样的字符串或者数字, 返回数字
+"""
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/telegram.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/adapters/telegram.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,86 @@
-from arclet.alconna import argv_config, set_default_argv_type
-from nepattern import UnionPattern
-from nonebot.adapters.telegram.message import (
-    BaseMessage,
-    Entity,
-    File,
-    Message,
-    MessageSegment,
-    UnCombinFile,
-)
-from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot_plugin_alconna.typings import SegmentPattern
-
-
-class TelegramMessageArgv(MessageArgv):
-    ...
-
-
-def is_text(x: MessageSegment):
-    return x.type in {"text", "bold", "italic", "underline", "strikethrough", "spoiler", "code"}
-
-
-set_default_argv_type(TelegramMessageArgv)
-argv_config(
-    TelegramMessageArgv,
-    filter_out=[],
-    checker=lambda x: isinstance(x, BaseMessage),
-    to_text=lambda x: x if x.__class__ is str else str(x) if is_text(x) else None,
-    converter=lambda x: Message(x)
-)
-
-Text = str
-Location = SegmentPattern("location", MessageSegment, MessageSegment.location)
-Venue = SegmentPattern("venue", MessageSegment, MessageSegment.venue)
-Poll = SegmentPattern("poll", MessageSegment, MessageSegment.poll)
-Dice = SegmentPattern("dice", MessageSegment, MessageSegment.dice)
-ChatAction = SegmentPattern("chat_action", MessageSegment, MessageSegment.chat_action)
-
-Mention = SegmentPattern("mention", Entity, Entity.mention)
-Hashtag = SegmentPattern("hashtag", Entity, Entity.hashtag)
-Cashtag = SegmentPattern("cashtag", Entity, Entity.cashtag)
-BotCommand = SegmentPattern("bot_command", Entity, Entity.bot_command)
-Url = SegmentPattern("url", Entity, Entity.url)
-Email = SegmentPattern("email", Entity, Entity.email)
-PhoneNumber = SegmentPattern("phone_number", Entity, Entity.phone_number)
-Bold = SegmentPattern("bold", Entity, Entity.bold)
-"""该 Pattern 只用于发送"""
-Italic = SegmentPattern("italic", Entity, Entity.italic)
-"""该 Pattern 只用于发送"""
-Underline = SegmentPattern("underline", Entity, Entity.underline)
-"""该 Pattern 只用于发送"""
-Strikethrough = SegmentPattern("strikethrough", Entity, Entity.strikethrough)
-"""该 Pattern 只用于发送"""
-Spoiler = SegmentPattern("spoiler", Entity, Entity.spoiler)
-"""该 Pattern 只用于发送"""
-Code = SegmentPattern("code", Entity, Entity.code)
-"""该 Pattern 只用于发送"""
-Pre = SegmentPattern("pre", Entity, Entity.pre)
-TextLink = SegmentPattern("text_link", Entity, Entity.text_link)
-TextMention = SegmentPattern("text_mention", Entity, Entity.text_mention)
-CustomEmoji = SegmentPattern("custom_emoji", Entity, Entity.custom_emoji)
-
-Image = Photo = SegmentPattern("photo", File, File.photo)
-Voice = SegmentPattern("voice", File, File.voice)
-Animation = SegmentPattern("animation", File, File.animation)
-Audio = SegmentPattern("audio", File, File.audio)
-Document = SegmentPattern("document", File, File.document)
-Video = SegmentPattern("video", File, File.video)
-
-Sticker = SegmentPattern("sticker", UnCombinFile, UnCombinFile.sticker)
-VideoNote = SegmentPattern("video_note", UnCombinFile, UnCombinFile.video_note)
-
-Mentions = UnionPattern([Mention, TextMention, TextLink])
-"""联合接收 Mention, TextMention, TextLink, 不能用于发送"""
-
-Videos = UnionPattern([Video, Animation])
-"""联合接收 Video, Animation, 不能用于发送"""
+from nepattern import UnionPattern
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.telegram.message import (
+    File,
+    Entity,
+    Message,
+    BaseMessage,
+    UnCombinFile,
+    MessageSegment,
+)
+
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
+
+
+class TelegramMessageArgv(MessageArgv):
+    ...
+
+
+def is_text(x: MessageSegment):
+    return x.type in {
+        "text",
+        "bold",
+        "italic",
+        "underline",
+        "strikethrough",
+        "spoiler",
+        "code",
+    }
+
+
+set_default_argv_type(TelegramMessageArgv)
+argv_config(
+    TelegramMessageArgv,
+    filter_out=[],
+    checker=lambda x: isinstance(x, BaseMessage),
+    to_text=lambda x: x if x.__class__ is str else str(x) if is_text(x) else None,
+    converter=lambda x: Message(x),
+)
+
+Text = str
+Location = SegmentPattern("location", MessageSegment, MessageSegment.location)
+Venue = SegmentPattern("venue", MessageSegment, MessageSegment.venue)
+Poll = SegmentPattern("poll", MessageSegment, MessageSegment.poll)
+Dice = SegmentPattern("dice", MessageSegment, MessageSegment.dice)
+ChatAction = SegmentPattern("chat_action", MessageSegment, MessageSegment.chat_action)
+
+Mention = SegmentPattern("mention", Entity, Entity.mention)
+Hashtag = SegmentPattern("hashtag", Entity, Entity.hashtag)
+Cashtag = SegmentPattern("cashtag", Entity, Entity.cashtag)
+BotCommand = SegmentPattern("bot_command", Entity, Entity.bot_command)
+Url = SegmentPattern("url", Entity, Entity.url)
+Email = SegmentPattern("email", Entity, Entity.email)
+PhoneNumber = SegmentPattern("phone_number", Entity, Entity.phone_number)
+Bold = SegmentPattern("bold", Entity, Entity.bold)
+"""该 Pattern 只用于发送"""
+Italic = SegmentPattern("italic", Entity, Entity.italic)
+"""该 Pattern 只用于发送"""
+Underline = SegmentPattern("underline", Entity, Entity.underline)
+"""该 Pattern 只用于发送"""
+Strikethrough = SegmentPattern("strikethrough", Entity, Entity.strikethrough)
+"""该 Pattern 只用于发送"""
+Spoiler = SegmentPattern("spoiler", Entity, Entity.spoiler)
+"""该 Pattern 只用于发送"""
+Code = SegmentPattern("code", Entity, Entity.code)
+"""该 Pattern 只用于发送"""
+Pre = SegmentPattern("pre", Entity, Entity.pre)
+TextLink = SegmentPattern("text_link", Entity, Entity.text_link)
+TextMention = SegmentPattern("text_mention", Entity, Entity.text_mention)
+CustomEmoji = SegmentPattern("custom_emoji", Entity, Entity.custom_emoji)
+
+Image = Photo = SegmentPattern("photo", File, File.photo)
+Voice = SegmentPattern("voice", File, File.voice)
+Animation = SegmentPattern("animation", File, File.animation)
+Audio = SegmentPattern("audio", File, File.audio)
+Document = SegmentPattern("document", File, File.document)
+Video = SegmentPattern("video", File, File.video)
+
+Sticker = SegmentPattern("sticker", UnCombinFile, UnCombinFile.sticker)
+VideoNote = SegmentPattern("video_note", UnCombinFile, UnCombinFile.video_note)
+
+Mentions = UnionPattern([Mention, TextMention, TextLink])
+"""联合接收 Mention, TextMention, TextLink, 不能用于发送"""
+
+Videos = UnionPattern([Video, Animation])
+"""联合接收 Video, Animation, 不能用于发送"""
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/matcher.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/matcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,102 @@
-from __future__ import annotations
-
-from typing import Callable
-
-from arclet.alconna import Alconna, command_manager
-from arclet.alconna.tools import AlconnaFormat
-from arclet.alconna.tools.construct import FuncMounter
-from tarina import is_awaitable
-from nonebot.matcher import Matcher
-from nonebot.plugin.on import on_message
-from nonebot.rule import Rule
-from nonebot.typing import T_RuleChecker
-from nonebot.internal.adapter import Bot, Event, Message, MessageSegment
-
-from .model import CompConfig
-from .rule import alconna
-from .typings import TConvert
-
-
-def on_alconna(
-    command: Alconna | str,
-    rule: Rule | T_RuleChecker | None = None,
-    skip_for_unmatch: bool = True,
-    auto_send_output: bool = False,
-    output_converter: TConvert | None = None,
-    aliases: set[str | tuple[str, ...]] | None = None,
-    comp_config: CompConfig | None = None,
-    *args,
-    _depth: int = 0,
-    **kwargs,
-) -> type[Matcher]:
-    """注册一个消息事件响应器，并且当消息由指定 Alconna 解析并传出有效结果时响应。
-
-    参数:
-        command: Alconna 命令
-        rule: 事件响应规则
-        skip_for_unmatch: 是否在解析失败时跳过
-        auto_send_output: 是否自动发送输出信息并跳过
-        output_converter: 输出信息字符串转换为 Message 方法
-        aliases: 命令别名
-        comp_config: 补全会话配置, 不传入则不启用补全会话
-        permission: 事件响应权限
-        handlers: 事件处理函数列表
-        temp: 是否为临时事件响应器（仅执行一次）
-        expire_time: 事件响应器最终有效时间点，过时即被删除
-        priority: 事件响应器优先级
-        block: 是否阻止事件向更低优先级传递
-        state: 默认 state
-    """
-    if isinstance(command, str):
-        command = AlconnaFormat(command)
-    if aliases and command.command:
-        command_manager.delete(command)
-        aliases.add(str(command.command))
-        command.command = "re:(" + "|".join(aliases) + ")"
-        command._hash = command._calc_hash()
-        command_manager.register(command)
-    return on_message(
-        alconna(
-            command,
-            skip_for_unmatch,
-            auto_send_output,
-            output_converter,
-            comp_config
-        ) & rule,
-        *args,
-        **kwargs,
-        _depth=_depth + 1  # type: ignore
-    )
-
-
-def funcommand(
-    name: str | None = None,
-    prefixes: list[str] | None = None,
-    description: str | None = None,
-):
-    _config = {"raise_exception": False}
-    if name:
-        _config["name"] = name
-    if prefixes:
-        _config["prefixes"] = prefixes
-    if description:
-        _config["description"] = description
-    def wrapper(func: Callable) -> type[Matcher]:
-        alc = FuncMounter(func, _config)  # type: ignore
-
-        async def handle(bot: Bot, event: Event):
-            msg = getattr(event, "original_message", event.get_message())
-            try:
-                arp, res = alc.exec(msg)
-            except Exception as e:
-                if _config["raise_exception"]:
-                    raise e
-                await bot.send(event, str(e))
-                return
-            if arp.matched:
-                if is_awaitable(res):
-                    res = await res
-                if isinstance(res, (str, Message, MessageSegment)):
-                    await bot.send(event, res)
-
-        matcher = on_alconna(alc)
-        matcher.handle()(handle)
-
-        return matcher
-
-    return wrapper
+from __future__ import annotations
+
+from typing import Callable
+
+from nonebot.rule import Rule
+from tarina import is_awaitable
+from nonebot.matcher import Matcher
+from nonebot.plugin.on import on_message
+from nonebot.typing import T_RuleChecker
+from arclet.alconna.tools import AlconnaFormat
+from arclet.alconna import Alconna, command_manager
+from arclet.alconna.tools.construct import FuncMounter
+from nonebot.internal.adapter import Bot, Event, Message, MessageSegment
+
+from .rule import alconna
+from .model import CompConfig
+from .typings import TConvert
+from .params import AlcExecResult
+
+
+def on_alconna(
+    command: Alconna | str,
+    rule: Rule | T_RuleChecker | None = None,
+    skip_for_unmatch: bool = True,
+    auto_send_output: bool = False,
+    output_converter: TConvert | None = None,
+    aliases: set[str | tuple[str, ...]] | None = None,
+    comp_config: CompConfig | None = None,
+    *args,
+    _depth: int = 0,
+    **kwargs,
+) -> type[Matcher]:
+    """注册一个消息事件响应器，并且当消息由指定 Alconna 解析并传出有效结果时响应。
+
+    参数:
+        command: Alconna 命令
+        rule: 事件响应规则
+        skip_for_unmatch: 是否在解析失败时跳过
+        auto_send_output: 是否自动发送输出信息并跳过
+        output_converter: 输出信息字符串转换为 Message 方法
+        aliases: 命令别名
+        comp_config: 补全会话配置, 不传入则不启用补全会话
+        permission: 事件响应权限
+        handlers: 事件处理函数列表
+        temp: 是否为临时事件响应器（仅执行一次）
+        expire_time: 事件响应器最终有效时间点，过时即被删除
+        priority: 事件响应器优先级
+        block: 是否阻止事件向更低优先级传递
+        state: 默认 state
+    """
+    if isinstance(command, str):
+        command = AlconnaFormat(command)
+    if aliases and command.command:
+        command_manager.delete(command)
+        aliases.add(str(command.command))
+        command.command = "re:(" + "|".join(aliases) + ")"
+        command._hash = command._calc_hash()
+        command_manager.register(command)
+    return on_message(
+        alconna(
+            command, skip_for_unmatch, auto_send_output, output_converter, comp_config
+        )
+        & rule,
+        *args,
+        **kwargs,
+        _depth=_depth + 1,  # type: ignore
+    )
+
+
+def funcommand(
+    name: str | None = None,
+    prefixes: list[str] | None = None,
+    description: str | None = None,
+    rule: Rule | T_RuleChecker | None = None,
+    *args,
+    _depth: int = 0,
+    **kwargs,
+):
+    _config = {"raise_exception": False}
+    if name:
+        _config["command"] = name
+    if prefixes:
+        _config["prefixes"] = prefixes
+    if description:
+        _config["description"] = description
+
+    def wrapper(func: Callable) -> type[Matcher]:
+        alc = FuncMounter(func, _config)  # type: ignore
+
+        async def handle(bot: Bot, event: Event, results: AlcExecResult):
+            if res := results.get(func.__name__):
+                if is_awaitable(res):
+                    res = await res
+                if isinstance(res, (str, Message, MessageSegment)):
+                    await bot.send(event, res)
+
+        matcher = on_alconna(alc, rule, *args, **kwargs, _depth=_depth + 1)
+        matcher.handle()(handle)
+
+        return matcher
+
+    return wrapper
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/model.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,64 @@
-from dataclasses import dataclass, field
-from typing import Generic, Optional, TypedDict, TypeVar
-from typing_extensions import NotRequired
-
-from arclet.alconna import Alconna, Arparma, Empty
-from arclet.alconna.duplication import Duplication
-
-T = TypeVar("T")
-T_Duplication = TypeVar("T_Duplication", bound=Duplication)
-
-
-@dataclass
-class Match(Generic[T]):
-    """
-    匹配项，表示参数是否存在于 `all_matched_args` 内
-    result (T): 匹配结果
-    available (bool): 匹配状态
-    """
-
-    result: T
-    available: bool
-
-
-class Query(Generic[T]):
-    """
-    查询项，表示参数是否可由 `Arparma.query` 查询并获得结果
-
-    result (T): 查询结果
-
-    available (bool): 查询状态
-
-    path (str): 查询路径
-    """
-    result: T
-    available: bool
-    path: str
-
-    def __init__(self, path: str, default: T = Empty):
-        self.path = path
-        self.result = default
-        self.available = False
-
-    def __repr__(self):
-        return f"Query({self.path}, {self.result})"
-
-
-@dataclass(frozen=True)
-class CommandResult:
-    source: Alconna
-    result: Arparma
-    output: Optional[str] = field(default=None)
-
-    @property
-    def matched(self) -> bool:
-        return self.result.matched
-
-
-class CompConfig(TypedDict):
-    priority: NotRequired[int]
-    tab: NotRequired[str]
-    enter: NotRequired[str]
-    exit: NotRequired[str]
-    timeout: NotRequired[int]
+from dataclasses import field, dataclass
+from typing_extensions import NotRequired
+from typing import Generic, TypeVar, Optional, TypedDict
+
+from arclet.alconna import Empty, Alconna, Arparma
+from arclet.alconna.duplication import Duplication
+
+T = TypeVar("T")
+T_Duplication = TypeVar("T_Duplication", bound=Duplication)
+
+
+@dataclass
+class Match(Generic[T]):
+    """
+    匹配项，表示参数是否存在于 `all_matched_args` 内
+    result (T): 匹配结果
+    available (bool): 匹配状态
+    """
+
+    result: T
+    available: bool
+
+
+class Query(Generic[T]):
+    """
+    查询项，表示参数是否可由 `Arparma.query` 查询并获得结果
+
+    result (T): 查询结果
+
+    available (bool): 查询状态
+
+    path (str): 查询路径
+    """
+
+    result: T
+    available: bool
+    path: str
+
+    def __init__(self, path: str, default: T = Empty):
+        self.path = path
+        self.result = default
+        self.available = False
+
+    def __repr__(self):
+        return f"Query({self.path}, {self.result})"
+
+
+@dataclass(frozen=True)
+class CommandResult:
+    source: Alconna
+    result: Arparma
+    output: Optional[str] = field(default=None)
+
+    @property
+    def matched(self) -> bool:
+        return self.result.matched
+
+
+class CompConfig(TypedDict):
+    priority: NotRequired[int]
+    tab: NotRequired[str]
+    enter: NotRequired[str]
+    exit: NotRequired[str]
+    timeout: NotRequired[int]
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/rule.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,225 +1,252 @@
-import asyncio
-import traceback
-from typing import ClassVar, Dict, Optional, Union
-
-from arclet.alconna import (
-    Alconna,
-    AllParam,
-    Args,
-    Arparma,
-    CommandMeta,
-    CompSession,
-    command_manager,
-    output_manager,
-)
-from arclet.alconna.exceptions import SpecialOptionTriggered
-from nonebot import get_driver
-from nonebot.adapters import Bot, Event, Message
-from nonebot.internal.matcher import matchers
-from nonebot.internal.rule import Rule as Rule
-from nonebot.params import EventMessage
-from nonebot.plugin.on import on_message
-from nonebot.typing import T_State
-from nonebot.utils import is_coroutine_callable, run_sync
-from tarina import lang
-
-from .config import Config
-from .consts import ALCONNA_RESULT
-from .model import CommandResult, CompConfig
-from .typings import TConvert
-
-
-class AlconnaRule:
-    """检查消息字符串是否能够通过此 Alconna 命令。
-
-    参数:
-        command: Alconna 命令
-        skip_for_unmatch: 是否在命令不匹配时跳过该响应
-        auto_send_output: 是否自动发送输出信息并跳过响应
-        output_converter: 输出信息字符串转换为 Message 方法
-        comp_config: 自动补全配置
-    """
-
-    default_converter: ClassVar[TConvert] = lambda _, x: Message(x)
-
-    __slots__ = (
-        "command",
-        "skip",
-        "auto_send",
-        "output_converter",
-        "comp_config",
-    )
-
-    def __init__(
-        self,
-        command: Alconna,
-        skip_for_unmatch: bool = True,
-        auto_send_output: bool = False,
-        output_converter: Optional[TConvert] = None,
-        comp_config: Optional[CompConfig] = None,
-    ):
-        self.comp_config = comp_config
-        try:
-            global_config = get_driver().config
-            config = Config.parse_obj(global_config)
-            self.auto_send = auto_send_output or config.alconna_auto_send_output
-            if config.alconna_use_command_start and global_config.command_start:
-                command_manager.delete(command)
-                command.prefixes = list(global_config.command_start)
-                command._hash = command._calc_hash()
-                command_manager.register(command)
-            if config.alconna_auto_completion and not self.comp_config:
-                self.comp_config = {}
-        except ValueError:
-            self.auto_send = auto_send_output
-        self.command = command
-        self.skip = skip_for_unmatch
-        self.output_converter = output_converter or self.__class__.default_converter
-        if not is_coroutine_callable(self.output_converter):
-            self.output_converter = run_sync(self.output_converter)
-
-    def __repr__(self) -> str:
-        return f"Alconna(command={self.command!r})"
-
-    def __eq__(self, other: object) -> bool:
-        return (
-            isinstance(other, AlconnaRule) and self.command.path == other.command.path
-        )
-
-    def __hash__(self) -> int:
-        return hash(self.command.__hash__())
-
-    async def handle(self, bot: Bot, event: Event, msg: Message):
-        interface = CompSession(self.command)
-        if self.comp_config is None:
-            return self.command.parse(msg)
-        res = None
-        with interface:
-            res = self.command.parse(msg)
-        if res:
-            return res
-        meta = CommandMeta(compact=True, hide=True)
-        _tab = Alconna(self.comp_config.get("tab", ".tab"), Args["offset", int, 1], [], meta=meta)
-        _enter = Alconna(self.comp_config.get("enter", ".enter"), Args["content", AllParam, []], [], meta=meta)
-        _exit = Alconna(self.comp_config.get("exit", ".exit"), [], meta=meta)
-
-        _waiter = on_message(priority=self.comp_config.get('priority', -1), block=True)
-        _futures: Dict[str, asyncio.Future] = {}
-        res = Arparma(self.command.path, msg, False, error_info=SpecialOptionTriggered("completion"))
-
-        @_waiter.handle()
-        async def _waiter_handle(_event: Event, content: Message = EventMessage()):
-            if _exit.parse(content).matched:
-                _futures["_"].set_result(False)
-                await _waiter.finish()
-            if (mat := _tab.parse(content)).matched:
-                interface.tab(mat.offset)
-                await _waiter.send(await self._convert("\n".join(interface.lines()), _event, res))
-                await _waiter.skip()
-            if (mat := _enter.parse(content)).matched:
-                _futures["_"].set_result(mat.content)
-                await _waiter.finish()
-            await _waiter.send(await self._convert(interface.current(), _event, res))
-            await _waiter.skip()
-
-        def clear():
-            interface.clear()
-            _waiter.destroy()
-            _waiter.handlers.clear()
-            matchers.pop(-1)
-            command_manager.delete(_tab)
-            command_manager.delete(_enter)
-            command_manager.delete(_exit)
-
-        while interface.available:
-            await bot.send(event, await self._convert(str(interface), event, res))
-            await bot.send(
-                event,
-                await self._convert(
-                    f"{lang.require('comp/nonebot', 'tab').format(cmd=_tab.command)}\n"
-                    f"{lang.require('comp/nonebot', 'enter').format(cmd=_enter.command)}\n"
-                    f"{lang.require('comp/nonebot', 'exit').format(cmd=_exit.command)}",
-                    event, res
-                )
-            )
-            _future = _futures.setdefault("_", asyncio.get_running_loop().create_future())
-            _future.add_done_callback(lambda x: _futures.pop("_"))
-            try:
-                await asyncio.wait_for(_future, timeout=self.comp_config.get('timeout', 60))
-            except asyncio.TimeoutError:
-                await bot.send(event, await self._convert(lang.require('comp/nonebot', 'timeout'), event, res))
-                clear()
-                return res
-            ans: Union[Message, bool] = _future.result()
-            if ans is False:
-                await bot.send(event, await self._convert(lang.require('comp/nonebot', 'exited'), event, res))
-                clear()
-                return res
-            param = list(ans)
-            if not param or not param[0]:
-                param = None
-            try:
-                with interface:
-                    res = interface.enter(param)
-            except Exception as e:
-                traceback.print_exc()
-                await bot.send(event, await self._convert(str(e), event, res))
-        clear()
-        return res
-
-    async def __call__(self, event: Event, state: T_State, bot: Bot) -> bool:
-        if event.get_type() != "message":
-            return False
-        try:
-            msg = getattr(event, "original_message", event.get_message())
-        except (NotImplementedError, ValueError):
-            return False
-        with output_manager.capture(self.command.name) as cap:
-            output_manager.set_action(lambda x: x, self.command.name)
-            try:
-                arp = await self.handle(bot, event, msg)
-            except Exception as e:
-                arp = Arparma(self.command.path, msg, False, error_info=e)
-            may_help_text: Optional[str] = cap.get("output", None)
-        if not arp.matched and not may_help_text and self.skip:
-            return False
-        if not may_help_text and arp.error_info:
-            may_help_text = repr(arp.error_info)
-        if self.auto_send and may_help_text:
-            await bot.send(event, await self._convert(may_help_text, event, arp))
-            return False
-        state[ALCONNA_RESULT] = CommandResult(self.command, arp, may_help_text)
-        return True
-
-    async def _convert(self, text: str, event: Event, arp: Arparma) -> Message:
-        _t = (
-            str(arp.error_info)
-            if isinstance(arp.error_info, SpecialOptionTriggered)
-            else "help"
-        )
-        try:
-            return await self.output_converter(_t, text)  # type: ignore
-        except NotImplementedError:
-            return event.get_message().__class__(text)
-
-
-def alconna(
-    command: Alconna,
-    skip_for_unmatch: bool = True,
-    auto_send_output: bool = False,
-    output_converter: Optional[TConvert] = None,
-    comp_config: Optional[CompConfig] = None,
-) -> Rule:
-    return Rule(
-        AlconnaRule(
-            command,
-            skip_for_unmatch,
-            auto_send_output,
-            output_converter,
-            comp_config,
-        )
-    )
-
-
-def set_output_converter(fn: TConvert):
-    AlconnaRule.default_converter = fn
+import asyncio
+import traceback
+from typing import Dict, Union, ClassVar, Optional
+
+from tarina import lang
+from nonebot import get_driver
+from nonebot.typing import T_State
+from nonebot.params import EventMessage
+from nonebot.plugin.on import on_message
+from nonebot.internal.matcher import matchers
+from nonebot.internal.rule import Rule as Rule
+from nonebot.adapters import Bot, Event, Message
+from nonebot.utils import run_sync, is_coroutine_callable
+from arclet.alconna.exceptions import SpecialOptionTriggered
+from arclet.alconna import (
+    Args,
+    Alconna,
+    Arparma,
+    AllParam,
+    CommandMeta,
+    CompSession,
+    output_manager,
+    command_manager,
+)
+
+from .config import Config
+from .typings import TConvert
+from .model import CompConfig, CommandResult
+from .consts import ALCONNA_RESULT, ALCONNA_EXEC_RESULT
+
+
+class AlconnaRule:
+    """检查消息字符串是否能够通过此 Alconna 命令。
+
+    参数:
+        command: Alconna 命令
+        skip_for_unmatch: 是否在命令不匹配时跳过该响应
+        auto_send_output: 是否自动发送输出信息并跳过响应
+        output_converter: 输出信息字符串转换为 Message 方法
+        comp_config: 自动补全配置
+    """
+
+    default_converter: ClassVar[TConvert] = lambda _, x: Message(x)
+
+    __slots__ = (
+        "command",
+        "skip",
+        "auto_send",
+        "output_converter",
+        "comp_config",
+    )
+
+    def __init__(
+        self,
+        command: Alconna,
+        skip_for_unmatch: bool = True,
+        auto_send_output: bool = False,
+        output_converter: Optional[TConvert] = None,
+        comp_config: Optional[CompConfig] = None,
+    ):
+        self.comp_config = comp_config
+        try:
+            global_config = get_driver().config
+            config = Config.parse_obj(global_config)
+            self.auto_send = auto_send_output or config.alconna_auto_send_output
+            if config.alconna_use_command_start and global_config.command_start:
+                command_manager.delete(command)
+                command.prefixes = list(global_config.command_start)
+                command._hash = command._calc_hash()
+                command_manager.register(command)
+            if config.alconna_auto_completion and not self.comp_config:
+                self.comp_config = {}
+        except ValueError:
+            self.auto_send = auto_send_output
+        self.command = command
+        self.skip = skip_for_unmatch
+        self.output_converter = output_converter or self.__class__.default_converter
+        if not is_coroutine_callable(self.output_converter):
+            self.output_converter = run_sync(self.output_converter)
+
+    def __repr__(self) -> str:
+        return f"Alconna(command={self.command!r})"
+
+    def __eq__(self, other: object) -> bool:
+        return (
+            isinstance(other, AlconnaRule) and self.command.path == other.command.path
+        )
+
+    def __hash__(self) -> int:
+        return hash(self.command.__hash__())
+
+    async def handle(self, bot: Bot, event: Event, msg: Message):
+        interface = CompSession(self.command)
+        if self.comp_config is None:
+            return self.command.parse(msg)
+        res = None
+        with interface:
+            res = self.command.parse(msg)
+        if res:
+            return res
+        meta = CommandMeta(compact=True, hide=True)
+        _tab = Alconna(
+            self.comp_config.get("tab", ".tab"), Args["offset", int, 1], [], meta=meta
+        )
+        _enter = Alconna(
+            self.comp_config.get("enter", ".enter"),
+            Args["content", AllParam, []],
+            [],
+            meta=meta,
+        )
+        _exit = Alconna(self.comp_config.get("exit", ".exit"), [], meta=meta)
+
+        _waiter = on_message(priority=self.comp_config.get("priority", -1), block=True)
+        _futures: Dict[str, asyncio.Future] = {}
+        res = Arparma(
+            self.command.path,
+            msg,
+            False,
+            error_info=SpecialOptionTriggered("completion"),
+        )
+
+        @_waiter.handle()
+        async def _waiter_handle(_event: Event, content: Message = EventMessage()):
+            if _exit.parse(content).matched:
+                _futures["_"].set_result(False)
+                await _waiter.finish()
+            if (mat := _tab.parse(content)).matched:
+                interface.tab(mat.offset)
+                await _waiter.send(
+                    await self._convert("\n".join(interface.lines()), _event, res)
+                )
+                await _waiter.skip()
+            if (mat := _enter.parse(content)).matched:
+                _futures["_"].set_result(mat.content)
+                await _waiter.finish()
+            await _waiter.send(await self._convert(interface.current(), _event, res))
+            await _waiter.skip()
+
+        def clear():
+            interface.clear()
+            _waiter.destroy()
+            _waiter.handlers.clear()
+            matchers.pop(-1)
+            command_manager.delete(_tab)
+            command_manager.delete(_enter)
+            command_manager.delete(_exit)
+
+        help_text = (
+            f"{lang.require('comp/nonebot', 'tab').format(cmd=_tab.command)}\n"
+            f"{lang.require('comp/nonebot', 'enter').format(cmd=_enter.command)}\n"
+            f"{lang.require('comp/nonebot', 'exit').format(cmd=_exit.command)}"
+        )
+
+        while interface.available:
+            await bot.send(event, await self._convert(str(interface), event, res))
+            await bot.send(event, await self._convert(help_text, event, res))
+            _future = _futures.setdefault(
+                "_", asyncio.get_running_loop().create_future()
+            )
+            _future.add_done_callback(lambda x: _futures.pop("_"))
+            try:
+                await asyncio.wait_for(
+                    _future, timeout=self.comp_config.get("timeout", 60)
+                )
+            except asyncio.TimeoutError:
+                await bot.send(
+                    event,
+                    await self._convert(
+                        lang.require("comp/nonebot", "timeout"), event, res
+                    ),
+                )
+                clear()
+                return res
+            ans: Union[Message, bool] = _future.result()
+            if ans is False:
+                await bot.send(
+                    event,
+                    await self._convert(
+                        lang.require("comp/nonebot", "exited"), event, res
+                    ),
+                )
+                clear()
+                return res
+            param = list(ans)
+            if not param or not param[0]:
+                param = None
+            try:
+                with interface:
+                    res = interface.enter(param)
+            except Exception as e:
+                traceback.print_exc()
+                await bot.send(event, await self._convert(str(e), event, res))
+        clear()
+        return res
+
+    async def __call__(self, event: Event, state: T_State, bot: Bot) -> bool:
+        if event.get_type() != "message":
+            return False
+        try:
+            msg = getattr(event, "original_message", event.get_message())
+        except (NotImplementedError, ValueError):
+            return False
+        with output_manager.capture(self.command.name) as cap:
+            output_manager.set_action(lambda x: x, self.command.name)
+            try:
+                arp = await self.handle(bot, event, msg)
+            except Exception as e:
+                arp = Arparma(self.command.path, msg, False, error_info=e)
+            may_help_text: Optional[str] = cap.get("output", None)
+        if not arp.matched and not may_help_text and self.skip:
+            return False
+        if not may_help_text and arp.error_info:
+            may_help_text = repr(arp.error_info)
+        if self.auto_send and may_help_text:
+            await bot.send(event, await self._convert(may_help_text, event, arp))
+            return False
+        state[ALCONNA_RESULT] = CommandResult(self.command, arp, may_help_text)
+        state[ALCONNA_EXEC_RESULT] = self.command.exec_result
+        return True
+
+    async def _convert(self, text: str, event: Event, arp: Arparma) -> Message:
+        _t = (
+            str(arp.error_info)
+            if isinstance(arp.error_info, SpecialOptionTriggered)
+            else "help"
+        )
+        try:
+            return await self.output_converter(_t, text)  # type: ignore
+        except NotImplementedError:
+            return event.get_message().__class__(text)
+
+
+def alconna(
+    command: Alconna,
+    skip_for_unmatch: bool = True,
+    auto_send_output: bool = False,
+    output_converter: Optional[TConvert] = None,
+    comp_config: Optional[CompConfig] = None,
+) -> Rule:
+    return Rule(
+        AlconnaRule(
+            command,
+            skip_for_unmatch,
+            auto_send_output,
+            output_converter,
+            comp_config,
+        )
+    )
+
+
+def set_output_converter(fn: TConvert):
+    AlconnaRule.default_converter = fn
```

### Comparing `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/typings.py` & `nonebot_plugin_alconna-0.9.3/src/nonebot_plugin_alconna/typings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,78 @@
-from __future__ import annotations
-
-from typing import Any, Awaitable, Callable, Generic, Literal, TypeVar, Union
-from typing_extensions import ParamSpec, TypeAlias
-
-from nepattern import BasePattern, MatchFailed, PatternModel
-from nonebot.internal.adapter.message import Message, MessageSegment
-from tarina import lang
-
-T = TypeVar("T")
-TMS = TypeVar("TMS", bound=MessageSegment)
-TCallable = TypeVar("TCallable", bound=Callable[..., Any])
-P = ParamSpec("P")
-
-
-class SegmentPattern(BasePattern[TMS], Generic[TMS, P]):
-    def __init__(
-        self,
-        name: str,
-        origin: type[TMS],
-        call: Callable[P, TMS],
-        additional: Callable[..., bool] | None = None,
-    ):
-        super().__init__(
-            name,
-            PatternModel.TYPE_CONVERT,
-            origin,
-            alias=name,
-            accepts=[MessageSegment],
-            validators=[additional] if additional else [],
-        )
-        self.call = call
-
-    def match(self, input_: str | Any) -> TMS:
-        if not isinstance(input_, self.origin):
-            raise MatchFailed(
-                lang.require("nepattern", "type_error").format(target=type(input_))
-            )
-        if input_.type != self.pattern:
-            raise MatchFailed(
-                lang.require("nepattern", "content_error").format(target=input_)
-            )
-        return input_
-
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> TMS:
-        return self.call(*args, **kwargs)  # type: ignore
-
-
-OutputType = Literal["help", "shortcut", "completion"]
-TConvert: TypeAlias = Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
-MReturn: TypeAlias = Union[Union[str, Message, MessageSegment], Awaitable[Union[str, Message, MessageSegment]]]
-
-def _isinstance(seg: MessageSegment, mapping: dict[str, Callable[[MessageSegment], Any]]):
-    if (key := seg.type) in mapping and (res := mapping[key](seg)):
-        return res
-    if "*" in mapping and (res := mapping["*"](seg)):
-        return res
-
-def gen_unit(
-    model: type[T],
-    mapping: dict[str, Callable[[MessageSegment], Union[T, Literal[False], None]]],
-    additional: Callable[..., bool] | None = None
-) -> BasePattern[T]:
-    return BasePattern(
-        model.__name__,
-        PatternModel.TYPE_CONVERT,
-        model,
-        lambda self, x: _isinstance(x, mapping),
-        accepts=[MessageSegment],
-        alias=model.__name__,
-        validators=[additional] if additional else [],
-    )
+from __future__ import annotations
+
+from typing_extensions import ParamSpec, TypeAlias
+from typing import Any, Union, Generic, Literal, TypeVar, Callable, Awaitable
+
+from tarina import lang
+from nepattern import BasePattern, MatchFailed, PatternModel
+from nonebot.internal.adapter.message import Message, MessageSegment
+
+T = TypeVar("T")
+TMS = TypeVar("TMS", bound=MessageSegment)
+TCallable = TypeVar("TCallable", bound=Callable[..., Any])
+P = ParamSpec("P")
+
+
+class SegmentPattern(BasePattern[TMS], Generic[TMS, P]):
+    def __init__(
+        self,
+        name: str,
+        origin: type[TMS],
+        call: Callable[P, TMS],
+        additional: Callable[..., bool] | None = None,
+    ):
+        super().__init__(
+            name,
+            PatternModel.TYPE_CONVERT,
+            origin,
+            alias=name,
+            accepts=[MessageSegment],
+            validators=[additional] if additional else [],
+        )
+        self.call = call
+
+    def match(self, input_: str | Any) -> TMS:
+        if not isinstance(input_, self.origin):
+            raise MatchFailed(
+                lang.require("nepattern", "type_error").format(target=type(input_))
+            )
+        if input_.type != self.pattern:
+            raise MatchFailed(
+                lang.require("nepattern", "content_error").format(target=input_)
+            )
+        return input_
+
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> TMS:
+        return self.call(*args, **kwargs)  # type: ignore
+
+
+OutputType = Literal["help", "shortcut", "completion"]
+TConvert: TypeAlias = Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
+MReturn: TypeAlias = Union[
+    Union[str, Message, MessageSegment], Awaitable[Union[str, Message, MessageSegment]]
+]
+
+
+def _isinstance(
+    seg: MessageSegment, mapping: dict[str, Callable[[MessageSegment], Any]]
+):
+    if (key := seg.type) in mapping and (res := mapping[key](seg)):
+        return res
+    if "*" in mapping and (res := mapping["*"](seg)):
+        return res
+
+
+def gen_unit(
+    model: type[T],
+    mapping: dict[str, Callable[[MessageSegment], T | Literal[False] | None]],
+    additional: Callable[..., bool] | None = None,
+) -> BasePattern[T]:
+    return BasePattern(
+        model.__name__,
+        PatternModel.TYPE_CONVERT,
+        model,
+        lambda self, x: _isinstance(x, mapping),
+        accepts=[MessageSegment],
+        alias=model.__name__,
+        validators=[additional] if additional else [],
+    )
```

### Comparing `nonebot-plugin-alconna-0.9.0/PKG-INFO` & `nonebot_plugin_alconna-0.9.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.9.0
+Version: 0.9.3
 Summary: Alconna Adapter for Nonebot
+Keywords: command argparse cli alconna nonebot
+Home-page: https://github.com/nonebot/plugin-alconna
+Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
-Keywords: command,argparse,cli,alconna,nonebot
-Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
+Project-URL: Homepage, https://github.com/nonebot/plugin-alconna
+Project-URL: Repository, https://github.com/nonebot/plugin-alconna
 Requires-Python: >=3.8
-Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
+Requires-Dist: nonebot2>=2.0.0rc4
+Requires-Dist: arclet-alconna<2.0.0,>=1.7.13
+Requires-Dist: arclet-alconna-tools<0.7.0,>=0.6.3
+Requires-Dist: nepattern<0.6.0,>=0.5.10
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
@@ -18,16 +24,16 @@
 # NoneBot Plugin Alconna
 
 _✨ Alconna Usage For NoneBot2 ✨_
 
 </div>
 
 <p align="center">
-  <a href="https://raw.githubusercontent.com/ArcletProject/nonebot-plugin-alconna/master/LICENSE">
-    <img src="https://img.shields.io/github/license/ArcletProject/nonebot-plugin-alconna.svg" alt="license">
+  <a href="https://raw.githubusercontent.com/nonebot/plugin-alconna/master/LICENSE">
+    <img src="https://img.shields.io/github/license/nonebot/plugin-alconna.svg" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-alconna">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-alconna.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 </p>
 
@@ -296,8 +302,7 @@
 async def echo(msg: str):
     return msg
 ```
 
 ## 体验
 
 [demo bot](./src/test/plugins/demo.py)
-
```

