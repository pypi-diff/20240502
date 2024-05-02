# Comparing `tmp/docker_shaper-2.0.0.tar.gz` & `tmp/docker_shaper-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-2.0.0.tar", max compression
+gzip compressed data, was "docker_shaper-2.0.1.tar", max compression
```

## Comparing `docker_shaper-2.0.0.tar` & `docker_shaper-2.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4558 2024-04-19 07:43:31.743076 docker_shaper-2.0.0/Readme.md
--rw-r--r--   0        0        0       74 2024-04-26 12:49:34.686323 docker_shaper-2.0.0/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0     1355 2024-04-24 08:49:58.546578 docker_shaper-2.0.0/docker_shaper/cli.py
--rw-r--r--   0        0        0    48946 2024-04-23 11:24:51.755605 docker_shaper-2.0.0/docker_shaper/docker_state.py
--rw-r--r--   0        0        0    34839 2024-04-26 13:21:36.086252 docker_shaper-2.0.0/docker_shaper/dynamic.py
--rwxr-xr-x   0        0        0      709 2023-11-13 15:44:58.815461 docker_shaper-2.0.0/docker_shaper/headless_examples/docker_events.py
--rwxr-xr-x   0        0        0     6398 2023-10-26 10:22:54.409443 docker_shaper-2.0.0/docker_shaper/headless_examples/docker_prune.py
--rwxr-xr-x   0        0        0    12458 2024-04-24 09:42:35.488952 docker_shaper-2.0.0/docker_shaper/headless_examples/dockermon.py
--rw-r--r--   0        0        0    21381 2024-04-26 12:37:07.471713 docker_shaper-2.0.0/docker_shaper/server.py
--rw-r--r--   0        0        0     7683 2024-04-24 09:42:37.260960 docker_shaper-2.0.0/docker_shaper/utils.py
--rw-r--r--   0        0        0     2408 2024-04-26 13:22:39.278568 docker_shaper-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 docker_shaper-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4558 2024-04-19 07:43:31.743076 docker_shaper-2.0.1/Readme.md
+-rw-r--r--   0        0        0       74 2024-05-02 14:06:15.313683 docker_shaper-2.0.1/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0     1355 2024-04-24 08:49:58.546578 docker_shaper-2.0.1/docker_shaper/cli.py
+-rw-r--r--   0        0        0    48946 2024-04-23 11:24:51.755605 docker_shaper-2.0.1/docker_shaper/docker_state.py
+-rw-r--r--   0        0        0    47874 2024-05-02 13:51:13.578453 docker_shaper-2.0.1/docker_shaper/dynamic.py
+-rwxr-xr-x   0        0        0      709 2023-11-13 15:44:58.815461 docker_shaper-2.0.1/docker_shaper/headless_examples/docker_events.py
+-rwxr-xr-x   0        0        0     6398 2023-10-26 10:22:54.409443 docker_shaper-2.0.1/docker_shaper/headless_examples/docker_prune.py
+-rwxr-xr-x   0        0        0    12458 2024-04-24 09:42:35.488952 docker_shaper-2.0.1/docker_shaper/headless_examples/dockermon.py
+-rw-r--r--   0        0        0    10162 2024-05-02 14:06:15.313683 docker_shaper-2.0.1/docker_shaper/server.py
+-rw-r--r--   0        0        0     5717 2024-05-02 13:52:51.078801 docker_shaper-2.0.1/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2442 2024-05-02 14:06:15.293683 docker_shaper-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5491 1970-01-01 00:00:00.000000 docker_shaper-2.0.1/PKG-INFO
```

### Comparing `docker_shaper-2.0.0/Readme.md` & `docker_shaper-2.0.1/Readme.md`

 * *Files identical despite different names*

### Comparing `docker_shaper-2.0.0/docker_shaper/cli.py` & `docker_shaper-2.0.1/docker_shaper/cli.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-2.0.0/docker_shaper/docker_state.py` & `docker_shaper-2.0.1/docker_shaper/docker_state.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-2.0.0/docker_shaper/dynamic.py` & `docker_shaper-2.0.1/docker_shaper/dynamic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 #!/usr/bin/env python3
 
 """Functionality that might change during runtime
 """
 
-# pylint: disable=invalid-name  # names come from aiodocker, not my fault
 # pylint: disable=too-many-instance-attributes
-# pylint: disable=too-many-lines
-# pylint: disable=too-few-public-methods
 # pylint: disable=too-many-branches
-# pylint: disable=too-many-return-statements
+# pylint: disable=too-many-lines
+# pylint: disable=too-many-locals
+# pylint: disable=too-many-statements
 # pylint: disable=missing-function-docstring
-# pylint: disable=missing-class-docstring
 # pylint: disable=fixme
+
 import asyncio
+import importlib
 import json
 import logging
 import os
 import re
 import sys
 import time
 import traceback
-from collections import Counter
 from collections.abc import Iterable, Mapping, MutableMapping, MutableSequence
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from typing import cast
+from types import ModuleType
+from typing import Protocol, cast
 
+import psutil
 from aiodocker import Docker, DockerError
 from aiodocker.volumes import DockerVolume
-from dateutil import tz
-from trickkiste.misc import age_str, date_str
+from rich.markup import escape as markup_escape
+from textual.widgets import Button, Label, Tree
+from textual.widgets.tree import TreeNode
+from trickkiste.misc import age_str, date_str, dur_str, process_output
 
-from docker_shaper.docker_state import (
+from . import __version__, utils
+from .docker_state import (
     Container,
     DockerState,
     Image,
     ImageIdent,
     MessageType,
     Network,
     Volume,
     is_uid,
     short_id,
     unique_ident,
 )
-#from docker_shaper.flask_table_patched import Col, Table
-from docker_shaper.utils import get_hostname, impatient, setup_introspection_on_signal
+from .utils import impatient
 
 BASE_DIR = Path("~/.docker_shaper").expanduser()
 
 
 def log() -> logging.Logger:
     """Logger for this module"""
     return logging.getLogger("docker-shaper")
@@ -57,15 +60,14 @@
 
 @dataclass
 class GlobalState:
     """The dirty globally shared state of docker-shaper"""
 
     intervals: MutableMapping[str, float]
     tag_rules: MutableMapping[str, int]
-    extra_links: MutableMapping[str, int]
     messages: MutableSequence[tuple[int, str, str, None | object]]
     switches: MutableMapping[str, bool]
     hostname: str
     expiration_ages: MutableMapping[str, int]
     update_mqueues: set[asyncio.Queue[str]]
     additional_values: MutableMapping[str, object]
     docker_state: DockerState
@@ -78,19 +80,17 @@
             "image_stats": 2,
             "container_stats": 2,
             "cleanup": 3600,
         }
         self.cleanup_fuse = 0
 
         self.tag_rules = {}
-        self.counter = 0
-        self.extra_links = {}
         self.switches = {}
         self.messages = []
-        self.hostname = get_hostname()
+        self.hostname = utils.get_hostname()
         self.expiration_ages = {}
         self.update_mqueues = set()
         self.additional_values = {}
 
     def __enter__(self) -> "GlobalState":
         return self
 
@@ -140,14 +140,43 @@
 
     @property
     def docker_client(self) -> Docker:
         assert self.docker_state.docker_client
         return self.docker_state.docker_client
 
 
+class DockerShaperUI(Protocol):
+    """Used to avoid importing DockerShaper TUI class"""
+
+    global_state: GlobalState
+
+    pattern_usage_count: MutableMapping[str, int]
+    removal_patterns: MutableMapping[str, int]
+
+    docker_stats_tree: Tree
+
+    containers_node: TreeNode
+    images_node: TreeNode
+    references_node: TreeNode
+    networks_node: TreeNode
+    volumes_node: TreeNode
+    patterns_node: TreeNode
+
+    lbl_event_horizon: Label
+    lbl_runtime: Label
+    lbl_switches: Label
+    lbl_expiration: Label
+    btn_clean: Button
+
+    def exit(self): ...
+    def update_status_bar(self, text: str): ...
+    def update_node_labels(self) -> None: ...
+    def write_message(self, text: str) -> None: ...
+
+
 async def run_listen_messages(global_state: GlobalState) -> None:
     """Print messages"""
     (BASE_DIR / "container-logs").mkdir(parents=True, exist_ok=True)
     while True:
         try:
             async for mtype, mtext, mobj in global_state.docker_state.wait_for_change():
                 handle_docker_state_message(global_state, mtype, mtext, mobj)
@@ -347,14 +376,586 @@
             "org.tribe29.cmk_version",
         )
         for w in l.split()
         if not (w.startswith("sha256") or len(w) == 64)
     )
 
 
+def would_cleanup_container(global_state: GlobalState, container: Container, now: int) -> bool:
+    if not container.show:
+        return False
+    if container.status == "exited":
+        return (
+            now - container.finished_at.timestamp()
+            > global_state.expiration_ages["container_exited"]
+        )
+    if container.status == "created":
+        return (
+            now - container.created_at.timestamp()
+            > global_state.expiration_ages["container_created"]
+        )
+    if container.status == "running":
+        return (
+            now - container.started_at.timestamp()
+            > global_state.expiration_ages["container_running"]
+        )
+    return False
+
+
+def expired_idents(global_state: GlobalState, image: Image, now) -> Iterable[tuple[str, str]]:
+    log().debug("check expiration for image %s, tags=%s", image.short_id, image.tags)
+
+    created_timestamp = int(image.created_at.timestamp())
+
+    for tag in image.tags:
+        is_expired, *_, reason = check_expiration(global_state, tag, now, created_timestamp)
+        if is_expired:
+            yield tag, reason
+
+    # only remove a container directly if there are no tags we could monitor
+    if not image.tags:
+        # todo: dangling images should be deleted
+        # is_expired, *_, reason = check_expiration(
+        #     global_state, image.short_id, now, created_timestamp
+        # )
+        # if is_expired:
+        #     yield image.short_id, reason
+        yield image.short_id, "no tags"
+
+
+async def remove_image_ident(global_state: GlobalState, ident: str) -> None:
+    report(global_state, "info", f"remove image/tag '{ident}'", None)
+    await global_state.docker_client.images.delete(ident)
+    # should be done outomatically
+    # await update_image_registration(global_state, ident)
+
+
+async def delete_container(global_state: GlobalState, ident: str | Container) -> None:
+    container = (global_state.containers[ident] if isinstance(ident, str) else ident).raw_container
+
+    report(
+        global_state,
+        "warning",
+        f"force removing container {short_id(container.id)}",
+        container,
+    )
+    await container.delete(force=True, v=True)
+
+    # Container should cleanup itself
+
+    # if container := await container_from(docker_client, container.id):
+    #    report(
+    #        global_state,
+    #        "error",
+    #        f"container {container_ident} still exists after deletion",
+    #        container,
+    #    )
+
+
+async def cleanup(global_state: GlobalState) -> None:
+    log().info("Cleanup!..")
+
+    report(global_state, "info", "start cleanup", None)
+
+    try:
+        now = int(datetime.now().timestamp())
+        # we could go through docker_client.containers/images/volumes, too, but to be more
+        # consistent, we operate on one structure only.
+        for container_info in list(
+            filter(
+                lambda cnt: would_cleanup_container(global_state, cnt, now),
+                global_state.containers.values(),
+            )
+        ):
+            if not global_state.switches.get("remove_container"):
+                log().info("skip removal of container %s", container_info.short_id)
+                continue
+            try:
+                await delete_container(global_state, container_info)
+            except DockerError as exc:
+                log().error(
+                    "Could not delete container %s, error was %s", container_info.short_id, exc
+                )
+
+        # traverse all images, remove expired tags
+        # use a DFT approach
+
+        # async def handle_branch(branch):
+        #    for image_id, children in list(branch.items()):
+        #        if not (image_info := global_state.images.get(image_id)):
+        #            continue
+        #        if children:
+        #            await handle_branch(children)
+        #        else:
+        #            for ident in expired_idents(global_state, image_info, now):
+        #                if not global_state.switches.get("remove_images"):
+        #                    log().info("skip removal of image/tag %s", ident)
+        #                    continue
+        #                try:
+        #                    await remove_image_ident(global_state, ident)
+        #                except DockerError as exc:
+        #                    log().error("Could not delete image %s, error was %s", ident, exc)
+        # await handle_branch(dep_tree)
+
+        # FOR NOW: only handle images without children
+        no_remove_images = not global_state.switches.get("remove_images")
+        image: Image
+        for image in list(global_state.images.values()):
+            if image.children:
+                continue
+
+            for ident, reason in expired_idents(global_state, image, now):
+                log().info("%sexpired: %s (%s)", "SKIP " if no_remove_images else "", ident, reason)
+                if no_remove_images:
+                    continue
+                try:
+                    await remove_image_ident(global_state, ident)
+                except DockerError as exc:
+                    report(global_state, "error", f"'{ident}' could not be removed: {exc}")
+
+        log().info("Prune docker volumes")
+        for volume_name in list(global_state.volumes):
+            log().info("try to delete %s..", volume_name)
+            try:
+                await DockerVolume(global_state.docker_client, volume_name).delete()
+                report(
+                    global_state,
+                    "warning",
+                    f"volume {short_id(volume_name)} has not been removed automatically",
+                )
+            except DockerError as exc:
+                log().info("not possible: %s", exc)
+
+        # TODO: react on disapearing volumes
+
+        report(global_state, "info", "invoke 'docker builder prune'")
+        _stdout, _stderr, result = await global_state.docker_state.prune_builder_cache()
+        if result == 0:
+            report(global_state, "info", "'docker builder prune' successful")
+        else:
+            report(global_state, "error", "'docker builder prune' returned non-zero")
+
+    finally:
+        report(global_state, "info", "cleanup done", None)
+
+
+def report(
+    global_state: GlobalState,
+    msg_type: None | str = None,
+    message: None | str = None,
+    extra: None | object = None,
+) -> None:
+    """Report an incident - maybe good or bad"""
+    if sys.exc_info()[1] and msg_type in {None, "exception"}:
+        log().exception(message and str(message) or "Exception:")
+        traceback_str = traceback.format_exc().strip("\n")
+        type_str, msg_str, extra_str = (
+            msg_type or "exception",
+            "\n".join((message, traceback_str)) if message else traceback_str,
+            None,
+        )
+    else:
+        type_str, msg_str, extra_str = (msg_type or "debug", message or "--", extra and str(extra))
+        log().log(getattr(logging, type_str.upper(), logging.WARNING), msg_str)
+
+    icon = {"info": "🔵", "warning": "🟠", "error": "🔴", "exception": "🟣"}.get(type_str, "⚪")
+    now = datetime.now()
+
+    BASE_DIR.mkdir(parents=True, exist_ok=True)
+    with open(
+        BASE_DIR / f"messages-{now.strftime('%Y.%m.%d')}.log", "a", encoding="utf-8"
+    ) as log_file:
+        log_file.write(
+            f"{icon} {type_str:<9s}"
+            f" │ {date_str(now)} ({age_str(datetime.now(), global_state.docker_state.started_at)})"
+            f" │ {os.getpid()} │ {msg_str} {extra_str or  ''}\n"
+        )
+
+    global_state.messages.insert(0, (int(now.timestamp()), type_str, msg_str, extra_str))
+
+    if isinstance(msize := global_state.additional_values.get("message_history_size", 100), int):
+        global_state.messages = global_state.messages[:msize]
+
+
+def reconfigure(global_state: GlobalState) -> None:
+    """Reacts on changes to the configuration, e.g. applies"""
+
+    # for ident, reference in global_state.last_referenced.items():
+    #    reference[1] = expiration_age_from_ident(global_state, ident)
+
+    # todo
+    # global_state.inform("refresh")
+    from . import utils as _utils  # pylint: disable=import-outside-toplevel
+
+    importlib.reload(_utils)
+
+    report(global_state, "info", "configuration reloaded")
+
+
+async def on_button_pressed(ui: DockerShaperUI, event: Button.Pressed) -> None:
+    log().debug("Button %r pressed", event.button.id)
+    if event.button.id == "quit":
+        ui.exit()
+    elif event.button.id == "clean":
+        await asyncio.ensure_future(cleanup(ui.global_state))
+    elif event.button.id == "rotate_log_level":
+        utils.increase_loglevel()
+        event.button.label = f"rotate log level ({logging.getLevelName(log().level)})"
+        log().info("changed log level to %s", logging.getLevelName(log().level))
+    elif event.button.id == "dump_trace":
+        trace_log_file_path = BASE_DIR / "traceback.log"
+        ui.write_message("dump trace")
+        with trace_log_file_path.open("w", encoding="utf-8") as log_file:
+            utils.dump_stacktrace(lambda msg: log_file.write(f"{msg}\n"), ui.write_message)
+            ui.write_message(f"traceback also written to {trace_log_file_path}")
+
+
+async def update_dashboard(ui: DockerShaperUI) -> None:
+    current_process = psutil.Process()
+    tasks = [
+        name for t in asyncio.all_tasks() if not (name := t.get_name()).startswith("message pump ")
+    ]
+    now = datetime.now()
+    ui.lbl_event_horizon.update(
+        f"Event horizon: {date_str(ui.global_state.docker_state.event_horizon)}"
+        f" / [bold cyan]{age_str(now, ui.global_state.docker_state.event_horizon)}[/]"
+    )
+    ui.lbl_runtime.update(
+        f"runtime: {date_str(ui.global_state.docker_state.started_at)}"
+        f" / [bold cyan]{age_str(now, ui.global_state.docker_state.started_at)}[/]"
+    )
+    ui.lbl_switches.update(
+        "\n".join(
+            f"{key:.<20}: [bold  cyan]{markup_escape('[x]' if value else '[ ]')}[/]"
+            for key, value in ui.global_state.switches.items()
+        )
+    )
+    ui.lbl_expiration.update(
+        "\n".join(
+            f"{key:.<20}: [bold cyan]{dur_str(value):>5s}[/]"
+            for key, value in ui.global_state.expiration_ages.items()
+        )
+    )
+    cleanup_interval = ui.global_state.intervals["cleanup"]
+    ui.btn_clean.label = (
+        f"Cleanup now! {dur_str(cleanup_interval - ui.global_state.cleanup_fuse)}"
+        f" (interval={dur_str(cleanup_interval)})"
+    )
+
+    # toggles: cleanup container / images / volumes / build cache
+    # │ connections:       1
+    # │ tasks:             34, missing / unknown: none /  none
+    # │ initially crawled: containers: True images: True volumes: True networks: True
+
+    # Tables:
+    # containers
+    # images
+    # rules
+    # unmatched tags
+    docker_version = (
+        process_output("docker --version").split("\n", maxsplit=1)[0].split(sep=" ", maxsplit=2)[2]
+    )
+    cpu_percent = psutil.cpu_percent()
+    cpu_count = psutil.cpu_count()
+    ui.update_status_bar(
+        f" PID: {current_process.pid}"
+        f" / {current_process.cpu_percent():6.1f}% CPU"
+        f" / {len(tasks)} tasks"
+        f" │ System CPU: {cpu_percent:5.1f}% / {int(cpu_percent * cpu_count):4d}%"
+        f" │ docker-shaper v{__version__}"
+        f" │ docker v{docker_version}"
+    )
+    # ui.lbl_stats1.update()
+    await asyncio.sleep(3)
+
+
+def update_node_labels(ui: DockerShaperUI) -> None:
+    """Fills some labels with useful information"""
+    total_cpu = sum(map(lambda c: c.cpu_usage(), ui.global_state.docker_state.containers.values()))
+    total_mem = sum(map(lambda c: c.mem_usage(), ui.global_state.docker_state.containers.values()))
+    ui.patterns_node.set_label(f"Image-pattern ({len(ui.removal_patterns)})")
+    ui.containers_node.set_label(
+        f"Containers ({len(ui.global_state.docker_state.containers):2d})"
+        f" {' ' * 56} [bold]{total_cpu * 100:7.2f}% - {total_mem >> 20:6d}MiB[/]"
+    )
+    ui.images_node.set_label(f"Images ({len(ui.global_state.docker_state.images)})")
+    ui.volumes_node.set_label(f"Volumes ({len(ui.global_state.docker_state.volumes)})")
+    ui.networks_node.set_label(f"Networks ({len(ui.global_state.docker_state.networks)})")
+
+
+async def schedule_cleanup(global_state: GlobalState) -> None:
+    while True:
+        if (
+            interval := global_state.intervals.get("cleanup", 3600)
+        ) and global_state.cleanup_fuse > interval:
+            global_state.cleanup_fuse = 0
+            break
+        if (interval - global_state.cleanup_fuse) % 60 == 0:
+            log().debug(
+                "cleanup: %s seconds to go..",
+                (interval - global_state.cleanup_fuse),
+            )
+        await asyncio.sleep(1)
+        global_state.cleanup_fuse += 1
+    await asyncio.ensure_future(cleanup(global_state))
+
+
+def load_config(global_state: GlobalState, config_file_path: Path) -> ModuleType:
+    """Load the config module and invoke `reconfigure`"""
+    module = utils.load_module(config_file_path)
+    try:
+        module.modify(global_state)
+        reconfigure(global_state)
+    except AttributeError:
+        log().warning("File %s does not provide a `modify(global_state)` function")
+    return module
+
+
+async def on_changed_file(global_state: GlobalState, config_file_path: Path, changes) -> None:
+    for changed_file, module in changes:
+        try:
+            changed_file_str = changed_file.as_posix().replace(Path.home().as_posix(), "~")
+            if changed_file == config_file_path:
+                log().info("config file %s changed - apply changes", changed_file_str)
+                load_config(global_state, config_file_path)
+            else:
+                log().info("file %s changed - reload module", changed_file_str)
+                assert module
+                importlib.reload(module)
+        except Exception:  # pylint: disable=broad-except
+            report(global_state)
+            await asyncio.sleep(5)
+
+
+def container_markup(container: Container) -> str:
+    status_markups = {"running": "cyan bold"}
+    image_str, status_str = (
+        ("", "")
+        if not container.show
+        else (
+            f" image:[bold]{short_id(container.show.Image)}[/]",
+            f" - [{status_markups.get(container.show.State.Status, 'grey53')}]"
+            f"{container.show.State.Status:7s}[/]",
+        )
+    )
+    return (
+        f"[bold]{container.short_id}[/] / {container.name:<26s}{image_str}{status_str}"
+        f" - {container.cpu_usage() * 100:7.2f}%"
+        f" - {container.mem_usage() >> 20:6d}MiB"
+    )
+
+
+async def maintain_docker_stats_tree(ui: DockerShaperUI) -> None:
+    container_nodes = {}
+    image_nodes = {}
+    reference_nodes: dict[ImageIdent, TreeNode] = {}
+    network_nodes = {}
+    volume_nodes = {}
+
+    ui.docker_stats_tree.root.expand()
+    ui.docker_stats_tree.root.allow_expand = False
+
+    # wait for all items to be registered
+    while not all(
+        (
+            ui.global_state.docker_state.containers_crawled,
+            ui.global_state.docker_state.images_crawled,
+            ui.global_state.docker_state.volumes_crawled,
+            ui.global_state.docker_state.networks_crawled,
+        )
+    ):
+        log().info(
+            "wait for initial crawls (C: %s, I: %s, V: %s, N: %s)",
+            ui.global_state.docker_state.containers_crawled,
+            ui.global_state.docker_state.images_crawled,
+            ui.global_state.docker_state.volumes_crawled,
+            ui.global_state.docker_state.networks_crawled,
+        )
+        await asyncio.sleep(1)
+
+    # add all containers
+    for container in ui.global_state.docker_state.containers.values():
+        container_nodes[container.id] = ui.containers_node.add(f"{container}")
+
+    # add all images
+    pattern_issues = []
+    for img in ui.global_state.docker_state.images.values():
+        img_node = image_nodes[img.id] = ui.images_node.add(f"{img}", expand=True)
+        for tag in img.tags:
+            dep_age, reason = expiration_age_from_image_name(ui.removal_patterns, tag, 666)
+            reason_markup = "bold red"
+            if reason in ui.removal_patterns:
+                if reason not in ui.pattern_usage_count:
+                    ui.pattern_usage_count[reason] = 0
+                ui.pattern_usage_count[reason] += 1
+                reason_markup = "sky_blue2"
+            else:
+                pattern_issues.append(f"{tag} # {reason}")
+            img_node.add(
+                f"dep_age=[sky_blue2]{dep_age:10d}[/]"
+                f" [bold]{tag}[/] '[{reason_markup}]{reason}[/]'"
+            )
+
+    # add all volumes
+    for volume in ui.global_state.docker_state.volumes.values():
+        volume_nodes[volume.Name] = ui.volumes_node.add(f"{volume}")
+
+    # add all networks
+    for network in ui.global_state.docker_state.networks.values():
+        network_nodes[network.Id] = ui.networks_node.add(f"{network}")
+
+    # add all pattern
+    for issue in pattern_issues:
+        ui.patterns_node.add(f"[bold red]{issue}[/]'")
+    for pattern, dep_age in ui.removal_patterns.items():
+        usage_count = ui.pattern_usage_count.get(pattern, 0)
+        if usage_count == 0:
+            pattern_issues.append(pattern)
+        ui.patterns_node.add(f"{usage_count:3d}: r'[sky_blue2]{pattern}[/]'")
+        # network_nodes[network.Id] = ui.networks_node.add(f"{network}")
+
+    with (BASE_DIR / "pattern-issues.txt").open("w", encoding="utf-8") as issues_file:
+        issues_file.write("\n".join(pattern_issues))
+
+    ui.update_node_labels()
+
+    async for mtype, mtext, mobj in ui.global_state.docker_state.wait_for_change():
+        ui.docker_stats_tree.root.set_label(
+            f"{utils.get_hostname()}"
+            f" / horizon={date_str(ui.global_state.docker_state.event_horizon)}"
+            f" ({dur_str(int(time.time()) - ui.global_state.docker_state.event_horizon)})"
+        )
+
+        if mtype == "exception":
+            log().exception("%s: %s", mtext, mobj)
+
+        elif mtype == "error":
+            log().error(mtext)
+
+        elif mtype == "warning":
+            log().warning(mtext)
+
+        elif mtype == "info":
+            log().info(mtext)
+
+        elif mtype == "client_disconnect":
+            raise SystemExit(1)
+
+        elif mtype in {"container_add", "container_del", "container_update"}:
+            cnt: Container = cast(Container, mobj)
+            log().info(
+                "container info: '%s' / %s (%d total)",
+                cnt.short_id,
+                mtype,
+                len(ui.global_state.docker_state.containers),
+            )
+            if mtype == "container_add" and cnt.id not in container_nodes:
+                container_nodes[cnt.id] = ui.containers_node.add(f"{cnt}")
+            if mtype == "container_update":
+                if cnt.id not in container_nodes:
+                    # todo: investigate - node should be available already
+                    log().warning("container %s not known to UI yet but should", cnt.id)
+                    container_nodes[cnt.id] = ui.containers_node.add(f"{cnt}")
+                container_nodes[cnt.id].set_label(container_markup(cnt))
+            if mtype == "container_del" and cnt.id in container_nodes:
+                if cnt.id in container_nodes:
+                    container_nodes[cnt.id].remove()
+                    del container_nodes[cnt.id]
+
+            ui.update_node_labels()
+
+        elif mtype in {"image_add", "image_del", "image_update"}:
+            image_id = mtext
+
+            log().info(
+                "image info: '%s' / %s (%d total)",
+                short_id(image_id),
+                mtype,
+                len(ui.global_state.docker_state.images),
+            )
+            if mtype == "image_del":
+                if image_id in image_nodes:
+                    image_nodes[image_id].remove()
+                    del image_nodes[image_id]
+                continue
+            image = ui.global_state.docker_state.images[image_id]
+            if mtype == "image_add" and image.id not in image_nodes:
+                image_nodes[image.id] = ui.images_node.add(f"{image}")
+            if mtype == "image_update":
+                if image.id not in image_nodes:
+                    # todo: investigate - node should be available already
+                    log().warning("image %s not known to UI yet but should", image.id)
+                    image_nodes[image.id] = ui.images_node.add(f"{image}")
+                image_nodes[image.id].set_label(f"{image} - +")
+
+            ui.update_node_labels()
+
+        elif mtype in {"volume_add", "volume_del"}:
+            volume_id = mtext
+
+            log().info(
+                "volume info: '%s' / %s (%d total)",
+                short_id(volume_id),
+                mtype,
+                len(ui.global_state.docker_state.volumes),
+            )
+            if mtype == "volume_add" and volume_id not in volume_nodes:
+                vol: Volume = cast(Volume, mobj)
+                volume_nodes[volume_id] = ui.volumes_node.add(f"{vol}")
+            if mtype == "volume_del":
+                if volume_id in volume_nodes:
+                    volume_nodes[volume_id].remove()
+                    del volume_nodes[volume_id]
+
+            ui.update_node_labels()
+
+        elif mtype in {"network_add", "network_del"}:
+            network_id = mtext
+
+            log().info(
+                "network info: '%s' / %s (%d total)",
+                short_id(network_id),
+                mtype,
+                len(ui.global_state.docker_state.networks),
+            )
+            if mtype == "network_add" and network_id not in network_nodes:
+                netw: Network = cast(Network, mobj)
+                network_nodes[network_id] = ui.networks_node.add(f"{netw}")
+            if mtype == "network_del":
+                if network_id in network_nodes:
+                    network_nodes[network_id].remove()
+                    del network_nodes[network_id]
+            ui.update_node_labels()
+
+        elif mtype in {"reference_update", "reference_del"}:
+            ident = cast(ImageIdent, mobj)
+            log().info(
+                "reference updated: %s (%d total)",
+                ident,
+                len(ui.global_state.docker_state.last_referenced),
+            )
+            if mtype == "reference_update":
+                if mtype in reference_nodes:
+                    reference_nodes[ident].set_label(
+                        f"{ident} - {ui.global_state.docker_state.last_referenced[ident]} - +"
+                    )
+                else:
+                    reference_nodes[ident] = ui.references_node.add(
+                        f"{ident} - {ui.global_state.docker_state.last_referenced[ident]}"
+                    )
+            if mtype == "reference_del" and ident in reference_nodes:
+                reference_nodes[ident].remove()
+                del reference_nodes[ident]
+
+        else:
+            log().error("don't know message type %s", mtype)
+
+
+"""
+
 async def dump_global_state(global_state: GlobalState):
     # TODO
     # dep_tree, max_depth = image_dependencies(global_state)
     # def handle_branch(branch, depth=0):
     #     for image_id, children in list(branch.items()):
     #         print(
     #             f"{'.' * (depth + 1)}"
@@ -362,15 +963,14 @@
     #             f" {'.' * (max_depth - depth + 1)}"
     #             f" {len(children)}"
     #             f" {global_state.images[image_id].tags}"
     #         )
     #         handle_branch(children, depth + 1)
     # handle_branch(dep_tree)
 
-    global_state.counter += 1
     all_tasks = asyncio.all_tasks()
     coro_name_count = Counter(
         name
         for t in all_tasks
         if (coro := t.get_coro())
         if (name := getattr(coro, "__name__"))
         # ignore
@@ -416,39 +1016,14 @@
             global_state,
             "error",
             f"mandatory tasks are not running anymore: {missing_tasks} => terminate!",
         )
         await asyncio.sleep(1)  # wait for message queues to be eaten up
         raise SystemExit(1)
 
-    print()
-    print(f"│=====[ http://{global_state.hostname}:5432/ ]===================================")
-    print(
-        f"│ started / frame:   {date_str(global_state.docker_state.started_at)}"
-        f" / {age_str(datetime.now(), global_state.docker_state.started_at)}"
-        f" / {global_state.counter}"
-    )
-    print(
-        f"│ event horizon:     {date_str(global_state.docker_state.event_horizon)}"
-        f" / {age_str(datetime.now(), global_state.docker_state.event_horizon)}"
-    )
-    print(f"| cycle log level:   `kill -USR1 {os.getpid()}`")
-    print(f"| write trace:       `kill -USR2 {os.getpid()}`")
-    print(
-        f"│ intervals:         "
-        f"{', '.join('='.join(map(str, i)) for i in global_state.intervals.items())}"
-    )
-    print(f"│ containers:        {len(global_state.containers)}")
-    print(f"│ images:            {len(global_state.images)}")
-    # print(f"│ image tree depth: {max_depth}")
-    print(f"│ volumes:           {len(global_state.volumes)}")
-    print(f"│ networks:          {len(global_state.networks)}")
-    print(f"│ references:        {len(global_state.last_referenced)}")
-    print(f"│ tag_rules:         {len(global_state.tag_rules)}")
-    print(f"│ connections:       {len(global_state.update_mqueues)}")
     print(
         f"│ tasks:             {len(all_tasks)}, missing / unknown:"
         f" {missing_tasks or 'none'} / "
         f" {(coro_name_count.keys() - expectd_coro_names) or 'none'}"
     )
     print(
         f"│ initially crawled:"
@@ -456,35 +1031,14 @@
         f" images: {global_state.docker_state.images_crawled}"
         f" volumes: {global_state.docker_state.volumes_crawled}"
         f" networks: {global_state.docker_state.networks_crawled}"
     )
     print("│===================================================================")
     print()
 
-'''
-class BaseTable(Table):
-    allow_sort = True
-    classes = ["table", "table-striped"]
-
-    def __init__(self, endpoint, items):
-        super().__init__(items)
-        self.endpoint = endpoint
-
-    def get_tr_attrs(self, item):
-        return {"class": item.get("class")}
-
-    def sort_url(self, col_id, reverse=False):
-        raise NotImplementedError()
-
-
-class PlainCol(Col):
-    def td_format(self, content):
-        return f"<tt><b>{content}</b></tt>"
-
-
 class ImageTable(BaseTable):
     short_id = PlainCol("short_id")
     tags = PlainCol("tags")
     children_count = PlainCol("#children")
     created_at = PlainCol("created_at")
     age = PlainCol("age")
 
@@ -653,15 +1207,14 @@
             endpoint,
             items=sorted(
                 map(dict_from, global_state.volumes.values()),
                 key=lambda e: e[sort],
                 reverse=reverse,
             ),
         ).__html__()
-'''
 
 async def response_remove_image_ident(global_state: GlobalState):
     try:
         if not (ident := request.args.get("ident")):
             raise RuntimeError("STRAGE: response_remove_image_ident called with empty `ident`")
         await remove_image_ident(global_state, ident)
     except Exception as exc:  # pylint: disable=broad-except
@@ -740,235 +1293,8 @@
         # if (
         #    (s["started_at"] and tds // 3600 > 5)
         #    or s["status"] == "exited"
         #    or not s["started_at"]
         # ):
         #    log(f"remove {s['short_id']}")
         #    await s["container"].delete(force=True)
-    print(
-        f"{'TOTAL':<12}  {len(stats):<25}"
-        f" {'':>9}"
-        f" {int(sum(s['cpu'] for s in stats)*1000) / 10:>8}%\033[0m"
-        f" {int(sum(s['usage'] for s in stats) / (1<<30)*10) / 10:>6}GiB\033[0m"
-        f" {''}"
-        f" {'':>9}"
-        f" {'':<60}"
-        f" {''}"
-    )
-
-
-def would_cleanup_container(global_state: GlobalState, container: Container, now: int) -> bool:
-    if not container.show:
-        return False
-    if container.status == "exited":
-        return (
-            now - container.finished_at.timestamp()
-            > global_state.expiration_ages["container_exited"]
-        )
-    if container.status == "created":
-        return (
-            now - container.created_at.timestamp()
-            > global_state.expiration_ages["container_created"]
-        )
-    if container.status == "running":
-        return (
-            now - container.started_at.timestamp()
-            > global_state.expiration_ages["container_running"]
-        )
-    return False
-
-
-def expired_idents(global_state: GlobalState, image: Image, now) -> Iterable[tuple[str, str]]:
-    log().debug("check expiration for image %s, tags=%s", image.short_id, image.tags)
-
-    created_timestamp = int(image.created_at.timestamp())
-
-    for tag in image.tags:
-        is_expired, *_, reason = check_expiration(global_state, tag, now, created_timestamp)
-        if is_expired:
-            yield tag, reason
-
-    # only remove a container directly if there are no tags we could monitor
-    if not image.tags:
-        # todo: dangling images should be deleted
-        # is_expired, *_, reason = check_expiration(
-        #     global_state, image.short_id, now, created_timestamp
-        # )
-        # if is_expired:
-        #     yield image.short_id, reason
-        yield image.short_id, "no tags"
-
-
-async def remove_image_ident(global_state: GlobalState, ident: str) -> None:
-    report(global_state, "info", f"remove image/tag '{ident}'", None)
-    await global_state.docker_client.images.delete(ident)
-    # should be done outomatically
-    # await update_image_registration(global_state, ident)
-
-
-async def delete_container(global_state: GlobalState, ident: str | Container) -> None:
-    container = (global_state.containers[ident] if isinstance(ident, str) else ident).raw_container
-
-    report(
-        global_state,
-        "warning",
-        f"force removing container {short_id(container.id)}",
-        container,
-    )
-    await container.delete(force=True, v=True)
-
-    # Container should cleanup itself
-
-    # if container := await container_from(docker_client, container.id):
-    #    report(
-    #        global_state,
-    #        "error",
-    #        f"container {container_ident} still exists after deletion",
-    #        container,
-    #    )
-
-
-async def cleanup(global_state: GlobalState) -> None:
-    log().info("Cleanup!..")
-
-    report(global_state, "info", "start cleanup", None)
-
-    try:
-        now = int(datetime.now().timestamp())
-        # we could go through docker_client.containers/images/volumes, too, but to be more
-        # consistent, we operate on one structure only.
-        for container_info in list(
-            filter(
-                lambda cnt: would_cleanup_container(global_state, cnt, now),
-                global_state.containers.values(),
-            )
-        ):
-            if not global_state.switches.get("remove_container"):
-                log().info("skip removal of container %s", container_info.short_id)
-                continue
-            try:
-                await delete_container(global_state, container_info)
-            except DockerError as exc:
-                log().error(
-                    "Could not delete container %s, error was %s", container_info.short_id, exc
-                )
-
-        # traverse all images, remove expired tags
-        # use a DFT approach
-
-        # async def handle_branch(branch):
-        #    for image_id, children in list(branch.items()):
-        #        if not (image_info := global_state.images.get(image_id)):
-        #            continue
-        #        if children:
-        #            await handle_branch(children)
-        #        else:
-        #            for ident in expired_idents(global_state, image_info, now):
-        #                if not global_state.switches.get("remove_images"):
-        #                    log().info("skip removal of image/tag %s", ident)
-        #                    continue
-        #                try:
-        #                    await remove_image_ident(global_state, ident)
-        #                except DockerError as exc:
-        #                    log().error("Could not delete image %s, error was %s", ident, exc)
-        # await handle_branch(dep_tree)
-
-        # FOR NOW: only handle images without children
-        no_remove_images = not global_state.switches.get("remove_images")
-        image: Image
-        for image in list(global_state.images.values()):
-            if image.children:
-                continue
-
-            for ident, reason in expired_idents(global_state, image, now):
-                log().info("%sexpired: %s (%s)", "SKIP " if no_remove_images else "", ident, reason)
-                if no_remove_images:
-                    continue
-                try:
-                    await remove_image_ident(global_state, ident)
-                except DockerError as exc:
-                    report(global_state, "error", f"'{ident}' could not be removed: {exc}")
-
-        log().info("Prune docker volumes")
-        for volume_name in list(global_state.volumes):
-            log().info("try to delete %s..", volume_name)
-            try:
-                await DockerVolume(global_state.docker_client, volume_name).delete()
-                report(
-                    global_state,
-                    "warning",
-                    f"volume {short_id(volume_name)} has not been removed automatically",
-                )
-            except DockerError as exc:
-                log().info("not possible: %s", exc)
-
-        # TODO: react on disapearing volumes
-
-        report(global_state, "info", "invoke 'docker builder prune'")
-        _stdout, _stderr, result = await global_state.docker_state.prune_builder_cache()
-        if result == 0:
-            report(global_state, "info", "'docker builder prune' successful")
-        else:
-            report(global_state, "error", "'docker builder prune' returned non-zero")
-
-    finally:
-        report(global_state, "info", "cleanup done", None)
-
-
-def report(
-    global_state: GlobalState,
-    msg_type: None | str = None,
-    message: None | str = None,
-    extra: None | object = None,
-) -> None:
-    """Report an incident - maybe good or bad"""
-    if sys.exc_info()[1] and msg_type in {None, "exception"}:
-        log().exception(message)
-        traceback_str = traceback.format_exc().strip("\n")
-        type_str, msg_str, extra_str = (
-            msg_type or "exception",
-            "\n".join((message, traceback_str)) if message else traceback_str,
-            None,
-        )
-    else:
-        type_str, msg_str, extra_str = (msg_type or "debug", message or "--", extra and str(extra))
-        log().log(getattr(logging, type_str.upper(), logging.WARNING), msg_str)
-
-    icon = {"info": "🔵", "warning": "🟠", "error": "🔴", "exception": "🟣"}.get(type_str, "⚪")
-    now = datetime.now()
-
-    BASE_DIR.mkdir(parents=True, exist_ok=True)
-    with open(
-        BASE_DIR / f"messages-{now.strftime('%Y.%m.%d')}.log", "a", encoding="utf-8"
-    ) as log_file:
-        log_file.write(
-            f"{icon} {type_str:<9s}"
-            f" │ {date_str(now)} ({age_str(datetime.now(), global_state.docker_state.started_at)})"
-            f" │ {os.getpid()} │ {msg_str} {extra_str or  ''}\n"
-        )
-
-    global_state.messages.insert(0, (int(now.timestamp()), type_str, msg_str, extra_str))
-
-    if isinstance(msize := global_state.additional_values.get("message_history_size", 100), int):
-        global_state.messages = global_state.messages[:msize]
-
-
-def reconfigure(global_state: GlobalState) -> None:
-    """Reacts on changes to the configuration, e.g. applies"""
-
-    # for ident, reference in global_state.last_referenced.items():
-    #    reference[1] = expiration_age_from_ident(global_state, ident)
-
-    # todo
-    # global_state.inform("refresh")
-    import importlib  # pylint: disable=import-outside-toplevel
-
-    from docker_shaper import utils  # pylint: disable=import-outside-toplevel
-
-    importlib.reload(utils)
-    # utils.setup_logging()
-
-    report(global_state, "info", "configuration reloaded")
-
-
-def setup_introspection():
-    setup_introspection_on_signal()
+"""
```

### Comparing `docker_shaper-2.0.0/docker_shaper/headless_examples/docker_events.py` & `docker_shaper-2.0.1/docker_shaper/headless_examples/docker_events.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-2.0.0/docker_shaper/headless_examples/docker_prune.py` & `docker_shaper-2.0.1/docker_shaper/headless_examples/docker_prune.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-2.0.0/docker_shaper/headless_examples/dockermon.py` & `docker_shaper-2.0.1/docker_shaper/headless_examples/dockermon.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-2.0.0/pyproject.toml` & `docker_shaper-2.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "2.0.0"
+version = "2.0.1"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
 ]
@@ -24,14 +24,15 @@
 rich = "^13"
 textual = "^0"
 psutil = "^5.9.8"
 
 trickkiste = "^0.0.10"
 #trickkiste  = {path = "/home/frafue/_HOME/trickkiste", develop = true}
 python-dateutil = "^2"  # needed by trickkiste but not set as dependency (intentionally)
+types-psutil = "^5.9.5.20240423"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
 flake8 = "*"
 pytest = "*"
@@ -46,14 +47,15 @@
 types-python-dateutil = "*"
 pre-commit = "*"
 
 # see https://pypi.org/project/poetry-bumpversion
 [tool.poetry_bumpversion.file."docker_shaper/__init__.py"]
 [tool.poetry_bumpversion.file."docker_shaper/server.py"]
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
 line-length = 100
```

### Comparing `docker_shaper-2.0.0/PKG-INFO` & `docker_shaper-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-shaper
-Version: 2.0.0
+Version: 2.0.1
 Summary: Keeps Docker resources in shape based on rules and usage
 Home-page: https://github.com/Checkmk/checkmk-dev-tools
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.10.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -14,14 +14,15 @@
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pydantic (>=2.4,<3.0)
 Requires-Dist: python-dateutil (>=2,<3)
 Requires-Dist: pytz (>=2023.3.post1,<2024.0)
 Requires-Dist: rich (>=13,<14)
 Requires-Dist: textual (>=0,<1)
 Requires-Dist: trickkiste (>=0.0.10,<0.0.11)
+Requires-Dist: types-psutil (>=5.9.5.20240423,<6.0.0.0)
 Project-URL: Repository, https://github.com/Checkmk/checkmk-dev-tools
 Description-Content-Type: text/markdown
 
 # Docker Shaper
 
 This is a spin-off package for the `docker-shaper` tool, which can be used to monitor Docker stuff
 like containers, images and volumes and automatically enforce certain cleanup-rules.
```

