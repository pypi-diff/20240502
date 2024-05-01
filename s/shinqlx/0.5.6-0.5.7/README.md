# Comparing `tmp/shinqlx-0.5.6.tar.gz` & `tmp/shinqlx-0.5.7.tar.gz`

## Comparing `shinqlx-0.5.6.tar` & `shinqlx-0.5.7.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 shinqlx-0.5.6/Cargo.toml
--rw-r--r--   0     1001      127     1502 2024-03-12 20:08:35.000000 shinqlx-0.5.6/LICENSE
--rw-r--r--   0     1001      127     5411 2024-03-12 20:08:35.000000 shinqlx-0.5.6/README.md
--rw-r--r--   0     1001      127      738 2024-03-12 20:08:35.000000 shinqlx-0.5.6/run_server_shinqlx.sh
--rw-r--r--   0     1001      127    36114 2024-03-12 20:08:48.000000 shinqlx-0.5.6/Cargo.lock
--rw-r--r--   0     1001      127     2236 2024-03-12 20:08:35.000000 shinqlx-0.5.6/pyproject.toml
--rw-r--r--   0     1001      127     2045 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_core.pyi
--rw-r--r--   0     1001      127     3536 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/database.pyi
--rw-r--r--   0     1001      127    31253 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_plugin.pyi
--rw-r--r--   0     1001      127    19667 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_player.py
--rw-r--r--   0     1001      127    19311 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_handlers.py
--rw-r--r--   0     1001      127    11991 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/__init__.pyi
--rw-r--r--   0     1001      127    12507 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_game.py
--rw-r--r--   0     1001      127    24879 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_events.py
--rw-r--r--   0     1001      127     4267 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_game.pyi
--rw-r--r--   0     1001      127     1128 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_zmq.pyi
--rw-r--r--   0     1001      127    19554 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_plugin.py
--rw-r--r--   0     1001      127     3544 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_commands.pyi
--rw-r--r--   0     1001      127    14220 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_commands.py
--rw-r--r--   0     1001      127    13908 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/database.py
--rw-r--r--   0     1001      127    17136 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_core.py
--rw-r--r--   0     1001      127     6386 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_player.pyi
--rw-r--r--   0     1001      127    14210 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/__init__.py
--rw-r--r--   0     1001      127     5652 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_shinqlx.pyi
--rw-r--r--   0     1001      127     4577 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_zmq.py
--rw-r--r--   0     1001      127     7917 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_events.pyi
--rw-r--r--   0     1001      127     1989 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/shinqlx/_handlers.pyi
--rw-r--r--   0     1001      127      105 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/minqlx/database.py
--rw-r--r--   0     1001      127    10423 2024-03-12 20:08:35.000000 shinqlx-0.5.6/python/minqlx/__init__.py
--rw-r--r--   0     1001      127    43825 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/commands.rs
--rw-r--r--   0     1001      127     2247 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/c/activator.rs
--rw-r--r--   0     1001      127    15425 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/c/client.rs
--rw-r--r--   0     1001      127    13844 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/c/current_level.rs
--rw-r--r--   0     1001      127     2234 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/c/cvar.rs
--rw-r--r--   0     1001      127    43716 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/c/game_client.rs
--rw-r--r--   0     1001      127    58510 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/c/game_entity.rs
--rw-r--r--   0     1001      127     8826 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/c/game_item.rs
--rw-r--r--   0     1001      127     1885 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/c/mod.rs
--rw-r--r--   0     1001      127    94031 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/c/quake_types.rs
--rw-r--r--   0     1001      127     9730 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/c/server_static.rs
--rw-r--r--   0     1001      127       41 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/mod.rs
--rw-r--r--   0     1001      127    61357 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/dispatchers.rs
--rw-r--r--   0     1001      127     1800 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/add_console_command.rs
--rw-r--r--   0     1001      127     1573 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/allow_single_player.rs
--rw-r--r--   0     1001      127     1821 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/callvote.rs
--rw-r--r--   0     1001      127     4895 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/client_command.rs
--rw-r--r--   0     1001      127     1682 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/console_command.rs
--rw-r--r--   0     1001      127     1048 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/console_print.rs
--rw-r--r--   0     1001      127     8759 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/destroy_kamikaze_timers.rs
--rw-r--r--   0     1001      127    10319 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/dev_print_items.rs
--rw-r--r--   0     1001      127     7443 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/drop_holdable.rs
--rw-r--r--   0     1001      127     7487 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/force_vote.rs
--rw-r--r--   0     1001      127     4789 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/force_weapon_respawn_time.rs
--rw-r--r--   0     1001      127     2444 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/get_configstring.rs
--rw-r--r--   0     1001      127     2750 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/get_cvar.rs
--rw-r--r--   0     1001      127     3175 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/get_targetting_entities.rs
--rw-r--r--   0     1001      127     5156 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/get_userinfo.rs
--rw-r--r--   0     1001      127     6930 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/kick.rs
--rw-r--r--   0     1001      127     3995 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/mod.rs
--rw-r--r--   0     1001      127     5225 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/noclip.rs
--rw-r--r--   0     1001      127     7636 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/player_info.rs
--rw-r--r--   0     1001      127     4641 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/player_spawn.rs
--rw-r--r--   0     1001      127     6706 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/player_state.rs
--rw-r--r--   0     1001      127     4720 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/player_stats.rs
--rw-r--r--   0     1001      127     5433 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/players_info.rs
--rw-r--r--   0     1001      127     6317 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/register_handler.rs
--rw-r--r--   0     1001      127     5559 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/remove_dropped_items.rs
--rw-r--r--   0     1001      127    21314 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/replace_items.rs
--rw-r--r--   0     1001      127     5789 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/send_server_command.rs
--rw-r--r--   0     1001      127     4643 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_ammo.rs
--rw-r--r--   0     1001      127     4092 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_armor.rs
--rw-r--r--   0     1001      127     1820 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_configstring.rs
--rw-r--r--   0     1001      127     3599 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_cvar.rs
--rw-r--r--   0     1001      127     2313 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_cvar_limit.rs
--rw-r--r--   0     1001      127     4311 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_flight.rs
--rw-r--r--   0     1001      127     3014 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_health.rs
--rw-r--r--   0     1001      127     4388 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_holdable.rs
--rw-r--r--   0     1001      127     4272 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_invulnerability.rs
--rw-r--r--   0     1001      127     4298 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_position.rs
--rw-r--r--   0     1001      127     4329 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_powerups.rs
--rw-r--r--   0     1001      127     4623 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_privileges.rs
--rw-r--r--   0     1001      127     4088 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_score.rs
--rw-r--r--   0     1001      127     4258 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_velocity.rs
--rw-r--r--   0     1001      127     5416 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_weapon.rs
--rw-r--r--   0     1001      127     4586 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/set_weapons.rs
--rw-r--r--   0     1001      127     6370 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/slay_with_mod.rs
--rw-r--r--   0     1001      127     2759 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/embed/spawn_item.rs
--rw-r--r--   0     1001      127     6078 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/flight.rs
--rw-r--r--   0     1001      127     3400 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/holdable.rs
--rw-r--r--   0     1001      127    19575 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/mod.rs
--rw-r--r--   0     1001      127     7184 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/player_info.rs
--rw-r--r--   0     1001      127    13295 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/player_state.rs
--rw-r--r--   0     1001      127     3758 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/player_stats.rs
--rw-r--r--   0     1001      127     7162 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/powerups.rs
--rw-r--r--   0     1001      127     7631 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/vector3.rs
--rw-r--r--   0     1001      127    12678 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/ffi/python/weapons.rs
--rw-r--r--   0     1001      127    58551 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/hooks.rs
--rw-r--r--   0     1001      127     3885 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/lib.rs
--rw-r--r--   0     1001      127     1382 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/patches.rs
--rw-r--r--   0     1001      127    79836 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/quake_live_engine.rs
--rw-r--r--   0     1001      127    30027 2024-03-12 20:08:35.000000 shinqlx-0.5.6/src/quake_live_functions.rs
--rw-r--r--   0     1001      127     2313 2024-03-12 20:08:35.000000 shinqlx-0.5.6/build.rs
--rw-r--r--   0     1001      127       86 2024-03-12 20:08:35.000000 shinqlx-0.5.6/.cargo/config.toml
--rw-r--r--   0        0        0     6223 1970-01-01 00:00:00.000000 shinqlx-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 shinqlx-0.5.7/Cargo.toml
+-rw-r--r--   0     1001      127     1502 2024-05-01 22:44:18.000000 shinqlx-0.5.7/LICENSE
+-rw-r--r--   0     1001      127     5411 2024-05-01 22:44:18.000000 shinqlx-0.5.7/README.md
+-rw-r--r--   0     1001      127      738 2024-05-01 22:44:18.000000 shinqlx-0.5.7/run_server_shinqlx.sh
+-rw-r--r--   0     1001      127    34860 2024-05-01 22:44:29.000000 shinqlx-0.5.7/Cargo.lock
+-rw-r--r--   0     1001      127     2236 2024-05-01 22:44:18.000000 shinqlx-0.5.7/pyproject.toml
+-rw-r--r--   0     1001      127    17136 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_core.py
+-rw-r--r--   0     1001      127     6386 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_player.pyi
+-rw-r--r--   0     1001      127     4267 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_game.pyi
+-rw-r--r--   0     1001      127    31253 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_plugin.pyi
+-rw-r--r--   0     1001      127    19554 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_plugin.py
+-rw-r--r--   0     1001      127     1989 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_handlers.pyi
+-rw-r--r--   0     1001      127    24879 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_events.py
+-rw-r--r--   0     1001      127     1128 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_zmq.pyi
+-rw-r--r--   0     1001      127    19667 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_player.py
+-rw-r--r--   0     1001      127     7917 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_events.pyi
+-rw-r--r--   0     1001      127    14210 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/__init__.py
+-rw-r--r--   0     1001      127     4577 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_zmq.py
+-rw-r--r--   0     1001      127    11991 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/__init__.pyi
+-rw-r--r--   0     1001      127     2045 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_core.pyi
+-rw-r--r--   0     1001      127     5652 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_shinqlx.pyi
+-rw-r--r--   0     1001      127     3541 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_commands.pyi
+-rw-r--r--   0     1001      127    19338 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_handlers.py
+-rw-r--r--   0     1001      127     3536 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/database.pyi
+-rw-r--r--   0     1001      127    14216 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_commands.py
+-rw-r--r--   0     1001      127    12507 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/_game.py
+-rw-r--r--   0     1001      127    13908 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/shinqlx/database.py
+-rw-r--r--   0     1001      127    10423 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/minqlx/__init__.py
+-rw-r--r--   0     1001      127      105 2024-05-01 22:44:18.000000 shinqlx-0.5.7/python/minqlx/database.py
+-rw-r--r--   0     1001      127    44294 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/commands.rs
+-rw-r--r--   0     1001      127     2257 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/c/activator.rs
+-rw-r--r--   0     1001      127    15448 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/c/client.rs
+-rw-r--r--   0     1001      127    13918 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/c/current_level.rs
+-rw-r--r--   0     1001      127     2343 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/c/cvar.rs
+-rw-r--r--   0     1001      127    43725 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/c/game_client.rs
+-rw-r--r--   0     1001      127    58929 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/c/game_entity.rs
+-rw-r--r--   0     1001      127     8840 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/c/game_item.rs
+-rw-r--r--   0     1001      127     1885 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/c/mod.rs
+-rw-r--r--   0     1001      127    94115 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/c/quake_types.rs
+-rw-r--r--   0     1001      127     9755 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/c/server_static.rs
+-rw-r--r--   0     1001      127       41 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/mod.rs
+-rw-r--r--   0     1001      127    62521 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/dispatchers.rs
+-rw-r--r--   0     1001      127     1800 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/add_console_command.rs
+-rw-r--r--   0     1001      127     1573 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/allow_single_player.rs
+-rw-r--r--   0     1001      127     1821 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/callvote.rs
+-rw-r--r--   0     1001      127     4895 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/client_command.rs
+-rw-r--r--   0     1001      127     1682 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/console_command.rs
+-rw-r--r--   0     1001      127     1048 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/console_print.rs
+-rw-r--r--   0     1001      127     8759 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/destroy_kamikaze_timers.rs
+-rw-r--r--   0     1001      127    10336 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/dev_print_items.rs
+-rw-r--r--   0     1001      127     7443 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/drop_holdable.rs
+-rw-r--r--   0     1001      127     7487 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/force_vote.rs
+-rw-r--r--   0     1001      127     4789 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/force_weapon_respawn_time.rs
+-rw-r--r--   0     1001      127     2449 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/get_configstring.rs
+-rw-r--r--   0     1001      127     2719 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/get_cvar.rs
+-rw-r--r--   0     1001      127     3175 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/get_targetting_entities.rs
+-rw-r--r--   0     1001      127     5241 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/get_userinfo.rs
+-rw-r--r--   0     1001      127     6930 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/kick.rs
+-rw-r--r--   0     1001      127     3995 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/mod.rs
+-rw-r--r--   0     1001      127     5225 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/noclip.rs
+-rw-r--r--   0     1001      127     7666 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/player_info.rs
+-rw-r--r--   0     1001      127     4641 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/player_spawn.rs
+-rw-r--r--   0     1001      127     6706 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/player_state.rs
+-rw-r--r--   0     1001      127     4720 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/player_stats.rs
+-rw-r--r--   0     1001      127     5458 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/players_info.rs
+-rw-r--r--   0     1001      127     6286 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/register_handler.rs
+-rw-r--r--   0     1001      127     5559 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/remove_dropped_items.rs
+-rw-r--r--   0     1001      127    22242 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/replace_items.rs
+-rw-r--r--   0     1001      127     5789 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/send_server_command.rs
+-rw-r--r--   0     1001      127     4643 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_ammo.rs
+-rw-r--r--   0     1001      127     4092 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_armor.rs
+-rw-r--r--   0     1001      127     1820 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_configstring.rs
+-rw-r--r--   0     1001      127     3599 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_cvar.rs
+-rw-r--r--   0     1001      127     2313 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_cvar_limit.rs
+-rw-r--r--   0     1001      127     4311 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_flight.rs
+-rw-r--r--   0     1001      127     3014 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_health.rs
+-rw-r--r--   0     1001      127     4388 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_holdable.rs
+-rw-r--r--   0     1001      127     4272 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_invulnerability.rs
+-rw-r--r--   0     1001      127     4298 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_position.rs
+-rw-r--r--   0     1001      127     4329 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_powerups.rs
+-rw-r--r--   0     1001      127     4623 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_privileges.rs
+-rw-r--r--   0     1001      127     4088 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_score.rs
+-rw-r--r--   0     1001      127     4258 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_velocity.rs
+-rw-r--r--   0     1001      127     5416 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_weapon.rs
+-rw-r--r--   0     1001      127     4586 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/set_weapons.rs
+-rw-r--r--   0     1001      127     6370 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/slay_with_mod.rs
+-rw-r--r--   0     1001      127     2759 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/embed/spawn_item.rs
+-rw-r--r--   0     1001      127     7015 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/flight.rs
+-rw-r--r--   0     1001      127     3480 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/holdable.rs
+-rw-r--r--   0     1001      127    19575 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/mod.rs
+-rw-r--r--   0     1001      127     6459 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/player_info.rs
+-rw-r--r--   0     1001      127    11050 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/player_state.rs
+-rw-r--r--   0     1001      127     3385 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/player_stats.rs
+-rw-r--r--   0     1001      127     7219 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/powerups.rs
+-rw-r--r--   0     1001      127     7637 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/vector3.rs
+-rw-r--r--   0     1001      127    12736 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/ffi/python/weapons.rs
+-rw-r--r--   0     1001      127    59195 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/hooks.rs
+-rw-r--r--   0     1001      127     3885 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/lib.rs
+-rw-r--r--   0     1001      127     1382 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/patches.rs
+-rw-r--r--   0     1001      127    84023 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/quake_live_engine.rs
+-rw-r--r--   0     1001      127    30027 2024-05-01 22:44:18.000000 shinqlx-0.5.7/src/quake_live_functions.rs
+-rw-r--r--   0     1001      127     2313 2024-05-01 22:44:18.000000 shinqlx-0.5.7/build.rs
+-rw-r--r--   0     1001      127       86 2024-05-01 22:44:18.000000 shinqlx-0.5.7/.cargo/config.toml
+-rw-r--r--   0        0        0     6223 1970-01-01 00:00:00.000000 shinqlx-0.5.7/PKG-INFO
```

### Comparing `shinqlx-0.5.6/Cargo.toml` & `shinqlx-0.5.7/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cargo-features = ["profile-rustflags"]
 
 [package]
 name = "shinqlx"
-version = "0.5.6"
+version = "0.5.7"
 authors = ["Markus 'ShiN0' Gaertner"]
 edition = "2021"
 readme = "README.md"
 description = "ShiN0's QuakeLive extension in Rust"
 repository = "https://github.com/mgaertne/shinqlx"
 license-file = "LICENSE"
 include = ["run_server_shinqlx.sh"]
@@ -33,48 +33,49 @@
 codegen-units = 1
 
 [profile.release.build-override]
 rustflags = ["-Zlocation-detail=none"]
 
 [dependencies]
 ctor = { version = ">=0.2", features = ["used_linker"] }
-rand = { version = ">=0.8", default-features = false, features = ["getrandom"] }
-pyo3 = { version = ">=0.21.0-beta.0", features = ["pyo3-macros", "extension-module", "nightly"] }
-retour = ">=0.3.1"
+rand = { version = ">=0.9.0-alpha.1", default-features = false, features = ["getrandom"] }
+pyo3 = { version = ">=0.21", features = ["pyo3-macros", "extension-module", "nightly"] }
+retour = { version = ">=0.4.0-alpha.2", default-features = false, features = ["nightly"] }
 derive_builder = { version = ">=0.20", default-features = false, features = ["clippy", "alloc"] }
 once_cell = { version = ">=1.19", default-features = false }
-region = ">=3.0"
 arc-swap = { version = ">=1.7", default-features = false }
 log = { version = ">=0.4", default-features = false }
 log4rs = { version = ">=1.3", default-features = false, features = ["console_appender", "pattern_encoder"] }
 signal-hook = { version = ">=0.3", default-features = false }
-signal-hook-registry = ">=1.4"
+signal-hook-registry = { version = ">=1.4", default-features = false }
 itertools = { version = ">=0.12", default-features = false }
-regex = { version = ">=1.10", features = ["perf"] }
+regex = { version = ">=1.10", features = ["perf", "unicode"] }
 arrayvec = { version = ">=0.7", default-features = false }
 cfg-if = { version = ">=1.0", default-features = false }
-mimalloc = { version = ">=0.1.34", optional = true }
+
+region = { version = ">=3.0", default-features = false, optional = true }
+mimalloc = { version = ">=0.1.34", default-features = false, optional = true }
 
 [target."cfg(target_os=\"linux\")".dependencies]
 procfs = { version = ">=0.16", default-features = false }
 procfs-core = { version = ">=0.16", default-features = false }
 
 [target."cfg(not(target_os=\"windows\"))".dependencies]
-tikv-jemallocator = { version = ">=0.5", optional = true }
+tikv-jemallocator = { version = ">=0.5", default-features = false, optional = true }
 
 [build-dependencies]
-pyo3-build-config = { version = ">=0.21.0-beta.0", features = ["resolve-config"] }
+pyo3-build-config = { version = ">=0.21", default-features = false, features = ["resolve-config"] }
 git2 = { version = ">=0.18", default-features = false }
 
 [dev-dependencies]
 pretty_assertions = { version = ">=1.4", default-features = false, features = ["alloc"] }
 rstest = { version = ">=0.18", default-features = false }
-mockall = { version = ">=0.12", features = ["nightly"] }
+mockall = { version = ">=0.12", default-features = false, features = ["nightly"] }
 serial_test = { version = ">=3.0", default-features = false }
 
 [features]
 default = ["alloc"]
-patches = []
+patches = ["dep:region"]
 alloc = ["dep:tikv-jemallocator", "dep:mimalloc"]
 
 [lints.rust]
 non_local_definitions = "allow"
```

### Comparing `shinqlx-0.5.6/LICENSE` & `shinqlx-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/README.md` & `shinqlx-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/run_server_shinqlx.sh` & `shinqlx-0.5.7/run_server_shinqlx.sh`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/Cargo.lock` & `shinqlx-0.5.7/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
@@ -30,96 +30,97 @@
 name = "anstyle"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
 
 [[package]]
 name = "anyhow"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "arc-swap"
-version = "1.7.0"
+version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b3d0060af21e8d11a926981cc00c6c1541aa91dd64b9f881985c3da1094425f"
+checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
 
 [[package]]
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
- "windows-targets 0.52.4",
+ "windows-targets",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "ctor"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad291aa74992b9b7a7e88c38acbbf6ad7e107f1d90ee8775b7bc1fc3394f485c"
+checksum = "edb49164822f3ee45b17acd4a208cfc1251410cf0cad9a833234c9890774dd9f"
 dependencies = [
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "darling"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
@@ -135,39 +136,26 @@
 checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core",
  "quote",
- "syn 2.0.52",
-]
-
-[[package]]
-name = "dashmap"
-version = "5.5.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978747c1d849a7d2ee5e8adc0159961c48fb7e5db2f06af6723b80123bb53856"
-dependencies = [
- "cfg-if",
- "hashbrown",
- "lock_api",
- "once_cell",
- "parking_lot_core",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "derivative"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcc3dd5e9e9c0b295d6e1e4d811fb6f157d5ffd784b8d202fc62eac8035a770b"
@@ -191,25 +179,25 @@
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "derive_builder_macro"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "206868b8242f27cecce124c19fd88157fbd0dd334df2587f36417bafbc85097b"
 dependencies = [
  "derive_builder_core",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "diff"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
@@ -218,17 +206,17 @@
 name = "downcast"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1435fa1053d8b2fbbe9be7e97eca7f33d37b28409959813daefc1446a14247f1"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "errno"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
@@ -265,49 +253,43 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "git2"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b3ba52851e73b46a4c3df1d89343741112003f0f6f13beb0dfac9e457c3fdcd"
+checksum = "232e6a7bfe35766bf715e55a88b39a700596c0ccfd88cd3680b4cdb40d66ef70"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "libc",
  "libgit2-sys",
  "log",
  "url",
 ]
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
-name = "hashbrown"
-version = "0.14.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
-
-[[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hex"
@@ -352,32 +334,32 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itertools"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -391,17 +373,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libgit2-sys"
 version = "0.16.2+1.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee4126d8b4ee5c9d9ea891dd875cfdc1e9d0950437179104b183d7d8a74d24e8"
 dependencies = [
@@ -409,17 +391,17 @@
  "libc",
  "libz-sys",
  "pkg-config",
 ]
 
 [[package]]
 name = "libmimalloc-sys"
-version = "0.1.35"
+version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3979b5c37ece694f1f5e51e7ecc871fdb0f517ed04ee45f88d15d6d553cb9664"
+checksum = "81eb4061c0582dedea1cbc7aff2240300dd6982e0239d1c99e65c1dbf4a30ba7"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "libudis86-sys"
@@ -429,17 +411,17 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.15"
+version = "1.1.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "037731f5d3aaa87a5675e895b63ddff1a87624bc29f77004ea829809654e48f6"
+checksum = "5e143b5e666b2695d28f6bca6497720813f699c9602dd7f5cac91008b8ada7f9"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -447,17 +429,17 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -488,42 +470,42 @@
  "once_cell",
  "thiserror",
  "thread-id",
  "winapi",
 ]
 
 [[package]]
-name = "mach"
-version = "0.3.2"
+name = "mach2"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b823e83b2affd8f40a9ee8c29dbc56404c1e34cd2710921f2801e2cf29527afa"
+checksum = "19b955cdeb2a02b9117f121ce63aa52d08ade45de53e48fe6a38b39c10f6f709"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
-version = "0.1.39"
+version = "0.1.41"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa01922b5ea280a911e323e4d2fd24b7fe5cc4042e0d2cda3c40775cdc4bdc9c"
+checksum = "9f41a2280ded0da56c8cf898babb86e8f10651a34adcfff190ae9a1159c6908d"
 dependencies = [
  "libmimalloc-sys",
 ]
 
 [[package]]
 name = "mmap-fixed-fixed"
 version = "0.1.3"
@@ -554,15 +536,15 @@
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af7cbce79ec385a1d4f54baa90a76401eb15d9cab93685f62e7e9f942aa00ae2"
 dependencies = [
  "cfg-if",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "num-traits"
 version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
@@ -574,33 +556,33 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -651,49 +633,49 @@
 dependencies = [
  "diff",
  "yansi",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "procfs"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "731e0d9356b0c25f16f33b5be79b1c57b562f141ebfcdb0ad8ac2c13a24293b4"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "hex",
  "lazy_static",
  "procfs-core",
  "rustix",
 ]
 
 [[package]]
 name = "procfs-core"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d3554923a69f4ce04c4a754260c338f505ce22642d3830e049a399fc2059a29"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "hex",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.0-beta.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d0c41d899f822e5f39186d6da130a822a0a43edb19992b51bf4ef6cd0b4cfd1"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -701,98 +683,100 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.0-beta.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5509c2aa78c7e770077e41ba86f806e60dcee812e924ccb2d6fe78c0a0128ce2"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.0-beta.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6bb234a86ed619a661f3bb3c2493aaff9cb937e33e198d17f5f20a15881e155"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.0-beta.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0b787de2c6832eb1eb393c9f82f976a5a87bda979780d9b853878846a8d2e4b"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.0-beta.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e3b7beed357786d2afe845871964e824ad8af0df38a403f7d01cdc81aadb211"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
-version = "0.8.5"
+version = "0.9.0-alpha.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+checksum = "8d31e63ea85be51c423e52ba8f2e68a3efd53eed30203ee029dd09947333693e"
 dependencies = [
  "rand_core",
+ "zerocopy",
 ]
 
 [[package]]
 name = "rand_core"
-version = "0.6.4"
+version = "0.9.0-alpha.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+checksum = "cc89dffba8377c5ec847d12bb41492bda235dba31a25e8b695cd0fe6589eb8c9"
 dependencies = [
  "getrandom",
+ "zerocopy",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
@@ -805,139 +789,154 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "region"
-version = "3.0.0"
+version = "3.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76e189c2369884dce920945e2ddf79b3dff49e071a167dd1817fa9c4c00d512e"
+checksum = "e6b6ebd13bc009aef9cd476c1310d49ac354d36e240cf1bd753290f3dc7199a7"
 dependencies = [
  "bitflags 1.3.2",
  "libc",
- "mach",
- "winapi",
+ "mach2",
+ "windows-sys",
 ]
 
 [[package]]
 name = "relative-path"
 version = "1.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e898588f33fdd5b9420719948f9f2a32c922a246964576f71ba7f24f80610fbc"
 
 [[package]]
 name = "retour"
-version = "0.3.1"
+version = "0.4.0-alpha.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9af44d40e2400b44d491bfaf8eae111b09f23ac4de6e92728e79d93e699c527"
+checksum = "b2bc7e8c671b7a1110edd34a3bab5090fe9d5f78520ff6c7e2a3871f9c159ce5"
 dependencies = [
  "cfg-if",
  "generic-array",
  "libc",
  "libudis86-sys",
  "mmap-fixed-fixed",
  "once_cell",
  "region",
  "slice-pool2",
 ]
 
 [[package]]
 name = "rstest"
-version = "0.18.2"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97eeab2f3c0a199bc4be135c36c924b6590b88c377d416494288c14f2db30199"
+checksum = "9d5316d2a1479eeef1ea21e7f9ddc67c191d497abc8fc3ba2467857abbb68330"
 dependencies = [
  "rstest_macros",
  "rustc_version",
 ]
 
 [[package]]
 name = "rstest_macros"
-version = "0.18.2"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d428f8247852f894ee1be110b375111b586d4fa431f6c46e64ba5a0dcccbe605"
+checksum = "04a9df72cc1f67020b0d63ad9bfe4a323e459ea7eb68e03bd9824db49f9a4c25"
 dependencies = [
  "cfg-if",
  "glob",
  "proc-macro2",
  "quote",
  "regex",
  "relative-path",
  "rustc_version",
- "syn 2.0.52",
+ "syn 2.0.60",
  "unicode-ident",
 ]
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
+name = "scc"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec96560eea317a9cc4e0bb1f6a2c93c09a19b8c4fc5cb3fcc0ec1c094cd783e2"
+dependencies = [
+ "sdd",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
+name = "sdd"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b84345e4c9bd703274a082fb80caaa99b7612be48dfaa1dd9266577ec412309d"
+
+[[package]]
 name = "semver"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serial_test"
-version = "3.0.0"
+version = "3.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "953ad9342b3aaca7cb43c45c097dd008d4907070394bd0751a0aa8817e5a018d"
+checksum = "4b4b487fe2acf240a021cf57c6b2b4903b1e78ca0ecd862a71b71d2a51fed77d"
 dependencies = [
- "dashmap",
- "lazy_static",
+ "once_cell",
  "parking_lot",
+ "scc",
  "serial_test_derive",
 ]
 
 [[package]]
 name = "serial_test_derive"
-version = "3.0.0"
+version = "3.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b93fb4adc70021ac1b47f7d45e8cc4169baaa7ea58483bc5b721d19a26202212"
+checksum = "82fe9db325bcef1fbcde82e078a5cc4efdf787e96b3b9cf45b50b529f2083d67"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "shinqlx"
-version = "0.5.6"
+version = "0.5.7"
 dependencies = [
  "arc-swap",
  "arrayvec",
  "cfg-if",
  "ctor",
  "derive_builder",
  "git2",
@@ -971,32 +970,32 @@
 dependencies = [
  "libc",
  "signal-hook-registry",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "slice-pool2"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a3d689654af89bdfeba29a914ab6ac0236d382eb3b764f7454dde052f2821f8"
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
@@ -1009,17 +1008,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1032,30 +1031,30 @@
 name = "termtree"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3369f5ac52d5eb6ab48c6b4ffdc8efbcad6b89c765749064ba298f2c68a16a76"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "thread-id"
 version = "4.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0ec81c46e9eb50deaa257be2f148adf052d1fb7701cfd55ccfab2525280b70b"
@@ -1178,15 +1177,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1200,15 +1199,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1239,138 +1238,108 @@
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.5",
- "windows_aarch64_msvc 0.48.5",
- "windows_i686_gnu 0.48.5",
- "windows_i686_msvc 0.48.5",
- "windows_x86_64_gnu 0.48.5",
- "windows_x86_64_gnullvm 0.48.5",
- "windows_x86_64_msvc 0.48.5",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
-dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
 
 [[package]]
-name = "windows_i686_gnu"
-version = "0.52.4"
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
-
-[[package]]
-name = "windows_i686_msvc"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+name = "windows_x86_64_msvc"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
-name = "windows_x86_64_msvc"
-version = "0.48.5"
+name = "yansi"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
 
 [[package]]
-name = "windows_x86_64_msvc"
-version = "0.52.4"
+name = "zerocopy"
+version = "0.8.0-alpha.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "db678a6ee512bd06adf35c35be471cae2f9c82a5aed2b5d15e03628c98bddd57"
+dependencies = [
+ "zerocopy-derive",
+]
 
 [[package]]
-name = "yansi"
-version = "0.5.1"
+name = "zerocopy-derive"
+version = "0.8.0-alpha.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
+checksum = "201585ea96d37ee69f2ac769925ca57160cef31acb137c16f38b02b76f4c1e62"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.60",
+]
```

### Comparing `shinqlx-0.5.6/pyproject.toml` & `shinqlx-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_core.pyi` & `shinqlx-0.5.7/python/shinqlx/_core.pyi`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/database.pyi` & `shinqlx-0.5.7/python/shinqlx/database.pyi`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_plugin.pyi` & `shinqlx-0.5.7/python/shinqlx/_plugin.pyi`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_player.py` & `shinqlx-0.5.7/python/shinqlx/_player.py`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_handlers.py` & `shinqlx-0.5.7/python/shinqlx/_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import shinqlx
 
 # ====================================================================
 #                        REGULAR EXPRESSIONS
 # ====================================================================
 
-_re_say = re.compile(r"^say +\"?(?P<msg>.+)\"?$", flags=re.IGNORECASE)
-_re_say_team = re.compile(r"^say_team +\"?(?P<msg>.+)\"?$", flags=re.IGNORECASE)
+_re_say = re.compile(r"^say +\"?(?P<msg>.+)\"$", flags=re.IGNORECASE)
+_re_say_team = re.compile(r"^say_team +\"?(?P<msg>.+)\"$", flags=re.IGNORECASE)
 _re_callvote = re.compile(
     r"^(?:cv|callvote) +(?P<cmd>[^ ]+)(?: \"?(?P<args>.+?)\"?)?$", flags=re.IGNORECASE
 )
 _re_vote = re.compile(r"^vote +(?P<arg>.)", flags=re.IGNORECASE)
 _re_team = re.compile(r"^team +(?P<arg>.)", flags=re.IGNORECASE)
 _re_vote_ended = re.compile(r"^print \"Vote (?P<result>passed|failed).\n\"$")
 _re_userinfo = re.compile(r"^userinfo \"(?P<vars>.+)\"$")
@@ -59,26 +59,26 @@
             return False
         if isinstance(retval, str):
             # Allow plugins to modify the command before passing it on.
             cmd = retval
 
         res = _re_say.match(cmd)
         if res:
-            msg = res.group("msg").replace('"', "")
+            msg = res.group("msg").replace('"', "'")
             channel = shinqlx.CHAT_CHANNEL
             if (
                 shinqlx.EVENT_DISPATCHERS["chat"].dispatch(player, msg, channel)
                 is False
             ):
                 return False
-            return cmd
+            return f'say "{msg}"'
 
         res = _re_say_team.match(cmd)
         if res:
-            msg = res.group("msg").replace('"', "")
+            msg = res.group("msg").replace('"', "'")
             if (
                 player.team == "free"
             ):  # I haven't tried this, but I don't think it's even possible.
                 channel = shinqlx.FREE_CHAT_CHANNEL
             elif player.team == "red":
                 channel = shinqlx.RED_TEAM_CHAT_CHANNEL
             elif player.team == "blue":
@@ -86,15 +86,15 @@
             else:
                 channel = shinqlx.SPECTATOR_CHAT_CHANNEL
             if (
                 shinqlx.EVENT_DISPATCHERS["chat"].dispatch(player, msg, channel)
                 is False
             ):
                 return False
-            return cmd
+            return f'say_team "{msg}"'
 
         res = _re_callvote.match(cmd)
         if res and not shinqlx.Plugin.is_vote_active():
             vote = res.group("cmd")
             args = res.group("args") if res.group("args") else ""
             # Set the caller for vote_started in case the vote goes through.
             # noinspection PyUnresolvedReferences
```

### Comparing `shinqlx-0.5.6/python/shinqlx/__init__.pyi` & `shinqlx-0.5.7/python/shinqlx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_game.py` & `shinqlx-0.5.7/python/shinqlx/_game.py`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_events.py` & `shinqlx-0.5.7/python/shinqlx/_events.py`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_game.pyi` & `shinqlx-0.5.7/python/shinqlx/_game.pyi`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_zmq.pyi` & `shinqlx-0.5.7/python/shinqlx/_zmq.pyi`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_plugin.py` & `shinqlx-0.5.7/python/shinqlx/_plugin.py`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_commands.pyi` & `shinqlx-0.5.7/python/shinqlx/_commands.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,28 +24,28 @@
     ) -> list[str]: ...
 
 class ChatChannel(AbstractChannel):
     fmt: str
 
     def __init__(self, name: str = ..., fmt: str = ...) -> None: ...
     @abstractmethod
-    def receipients(self) -> list[int] | None: ...
+    def recipients(self) -> list[int] | None: ...
     def reply(self, msg: str, limit: int = ..., delimiter: str = ...) -> None: ...
 
 class TeamChatChannel(ChatChannel):
     team: str
     def __init__(self, team: str = ..., name: str = ..., fmt: str = ...) -> None: ...
-    def receipients(self) -> list[int] | None: ...
+    def recipients(self) -> list[int] | None: ...
 
 class TellChannel(ChatChannel):
     recipient: str | int | Player
 
     def __init__(self, player: str | int | Player) -> None: ...
     def __repr__(self) -> str: ...
-    def receipients(self) -> list[int] | None: ...
+    def recipients(self) -> list[int] | None: ...
 
 class ConsoleChannel(AbstractChannel):
     def __init__(self) -> None: ...
     def reply(self, msg: str, limit: int = ..., delimiter: str = ...) -> None: ...
 
 class ClientCommandChannel(AbstractChannel):
     recipient: Player
```

### Comparing `shinqlx-0.5.6/python/shinqlx/_commands.py` & `shinqlx-0.5.7/python/shinqlx/_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,26 +90,26 @@
     """A channel for chat to and from the server."""
 
     def __init__(self, name="chat", fmt='print "{}\n"\n'):
         super().__init__(name)
         self.fmt = fmt
 
     @abstractmethod
-    def receipients(self):
+    def recipients(self):
         pass
 
     @shinqlx.next_frame
     def reply(self, msg, limit=100, delimiter=" "):
         # We convert whatever we got to a string and replace all double quotes
         # to single quotes, since the engine doesn't support escaping them.
         # TODO: rcon can print quotes to clients using NET_OutOfBandPrint. Maybe we should too?
         msg = str(msg).replace('"', "'")
         # Can deal with all the below ChatChannel subclasses.
         last_color = ""
-        targets = self.receipients()
+        targets = self.recipients()
 
         split_msgs = self.split_long_lines(msg, limit, delimiter)
         # We've split messages, but we can still just join them up to 1000-ish
         # bytes before we need to send multiple server cmds.
         joined_msgs: list[str] = []
         for s in split_msgs:
             if len(joined_msgs) == 0:
@@ -136,15 +136,15 @@
 class TeamChatChannel(ChatChannel):
     """A channel for chat to and from the server."""
 
     def __init__(self, team="all", name="chat", fmt='print "{}\n"\n'):
         super().__init__(name=name, fmt=fmt)
         self.team = team
 
-    def receipients(self):
+    def recipients(self):
         if self.team == "all":
             return None
 
         return [
             player.id
             for player in shinqlx.Player.all_players()
             if player.team == self.team
@@ -160,15 +160,15 @@
 
     def __repr__(self):
         player = shinqlx.Plugin.player(self.recipient)
         if player is None:
             return ""
         return f"tell {player.steam_id}"
 
-    def receipients(self):
+    def recipients(self):
         cid = shinqlx.Plugin.client_id(self.recipient)
         if cid is None:
             raise ValueError("Invalid recipient.")
         return [cid]
 
 
 class ConsoleChannel(AbstractChannel):
```

### Comparing `shinqlx-0.5.6/python/shinqlx/database.py` & `shinqlx-0.5.7/python/shinqlx/database.py`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_core.py` & `shinqlx-0.5.7/python/shinqlx/_core.py`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_player.pyi` & `shinqlx-0.5.7/python/shinqlx/_player.pyi`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/__init__.py` & `shinqlx-0.5.7/python/shinqlx/__init__.py`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_shinqlx.pyi` & `shinqlx-0.5.7/python/shinqlx/_shinqlx.pyi`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_zmq.py` & `shinqlx-0.5.7/python/shinqlx/_zmq.py`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_events.pyi` & `shinqlx-0.5.7/python/shinqlx/_events.pyi`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/shinqlx/_handlers.pyi` & `shinqlx-0.5.7/python/shinqlx/_handlers.pyi`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/python/minqlx/__init__.py` & `shinqlx-0.5.7/python/minqlx/__init__.py`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/commands.rs` & `shinqlx-0.5.7/src/commands.rs`

 * *Files 3% similar despite different names*

```diff
@@ -6,49 +6,37 @@
 };
 use crate::MAIN_ENGINE;
 
 use rand::Rng;
 
 #[no_mangle]
 pub extern "C" fn cmd_send_server_command() {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    let Some(cmd_args) = main_engine.cmd_args() else {
-        return;
-    };
-
-    main_engine.send_server_command(None::<Client>, &format!("{}\n", cmd_args));
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine.cmd_args().iter().for_each(|cmd_args| {
+            main_engine.send_server_command(None::<Client>, &format!("{}\n", cmd_args));
+        });
+    });
 }
 
 #[no_mangle]
 pub extern "C" fn cmd_center_print() {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    let Some(cmd_args) = main_engine.cmd_args() else {
-        return;
-    };
-
-    main_engine.send_server_command(None::<Client>, &format!("cp \"{}\"\n", cmd_args));
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine.cmd_args().iter().for_each(|cmd_args| {
+            main_engine.send_server_command(None::<Client>, &format!("cp \"{}\"\n", cmd_args));
+        });
+    });
 }
 
 #[no_mangle]
 pub extern "C" fn cmd_regular_print() {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    let Some(cmd_args) = main_engine.cmd_args() else {
-        return;
-    };
-
-    main_engine.send_server_command(None::<Client>, &format!("print \"{}\n\"\n", cmd_args));
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine.cmd_args().iter().for_each(|cmd_args| {
+            main_engine.send_server_command(None::<Client>, &format!("print \"{}\n\"\n", cmd_args));
+        });
+    });
 }
 
 #[no_mangle]
 pub extern "C" fn cmd_slap() {
     let Some(ref main_engine) = *MAIN_ENGINE.load() else {
         return;
     };
@@ -83,16 +71,18 @@
             "client_id must be a number between 0 and {}.\n",
             maxclients - 1
         ));
         return;
     }
 
     let dmg = if argc > 2 {
-        let passed_dmg = main_engine.cmd_argv(2).unwrap_or("0".into());
-        passed_dmg.parse::<i32>().unwrap_or(0)
+        main_engine
+            .cmd_argv(2)
+            .and_then(|value| value.parse::<i32>().ok())
+            .unwrap_or(0)
     } else {
         0
     };
 
     #[cfg_attr(test, allow(clippy::unnecessary_fallible_conversions))]
     let Ok(mut client_entity) = GameEntity::try_from(client_id) else {
         return;
@@ -214,77 +204,74 @@
     );
 }
 
 #[no_mangle]
 // Execute a pyshinqlx command as if it were the owner executing it.
 // Output will appear in the console.
 pub extern "C" fn cmd_py_rcon() {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    let Some(commands) = main_engine.cmd_args() else {
-        return;
-    };
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        let Some(commands) = main_engine.cmd_args() else {
+            return;
+        };
 
-    rcon_dispatcher(commands);
+        rcon_dispatcher(commands);
+    });
 }
 
 #[no_mangle]
 pub extern "C" fn cmd_py_command() {
-    let Some(ref custom_command_handler) = *CUSTOM_COMMAND_HANDLER.load() else {
-        return;
-    };
-
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    let cmd_args = main_engine.cmd_args();
-
-    Python::with_gil(|py| {
-        let result = match cmd_args {
-            None => custom_command_handler.call0(py),
-            Some(args) => custom_command_handler.call1(py, (args,)),
-        };
-
-        if result.is_err()
-            || result.is_ok_and(|value| value.is_truthy(py).is_ok_and(|result| !result))
-        {
-            main_engine
-                .com_printf("The command failed to be executed. pyshinqlx found no handler.\n");
-        }
-    });
+    CUSTOM_COMMAND_HANDLER
+        .load()
+        .iter()
+        .for_each(|custom_command_handler| {
+            MAIN_ENGINE.load().iter().for_each(|main_engine| {
+                let cmd_args = main_engine.cmd_args();
+
+                Python::with_gil(|py| {
+                    let result = match cmd_args {
+                        None => custom_command_handler.call0(py),
+                        Some(args) => custom_command_handler.call1(py, (args,)),
+                    };
+
+                    if result.is_err()
+                        || result.is_ok_and(|value| {
+                            value.bind(py).is_truthy().is_ok_and(|result| !result)
+                        })
+                    {
+                        main_engine.com_printf(
+                            "The command failed to be executed. pyshinqlx found no handler.\n",
+                        );
+                    }
+                });
+            });
+        });
 }
 
 #[no_mangle]
 pub extern "C" fn cmd_restart_python() {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine.com_printf("Restarting Python...\n");
 
-    main_engine.com_printf("Restarting Python...\n");
-
-    if pyshinqlx_is_initialized() {
-        if pyshinqlx_reload().is_err() {
-            return;
-        };
-        // shinqlx initializes after the first new game starts, but since the game already
-        // start, we manually trigger the event to make it initialize properly.
-        new_game_dispatcher(false);
-        return;
-    }
-
-    if pyshinqlx_initialize().is_err() {
-        return;
-    };
-
-    // shinqlx initializes after the first new game starts, but since the game already
-    // start, we manually trigger the event to make it initialize properly.
-    new_game_dispatcher(false);
+        match pyshinqlx_is_initialized() {
+            true => {
+                pyshinqlx_reload().iter().for_each(|_| {
+                    // shinqlx initializes after the first new game starts, but since the game already
+                    // start, we manually trigger the event to make it initialize properly.
+                    new_game_dispatcher(false);
+                });
+            }
+            false => {
+                pyshinqlx_initialize().iter().for_each(|_| {
+                    // shinqlx initializes after the first new game starts, but since the game already
+                    // start, we manually trigger the event to make it initialize properly.
+                    new_game_dispatcher(false);
+                });
+            }
+        }
+    });
 }
 
 #[cfg(test)]
 mod commands_tests {
     use super::MAIN_ENGINE;
     use super::{
         cmd_center_print, cmd_py_command, cmd_py_rcon, cmd_regular_print, cmd_restart_python,
@@ -318,15 +305,15 @@
 
     #[test]
     #[serial]
     fn cmd_send_server_command_with_server_command() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine
             .expect_cmd_args()
-            .return_const(Some("asdf".into()))
+            .return_const(Some("asdf".to_string()))
             .times(1);
         mock_engine
             .expect_send_server_command()
             .withf(|client, command| client.is_none() && command == "asdf\n")
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
@@ -353,15 +340,15 @@
 
     #[test]
     #[serial]
     fn cmd_center_print_with_server_command() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine
             .expect_cmd_args()
-            .return_const(Some("asdf".into()))
+            .return_const(Some("asdf".to_string()))
             .times(1);
         mock_engine
             .expect_send_server_command()
             .withf(|client, command| client.is_none() && command == "cp \"asdf\"\n")
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
@@ -388,15 +375,15 @@
 
     #[test]
     #[serial]
     fn cmd_regular_print_with_server_command() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine
             .expect_cmd_args()
-            .return_const(Some("asdf".into()))
+            .return_const(Some("asdf".to_string()))
             .times(1);
         mock_engine
             .expect_send_server_command()
             .withf(|client, command| client.is_none() && command == "print \"asdf\n\"\n")
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
@@ -414,15 +401,15 @@
     #[serial]
     fn cmd_slap_with_too_few_args() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(1).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(0))
-            .return_const(Some("!slap".into()))
+            .return_const(Some("!slap".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("Usage: !slap <client_id> [damage]\n"))
             .times(1);
         mock_engine.expect_get_max_clients().return_const(16);
         MAIN_ENGINE.store(Some(mock_engine.into()));
@@ -434,15 +421,15 @@
     #[serial]
     fn cmd_slap_with_unparseable_client_id() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2147483648".into()))
+            .return_const(Some("2147483648".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq(
                 "client_id must be a number between 0 and 15.\n",
             ))
             .times(1);
@@ -456,15 +443,15 @@
     #[serial]
     fn cmd_slap_with_too_small_client_id() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("-1".into()))
+            .return_const(Some("-1".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq(
                 "client_id must be a number between 0 and 15.\n",
             ))
             .times(1);
@@ -478,15 +465,15 @@
     #[serial]
     fn cmd_slap_with_too_large_client_id() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("42".into()))
+            .return_const(Some("42".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq(
                 "client_id must be a number between 0 and 15.\n",
             ))
             .times(1);
@@ -501,15 +488,15 @@
     #[serial]
     fn cmd_slap_with_game_entity_not_in_use() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2".into()))
+            .return_const(Some("2".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("The player is currently not active.\n"))
             .times(1);
         mock_engine.expect_get_max_clients().return_const(16);
         MAIN_ENGINE.store(Some(mock_engine.into()));
@@ -536,15 +523,15 @@
     #[serial]
     fn cmd_slap_with_game_entity_no_health() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2".into()))
+            .return_const(Some("2".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("The player is currently not active.\n"))
             .times(1);
         mock_engine.expect_get_max_clients().return_const(16);
         MAIN_ENGINE.store(Some(mock_engine.into()));
@@ -572,15 +559,15 @@
     #[serial]
     fn cmd_slap_with_no_damage_provided_slaps() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2".into()))
+            .return_const(Some("2".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("Slapping...\n"))
             .times(1);
         mock_engine
             .expect_send_server_command()
@@ -643,20 +630,20 @@
     #[serial]
     fn cmd_slap_with_provided_damage_slaps() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(3).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2".into()))
+            .return_const(Some("2".to_string()))
             .times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(2))
-            .return_const(Some("1".into()))
+            .return_const(Some("1".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("Slapping...\n"))
             .times(1);
         mock_engine
             .expect_send_server_command()
@@ -724,20 +711,20 @@
     #[serial]
     fn cmd_slap_with_provided_damage_provided_slaps_and_kills() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(3).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2".into()))
+            .return_const(Some("2".to_string()))
             .times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(2))
-            .return_const(Some("666".into()))
+            .return_const(Some("666".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("Slapping...\n"))
             .times(1);
         mock_engine
             .expect_send_server_command()
@@ -809,20 +796,20 @@
     #[serial]
     fn cmd_slap_with_unparseable_provided_damage_slaps() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(3).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2".into()))
+            .return_const(Some("2".to_string()))
             .times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(2))
-            .return_const(Some("2147483648".into()))
+            .return_const(Some("2147483648".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("Slapping...\n"))
             .times(1);
         mock_engine
             .expect_send_server_command()
@@ -891,15 +878,15 @@
     #[serial]
     fn cmd_slay_with_too_few_args() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(1).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(0))
-            .return_const(Some("!slap".into()))
+            .return_const(Some("!slap".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("Usage: !slap <client_id> [damage]\n"))
             .times(1);
         mock_engine.expect_get_max_clients().return_const(16);
         MAIN_ENGINE.store(Some(mock_engine.into()));
@@ -911,15 +898,15 @@
     #[serial]
     fn cmd_slay_with_unparseable_client_id() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2147483648".into()))
+            .return_const(Some("2147483648".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq(
                 "client_id must be a number between 0 and 15.\n",
             ))
             .times(1);
@@ -933,15 +920,15 @@
     #[serial]
     fn cmd_slay_with_too_small_client_id() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("-1".into()))
+            .return_const(Some("-1".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq(
                 "client_id must be a number between 0 and 15.\n",
             ))
             .times(1);
@@ -955,15 +942,15 @@
     #[serial]
     fn cmd_slay_with_too_large_client_id() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("42".into()))
+            .return_const(Some("42".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq(
                 "client_id must be a number between 0 and 15.\n",
             ))
             .times(1);
@@ -978,15 +965,15 @@
     #[serial]
     fn cmd_slay_with_game_entity_not_in_use() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2".into()))
+            .return_const(Some("2".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("The player is currently not active.\n"))
             .times(1);
         mock_engine.expect_get_max_clients().return_const(16);
         MAIN_ENGINE.store(Some(mock_engine.into()));
@@ -1013,15 +1000,15 @@
     #[serial]
     fn cmd_slay_with_game_entity_no_health() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2".into()))
+            .return_const(Some("2".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("The player is currently not active.\n"))
             .times(1);
         mock_engine.expect_get_max_clients().return_const(16);
         MAIN_ENGINE.store(Some(mock_engine.into()));
@@ -1048,15 +1035,15 @@
     #[serial]
     fn cmd_slay_player_is_slain() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine.expect_cmd_argc().return_const(2).times(1);
         mock_engine
             .expect_cmd_argv()
             .with(predicate::eq(1))
-            .return_const(Some("2".into()))
+            .return_const(Some("2".to_string()))
             .times(1);
         mock_engine
             .expect_com_printf()
             .with(predicate::eq("Slaying player...\n"))
             .times(1);
         mock_engine
             .expect_send_server_command()
@@ -1134,15 +1121,15 @@
 
     #[test]
     #[serial]
     fn cmd_py_rcon_forwards_args() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine
             .expect_cmd_args()
-            .return_const(Some("!version".into()))
+            .return_const(Some("!version".to_string()))
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
         let rcon_dispatcher_ctx = rcon_dispatcher_context();
         rcon_dispatcher_ctx
             .expect::<String>()
             .with(predicate::eq("!version".to_string()))
@@ -1161,15 +1148,15 @@
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn cmd_py_command_with_arguments(_pyshinqlx_setup: ()) {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine
             .expect_cmd_args()
-            .return_const(Some("custom parameter".into()))
+            .return_const(Some("custom parameter".to_string()))
             .times(1);
         mock_engine.expect_com_printf().times(0);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
         Python::with_gil(|py| {
             let pymodule = PyModule::from_code_bound(
                 py,
@@ -1179,15 +1166,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let custom_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CUSTOM_COMMAND_HANDLER.store(Some(custom_command_handler.into_py(py).into()));
+            CUSTOM_COMMAND_HANDLER.store(Some(custom_command_handler.unbind().into()));
 
             cmd_py_command();
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -1207,15 +1194,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let custom_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CUSTOM_COMMAND_HANDLER.store(Some(custom_command_handler.into_py(py).into()));
+            CUSTOM_COMMAND_HANDLER.store(Some(custom_command_handler.unbind().into()));
 
             cmd_py_command();
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -1240,15 +1227,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let custom_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CUSTOM_COMMAND_HANDLER.store(Some(custom_command_handler.into_py(py).into()));
+            CUSTOM_COMMAND_HANDLER.store(Some(custom_command_handler.unbind().into()));
 
             cmd_py_command();
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -1273,15 +1260,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let custom_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CUSTOM_COMMAND_HANDLER.store(Some(custom_command_handler.into_py(py).into()));
+            CUSTOM_COMMAND_HANDLER.store(Some(custom_command_handler.unbind().into()));
 
             cmd_py_command();
         });
     }
 
     #[test]
     #[serial]
```

### Comparing `shinqlx-0.5.6/src/ffi/c/activator.rs` & `shinqlx-0.5.7/src/ffi/c/activator.rs`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 impl TryFrom<*mut gentity_t> for Activator {
     type Error = QuakeLiveEngineError;
 
     fn try_from(game_entity: *mut gentity_t) -> Result<Self, Self::Error> {
         unsafe { game_entity.as_ref() }
             .map(|gentity| Self { activator: gentity })
             .ok_or(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into(),
+                "null pointer passed".to_string(),
             ))
     }
 }
 
 impl Activator {
     pub(crate) fn get_owner_num(&self) -> i32 {
         self.activator.r.ownerNum
@@ -46,15 +46,15 @@
     use pretty_assertions::assert_eq;
 
     #[test]
     fn activator_try_from_null_results_in_error() {
         assert_eq!(
             Activator::try_from(ptr::null_mut() as *mut gentity_t),
             Err(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into()
+                "null pointer passed".to_string()
             ))
         );
     }
 
     #[test]
     fn activator_try_from_valid_entity() {
         let mut gentity = GEntityBuilder::default()
```

### Comparing `shinqlx-0.5.6/src/ffi/c/client.rs` & `shinqlx-0.5.7/src/ffi/c/client.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use super::prelude::*;
 use crate::prelude::*;
 use crate::MAIN_ENGINE;
 
-use alloc::ffi::CString;
+use alloc::{borrow::Cow, ffi::CString};
 use core::ffi::{c_char, CStr};
 
 #[derive(Debug, PartialEq)]
 #[repr(transparent)]
 pub(crate) struct Client {
     client_t: &'static mut client_t,
 }
@@ -22,27 +22,27 @@
 impl TryFrom<*mut client_t> for Client {
     type Error = QuakeLiveEngineError;
 
     fn try_from(client: *mut client_t) -> Result<Self, Self::Error> {
         unsafe { client.as_mut() }
             .map(|client_t| Self { client_t })
             .ok_or(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into(),
+                "null pointer passed".to_string(),
             ))
     }
 }
 
 impl TryFrom<i32> for Client {
     type Error = QuakeLiveEngineError;
 
     fn try_from(client_id: i32) -> Result<Self, Self::Error> {
         let server_static = ServerStatic::try_get()?;
         let client = unsafe { server_static.try_get_client_by_id(client_id) }?;
         Self::try_from(client)
-            .map_err(|_| QuakeLiveEngineError::ClientNotFound("client not found".into()))
+            .map_err(|_| QuakeLiveEngineError::ClientNotFound("client not found".to_string()))
     }
 }
 
 impl AsMut<client_t> for Client {
     fn as_mut(&mut self) -> &mut client_t {
         self.client_t
     }
@@ -72,51 +72,46 @@
 
     pub(crate) fn disconnect<T>(&mut self, reason: T)
     where
         T: AsRef<str>,
     {
         let c_reason = CString::new(reason.as_ref()).unwrap_or_else(|_| CString::new("").unwrap());
 
-        let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-            return;
-        };
-
-        let Ok(detour) = main_engine.sv_dropclient_detour() else {
-            return;
-        };
-
-        detour.call(self.client_t, c_reason.as_ptr());
+        MAIN_ENGINE.load().iter().for_each(|main_engine| {
+            main_engine
+                .sv_dropclient_detour()
+                .iter()
+                .for_each(|detour| {
+                    detour.call(self.client_t, c_reason.as_ptr());
+                });
+        });
     }
 
-    pub(crate) fn get_name(&self) -> String {
-        unsafe { CStr::from_ptr(&self.client_t.name as *const c_char) }
-            .to_string_lossy()
-            .into()
+    pub(crate) fn get_name(&self) -> Cow<str> {
+        unsafe { CStr::from_ptr(&self.client_t.name as *const c_char) }.to_string_lossy()
     }
 
-    pub(crate) fn get_user_info(&self) -> String {
-        unsafe { CStr::from_ptr(self.client_t.userinfo.as_ptr()) }
-            .to_string_lossy()
-            .into()
+    pub(crate) fn get_user_info(&self) -> Cow<'_, str> {
+        unsafe { CStr::from_ptr(self.client_t.userinfo.as_ptr()) }.to_string_lossy()
     }
 
     pub(crate) fn get_steam_id(&self) -> u64 {
         self.client_t.steam_id
     }
 }
 
 #[cfg(test)]
 mockall::mock! {
     pub(crate) Client {
-        pub(crate) fn get_name(&self) -> String;
+        pub(crate) fn get_name(&self) -> Cow<'_, str>;
         pub(crate) fn has_gentity(&self) -> bool;
         pub(crate) fn get_client_id(&self) -> i32;
         pub(crate) fn get_state(&self) -> clientState_t;
         pub(crate) fn disconnect(&mut self, reason: &str);
-        pub(crate) fn get_user_info(&self) -> String;
+        pub(crate) fn get_user_info(&self) -> Cow<'_, str>;
         pub(crate) fn get_steam_id(&self) -> u64;
     }
 
     impl TryFrom<*mut client_t> for Client {
         type Error = QuakeLiveEngineError;
         fn try_from(client: *mut client_t) -> Result<Self, QuakeLiveEngineError>;
     }
@@ -149,15 +144,15 @@
     use retour::GenericDetour;
 
     #[test]
     fn client_try_from_null_results_in_error() {
         assert_eq!(
             Client::try_from(ptr::null() as *const client_t),
             Err(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into()
+                "null pointer passed".to_string()
             ))
         );
     }
 
     #[test]
     fn client_try_from_valid_client() {
         let mut client = ClientBuilder::default()
@@ -215,15 +210,15 @@
                 .returning(|_| Ok(ptr::null_mut() as *mut client_t));
             Ok(server_static_mock)
         });
 
         assert_eq!(
             Client::try_from(2),
             Err(QuakeLiveEngineError::ClientNotFound(
-                "client not found".into()
+                "client not found".to_string()
             ))
         );
     }
 
     #[test]
     #[serial]
     fn client_get_client_id_when_no_serverstatic_found() {
```

### Comparing `shinqlx-0.5.6/src/ffi/c/current_level.rs` & `shinqlx-0.5.7/src/ffi/c/current_level.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 impl TryFrom<*mut level_locals_t> for CurrentLevel {
     type Error = QuakeLiveEngineError;
 
     fn try_from(level_locals: *mut level_locals_t) -> Result<Self, Self::Error> {
         unsafe { level_locals.as_mut() }
             .map(|level| Self { level })
             .ok_or(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into(),
+                "null pointer passed".to_string(),
             ))
     }
 }
 
 const OFFSET_LEVEL: usize = 0x4A1;
 
 impl CurrentLevel {
@@ -50,46 +50,44 @@
     }
 
     pub(crate) fn get_leveltime(&self) -> i32 {
         self.level.time
     }
 
     pub(crate) fn callvote(&mut self, vote: &str, vote_disp: &str, vote_time: Option<i32>) {
-        let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-            return;
-        };
-
-        let actual_vote_time = vote_time.unwrap_or(30);
+        MAIN_ENGINE.load().iter().for_each(|main_engine| {
+            let actual_vote_time = vote_time.unwrap_or(30);
 
-        let mut vote_bytes_iter = vote.bytes();
-        self.level.voteString[0..vote.len()]
-            .fill_with(|| vote_bytes_iter.next().unwrap() as c_char);
-        self.level.voteString[vote.len()..].fill(0 as c_char);
-
-        let mut vote_disp_bytes_iter = vote_disp.bytes();
-        self.level.voteDisplayString[0..vote_disp.len()]
-            .fill_with(|| vote_disp_bytes_iter.next().unwrap() as c_char);
-        self.level.voteDisplayString[vote_disp.len()..].fill(0 as c_char);
-
-        self.level.voteTime = self.level.time - 30000 + actual_vote_time * 1000;
-        self.level.voteYes = 0;
-        self.level.voteNo = 0;
-
-        let maxclients = main_engine.get_max_clients();
-
-        #[cfg_attr(test, allow(clippy::unnecessary_fallible_conversions))]
-        (0..maxclients)
-            .filter_map(|client_id| GameEntity::try_from(client_id).ok())
-            .filter_map(|game_entity| game_entity.get_game_client().ok())
-            .for_each(|mut game_client| game_client.set_vote_pending());
-
-        shinqlx_set_configstring(CS_VOTE_STRING, vote_disp);
-        shinqlx_set_configstring(CS_VOTE_TIME, &format!("{}", self.level.voteTime));
-        shinqlx_set_configstring(CS_VOTE_YES, "0");
-        shinqlx_set_configstring(CS_VOTE_NO, "0");
+            let mut vote_bytes_iter = vote.bytes();
+            self.level.voteString[0..vote.len()]
+                .fill_with(|| vote_bytes_iter.next().unwrap() as c_char);
+            self.level.voteString[vote.len()..].fill(0 as c_char);
+
+            let mut vote_disp_bytes_iter = vote_disp.bytes();
+            self.level.voteDisplayString[0..vote_disp.len()]
+                .fill_with(|| vote_disp_bytes_iter.next().unwrap() as c_char);
+            self.level.voteDisplayString[vote_disp.len()..].fill(0 as c_char);
+
+            self.level.voteTime = self.level.time - 30000 + actual_vote_time * 1000;
+            self.level.voteYes = 0;
+            self.level.voteNo = 0;
+
+            let maxclients = main_engine.get_max_clients();
+
+            #[cfg_attr(test, allow(clippy::unnecessary_fallible_conversions))]
+            (0..maxclients)
+                .filter_map(|client_id| GameEntity::try_from(client_id).ok())
+                .filter_map(|game_entity| game_entity.get_game_client().ok())
+                .for_each(|mut game_client| game_client.set_vote_pending());
+
+            shinqlx_set_configstring(CS_VOTE_STRING, vote_disp);
+            shinqlx_set_configstring(CS_VOTE_TIME, &format!("{}", self.level.voteTime));
+            shinqlx_set_configstring(CS_VOTE_YES, "0");
+            shinqlx_set_configstring(CS_VOTE_NO, "0");
+        });
     }
 
     pub(crate) fn set_training_map(&mut self, is_training_map: bool) {
         self.level.mapIsTrainingMap = is_training_map.into();
     }
 }
 
@@ -151,15 +149,15 @@
     }
 
     #[test]
     fn current_level_from_null() {
         assert_eq!(
             CurrentLevel::try_from(ptr::null_mut()),
             Err(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into()
+                "null pointer passed".to_string()
             )),
         );
     }
 
     #[test]
     fn current_level_from_valid_level_locals() {
         let mut level = LevelLocalsBuilder::default()
```

### Comparing `shinqlx-0.5.6/src/ffi/c/cvar.rs` & `shinqlx-0.5.7/src/ffi/c/cvar.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 use super::prelude::*;
 use crate::prelude::*;
 
+use alloc::borrow::Cow;
 use core::ffi::CStr;
 
 #[derive(Debug, PartialEq)]
 #[repr(transparent)]
 pub(crate) struct CVar {
     cvar: &'static mut cvar_t,
 }
 
 impl TryFrom<*mut cvar_t> for CVar {
     type Error = QuakeLiveEngineError;
 
     fn try_from(cvar: *mut cvar_t) -> Result<Self, Self::Error> {
         unsafe { cvar.as_mut() }.map(|cvar| Self { cvar }).ok_or(
-            QuakeLiveEngineError::NullPointerPassed("null pointer passed".into()),
+            QuakeLiveEngineError::NullPointerPassed("null pointer passed".to_string()),
         )
     }
 }
 
 impl CVar {
-    pub(crate) fn get_string(&self) -> String {
-        unsafe { CStr::from_ptr(self.cvar.string).to_string_lossy().into() }
+    pub(crate) fn get_string(&self) -> Cow<str> {
+        if self.cvar.string.is_null() {
+            return "".into();
+        }
+        unsafe { CStr::from_ptr(self.cvar.string).to_string_lossy() }
     }
 
     pub(crate) fn get_integer(&self) -> i32 {
         self.cvar.integer
     }
 }
 
@@ -39,15 +43,15 @@
     use pretty_assertions::assert_eq;
 
     #[test]
     fn cvar_try_from_null_results_in_error() {
         assert_eq!(
             CVar::try_from(ptr::null_mut() as *mut cvar_t),
             Err(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into()
+                "null pointer passed".to_string()
             ))
         );
     }
 
     #[test]
     fn cvar_try_from_valid_cvar() {
         let mut cvar = CVarBuilder::default()
```

### Comparing `shinqlx-0.5.6/src/ffi/c/game_client.rs` & `shinqlx-0.5.7/src/ffi/c/game_client.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use super::prelude::*;
 use crate::prelude::*;
 
+use alloc::borrow::Cow;
 use core::ffi::{c_int, CStr};
 
 #[derive(Debug, PartialEq)]
 #[repr(transparent)]
 pub(crate) struct GameClient {
     game_client: &'static mut gclient_t,
 }
@@ -14,32 +15,30 @@
 
     fn try_from(game_client: *mut gclient_t) -> Result<Self, Self::Error> {
         unsafe { game_client.as_mut() }
             .map(|gclient_t| Self {
                 game_client: gclient_t,
             })
             .ok_or(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into(),
+                "null pointer passed".to_string(),
             ))
     }
 }
 
 impl GameClient {
     pub(crate) fn get_client_num(&self) -> i32 {
         self.game_client.ps.clientNum
     }
 
     pub(crate) fn get_connection_state(&self) -> clientConnected_t {
         self.game_client.pers.connected
     }
 
-    pub(crate) fn get_player_name(&self) -> String {
-        unsafe { CStr::from_ptr(self.game_client.pers.netname.as_ptr()) }
-            .to_string_lossy()
-            .into()
+    pub(crate) fn get_player_name(&self) -> Cow<str> {
+        unsafe { CStr::from_ptr(self.game_client.pers.netname.as_ptr()) }.to_string_lossy()
     }
 
     pub(crate) fn get_team(&self) -> team_t {
         self.game_client.sess.sessionTeam
     }
 
     pub(crate) fn get_privileges(&self) -> privileges_t {
@@ -324,15 +323,15 @@
 }
 
 #[cfg(test)]
 mockall::mock! {
     pub(crate) GameClient {
         pub(crate) fn get_client_num(&self) -> i32;
         pub(crate) fn get_connection_state(&self) -> clientConnected_t;
-        pub(crate) fn get_player_name(&self) -> String;
+        pub(crate) fn get_player_name(&self) -> Cow<'_, str>;
         pub(crate) fn get_team(&self) -> team_t;
         pub(crate) fn get_privileges(&self) -> privileges_t;
         pub(crate) fn remove_kamikaze_flag(&mut self);
         pub(crate) fn set_privileges<T>(&mut self, privileges: T)
         where
             T: Into<privileges_t> + 'static;
         pub(crate) fn is_alive(&self) -> bool;
@@ -406,15 +405,15 @@
     use rstest::*;
 
     #[test]
     fn game_client_try_from_null_results_in_error() {
         assert_eq!(
             GameClient::try_from(ptr::null_mut() as *mut gclient_t),
             Err(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into()
+                "null pointer passed".to_string()
             ))
         );
     }
 
     #[test]
     fn game_client_try_from_valid_value_result() {
         let mut gclient = GClientBuilder::default()
```

### Comparing `shinqlx-0.5.6/src/ffi/c/game_entity.rs` & `shinqlx-0.5.7/src/ffi/c/game_entity.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use crate::hooks::shinqlx_set_configstring;
 use crate::prelude::*;
 use crate::quake_live_engine::{
     ComPrintf, FreeEntity, GetConfigstring, RegisterDamage, StartKamikaze, TryLaunchItem,
 };
 use crate::MAIN_ENGINE;
 
-use alloc::vec;
+use alloc::{borrow::Cow, vec};
 use core::{
     f32::consts::PI,
     ffi::{c_char, c_float, c_int, CStr},
 };
 
 #[derive(Debug, PartialEq)]
 #[repr(transparent)]
@@ -27,15 +27,15 @@
 impl TryFrom<*mut gentity_t> for GameEntity {
     type Error = QuakeLiveEngineError;
 
     fn try_from(game_entity: *mut gentity_t) -> Result<Self, Self::Error> {
         unsafe { game_entity.as_mut() }
             .map(|gentity| Self { gentity_t: gentity })
             .ok_or(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into(),
+                "null pointer passed".to_string(),
             ))
     }
 }
 
 impl TryFrom<i32> for GameEntity {
     type Error = QuakeLiveEngineError;
 
@@ -48,91 +48,86 @@
         if entity_id < 0 {
             return Err(QuakeLiveEngineError::InvalidId(entity_id));
         }
 
         let g_entities = GameEntity::get_entities_list();
         if g_entities.is_null() {
             return Err(QuakeLiveEngineError::EntityNotFound(
-                "g_entities not initialized".into(),
+                "g_entities not initialized".to_string(),
             ));
         }
 
         Self::try_from(unsafe { g_entities.offset(entity_id as isize) })
-            .map_err(|_| QuakeLiveEngineError::EntityNotFound("entity not found".into()))
+            .map_err(|_| QuakeLiveEngineError::EntityNotFound("entity not found".to_string()))
     }
 }
 
 impl TryFrom<u32> for GameEntity {
     type Error = QuakeLiveEngineError;
 
     fn try_from(entity_id: u32) -> Result<Self, Self::Error> {
         if entity_id >= MAX_GENTITIES {
             return Err(QuakeLiveEngineError::InvalidId(entity_id as i32));
         }
         let g_entities = GameEntity::get_entities_list();
         if g_entities.is_null() {
             return Err(QuakeLiveEngineError::EntityNotFound(
-                "g_entities not initialized".into(),
+                "g_entities not initialized".to_string(),
             ));
         }
 
         Self::try_from(unsafe { g_entities.offset(entity_id as isize) })
-            .map_err(|_| QuakeLiveEngineError::EntityNotFound("entity not found".into()))
+            .map_err(|_| QuakeLiveEngineError::EntityNotFound("entity not found".to_string()))
     }
 }
 
 #[no_mangle]
 pub(crate) extern "C" fn ShiNQlx_Touch_Item(
     ent: *mut gentity_t,
     other: *mut gentity_t,
     trace: *mut trace_t,
 ) {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    let Ok(original_func) = main_engine.touch_item_orig() else {
-        return;
-    };
-
-    let Some(entity) = (unsafe { ent.as_ref() }) else {
-        return;
-    };
-
-    if entity.parent != other {
-        original_func(ent, other, trace);
-    }
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine
+            .touch_item_orig()
+            .iter()
+            .for_each(|original_func| {
+                (unsafe { ent.as_ref() }).iter().for_each(|entity| {
+                    if entity.parent != other {
+                        original_func(ent, other, trace);
+                    }
+                });
+            });
+    });
 }
 
 #[no_mangle]
 pub(crate) extern "C" fn ShiNQlx_Switch_Touch_Item(ent: *mut gentity_t) {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    let Ok(touch_item_func) = main_engine.touch_item_orig() else {
-        return;
-    };
-
-    let Ok(free_entity_func) = main_engine.g_free_entity_orig() else {
-        return;
-    };
-
-    let Some(mut_ent) = (unsafe { ent.as_mut() }) else {
-        return;
-    };
-
-    let level_time = CurrentLevel::try_get()
-        .ok()
-        .map(|current_level| current_level.get_leveltime())
-        .unwrap_or_default();
-
-    mut_ent.touch = Some(touch_item_func);
-    mut_ent.think = Some(free_entity_func);
-    mut_ent.nextthink = level_time + 29000;
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine
+            .touch_item_orig()
+            .iter()
+            .for_each(|touch_item_func| {
+                main_engine
+                    .g_free_entity_orig()
+                    .iter()
+                    .for_each(|free_entity_func| {
+                        (unsafe { ent.as_mut() }).iter_mut().for_each(|mut_ent| {
+                            let level_time = CurrentLevel::try_get()
+                                .ok()
+                                .map(|current_level| current_level.get_leveltime())
+                                .unwrap_or_default();
+
+                            mut_ent.touch = Some(*touch_item_func);
+                            mut_ent.think = Some(*free_entity_func);
+                            mut_ent.nextthink = level_time + 29000;
+                        });
+                    });
+            });
+    });
 }
 
 const OFFSET_G_ENTITIES: usize = 0x11B;
 
 impl GameEntity {
     fn get_entities_list() -> *mut gentity_t {
         #[cfg(test)]
@@ -178,15 +173,15 @@
     pub(crate) fn get_player_name(&self) -> String {
         match self.get_game_client() {
             Err(_) => "".into(),
             Ok(game_client) => {
                 if game_client.get_connection_state() == clientConnected_t::CON_DISCONNECTED {
                     "".into()
                 } else {
-                    game_client.get_player_name()
+                    game_client.get_player_name().into()
                 }
             }
         }
     }
 
     pub(crate) fn get_team(&self) -> team_t {
         match self.get_game_client() {
@@ -253,18 +248,16 @@
         );
     }
 
     pub(crate) fn in_use(&self) -> bool {
         self.gentity_t.inuse.into()
     }
 
-    pub(crate) fn get_classname(&self) -> String {
-        unsafe { CStr::from_ptr(self.gentity_t.classname) }
-            .to_string_lossy()
-            .into()
+    pub(crate) fn get_classname(&self) -> Cow<str> {
+        unsafe { CStr::from_ptr(self.gentity_t.classname) }.to_string_lossy()
     }
 
     pub(crate) fn is_game_item(&self, item_type: entityType_t) -> bool {
         self.gentity_t.s.eType == item_type as i32
     }
 
     pub(crate) fn is_respawning_weapon(&self) -> bool {
@@ -356,15 +349,15 @@
                 return;
             };
             self.gentity_t.s.modelindex = item_id;
             self.gentity_t.classname = gitem.get_classname().as_ptr() as *const c_char;
             self.gentity_t.item = gitem.as_ref();
 
             // this forces client to load new item
-            let mut items = main_engine.get_configstring(CS_ITEMS as u16);
+            let mut items = main_engine.get_configstring(CS_ITEMS as u16).to_string();
             items.replace_range(item_id as usize..=item_id as usize, "1");
             shinqlx_set_configstring(item_id as u32, &items);
         } else {
             self.free_entity();
         }
     }
 
@@ -423,15 +416,15 @@
         pub(crate) fn get_privileges(&self) -> privileges_t;
         pub(crate) fn get_game_client(&self) -> Result<GameClient, QuakeLiveEngineError>;
         pub(crate) fn get_activator(&self) -> Result<Activator, QuakeLiveEngineError>;
         pub(crate) fn get_health(&self) -> i32;
         pub(crate) fn set_health(&mut self, new_health: i32);
         pub(crate) fn slay_with_mod(&mut self, mean_of_death: meansOfDeath_t);
         pub(crate) fn in_use(&self) -> bool;
-        pub(crate) fn get_classname(&self) -> String;
+        pub(crate) fn get_classname(&self) -> Cow<'_, str>;
         pub(crate) fn is_game_item(&self, item_type: entityType_t) -> bool;
         pub(crate) fn is_respawning_weapon(&self) -> bool;
         pub(crate) fn set_respawn_time(&mut self, respawn_time: i32);
         pub(crate) fn has_flags(&self) -> bool;
         pub(crate) fn is_dropped_item(&self) -> bool;
         pub(crate) fn get_client_number(&self) -> i32;
         pub(crate) fn drop_holdable(&mut self);
@@ -694,15 +687,15 @@
     }
 
     #[test]
     fn game_entity_try_from_null_results_in_error() {
         assert_eq!(
             GameEntity::try_from(ptr::null_mut() as *mut gentity_t),
             Err(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into()
+                "null pointer passed".to_string()
             ))
         );
     }
 
     #[test]
     fn game_entity_try_from_valid_gentity() {
         let mut gentity = GEntityBuilder::default()
@@ -742,15 +735,15 @@
         get_entities_list_ctx
             .expect()
             .returning(|| ptr::null_mut() as *mut gentity_t);
 
         assert_eq!(
             GameEntity::try_from(42i32),
             Err(QuakeLiveEngineError::EntityNotFound(
-                "g_entities not initialized".into()
+                "g_entities not initialized".to_string()
             ))
         );
     }
 
     //noinspection DuplicatedCode
     #[test]
     #[serial]
@@ -798,15 +791,15 @@
         get_entities_list_ctx
             .expect()
             .returning(|| ptr::null_mut() as *mut gentity_t);
 
         assert_eq!(
             GameEntity::try_from(42u32),
             Err(QuakeLiveEngineError::EntityNotFound(
-                "g_entities not initialized".into()
+                "g_entities not initialized".to_string()
             ))
         );
     }
 
     //noinspection DuplicatedCode
     #[test]
     #[serial]
```

### Comparing `shinqlx-0.5.6/src/ffi/c/game_item.rs` & `shinqlx-0.5.7/src/ffi/c/game_item.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use super::prelude::*;
 use crate::prelude::*;
 use crate::quake_live_engine::{GameAddEvent, TryLaunchItem};
 use crate::MAIN_ENGINE;
 
+use alloc::borrow::Cow;
 use core::ffi::{c_float, CStr};
 
 #[derive(Debug, PartialEq)]
 #[repr(transparent)]
 pub(crate) struct GameItem {
     gitem_t: &'static mut gitem_t,
 }
@@ -26,29 +27,29 @@
 impl TryFrom<*mut gitem_t> for GameItem {
     type Error = QuakeLiveEngineError;
 
     fn try_from(game_item: *mut gitem_t) -> Result<Self, Self::Error> {
         unsafe { game_item.as_mut() }
             .map(|gitem| Self { gitem_t: gitem })
             .ok_or(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into(),
+                "null pointer passed".to_string(),
             ))
     }
 }
 
 impl TryFrom<i32> for GameItem {
     type Error = QuakeLiveEngineError;
 
     fn try_from(item_id: i32) -> Result<Self, Self::Error> {
         if item_id < 0 || item_id >= GameItem::get_num_items() {
             return Err(QuakeLiveEngineError::InvalidId(item_id));
         }
         let bg_itemlist = GameItem::get_item_list();
         Self::try_from(unsafe { bg_itemlist.offset(item_id as isize) as *mut gitem_t })
-            .map_err(|_| QuakeLiveEngineError::EntityNotFound("entity not found".into()))
+            .map_err(|_| QuakeLiveEngineError::EntityNotFound("entity not found".to_string()))
     }
 }
 
 const OFFSET_BG_ITEMLIST: usize = 0x2A;
 
 impl GameItem {
     pub(crate) fn get_num_items() -> i32 {
@@ -94,18 +95,16 @@
         let bg_itemlist_ptr_ptr =
             base_address as usize + launch_item_orig as usize + OFFSET_BG_ITEMLIST + 4;
 
         let bg_itemlist_ptr = unsafe { ptr::read(bg_itemlist_ptr_ptr as *const u64) };
         bg_itemlist_ptr as *mut gitem_t
     }
 
-    pub(crate) fn get_classname(&self) -> String {
-        unsafe { CStr::from_ptr(self.gitem_t.classname) }
-            .to_string_lossy()
-            .into()
+    pub(crate) fn get_classname(&self) -> Cow<str> {
+        unsafe { CStr::from_ptr(self.gitem_t.classname) }.to_string_lossy()
     }
 
     pub(crate) fn spawn(&mut self, origin: (i32, i32, i32)) {
         let Some(ref main_engine) = *MAIN_ENGINE.load() else {
             return;
         };
 
@@ -129,15 +128,15 @@
 }
 
 #[cfg(test)]
 mockall::mock! {
     pub(crate) GameItem {
         pub(crate) fn get_mocked_item_list() -> *mut gitem_t;
         pub(crate) fn get_num_items() -> i32;
-        pub(crate) fn get_classname(&self) -> String;
+        pub(crate) fn get_classname(&self) -> Cow<'_, str>;
         pub(crate) fn spawn(&mut self, _origin: (i32, i32, i32));
     }
 
     impl TryFrom<*mut gitem_t> for GameItem {
         type Error = QuakeLiveEngineError;
         fn try_from(game_item: *mut gitem_t) -> Result<Self, QuakeLiveEngineError> {}
     }
@@ -168,15 +167,15 @@
     use pretty_assertions::assert_eq;
 
     #[test]
     fn game_item_from_null_pointer() {
         assert_eq!(
             GameItem::try_from(ptr::null_mut() as *mut gitem_t),
             Err(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into()
+                "null pointer passed".to_string()
             ))
         );
     }
 
     #[test]
     fn game_item_from_valid_item() {
         let mut gitem = GItemBuilder::default()
```

### Comparing `shinqlx-0.5.6/src/ffi/c/mod.rs` & `shinqlx-0.5.7/src/ffi/c/mod.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/c/quake_types.rs` & `shinqlx-0.5.7/src/ffi/c/quake_types.rs`

 * *Files 1% similar despite different names*

```diff
@@ -609,15 +609,15 @@
         match value {
             0 => Ok(powerup_t::PW_QUAD),
             1 => Ok(powerup_t::PW_BATTLESUIT),
             2 => Ok(powerup_t::PW_HASTE),
             3 => Ok(powerup_t::PW_INVIS),
             4 => Ok(powerup_t::PW_REGEN),
             5 => Ok(powerup_t::PW_INVULNERABILITY),
-            _ => Err("invalid power up".into()),
+            _ => Err("invalid power up".to_string()),
         }
     }
 }
 
 #[cfg(test)]
 pub(crate) mod powerup_t_tests {
     use super::powerup_t;
@@ -628,15 +628,18 @@
     pub(crate) fn powerup_t_from_integer() {
         assert_eq!(powerup_t::try_from(0), Ok(powerup_t::PW_QUAD));
         assert_eq!(powerup_t::try_from(1), Ok(powerup_t::PW_BATTLESUIT));
         assert_eq!(powerup_t::try_from(2), Ok(powerup_t::PW_HASTE));
         assert_eq!(powerup_t::try_from(3), Ok(powerup_t::PW_INVIS));
         assert_eq!(powerup_t::try_from(4), Ok(powerup_t::PW_REGEN));
         assert_eq!(powerup_t::try_from(5), Ok(powerup_t::PW_INVULNERABILITY));
-        assert_eq!(powerup_t::try_from(666), Err("invalid power up".into()));
+        assert_eq!(
+            powerup_t::try_from(666),
+            Err("invalid power up".to_string())
+        );
     }
 
     #[test]
     pub(crate) fn powerup_t_from_usize() {
         assert_eq!(powerup_t::try_from(0usize), Ok(powerup_t::PW_QUAD));
         assert_eq!(powerup_t::try_from(1usize), Ok(powerup_t::PW_BATTLESUIT));
         assert_eq!(powerup_t::try_from(2usize), Ok(powerup_t::PW_HASTE));
@@ -644,15 +647,15 @@
         assert_eq!(powerup_t::try_from(4usize), Ok(powerup_t::PW_REGEN));
         assert_eq!(
             powerup_t::try_from(5usize),
             Ok(powerup_t::PW_INVULNERABILITY)
         );
         assert_eq!(
             powerup_t::try_from(666usize),
-            Err("invalid power up".into())
+            Err("invalid power up".to_string())
         );
     }
 }
 
 #[derive(Debug, Copy, Clone, PartialEq, Eq, Hash)]
 #[repr(u32)]
 pub enum holdable_t {
@@ -714,15 +717,15 @@
             9 => Ok(weapon_t::WP_BFG),
             10 => Ok(weapon_t::WP_GRAPPLING_HOOK),
             11 => Ok(weapon_t::WP_NAILGUN),
             12 => Ok(weapon_t::WP_PROX_LAUNCHER),
             13 => Ok(weapon_t::WP_CHAINGUN),
             14 => Ok(weapon_t::WP_HMG),
             15 => Ok(weapon_t::WP_HANDS),
-            _ => Err("invalid weapon".into()),
+            _ => Err("invalid weapon".to_string()),
         }
     }
 }
 
 #[cfg(test)]
 pub(crate) mod weapon_t_tests {
     use super::weapon_t;
@@ -764,17 +767,17 @@
         assert_eq!(weapon_t::try_from(9), Ok(weapon_t::WP_BFG));
         assert_eq!(weapon_t::try_from(10), Ok(weapon_t::WP_GRAPPLING_HOOK));
         assert_eq!(weapon_t::try_from(11), Ok(weapon_t::WP_NAILGUN));
         assert_eq!(weapon_t::try_from(12), Ok(weapon_t::WP_PROX_LAUNCHER));
         assert_eq!(weapon_t::try_from(13), Ok(weapon_t::WP_CHAINGUN));
         assert_eq!(weapon_t::try_from(14), Ok(weapon_t::WP_HMG));
         assert_eq!(weapon_t::try_from(15), Ok(weapon_t::WP_HANDS));
-        assert_eq!(weapon_t::try_from(16), Err("invalid weapon".into()));
-        assert_eq!(weapon_t::try_from(-1), Err("invalid weapon".into()));
-        assert_eq!(weapon_t::try_from(666), Err("invalid weapon".into()));
+        assert_eq!(weapon_t::try_from(16), Err("invalid weapon".to_string()));
+        assert_eq!(weapon_t::try_from(-1), Err("invalid weapon".to_string()));
+        assert_eq!(weapon_t::try_from(666), Err("invalid weapon".to_string()));
     }
 }
 
 #[derive(Debug, Copy, Clone, PartialEq, Eq, Hash)]
 #[repr(u32)]
 pub enum weaponstate_t {
     WEAPON_READY = 0,
@@ -887,15 +890,15 @@
             27 => Ok(meansOfDeath_t::MOD_JUICED),
             28 => Ok(meansOfDeath_t::MOD_GRAPPLE),
             29 => Ok(meansOfDeath_t::MOD_SWITCH_TEAMS),
             30 => Ok(meansOfDeath_t::MOD_THAW),
             31 => Ok(meansOfDeath_t::MOD_LIGHTNING_DISCHARGE),
             32 => Ok(meansOfDeath_t::MOD_HMG),
             33 => Ok(meansOfDeath_t::MOD_RAILGUN_HEADSHOT),
-            _ => Err("invalid means of death".into()),
+            _ => Err("invalid means of death".to_string()),
         }
     }
 }
 
 #[cfg(test)]
 pub(crate) mod meansofdeath_t_tests {
     use super::meansOfDeath_t;
@@ -996,19 +999,19 @@
         assert_eq!(meansOfDeath_t::try_from(32), Ok(meansOfDeath_t::MOD_HMG));
         assert_eq!(
             meansOfDeath_t::try_from(33),
             Ok(meansOfDeath_t::MOD_RAILGUN_HEADSHOT)
         );
         assert_eq!(
             meansOfDeath_t::try_from(-1),
-            Err("invalid means of death".into())
+            Err("invalid means of death".to_string())
         );
         assert_eq!(
             meansOfDeath_t::try_from(666),
-            Err("invalid means of death".into())
+            Err("invalid means of death".to_string())
         );
     }
 }
 
 #[derive(Debug, Copy, Clone, PartialEq, Eq, Hash)]
 #[repr(u32)]
 pub enum spectatorState_t {
```

### Comparing `shinqlx-0.5.6/src/ffi/c/server_static.rs` & `shinqlx-0.5.7/src/ffi/c/server_static.rs`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     fn try_from(server_static: *mut serverStatic_t) -> Result<Self, Self::Error> {
         unsafe { server_static.as_mut() }
             .map(|svs| Self {
                 serverStatic_t: svs,
             })
             .ok_or(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into(),
+                "null pointer passed".to_string(),
             ))
     }
 }
 
 impl ServerStatic {
     pub(crate) fn try_get() -> Result<Self, QuakeLiveEngineError> {
         let Some(ref main_engine) = *MAIN_ENGINE.load() else {
@@ -55,21 +55,21 @@
         &self,
         client_t: &client_t,
     ) -> Result<i32, QuakeLiveEngineError> {
         let offset = (client_t as *const client_t).offset_from(self.serverStatic_t.clients);
 
         if !(0..MAX_CLIENTS as isize).contains(&offset) {
             return Err(QuakeLiveEngineError::ClientNotFound(
-                "client not found".into(),
+                "client not found".to_string(),
             ));
         }
 
         offset
             .try_into()
-            .map_err(|_| QuakeLiveEngineError::ClientNotFound("client not found".into()))
+            .map_err(|_| QuakeLiveEngineError::ClientNotFound("client not found".to_string()))
     }
 }
 
 #[cfg(test)]
 mockall::mock! {
     pub(crate) TestServerStatic {
         pub(crate) fn try_get() -> Result<Self, QuakeLiveEngineError>;
@@ -99,15 +99,15 @@
     use pretty_assertions::assert_eq;
 
     #[test]
     fn server_static_try_from_null_results_in_error() {
         assert_eq!(
             ServerStatic::try_from(ptr::null_mut()),
             Err(QuakeLiveEngineError::NullPointerPassed(
-                "null pointer passed".into()
+                "null pointer passed".to_string()
             ))
         );
     }
 
     #[test]
     fn server_static_try_from_valid_server_static() {
         let mut server_static = ServerStaticBuilder::default()
@@ -230,15 +230,15 @@
             .build()
             .expect("this should not happen");
         let rust_server_static = ServerStatic::try_from(&mut server_static as *mut serverStatic_t)
             .expect("this should not happen");
         assert_eq!(
             unsafe { rust_server_static.try_determine_client_id(&client) },
             Err(QuakeLiveEngineError::ClientNotFound(
-                "client not found".into()
+                "client not found".to_string()
             ))
         );
     }
 
     #[test]
     fn server_static_determine_client_id_from_ok_client() {
         let mut client = ClientBuilder::default()
```

### Comparing `shinqlx-0.5.6/src/ffi/python/dispatchers.rs` & `shinqlx-0.5.7/src/ffi/python/dispatchers.rs`

 * *Files 7% similar despite different names*

```diff
@@ -4,361 +4,374 @@
 use log::error;
 
 pub(crate) fn client_command_dispatcher<T>(client_id: i32, cmd: T) -> Option<String>
 where
     T: AsRef<str>,
 {
     if !pyshinqlx_is_initialized() {
-        return Some(cmd.as_ref().into());
+        return Some(cmd.as_ref().to_string());
     }
 
-    let Some(ref client_command_handler) = *CLIENT_COMMAND_HANDLER.load() else {
-        return Some(cmd.as_ref().into());
-    };
-
-    Python::with_gil(
-        |py| match client_command_handler.call1(py, (client_id, cmd.as_ref())) {
-            Err(_) => {
-                error!(target: "shinqlx", "client_command_handler returned an error.");
-                Some(cmd.as_ref().into())
-            }
-            Ok(returned) => match returned.extract::<String>(py) {
-                Err(_) => match returned.extract::<bool>(py) {
-                    Err(_) => Some(cmd.as_ref().into()),
-                    Ok(result_bool) => {
-                        if !result_bool {
-                            None
+    CLIENT_COMMAND_HANDLER
+        .load()
+        .as_ref()
+        .map(|client_command_handler| {
+            Python::with_gil(|py| {
+                client_command_handler
+            .bind(py)
+            .call1((client_id, cmd.as_ref()))
+            .map(|returned| {
+                returned
+                    .extract::<bool>()
+                    .map(|bool_value| {
+                        if bool_value {
+                            Some(cmd.as_ref().to_string())
                         } else {
-                            Some(cmd.as_ref().into())
+                            None
                         }
-                    }
-                },
-                Ok(result_string) => Some(result_string),
-            },
-        },
-    )
+                    })
+                    .unwrap_or(Some(
+                        returned.extract::<String>().unwrap_or(cmd.as_ref().to_string()),
+                    ))
+            })
+            .unwrap_or_else(|e| {
+                error!(target: "shinqlx", "client_command_handler returned an error: {:?}.", e);
+                Some(cmd.as_ref().to_string())
+            })
+            })
+        })
+        .unwrap_or(Some(cmd.as_ref().to_string()))
 }
 
 pub(crate) fn server_command_dispatcher<T>(client_id: Option<i32>, cmd: T) -> Option<String>
 where
     T: AsRef<str>,
 {
     if !pyshinqlx_is_initialized() {
-        return Some(cmd.as_ref().into());
+        return Some(cmd.as_ref().to_string());
     }
 
-    let Some(ref server_command_handler) = *SERVER_COMMAND_HANDLER.load() else {
-        return Some(cmd.as_ref().into());
-    };
-
-    Python::with_gil(|py| {
-        match server_command_handler.call1(py, (client_id.unwrap_or(-1), cmd.as_ref())) {
-            Err(_) => {
-                error!(target: "shinqlx", "server_command_handler returned an error.");
-                Some(cmd.as_ref().into())
-            }
-            Ok(returned) => match returned.extract::<String>(py) {
-                Err(_) => match returned.extract::<bool>(py) {
-                    Err(_) => Some(cmd.as_ref().into()),
-                    Ok(result_bool) => {
-                        if !result_bool {
-                            None
-                        } else {
-                            Some(cmd.as_ref().into())
-                        }
-                    }
-                },
-                Ok(result_string) => Some(result_string),
-            },
-        }
-    })
+    SERVER_COMMAND_HANDLER
+        .load()
+        .as_ref()
+        .map(|server_command_handler| {
+            Python::with_gil(|py| {
+                server_command_handler
+                .bind(py)
+                .call1((client_id.unwrap_or(-1), cmd.as_ref()))
+                .map(|returned| {
+                    returned
+                        .extract::<bool>()
+                        .map(|bool_value| {
+                            if bool_value {
+                                Some(cmd.as_ref().to_string())
+                            } else {
+                                None
+                            }
+                        })
+                        .unwrap_or(Some(
+                            returned.extract::<String>().unwrap_or(cmd.as_ref().to_string()),
+                        ))
+                })
+                .unwrap_or_else(|e| {
+                    error!(target: "shinqlx", "server_command_handler returned an error: {:?}.", e);
+                    Some(cmd.as_ref().to_string())
+                })
+            })
+        })
+        .unwrap_or(Some(cmd.as_ref().to_string()))
 }
 
 pub(crate) fn frame_dispatcher() {
     if !pyshinqlx_is_initialized() {
         return;
     }
 
-    let Some(ref frame_handler) = *FRAME_HANDLER.load() else {
-        return;
-    };
-
-    let result = Python::with_gil(|py| frame_handler.call0(py));
-    if result.is_err() {
-        error!(target: "shinqlx", "frame_handler returned an error.");
-    }
+    FRAME_HANDLER.load().iter().for_each(|frame_handler| {
+        Python::with_gil(|py| {
+            if let Err(e) = frame_handler.bind(py).call0() {
+                error!(target: "shinqlx", "frame_handler returned an error: {:?}.", e);
+            }
+        });
+    });
 }
 
 #[allow(clippy::question_mark)]
 pub(crate) fn client_connect_dispatcher(client_id: i32, is_bot: bool) -> Option<String> {
     if !pyshinqlx_is_initialized() {
         return None;
     }
 
-    let Some(ref client_connect_handler) = *PLAYER_CONNECT_HANDLER.load() else {
-        return None;
-    };
-
-    {
-        let allowed_clients = ALLOW_FREE_CLIENT.load(Ordering::SeqCst);
-        ALLOW_FREE_CLIENT.store(allowed_clients | (1 << client_id as u64), Ordering::SeqCst);
-    }
-
-    let result: Option<String> =
-        Python::with_gil(
-            |py| match client_connect_handler.call1(py, (client_id, is_bot)) {
-                Err(_) => None,
-                Ok(returned) => match returned.extract::<String>(py) {
-                    Err(_) => match returned.extract::<bool>(py) {
-                        Err(_) => None,
-                        Ok(result_bool) => {
-                            if !result_bool {
-                                Some("You are banned from this server.".into())
-                            } else {
-                                None
-                            }
-                        }
-                    },
-                    Ok(result_string) => Some(result_string),
-                },
-            },
-        );
-
-    {
-        let allowed_clients = ALLOW_FREE_CLIENT.load(Ordering::SeqCst);
-        ALLOW_FREE_CLIENT.store(allowed_clients & !(1 << client_id as u64), Ordering::SeqCst);
-    }
+    PLAYER_CONNECT_HANDLER
+        .load()
+        .as_ref()
+        .map(|client_connect_handler| {
+            {
+                let allowed_clients = ALLOW_FREE_CLIENT.load(Ordering::SeqCst);
+                ALLOW_FREE_CLIENT
+                    .store(allowed_clients | (1 << client_id as u64), Ordering::SeqCst);
+            }
 
-    result
+            let result = Python::with_gil(|py| {
+                client_connect_handler
+                    .bind(py)
+                    .call1((client_id, is_bot))
+                    .ok()
+                    .and_then(|returned| {
+                        returned
+                            .extract::<bool>()
+                            .map(|bool_value| {
+                                if !bool_value {
+                                    Some("You are banned from this server.".to_string())
+                                } else {
+                                    None
+                                }
+                            })
+                            .unwrap_or(returned.extract::<String>().ok())
+                    })
+            });
+
+            {
+                let allowed_clients = ALLOW_FREE_CLIENT.load(Ordering::SeqCst);
+                ALLOW_FREE_CLIENT
+                    .store(allowed_clients & !(1 << client_id as u64), Ordering::SeqCst);
+            }
+            result
+        })
+        .unwrap_or(None)
 }
 
 pub(crate) fn client_disconnect_dispatcher<T>(client_id: i32, reason: T)
 where
     T: AsRef<str>,
 {
     if !pyshinqlx_is_initialized() {
         return;
     }
 
-    let Some(ref client_disconnect_handler) = *PLAYER_DISCONNECT_HANDLER.load() else {
-        return;
-    };
-
-    {
-        let allowed_clients = ALLOW_FREE_CLIENT.load(Ordering::SeqCst);
-        ALLOW_FREE_CLIENT.store(allowed_clients | (1 << client_id as u64), Ordering::SeqCst);
-    }
+    PLAYER_DISCONNECT_HANDLER
+        .load()
+        .iter()
+        .for_each(|client_disconnect_handler| {
+            {
+                let allowed_clients = ALLOW_FREE_CLIENT.load(Ordering::SeqCst);
+                ALLOW_FREE_CLIENT
+                    .store(allowed_clients | (1 << client_id as u64), Ordering::SeqCst);
+            }
 
-    let result =
-        Python::with_gil(|py| client_disconnect_handler.call1(py, (client_id, reason.as_ref())));
-    if result.is_err() {
-        error!(target: "shinqlx", "client_disconnect_handler returned an error.");
-    }
+            let result = Python::with_gil(|py| {
+                client_disconnect_handler.call1(py, (client_id, reason.as_ref()))
+            });
+            if result.is_err() {
+                error!(target: "shinqlx", "client_disconnect_handler returned an error.");
+            }
 
-    {
-        let allowed_clients = ALLOW_FREE_CLIENT.load(Ordering::SeqCst);
-        ALLOW_FREE_CLIENT.store(allowed_clients & !(1 << client_id as u64), Ordering::SeqCst);
-    }
+            {
+                let allowed_clients = ALLOW_FREE_CLIENT.load(Ordering::SeqCst);
+                ALLOW_FREE_CLIENT
+                    .store(allowed_clients & !(1 << client_id as u64), Ordering::SeqCst);
+            }
+        });
 }
 
 pub(crate) fn client_loaded_dispatcher(client_id: i32) {
     if !pyshinqlx_is_initialized() {
         return;
     }
 
-    let Some(ref client_loaded_handler) = *PLAYER_LOADED_HANDLER.load() else {
-        return;
-    };
-
-    let result = Python::with_gil(|py| client_loaded_handler.call1(py, (client_id,)));
-    if result.is_err() {
-        error!(target: "shinqlx", "client_loaded_handler returned an error.");
-    }
+    PLAYER_LOADED_HANDLER
+        .load()
+        .iter()
+        .for_each(|client_loaded_handler| {
+            Python::with_gil(|py| {
+                if let Err(e) = client_loaded_handler.bind(py).call1((client_id,)) {
+                    error!(target: "shinqlx", "client_loaded_handler returned an error: {:?}.", e);
+                }
+            });
+        });
 }
 
 pub(crate) fn new_game_dispatcher(restart: bool) {
     if !pyshinqlx_is_initialized() {
         return;
     }
 
-    let Some(ref new_game_handler) = *NEW_GAME_HANDLER.load() else {
-        return;
-    };
-
-    let result = Python::with_gil(|py| new_game_handler.call1(py, (restart,)));
-    if result.is_err() {
-        error!(target: "shinqlx", "new_game_handler returned an error.");
-    }
+    NEW_GAME_HANDLER.load().iter().for_each(|new_game_handler| {
+        Python::with_gil(|py| {
+            if let Err(e) = new_game_handler.bind(py).call1((restart,)) {
+                error!(target: "shinqlx", "new_game_handler returned an error: {:?}.", e);
+            }
+        });
+    });
 }
 
 pub(crate) fn set_configstring_dispatcher<T, U>(index: T, value: U) -> Option<String>
 where
     T: Into<u32>,
     U: AsRef<str>,
 {
     if !pyshinqlx_is_initialized() {
-        return Some(value.as_ref().into());
+        return Some(value.as_ref().to_string());
     }
 
-    let Some(ref set_configstring_handler) = *SET_CONFIGSTRING_HANDLER.load() else {
-        return Some(value.as_ref().into());
-    };
-
-    Python::with_gil(|py| {
-        match set_configstring_handler.call1(py, (index.into(), value.as_ref())) {
-            Err(_) => {
-                error!(target: "shinqlx", "set_configstring_handler returned an error.");
-                Some(value.as_ref().into())
-            }
-            Ok(returned) => match returned.extract::<String>(py) {
-                Err(_) => match returned.extract::<bool>(py) {
-                    Err(_) => Some(value.as_ref().into()),
-                    Ok(result_bool) => {
-                        if !result_bool {
-                            None
-                        } else {
-                            Some(value.as_ref().into())
-                        }
-                    }
-                },
-                Ok(result_string) => Some(result_string),
-            },
-        }
-    })
+    SET_CONFIGSTRING_HANDLER
+        .load()
+        .as_ref()
+        .map(|set_configstring_handler| {
+            Python::with_gil(|py| {
+                set_configstring_handler
+                    .bind(py)
+                    .call1((index.into(), value.as_ref()))
+                    .map(|returned| {
+                        returned
+                            .extract::<bool>()
+                            .map(|bool_value| {
+                                if bool_value {
+                                    Some(value.as_ref().to_string())
+                                } else {
+                                    None
+                                }
+                            })
+                            .unwrap_or(Some(
+                                returned
+                                    .extract::<String>()
+                                    .unwrap_or(value.as_ref().to_string()),
+                            ))
+                    })
+                    .unwrap_or_else(|e| {
+                        error!(target: "shinqlx", "set_configstring_handler returned an error: {:?}.", e);
+                        Some(value.as_ref().to_string())})
+            })
+        })
+        .unwrap_or(Some(value.as_ref().to_string()))
 }
 
 pub(crate) fn rcon_dispatcher<T>(cmd: T)
 where
     T: AsRef<str>,
 {
     if !pyshinqlx_is_initialized() {
         return;
     }
 
-    let Some(ref rcon_handler) = *RCON_HANDLER.load() else {
-        return;
-    };
-
-    let result = Python::with_gil(|py| rcon_handler.call1(py, (cmd.as_ref(),)));
-    if result.is_err() {
-        error!(target: "shinqlx", "rcon_handler returned an error.");
-    }
+    RCON_HANDLER.load().iter().for_each(|rcon_handler| {
+        Python::with_gil(|py| {
+            if let Err(e) = rcon_handler.bind(py).call1((cmd.as_ref(),)) {
+                error!(target: "shinqlx", "rcon_handler returned an error: {:?}.", e);
+            }
+        });
+    });
 }
 
 pub(crate) fn console_print_dispatcher<T>(text: T) -> Option<String>
 where
     T: AsRef<str>,
 {
     if !pyshinqlx_is_initialized() {
-        return Some(text.as_ref().into());
+        return Some(text.as_ref().to_string());
     }
 
-    let Some(ref console_print_handler) = *CONSOLE_PRINT_HANDLER.load() else {
-        return Some(text.as_ref().into());
-    };
-
-    Python::with_gil(
-        |py| match console_print_handler.call1(py, (text.as_ref(),)) {
-            Err(_) => {
-                error!(target: "shinqlx", "console_print_handler returned an error.");
-                Some(text.as_ref().into())
-            }
-            Ok(returned) => match returned.extract::<String>(py) {
-                Err(_) => match returned.extract::<bool>(py) {
-                    Err(_) => Some(text.as_ref().into()),
-                    Ok(result_bool) => {
-                        if !result_bool {
-                            None
-                        } else {
-                            Some(text.as_ref().into())
-                        }
-                    }
+    CONSOLE_PRINT_HANDLER
+        .load()
+        .as_ref()
+        .map(|console_print_handler| {
+            Python::with_gil(
+                |py| {
+                    console_print_handler.bind(py).call1((text.as_ref(),)).map(|returned| {
+                        returned.extract::<bool>().map(|bool_value| {
+                            if bool_value {
+                                Some(text.as_ref().to_string())
+                            } else {
+                                None
+                            }
+                        }).unwrap_or({
+                            Some(returned.extract::<String>().unwrap_or(text.as_ref().to_string()))
+                        })
+                    }).unwrap_or_else(|e| {
+                        error!(target: "shinqlx", "console_print_handler returned an error: {:?}.", e);
+                        Some(text.as_ref().to_string())
+                    })
                 },
-                Ok(result_string) => Some(result_string),
-            },
-        },
-    )
+            )
+        })
+        .unwrap_or(Some(text.as_ref().to_string()))
 }
 
 pub(crate) fn client_spawn_dispatcher(client_id: i32) {
     if !pyshinqlx_is_initialized() {
         return;
     }
 
-    let Some(ref client_spawn_handler) = *PLAYER_SPAWN_HANDLER.load() else {
-        return;
-    };
-
-    let result = Python::with_gil(|py| client_spawn_handler.call1(py, (client_id,)));
-    if result.is_err() {
-        error!(target: "shinqlx", "client_spawn_handler returned an error.");
-    }
+    PLAYER_SPAWN_HANDLER
+        .load()
+        .iter()
+        .for_each(|client_spawn_handler| {
+            Python::with_gil(|py| {
+                if let Err(e) = client_spawn_handler.bind(py).call1((client_id,)) {
+                    error!(target: "shinqlx", "client_spawn_handler returned an error: {:?}.", e);
+                }
+            });
+        });
 }
 
 pub(crate) fn kamikaze_use_dispatcher(client_id: i32) {
     if !pyshinqlx_is_initialized() {
         return;
     }
 
-    let Some(ref kamikaze_use_handler) = *KAMIKAZE_USE_HANDLER.load() else {
-        return;
-    };
-
-    let result = Python::with_gil(|py| kamikaze_use_handler.call1(py, (client_id,)));
-    if result.is_err() {
-        error!(target: "shinqlx", "kamikaze_use_handler returned an error.");
-    }
+    KAMIKAZE_USE_HANDLER
+        .load()
+        .iter()
+        .for_each(|kamikaze_use_handler| {
+            Python::with_gil(|py| {
+                if let Err(e) = kamikaze_use_handler.bind(py).call1((client_id,)) {
+                    error!(target: "shinqlx", "kamikaze_use_handler returned an error: {:?}.", e);
+                }
+            });
+        });
 }
 
 pub(crate) fn kamikaze_explode_dispatcher(client_id: i32, is_used_on_demand: bool) {
     if !pyshinqlx_is_initialized() {
         return;
     }
 
-    let Some(ref kamikaze_explode_handler) = *KAMIKAZE_EXPLODE_HANDLER.load() else {
-        return;
-    };
-
-    let result =
-        Python::with_gil(|py| kamikaze_explode_handler.call1(py, (client_id, is_used_on_demand)));
-    if result.is_err() {
-        error!(target: "shinqlx", "kamikaze_explode_handler returned an error.");
-    }
+    KAMIKAZE_EXPLODE_HANDLER.load().iter().for_each(|kamikaze_explode_handler| {
+        Python::with_gil(|py| {
+            if let Err(e) = kamikaze_explode_handler.bind(py).call1((client_id, is_used_on_demand)) {
+                error!(target: "shinqlx", "kamikaze_explode_handler returned an error: {:?}.", e);
+            }
+        });
+    });
 }
 
 pub(crate) fn damage_dispatcher(
     target_client_id: i32,
     attacker_client_id: Option<i32>,
     damage: i32,
     dflags: i32,
     means_of_death: i32,
 ) {
     if !pyshinqlx_is_initialized() {
         return;
     }
 
-    let Some(ref damage_handler) = *DAMAGE_HANDLER.load() else {
-        return;
-    };
-
-    let result = Python::with_gil(|py| {
-        damage_handler.call1(
-            py,
-            (
+    DAMAGE_HANDLER.load().iter().for_each(|damage_handler| {
+        Python::with_gil(|py| {
+            if let Err(e) = damage_handler.bind(py).call1((
                 target_client_id,
                 attacker_client_id,
                 damage,
                 dflags,
                 means_of_death,
-            ),
-        )
+            )) {
+                error!(target: "shinqlx", "damage_handler returned an error: {:?}.", e);
+            }
+        });
     });
-    if result.is_err() {
-        error!(target: "shinqlx", "damage_handler returned an error.");
-    }
 }
 
 #[cfg(test)]
 mod pyshinqlx_dispatcher_tests {
     use super::{
         client_command_dispatcher, client_connect_dispatcher, client_disconnect_dispatcher,
         client_loaded_dispatcher, client_spawn_dispatcher, console_print_dispatcher,
@@ -376,26 +389,26 @@
     #[test]
     #[serial]
     fn client_command_dispatcher_when_python_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
         is_initialized_context.expect().returning(|| false);
 
         let result = client_command_dispatcher(123, "asdf");
-        assert_eq!(result, Some("asdf".into()));
+        assert_eq!(result, Some("asdf".to_string()));
     }
 
     #[test]
     #[serial]
     fn client_command_dispatcher_when_dispatcher_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
         is_initialized_context.expect().returning(|| true);
         CLIENT_COMMAND_HANDLER.store(None);
 
         let result = client_command_dispatcher(123, "asdf");
-        assert_eq!(result, Some("asdf".into()));
+        assert_eq!(result, Some("asdf".to_string()));
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn client_command_dispatcher_dispatcher_returns_original_cmd(_pyshinqlx_setup: ()) {
         let is_initialized_context = pyshinqlx_is_initialized_context();
@@ -410,18 +423,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.into_py(py).into()));
+            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.unbind().into()));
 
             let result = client_command_dispatcher(123, "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn client_command_dispatcher_dispatcher_returns_another_cmd(_pyshinqlx_setup: ()) {
@@ -437,18 +450,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.into_py(py).into()));
+            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.unbind().into()));
 
             let result = client_command_dispatcher(123, "asdf");
-            assert_eq!(result, Some("qwertz".into()));
+            assert_eq!(result, Some("qwertz".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn client_command_dispatcher_dispatcher_returns_boolean_true(_pyshinqlx_setup: ()) {
@@ -464,18 +477,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.into_py(py).into()));
+            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.unbind().into()));
 
             let result = client_command_dispatcher(123, "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn client_command_dispatcher_dispatcher_returns_false(_pyshinqlx_setup: ()) {
@@ -491,15 +504,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.into_py(py).into()));
+            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.unbind().into()));
 
             let result = client_command_dispatcher(123, "asdf");
             assert_eq!(result, None);
         });
     }
 
     #[rstest]
@@ -518,18 +531,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.into_py(py).into()));
+            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.unbind().into()));
 
             let result = client_command_dispatcher(123, "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn client_command_dispatcher_dispatcher_returns_not_supported_value(_pyshinqlx_setup: ()) {
@@ -545,40 +558,40 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.into_py(py).into()));
+            CLIENT_COMMAND_HANDLER.store(Some(client_command_handler.unbind().into()));
 
             let result = client_command_dispatcher(123, "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[test]
     #[serial]
     fn server_command_dispatcher_when_python_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
         is_initialized_context.expect().returning(|| false);
 
         let result = server_command_dispatcher(Some(123), "asdf");
-        assert_eq!(result, Some("asdf".into()));
+        assert_eq!(result, Some("asdf".to_string()));
     }
 
     #[test]
     #[serial]
     fn server_command_dispatcher_when_dispatcher_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
         is_initialized_context.expect().returning(|| true);
         SERVER_COMMAND_HANDLER.store(None);
 
         let result = server_command_dispatcher(Some(123), "asdf");
-        assert_eq!(result, Some("asdf".into()));
+        assert_eq!(result, Some("asdf".to_string()));
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn server_command_dispatcher_dispatcher_returns_original_cmd(_pyshinqlx_setup: ()) {
         let is_initialized_context = pyshinqlx_is_initialized_context();
@@ -593,18 +606,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let server_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.into_py(py).into()));
+            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.unbind().into()));
 
             let result = server_command_dispatcher(Some(123), "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn server_command_dispatcher_dispatcher_returns_another_cmd(_pyshinqlx_setup: ()) {
@@ -620,18 +633,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let server_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.into_py(py).into()));
+            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.unbind().into()));
 
             let result = server_command_dispatcher(Some(123), "asdf");
-            assert_eq!(result, Some("qwertz".into()));
+            assert_eq!(result, Some("qwertz".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn server_command_dispatcher_dispatcher_returns_boolean_true(_pyshinqlx_setup: ()) {
@@ -647,18 +660,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let server_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.into_py(py).into()));
+            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.unbind().into()));
 
             let result = server_command_dispatcher(Some(123), "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn server_command_dispatcher_dispatcher_returns_false(_pyshinqlx_setup: ()) {
@@ -674,15 +687,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let server_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.into_py(py).into()));
+            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.unbind().into()));
 
             let result = server_command_dispatcher(Some(123), "asdf");
             assert_eq!(result, None);
         });
     }
 
     #[rstest]
@@ -701,18 +714,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let server_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.into_py(py).into()));
+            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.unbind().into()));
 
             let result = server_command_dispatcher(Some(123), "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn server_command_dispatcher_dispatcher_returns_not_supported_value(_pyshinqlx_setup: ()) {
@@ -728,18 +741,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let server_command_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.into_py(py).into()));
+            SERVER_COMMAND_HANDLER.store(Some(server_command_handler.unbind().into()));
 
             let result = server_command_dispatcher(Some(123), "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[test]
     #[serial]
     fn frame_dispatcher_when_python_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
@@ -773,15 +786,15 @@
     pass
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let frame_handler = pymodule.getattr("handler").expect("this should not happen");
-            FRAME_HANDLER.store(Some(frame_handler.into_py(py).into()));
+            FRAME_HANDLER.store(Some(frame_handler.unbind().into()));
 
             frame_dispatcher();
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -798,15 +811,15 @@
     raise Exception
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let frame_handler = pymodule.getattr("handler").expect("this should not happen");
-            FRAME_HANDLER.store(Some(frame_handler.into_py(py).into()));
+            FRAME_HANDLER.store(Some(frame_handler.unbind().into()));
 
             frame_dispatcher();
         });
     }
 
     #[test]
     #[serial]
@@ -845,18 +858,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_connect_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_CONNECT_HANDLER.store(Some(client_connect_handler.into_py(py).into()));
+            PLAYER_CONNECT_HANDLER.store(Some(client_connect_handler.unbind().into()));
 
             let result = client_connect_dispatcher(42, false);
-            assert_eq!(result, Some("qwertz".into()));
+            assert_eq!(result, Some("qwertz".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn client_connect_dispatcher_dispatcher_returns_boolean_true(_pyshinqlx_setup: ()) {
@@ -872,15 +885,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_connect_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_CONNECT_HANDLER.store(Some(client_connect_handler.into_py(py).into()));
+            PLAYER_CONNECT_HANDLER.store(Some(client_connect_handler.unbind().into()));
 
             let result = client_connect_dispatcher(42, true);
             assert_eq!(result, None);
         });
     }
 
     #[rstest]
@@ -899,18 +912,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_connect_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_CONNECT_HANDLER.store(Some(client_connect_handler.into_py(py).into()));
+            PLAYER_CONNECT_HANDLER.store(Some(client_connect_handler.unbind().into()));
 
             let result = client_connect_dispatcher(42, true);
-            assert_eq!(result, Some("You are banned from this server.".into()));
+            assert_eq!(result, Some("You are banned from this server.".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn client_connect_dispatcher_dispatcher_throws_exception(_pyshinqlx_setup: ()) {
@@ -926,15 +939,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_connect_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_CONNECT_HANDLER.store(Some(client_connect_handler.into_py(py).into()));
+            PLAYER_CONNECT_HANDLER.store(Some(client_connect_handler.unbind().into()));
 
             let result = client_connect_dispatcher(42, false);
             assert_eq!(result, None);
         });
     }
 
     #[rstest]
@@ -953,15 +966,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let player_connect_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_CONNECT_HANDLER.store(Some(player_connect_handler.into_py(py).into()));
+            PLAYER_CONNECT_HANDLER.store(Some(player_connect_handler.unbind().into()));
 
             let result = client_connect_dispatcher(42, false);
             assert_eq!(result, None);
         });
     }
 
     #[test]
@@ -999,15 +1012,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_disconnect_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_DISCONNECT_HANDLER.store(Some(client_disconnect_handler.into_py(py).into()));
+            PLAYER_DISCONNECT_HANDLER.store(Some(client_disconnect_handler.unbind().into()));
 
             client_disconnect_dispatcher(42, "ragequit");
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -1025,15 +1038,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_disconnect_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_DISCONNECT_HANDLER.store(Some(client_disconnect_handler.into_py(py).into()));
+            PLAYER_DISCONNECT_HANDLER.store(Some(client_disconnect_handler.unbind().into()));
 
             client_disconnect_dispatcher(42, "ragequit");
         });
     }
 
     #[test]
     #[serial]
@@ -1070,15 +1083,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_loaded_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_LOADED_HANDLER.store(Some(client_loaded_handler.into_py(py).into()));
+            PLAYER_LOADED_HANDLER.store(Some(client_loaded_handler.unbind().into()));
 
             client_loaded_dispatcher(123);
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -1096,15 +1109,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_loaded_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_LOADED_HANDLER.store(Some(client_loaded_handler.into_py(py).into()));
+            PLAYER_LOADED_HANDLER.store(Some(client_loaded_handler.unbind().into()));
 
             client_loaded_dispatcher(123);
         });
     }
 
     #[test]
     #[serial]
@@ -1140,15 +1153,15 @@
     pass
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let new_game_handler = pymodule.getattr("handler").expect("this should not happen");
-            NEW_GAME_HANDLER.store(Some(new_game_handler.into_py(py).into()));
+            NEW_GAME_HANDLER.store(Some(new_game_handler.unbind().into()));
 
             new_game_dispatcher(false);
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -1165,39 +1178,39 @@
     raise Exception
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let new_game_handler = pymodule.getattr("handler").expect("this should not happen");
-            NEW_GAME_HANDLER.store(Some(new_game_handler.into_py(py).into()));
+            NEW_GAME_HANDLER.store(Some(new_game_handler.unbind().into()));
 
             new_game_dispatcher(true);
         });
     }
 
     #[test]
     #[serial]
     fn set_configstring_dispatcher_when_python_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
         is_initialized_context.expect().returning(|| false);
 
         let result = set_configstring_dispatcher(666u32, "asdf");
-        assert_eq!(result, Some("asdf".into()));
+        assert_eq!(result, Some("asdf".to_string()));
     }
 
     #[test]
     #[serial]
     fn set_configstring_dispatcher_when_dispatcher_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
         is_initialized_context.expect().returning(|| true);
         SET_CONFIGSTRING_HANDLER.store(None);
 
         let result = set_configstring_dispatcher(666u32, "asdf");
-        assert_eq!(result, Some("asdf".into()));
+        assert_eq!(result, Some("asdf".to_string()));
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn set_configstring_dispatcher_dispatcher_returns_original_cmd(_pyshinqlx_setup: ()) {
         let is_initialized_context = pyshinqlx_is_initialized_context();
@@ -1212,18 +1225,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let set_configstring_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.into_py(py).into()));
+            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.unbind().into()));
 
             let result = set_configstring_dispatcher(123u32, "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn set_configstring_dispatcher_dispatcher_returns_another_cmd(_pyshinqlx_setup: ()) {
@@ -1239,18 +1252,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let set_configstring_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.into_py(py).into()));
+            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.unbind().into()));
 
             let result = set_configstring_dispatcher(123u32, "asdf");
-            assert_eq!(result, Some("qwertz".into()));
+            assert_eq!(result, Some("qwertz".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn set_configstring_dispatcher_dispatcher_returns_boolean_true(_pyshinqlx_setup: ()) {
@@ -1266,18 +1279,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let set_configstring_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.into_py(py).into()));
+            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.unbind().into()));
 
             let result = set_configstring_dispatcher(123u32, "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn set_configstring_dispatcher_dispatcher_returns_false(_pyshinqlx_setup: ()) {
@@ -1293,15 +1306,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let set_configstring_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.into_py(py).into()));
+            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.unbind().into()));
 
             let result = set_configstring_dispatcher(123u32, "asdf");
             assert_eq!(result, None);
         })
     }
 
     #[rstest]
@@ -1320,18 +1333,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let set_configstring_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.into_py(py).into()));
+            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.unbind().into()));
 
             let result = set_configstring_dispatcher(123u32, "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn set_configstring_dispatcher_dispatcher_returns_not_supported_value(_pyshinqlx_setup: ()) {
@@ -1347,18 +1360,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let set_configstring_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.into_py(py).into()));
+            SET_CONFIGSTRING_HANDLER.store(Some(set_configstring_handler.unbind().into()));
 
             let result = set_configstring_dispatcher(123u32, "asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[test]
     #[serial]
     fn rcon_dispatcher_when_python_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
@@ -1392,15 +1405,15 @@
     pass
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let rcon_handler = pymodule.getattr("handler").expect("this should not happen");
-            RCON_HANDLER.store(Some(rcon_handler.into_py(py).into()));
+            RCON_HANDLER.store(Some(rcon_handler.unbind().into()));
 
             rcon_dispatcher("asdf");
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -1417,39 +1430,39 @@
     raise Exception
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let rcon_handler = pymodule.getattr("handler").expect("this should not happen");
-            RCON_HANDLER.store(Some(rcon_handler.into_py(py).into()));
+            RCON_HANDLER.store(Some(rcon_handler.unbind().into()));
 
             rcon_dispatcher("asdf");
         });
     }
 
     #[test]
     #[serial]
     fn console_print_dispatcher_when_python_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
         is_initialized_context.expect().returning(|| false);
 
         let result = console_print_dispatcher("asdf");
-        assert_eq!(result, Some("asdf".into()));
+        assert_eq!(result, Some("asdf".to_string()));
     }
 
     #[test]
     #[serial]
     fn console_print_dispatcher_when_dispatcher_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
         is_initialized_context.expect().returning(|| true);
         CONSOLE_PRINT_HANDLER.store(None);
 
         let result = console_print_dispatcher("asdf");
-        assert_eq!(result, Some("asdf".into()));
+        assert_eq!(result, Some("asdf".to_string()));
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn console_print_dispatcher_dispatcher_returns_original_cmd(_pyshinqlx_setup: ()) {
         let is_initialized_context = pyshinqlx_is_initialized_context();
@@ -1464,18 +1477,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let console_print_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.into_py(py).into()));
+            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.unbind().into()));
 
             let result = console_print_dispatcher("asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn console_print_dispatcher_dispatcher_returns_another_cmd(_pyshinqlx_setup: ()) {
@@ -1491,18 +1504,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let console_print_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.into_py(py).into()));
+            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.unbind().into()));
 
             let result = console_print_dispatcher("asdf");
-            assert_eq!(result, Some("qwertz".into()));
+            assert_eq!(result, Some("qwertz".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn console_print_dispatcher_dispatcher_returns_boolean_true(_pyshinqlx_setup: ()) {
@@ -1518,18 +1531,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let console_print_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.into_py(py).into()));
+            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.unbind().into()));
 
             let result = console_print_dispatcher("asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn console_print_dispatcher_dispatcher_returns_false(_pyshinqlx_setup: ()) {
@@ -1545,15 +1558,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let console_print_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.into_py(py).into()));
+            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.unbind().into()));
 
             let result = console_print_dispatcher("asdf");
             assert_eq!(result, None);
         });
     }
 
     #[rstest]
@@ -1572,18 +1585,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let console_print_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.into_py(py).into()));
+            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.unbind().into()));
 
             let result = console_print_dispatcher("asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn console_print_dispatcher_dispatcher_returns_not_supported_value(_pyshinqlx_setup: ()) {
@@ -1599,18 +1612,18 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let console_print_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.into_py(py).into()));
+            CONSOLE_PRINT_HANDLER.store(Some(console_print_handler.unbind().into()));
 
             let result = console_print_dispatcher("asdf");
-            assert_eq!(result, Some("asdf".into()));
+            assert_eq!(result, Some("asdf".to_string()));
         });
     }
 
     #[test]
     #[serial]
     fn client_spawn_dispatcher_when_python_not_initiailized() {
         let is_initialized_context = pyshinqlx_is_initialized_context();
@@ -1644,15 +1657,15 @@
     pass
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_spawn_handler = pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_SPAWN_HANDLER.store(Some(client_spawn_handler.into_py(py).into()));
+            PLAYER_SPAWN_HANDLER.store(Some(client_spawn_handler.unbind().into()));
 
             client_spawn_dispatcher(123);
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -1669,15 +1682,15 @@
     raise Exception
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let client_spawn_handler = pymodule.getattr("handler").expect("this should not happen");
-            PLAYER_SPAWN_HANDLER.store(Some(client_spawn_handler.into_py(py).into()));
+            PLAYER_SPAWN_HANDLER.store(Some(client_spawn_handler.unbind().into()));
 
             client_spawn_dispatcher(123);
         });
     }
 
     #[test]
     #[serial]
@@ -1713,15 +1726,15 @@
     pass
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let kamikaze_use_handler = pymodule.getattr("handler").expect("this should not happen");
-            KAMIKAZE_USE_HANDLER.store(Some(kamikaze_use_handler.into_py(py).into()));
+            KAMIKAZE_USE_HANDLER.store(Some(kamikaze_use_handler.unbind().into()));
 
             kamikaze_use_dispatcher(123);
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -1738,15 +1751,15 @@
     raise Exception
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let kamikaze_use_handler = pymodule.getattr("handler").expect("this should not happen");
-            KAMIKAZE_USE_HANDLER.store(Some(kamikaze_use_handler.into_py(py).into()));
+            KAMIKAZE_USE_HANDLER.store(Some(kamikaze_use_handler.unbind().into()));
 
             kamikaze_use_dispatcher(123);
         });
     }
 
     #[test]
     #[serial]
@@ -1783,15 +1796,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let kamikaze_explode_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            KAMIKAZE_EXPLODE_HANDLER.store(Some(kamikaze_explode_handler.into_py(py).into()));
+            KAMIKAZE_EXPLODE_HANDLER.store(Some(kamikaze_explode_handler.unbind().into()));
 
             kamikaze_explode_dispatcher(123, false);
         });
     }
 
     #[rstest]
     #[cfg_attr(miri, ignore)]
@@ -1809,15 +1822,15 @@
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let kamikaze_explode_handler =
                 pymodule.getattr("handler").expect("this should not happen");
-            KAMIKAZE_EXPLODE_HANDLER.store(Some(kamikaze_explode_handler.into_py(py).into()));
+            KAMIKAZE_EXPLODE_HANDLER.store(Some(kamikaze_explode_handler.unbind().into()));
 
             kamikaze_explode_dispatcher(123, true);
         });
     }
 
     #[test]
     #[serial]
@@ -1865,15 +1878,15 @@
     pass
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let damage_handler = pymodule.getattr("handler").expect("this should not happen");
-            DAMAGE_HANDLER.store(Some(damage_handler.into_py(py).into()));
+            DAMAGE_HANDLER.store(Some(damage_handler.unbind().into()));
 
             damage_dispatcher(
                 123,
                 Some(456),
                 100,
                 DAMAGE_NO_TEAM_PROTECTION as i32,
                 meansOfDeath_t::MOD_ROCKET as i32,
@@ -1896,15 +1909,15 @@
     raise Exception
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let damage_handler = pymodule.getattr("handler").expect("this should not happen");
-            DAMAGE_HANDLER.store(Some(damage_handler.into_py(py).into()));
+            DAMAGE_HANDLER.store(Some(damage_handler.unbind().into()));
 
             damage_dispatcher(
                 123,
                 None,
                 666,
                 DAMAGE_NO_PROTECTION as i32,
                 meansOfDeath_t::MOD_TRIGGER_HURT as i32,
```

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/add_console_command.rs` & `shinqlx-0.5.7/src/ffi/python/embed/add_console_command.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/allow_single_player.rs` & `shinqlx-0.5.7/src/ffi/python/embed/allow_single_player.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/callvote.rs` & `shinqlx-0.5.7/src/ffi/python/embed/callvote.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/client_command.rs` & `shinqlx-0.5.7/src/ffi/python/embed/client_command.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/console_command.rs` & `shinqlx-0.5.7/src/ffi/python/embed/console_command.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/console_print.rs` & `shinqlx-0.5.7/src/ffi/python/embed/console_print.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/destroy_kamikaze_timers.rs` & `shinqlx-0.5.7/src/ffi/python/embed/destroy_kamikaze_timers.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/dev_print_items.rs` & `shinqlx-0.5.7/src/ffi/python/embed/dev_print_items.rs`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         let mut str_length = 0;
         let printed_items: Vec<String> = formatted_items
             .iter()
             .take_while(|&item| {
                 str_length += item.len();
                 str_length < 1024
             })
-            .map(|item| item.into())
+            .map(|item| item.to_string())
             .collect();
 
         let Some(ref main_engine) = *MAIN_ENGINE.load() else {
             return Err(PyEnvironmentError::new_err(
                 "main quake live engine not set",
             ));
         };
@@ -49,15 +49,15 @@
             None::<Client>,
             &format!("print \"{}\n\"", printed_items.join("\n")),
         );
 
         let remaining_items: Vec<String> = formatted_items
             .iter()
             .skip(printed_items.len())
-            .map(|item| item.into())
+            .map(|item| item.to_string())
             .collect();
 
         if !remaining_items.is_empty() {
             main_engine.send_server_command(
                 None::<Client>,
                 "print \"Check server console for other items\n\"\n",
             );
@@ -273,15 +273,15 @@
                 .with(predicate::eq(entityType_t::ET_ITEM))
                 .returning(|_| true);
             mock_game_entity
                 .expect_get_entity_id()
                 .returning(move || entity_id);
             mock_game_entity
                 .expect_get_classname()
-                .returning(move || format!("super important entity {}", entity_id));
+                .returning(move || format!("super important entity {}", entity_id).into());
             mock_game_entity
         });
 
         let result = Python::with_gil(pyshinqlx_dev_print_items);
         assert!(result.is_ok());
     }
 }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/drop_holdable.rs` & `shinqlx-0.5.7/src/ffi/python/embed/drop_holdable.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/force_vote.rs` & `shinqlx-0.5.7/src/ffi/python/embed/force_vote.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/force_weapon_respawn_time.rs` & `shinqlx-0.5.7/src/ffi/python/embed/force_weapon_respawn_time.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/get_configstring.rs` & `shinqlx-0.5.7/src/ffi/python/embed/get_configstring.rs`

 * *Files 12% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn get_configstring_forwards_call_to_engine() {
         let mut mock_engine = MockQuakeEngine::new();
         mock_engine
             .expect_get_configstring()
             .with(predicate::eq(666))
-            .returning(|_| "asdf".into())
+            .returning(|_| "asdf".to_string())
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
         let result = Python::with_gil(|py| pyshinqlx_get_configstring(py, 666));
         assert_eq!(result.expect("result was not OK"), "asdf");
     }
 }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/get_cvar.rs` & `shinqlx-0.5.7/src/ffi/python/embed/get_cvar.rs`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,17 @@
     py.allow_threads(|| {
         let Some(ref main_engine) = *MAIN_ENGINE.load() else {
             return Err(PyEnvironmentError::new_err(
                 "main quake live engine not set",
             ));
         };
 
-        match main_engine.find_cvar(cvar) {
-            None => Ok(None),
-            Some(cvar_result) => Ok(Some(cvar_result.get_string())),
-        }
+        Ok(main_engine
+            .find_cvar(cvar)
+            .map(|cvar_result| cvar_result.get_string().into()))
     })
 }
 
 #[cfg(test)]
 mod get_cvar_tests {
     use super::MAIN_ENGINE;
     use crate::ffi::c::prelude::*;
@@ -78,10 +77,10 @@
                     .expect("this should not happen");
                 CVar::try_from(&mut raw_cvar as *mut cvar_t).ok()
             })
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
         let result = Python::with_gil(|py| pyshinqlx_get_cvar(py, "sv_maxclients"));
-        assert_eq!(result.expect("result was not OK"), Some("16".into()));
+        assert_eq!(result.expect("result was not OK"), Some("16".to_string()));
     }
 }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/get_targetting_entities.rs` & `shinqlx-0.5.7/src/ffi/python/embed/get_targetting_entities.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/get_userinfo.rs` & `shinqlx-0.5.7/src/ffi/python/embed/get_userinfo.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     py.allow_threads(|| {
         #[cfg_attr(test, allow(clippy::unnecessary_fallible_conversions))]
         let opt_client = Client::try_from(client_id).ok().filter(|client| {
             let allowed_free_clients = ALLOW_FREE_CLIENT.load(Ordering::SeqCst);
             client.get_state() != clientState_t::CS_FREE
                 || allowed_free_clients & (1 << client_id as u64) != 0
         });
-        Ok(opt_client.map(|client| client.get_user_info()))
+        Ok(opt_client.map(|client| client.get_user_info().into()))
     })
 }
 
 #[cfg(test)]
 mod get_userinfo_tests {
     use crate::ffi::c::prelude::*;
     use crate::ffi::python::prelude::*;
@@ -85,15 +85,18 @@
             mock_client
                 .expect_get_user_info()
                 .returning(|| "asdf".into());
             mock_client
         });
 
         let userinfo = Python::with_gil(|py| pyshinqlx_get_userinfo(py, 2));
-        assert_eq!(userinfo.expect("result was not OK"), Some("asdf".into()));
+        assert_eq!(
+            userinfo.expect("result was not OK"),
+            Some("asdf".to_string())
+        );
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn get_userinfo_for_non_allowed_free_client() {
         let mut mock_engine = MockQuakeEngine::new();
@@ -135,10 +138,13 @@
             mock_client
                 .expect_get_user_info()
                 .returning(|| "asdf".into());
             mock_client
         });
 
         let userinfo = Python::with_gil(|py| pyshinqlx_get_userinfo(py, 2));
-        assert_eq!(userinfo.expect("result was not OK"), Some("asdf".into()));
+        assert_eq!(
+            userinfo.expect("result was not OK"),
+            Some("asdf".to_string())
+        );
     }
 }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/kick.rs` & `shinqlx-0.5.7/src/ffi/python/embed/kick.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/mod.rs` & `shinqlx-0.5.7/src/ffi/python/embed/mod.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/noclip.rs` & `shinqlx-0.5.7/src/ffi/python/embed/noclip.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/player_info.rs` & `shinqlx-0.5.7/src/ffi/python/embed/player_info.rs`

 * *Files 2% similar despite different names*

```diff
@@ -106,32 +106,32 @@
         });
 
         let game_entity_try_from_ctx = MockGameEntity::from_context();
         game_entity_try_from_ctx.expect().returning(|_client_id| {
             let mut mock_game_entity = MockGameEntity::new();
             mock_game_entity
                 .expect_get_player_name()
-                .returning(|| "Mocked Player".into());
+                .returning(|| "Mocked Player".to_string());
             mock_game_entity
                 .expect_get_team()
                 .returning(|| team_t::TEAM_RED);
             mock_game_entity
                 .expect_get_privileges()
                 .returning(|| privileges_t::PRIV_NONE);
             mock_game_entity
         });
 
         let player_info = Python::with_gil(|py| pyshinqlx_player_info(py, 2));
         assert_eq!(
             player_info.expect("result was not OK"),
             Some(PlayerInfo {
                 client_id: 2,
-                name: "Mocked Player".into(),
+                name: "Mocked Player".to_string(),
                 connection_state: clientState_t::CS_ACTIVE as i32,
-                userinfo: "asdf".into(),
+                userinfo: "asdf".to_string(),
                 steam_id: 1234,
                 team: team_t::TEAM_RED as i32,
                 privileges: privileges_t::PRIV_NONE as i32
             })
         );
     }
 
@@ -184,32 +184,32 @@
         });
 
         let game_entity_try_from_ctx = MockGameEntity::from_context();
         game_entity_try_from_ctx.expect().returning(|_client_id| {
             let mut mock_game_entity = MockGameEntity::new();
             mock_game_entity
                 .expect_get_player_name()
-                .returning(|| "Mocked Player".into());
+                .returning(|| "Mocked Player".to_string());
             mock_game_entity
                 .expect_get_team()
                 .returning(|| team_t::TEAM_RED);
             mock_game_entity
                 .expect_get_privileges()
                 .returning(|| privileges_t::PRIV_NONE);
             mock_game_entity
         });
 
         let player_info = Python::with_gil(|py| pyshinqlx_player_info(py, 2));
         assert_eq!(
             player_info.expect("result was not OK"),
             Some(PlayerInfo {
                 client_id: 2,
-                name: "Mocked Player".into(),
+                name: "Mocked Player".to_string(),
                 connection_state: clientState_t::CS_FREE as i32,
-                userinfo: "asdf".into(),
+                userinfo: "asdf".to_string(),
                 steam_id: 1234,
                 team: team_t::TEAM_RED as i32,
                 privileges: privileges_t::PRIV_NONE as i32
             })
         );
     }
 }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/player_spawn.rs` & `shinqlx-0.5.7/src/ffi/python/embed/player_spawn.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/player_state.rs` & `shinqlx-0.5.7/src/ffi/python/embed/player_state.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/player_stats.rs` & `shinqlx-0.5.7/src/ffi/python/embed/player_stats.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/players_info.rs` & `shinqlx-0.5.7/src/ffi/python/embed/players_info.rs`

 * *Files 8% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             });
 
         let game_entity_try_from_ctx = MockGameEntity::from_context();
         game_entity_try_from_ctx.expect().returning(|_client_id| {
             let mut mock_game_entity = MockGameEntity::new();
             mock_game_entity
                 .expect_get_player_name()
-                .returning(|| "Mocked Player".into());
+                .returning(|| "Mocked Player".to_string());
             mock_game_entity
                 .expect_get_team()
                 .returning(|| team_t::TEAM_RED);
             mock_game_entity
                 .expect_get_privileges()
                 .returning(|| privileges_t::PRIV_NONE);
             mock_game_entity
@@ -126,26 +126,26 @@
 
         let players_info = Python::with_gil(pyshinqlx_players_info);
         assert_eq!(
             players_info.expect("result was not OK"),
             vec![
                 Some(PlayerInfo {
                     client_id: 0,
-                    name: "Mocked Player".into(),
+                    name: "Mocked Player".to_string(),
                     connection_state: clientState_t::CS_ACTIVE as i32,
-                    userinfo: "asdf".into(),
+                    userinfo: "asdf".to_string(),
                     steam_id: 1234,
                     team: team_t::TEAM_RED as i32,
                     privileges: privileges_t::PRIV_NONE as i32
                 }),
                 Some(PlayerInfo {
                     client_id: 2,
-                    name: "Mocked Player".into(),
+                    name: "Mocked Player".to_string(),
                     connection_state: clientState_t::CS_ACTIVE as i32,
-                    userinfo: "asdf".into(),
+                    userinfo: "asdf".to_string(),
                     steam_id: 1234,
                     team: team_t::TEAM_RED as i32,
                     privileges: privileges_t::PRIV_NONE as i32
                 })
             ]
         );
     }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/register_handler.rs` & `shinqlx-0.5.7/src/ffi/python/embed/register_handler.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 use crate::ffi::python::prelude::*;
 
 use pyo3::exceptions::{PyTypeError, PyValueError};
 
-use alloc::sync::Arc;
-
 /// Register an event handler. Can be called more than once per event, but only the last one will work.
 #[pyfunction]
 #[pyo3(name = "register_handler")]
 #[pyo3(signature = (event, handler=None))]
 pub(crate) fn pyshinqlx_register_handler(
-    py: Python<'_>,
+    _py: Python<'_>,
     event: &str,
     handler: Option<Bound<'_, PyAny>>,
 ) -> PyResult<()> {
     if handler
         .as_ref()
         .is_some_and(|handler_function| !handler_function.is_callable())
     {
@@ -35,15 +33,15 @@
         "player_spawn" => &PLAYER_SPAWN_HANDLER,
         "kamikaze_use" => &KAMIKAZE_USE_HANDLER,
         "kamikaze_explode" => &KAMIKAZE_EXPLODE_HANDLER,
         "damage" => &DAMAGE_HANDLER,
         _ => return Err(PyValueError::new_err("Unsupported event.")),
     };
 
-    handler_lock.store(handler.map(|handler_func| Arc::new(handler_func.into_py(py))));
+    handler_lock.store(handler.map(|handler_func| handler_func.unbind().into()));
     Ok(())
 }
 
 #[cfg(test)]
 mod register_handler_tests {
     use crate::ffi::python::prelude::*;
     use crate::prelude::*;
@@ -83,15 +81,15 @@
     pass
 "#,
                 "",
                 "",
             )
             .expect("this should not happen");
             let py_handler = pymodule.getattr("handler").expect("this should not happen");
-            handler.store(Some(py_handler.into_py(py).into()));
+            handler.store(Some(py_handler.unbind().into()));
 
             let result = pyshinqlx_register_handler(py, event, None);
             assert!(result.is_ok());
 
             let stored_handler = handler.load();
             assert!(stored_handler.is_none());
         });
```

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/remove_dropped_items.rs` & `shinqlx-0.5.7/src/ffi/python/embed/remove_dropped_items.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/replace_items.rs` & `shinqlx-0.5.7/src/ffi/python/embed/replace_items.rs`

 * *Files 10% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 
 /// Replaces target entity's item with specified one.
 #[pyfunction]
 #[pyo3(name = "replace_items")]
 #[pyo3(signature = (item1, item2))]
 pub(crate) fn pyshinqlx_replace_items(
     py: Python<'_>,
-    item1: Py<PyAny>,
-    item2: Py<PyAny>,
+    item1: &Bound<'_, PyAny>,
+    item2: &Bound<'_, PyAny>,
 ) -> PyResult<bool> {
-    let item2_id = determine_item_id(item2.bind(py))?;
+    let item2_id = determine_item_id(item2)?;
     // Note: if item_id == 0 and item_classname == NULL, then item will be removed
 
-    if let Ok(item1_id) = item1.extract::<i32>(py) {
+    if let Ok(item1_id) = item1.extract::<i32>() {
         // replacing item by entity_id
 
         // entity_id checking
         if !(0..GameItem::get_num_items()).contains(&item1_id) {
             return Err(PyValueError::new_err(format!(
                 "item1 needs to be between 0 and {}.",
                 GameItem::get_num_items() - 1
@@ -73,15 +73,15 @@
                 .iter_mut()
                 .for_each(|game_entity| game_entity.replace_item(item2_id));
 
             Ok(true)
         });
     }
 
-    if let Ok(item1_classname) = item1.extract::<String>(py) {
+    if let Ok(item1_classname) = item1.extract::<String>() {
         return py.allow_threads(|| {
             #[cfg_attr(test, allow(clippy::unnecessary_fallible_conversions))]
             let mut matching_item1_entities: Vec<GameEntity> = (0..MAX_GENTITIES)
                 .filter_map(|i| GameEntity::try_from(i as i32).ok())
                 .filter(|game_entity| {
                     game_entity.in_use()
                         && game_entity.is_game_item(entityType_t::ET_ITEM)
@@ -107,97 +107,108 @@
     use crate::ffi::c::prelude::*;
     use crate::ffi::python::prelude::*;
     use crate::prelude::*;
 
     use mockall::predicate;
     use pretty_assertions::assert_eq;
     use pyo3::exceptions::PyValueError;
+    use pyo3::types::{PyString, PyTuple};
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn replace_items_for_too_small_item1_id() {
         let get_num_items_ctx = MockGameItem::get_num_items_context();
         get_num_items_ctx.expect().returning(|| 42);
 
         Python::with_gil(|py| {
             let result = pyshinqlx_replace_items(
                 py,
-                <i32 as IntoPy<Py<PyAny>>>::into_py(-1, py),
-                1.into_py(py),
+                (-1i32).into_py(py).bind(py),
+                1i32.into_py(py).bind(py),
             );
             assert!(result.is_err_and(|err| err.is_instance_of::<PyValueError>(py)));
         });
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn replace_items_for_too_large_item1_id() {
         let get_num_items_ctx = MockGameItem::get_num_items_context();
         get_num_items_ctx.expect().returning(|| 42);
 
         Python::with_gil(|py| {
-            let result = pyshinqlx_replace_items(py, 43.into_py(py), 1.into_py(py));
+            let result =
+                pyshinqlx_replace_items(py, 43i32.into_py(py).bind(py), 1i32.into_py(py).bind(py));
             assert!(result.is_err_and(|err| err.is_instance_of::<PyValueError>(py)));
         });
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn replace_items_for_too_small_item2_id() {
         let get_num_items_ctx = MockGameItem::get_num_items_context();
         get_num_items_ctx.expect().returning(|| 42);
 
         Python::with_gil(|py| {
             let result = pyshinqlx_replace_items(
                 py,
-                1.into_py(py),
-                <i32 as IntoPy<Py<PyAny>>>::into_py(-1, py),
+                1i32.into_py(py).bind(py),
+                (-1i32).into_py(py).bind(py),
             );
             assert!(result.is_err_and(|err| err.is_instance_of::<PyValueError>(py)));
         });
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn replace_items_for_too_large_item2_id() {
         let get_num_items_ctx = MockGameItem::get_num_items_context();
         get_num_items_ctx.expect().returning(|| 42);
 
         Python::with_gil(|py| {
-            let result = pyshinqlx_replace_items(py, 1.into_py(py), 43.into_py(py));
+            let result =
+                pyshinqlx_replace_items(py, 1i32.into_py(py).bind(py), 43i32.into_py(py).bind(py));
             assert!(result.is_err_and(|err| err.is_instance_of::<PyValueError>(py)));
         });
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn replace_items_for_item1_not_integer_nor_string() {
         let get_num_items_ctx = MockGameItem::get_num_items_context();
         get_num_items_ctx.expect().returning(|| 42);
 
         Python::with_gil(|py| {
-            let result = pyshinqlx_replace_items(py, (1, 2).into_py(py), 1.into_py(py));
+            let result = pyshinqlx_replace_items(
+                py,
+                PyTuple::new_bound(py, [1i32, 2i32]).as_ref(),
+                1i32.into_py(py).bind(py),
+            );
             assert!(result.is_err_and(|err| err.is_instance_of::<PyValueError>(py)));
         });
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn replace_items_for_item2_not_integer_nor_string() {
         let get_num_items_ctx = MockGameItem::get_num_items_context();
         get_num_items_ctx.expect().returning(|| 42);
 
         Python::with_gil(|py| {
-            let result = pyshinqlx_replace_items(py, 1.into_py(py), (1, 2).into_py(py));
+            let result = pyshinqlx_replace_items(
+                py,
+                1i32.into_py(py).bind(py),
+                PyTuple::new_bound(py, [1i32, 2i32]).as_ref(),
+            );
             assert!(result.is_err_and(|err| err.is_instance_of::<PyValueError>(py)));
         });
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
@@ -216,15 +227,19 @@
             mock_game_entity
                 .expect_get_classname()
                 .returning(|| "available_classname".into());
             mock_game_entity
         });
 
         let result = Python::with_gil(|py| {
-            pyshinqlx_replace_items(py, "not existing classname".into_py(py), 1.into_py(py))
+            pyshinqlx_replace_items(
+                py,
+                PyString::new_bound(py, "not existing classname").as_ref(),
+                1i32.into_py(py).bind(py),
+            )
         });
         assert_eq!(result.expect("result was not OK"), false);
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
@@ -238,16 +253,19 @@
             mock_game_item
                 .expect_get_classname()
                 .returning(|| "available_classname".into());
             mock_game_item
         });
 
         Python::with_gil(|py| {
-            let result =
-                pyshinqlx_replace_items(py, 1.into_py(py), "not existing classname".into_py(py));
+            let result = pyshinqlx_replace_items(
+                py,
+                1i32.into_py(py).bind(py),
+                PyString::new_bound(py, "not existing classname").as_ref(),
+            );
             assert!(result.is_err_and(|err| err.is_instance_of::<PyValueError>(py)));
         });
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
@@ -262,15 +280,16 @@
             .returning(|_| {
                 let mut mock_game_entity = MockGameEntity::new();
                 mock_game_entity.expect_in_use().returning(|| false);
                 mock_game_entity
             });
 
         Python::with_gil(|py| {
-            let result = pyshinqlx_replace_items(py, 1.into_py(py), 2.into_py(py));
+            let result =
+                pyshinqlx_replace_items(py, 1i32.into_py(py).bind(py), 2i32.into_py(py).bind(py));
             assert!(result.is_err_and(|err| err.is_instance_of::<PyValueError>(py)));
         });
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
@@ -289,15 +308,16 @@
                     .expect_is_game_item()
                     .with(predicate::eq(entityType_t::ET_ITEM))
                     .returning(|_| false);
                 mock_game_entity
             });
 
         Python::with_gil(|py| {
-            let result = pyshinqlx_replace_items(py, 1.into_py(py), 2.into_py(py));
+            let result =
+                pyshinqlx_replace_items(py, 1i32.into_py(py).bind(py), 2i32.into_py(py).bind(py));
             assert!(result.is_err_and(|err| err.is_instance_of::<PyValueError>(py)));
         });
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
@@ -319,16 +339,17 @@
                 mock_game_entity
                     .expect_replace_item()
                     .with(predicate::eq(2))
                     .times(1);
                 mock_game_entity
             });
 
-        let result =
-            Python::with_gil(|py| pyshinqlx_replace_items(py, 1.into_py(py), 2.into_py(py)));
+        let result = Python::with_gil(|py| {
+            pyshinqlx_replace_items(py, 1i32.into_py(py).bind(py), 2i32.into_py(py).bind(py))
+        });
         assert_eq!(result.expect("result was not OK"), true);
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
     fn replace_items_replaces_item1_id_by_item2_clssname() {
@@ -369,15 +390,19 @@
                     .expect_replace_item()
                     .with(predicate::eq(2))
                     .times(1);
                 mock_game_entity
             });
 
         let result = Python::with_gil(|py| {
-            pyshinqlx_replace_items(py, 1.into_py(py), "weapon_bfg".into_py(py))
+            pyshinqlx_replace_items(
+                py,
+                1i32.into_py(py).bind(py),
+                PyString::new_bound(py, "weapon_bfg").as_ref(),
+            )
         });
         assert_eq!(result.expect("result was not OK"), true);
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
@@ -483,15 +508,19 @@
                 .expect_get_classname()
                 .returning(|| "other_classname".into());
             mock_game_entity.expect_replace_item().times(0);
             mock_game_entity
         });
 
         let result = Python::with_gil(|py| {
-            pyshinqlx_replace_items(py, "weapon_railgun".into_py(py), "weapon_bfg".into_py(py))
+            pyshinqlx_replace_items(
+                py,
+                PyString::new_bound(py, "weapon_railgun").as_ref(),
+                PyString::new_bound(py, "weapon_bfg").as_ref(),
+            )
         });
         assert_eq!(result.expect("result was not OK"), true);
     }
 
     #[test]
     #[cfg_attr(miri, ignore)]
     #[serial]
@@ -568,12 +597,16 @@
                 .expect_get_classname()
                 .returning(|| "other_classname".into());
             mock_game_entity.expect_replace_item().times(0);
             mock_game_entity
         });
 
         let result = Python::with_gil(|py| {
-            pyshinqlx_replace_items(py, "weapon_railgun".into_py(py), "weapon_bfg".into_py(py))
+            pyshinqlx_replace_items(
+                py,
+                PyString::new_bound(py, "weapon_railgun").as_ref(),
+                PyString::new_bound(py, "weapon_bfg").as_ref(),
+            )
         });
         assert_eq!(result.expect("result was not OK"), true);
     }
 }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/send_server_command.rs` & `shinqlx-0.5.7/src/ffi/python/embed/send_server_command.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_ammo.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_ammo.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_armor.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_armor.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_configstring.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_configstring.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_cvar.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_cvar.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_cvar_limit.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_cvar_limit.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_flight.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_flight.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_health.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_health.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_holdable.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_holdable.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_invulnerability.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_invulnerability.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_position.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_position.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_powerups.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_powerups.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_privileges.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_privileges.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_score.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_score.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_velocity.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_velocity.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_weapon.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_weapon.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/set_weapons.rs` & `shinqlx-0.5.7/src/ffi/python/embed/set_weapons.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/slay_with_mod.rs` & `shinqlx-0.5.7/src/ffi/python/embed/slay_with_mod.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/embed/spawn_item.rs` & `shinqlx-0.5.7/src/ffi/python/embed/spawn_item.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/flight.rs` & `shinqlx-0.5.7/src/ffi/python/flight.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use super::prelude::*;
 
+use alloc::borrow::Cow;
 use pyo3::{basic::CompareOp, exceptions::PyValueError, types::PyTuple};
 
 /// A struct sequence containing parameters for the flight holdable item.
-#[pyclass(frozen)]
-#[pyo3(module = "shinqlx", name = "Flight", get_all)]
+#[pyclass(module = "_shinqlx", name = "Flight", frozen, get_all, sequence)]
 #[derive(PartialEq, Eq, Debug, Clone, Copy)]
 pub(crate) struct Flight(
     #[pyo3(name = "fuel")] pub(crate) i32,
     #[pyo3(name = "max_fuel")] pub(crate) i32,
     #[pyo3(name = "thrust")] pub(crate) i32,
     #[pyo3(name = "refuel")] pub(crate) i32,
 );
@@ -18,15 +18,15 @@
         [flight.0, flight.1, flight.2, flight.3]
     }
 }
 
 #[pymethods]
 impl Flight {
     #[new]
-    fn py_new(values: &PyTuple) -> PyResult<Self> {
+    fn py_new(values: &Bound<'_, PyTuple>) -> PyResult<Self> {
         if values.len() < 4 {
             return Err(PyValueError::new_err(
                 "tuple did not provide values for all 4 flight parameters",
             ));
         }
 
         if values.len() > 4 {
@@ -56,26 +56,28 @@
         match op {
             CompareOp::Eq => (self == other).into_py(py),
             CompareOp::Ne => (self != other).into_py(py),
             _ => py.NotImplemented(),
         }
     }
 
-    pub(crate) fn __str__(&self) -> String {
+    pub(crate) fn __str__(&self) -> Cow<str> {
         format!(
             "Flight(fuel={}, max_fuel={}, thrust={}, refuel={})",
             self.0, self.1, self.2, self.3
         )
+        .into()
     }
 
-    fn __repr__(&self) -> String {
+    fn __repr__(&self) -> Cow<str> {
         format!(
             "Flight(fuel={}, max_fuel={}, thrust={}, refuel={})",
             self.0, self.1, self.2, self.3
         )
+        .into()
     }
 }
 
 #[cfg(test)]
 mod flight_tests {
     use crate::ffi::python::prelude::*;
 
@@ -204,16 +206,48 @@
         let flight = Flight(1, 2, 3, 4);
         assert_eq!(
             flight.__str__(),
             "Flight(fuel=1, max_fuel=2, thrust=3, refuel=4)"
         );
     }
 
+    #[rstest]
+    #[cfg_attr(miri, ignore)]
+    fn flight_to_str_in_python(_pyshinqlx_setup: ()) {
+        Python::with_gil(|py| {
+            let result = py.run_bound(
+                r#"
+import _shinqlx
+assert(str(_shinqlx.Flight((1, 2, 3, 4))) == "Flight(fuel=1, max_fuel=2, thrust=3, refuel=4)")
+            "#,
+                None,
+                None,
+            );
+            assert!(result.is_ok());
+        });
+    }
+
     #[test]
     fn flight_repr() {
         let flight = Flight(1, 2, 3, 4);
         assert_eq!(
             flight.__repr__(),
             "Flight(fuel=1, max_fuel=2, thrust=3, refuel=4)"
         );
     }
+
+    #[rstest]
+    #[cfg_attr(miri, ignore)]
+    fn flight_repr_in_python(_pyshinqlx_setup: ()) {
+        Python::with_gil(|py| {
+            let result = py.run_bound(
+                r#"
+import _shinqlx
+assert(repr(_shinqlx.Flight((1, 2, 3, 4))) == "Flight(fuel=1, max_fuel=2, thrust=3, refuel=4)")
+            "#,
+                None,
+                None,
+            );
+            assert!(result.is_ok());
+        });
+    }
 }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/holdable.rs` & `shinqlx-0.5.7/src/ffi/python/holdable.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use super::prelude::*;
 
-#[pyclass(frozen)]
-#[pyo3(module = "shinqlx", name = "Holdable")]
+use alloc::borrow::Cow;
+
+#[pyclass(module = "_shinqlx", name = "Holdable", frozen)]
 #[derive(PartialEq, Debug, Clone, Copy)]
 pub(crate) enum Holdable {
     None = 0,
     Teleporter = 27,
     MedKit = 28,
     Kamikaze = 37,
     Portal = 38,
@@ -40,15 +41,15 @@
             Holdable::Portal => 38,
             Holdable::Invulnerability => 39,
             Holdable::Unknown => 0,
         }
     }
 }
 
-impl From<Holdable> for Option<String> {
+impl From<Holdable> for Option<Cow<'static, str>> {
     fn from(holdable: Holdable) -> Self {
         match holdable {
             Holdable::None => None,
             Holdable::Teleporter => Some("teleporter".into()),
             Holdable::MedKit => Some("medkit".into()),
             Holdable::Kamikaze => Some("kamikaze".into()),
             Holdable::Portal => Some("portal".into()),
@@ -59,14 +60,16 @@
     }
 }
 
 #[cfg(test)]
 mod holdable_tests {
     use super::Holdable;
 
+    use alloc::borrow::Cow;
+
     use pretty_assertions::assert_eq;
     use rstest::rstest;
 
     #[rstest]
     #[case(0, Holdable::None)]
     #[case(27, Holdable::Teleporter)]
     #[case(28, Holdable::MedKit)]
@@ -99,12 +102,12 @@
     #[case(Holdable::Flight, Some("flight".into()))]
     #[case(Holdable::Kamikaze, Some("kamikaze".into()))]
     #[case(Holdable::Portal, Some("portal".into()))]
     #[case(Holdable::Invulnerability, Some("invulnerability".into()))]
     #[case(Holdable::Unknown, Some("unknown".into()))]
     fn opt_string_from_holdable(
         #[case] holdable: Holdable,
-        #[case] expected_result: Option<String>,
+        #[case] expected_result: Option<Cow<'static, str>>,
     ) {
-        assert_eq!(Option::<String>::from(holdable), expected_result);
+        assert_eq!(Option::<Cow<'static, str>>::from(holdable), expected_result);
     }
 }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/mod.rs` & `shinqlx-0.5.7/src/ffi/python/mod.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/ffi/python/player_info.rs` & `shinqlx-0.5.7/src/ffi/python/player_info.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use super::prelude::*;
 use crate::ffi::c::prelude::*;
 
+use alloc::borrow::Cow;
+
 /// Information about a player, such as Steam ID, name, client ID, and whatnot.
-#[pyclass(frozen)]
-#[pyo3(module = "shinqlx", name = "PlayerInfo", get_all)]
+#[pyclass(module = "_shinqlx", name = "PlayerInfo", frozen, get_all, sequence)]
 #[derive(Debug, PartialEq)]
 #[allow(unused)]
 pub(crate) struct PlayerInfo {
     /// The player's client ID.
     pub(crate) client_id: i32,
     /// The player's name.
     pub(crate) name: String,
@@ -34,34 +35,34 @@
             userinfo: tuple.3,
             steam_id: tuple.4,
             team: tuple.5,
             privileges: tuple.6,
         }
     }
 
-    fn __str__(&self) -> String {
+    fn __str__(&self) -> Cow<str> {
         format!("PlayerInfo(client_id={}, name={}, connection_state={}, userinfo={}, steam_id={}, team={}, privileges={})",
                 self.client_id,
                 self.name,
                 self.connection_state,
                 self.userinfo,
                 self.steam_id,
                 self.team,
-                self.privileges)
+                self.privileges).into()
     }
 
-    fn __repr__(&self) -> String {
+    fn __repr__(&self) -> Cow<str> {
         format!("PlayerInfo(client_id={}, name={}, connection_state={}, userinfo={}, steam_id={}, team={}, privileges={})",
                 self.client_id,
                 self.name,
                 self.connection_state,
                 self.userinfo,
                 self.steam_id,
                 self.team,
-                self.privileges)
+                self.privileges).into()
     }
 }
 
 impl From<i32> for PlayerInfo {
     fn from(client_id: i32) -> Self {
         let mut returned = PlayerInfo {
             client_id,
@@ -82,15 +83,15 @@
                 returned.team = game_entity.get_team() as i32;
                 returned.privileges = game_entity.get_privileges() as i32;
             });
 
         #[cfg_attr(test, allow(clippy::unnecessary_fallible_conversions))]
         Client::try_from(client_id).ok().iter().for_each(|client| {
             returned.connection_state = client.get_state() as i32;
-            returned.userinfo = client.get_user_info();
+            returned.userinfo = client.get_user_info().into();
             returned.steam_id = client.get_steam_id() as i64;
         });
 
         returned
     }
 }
 
@@ -127,69 +128,57 @@
                 _shinqlx.PRIV_NONE,
             )
         )
             "#,
                 None,
                 None,
             );
-            assert!(
-                player_info_constructor.is_ok(),
-                "{}",
-                player_info_constructor.expect_err("this should not happen")
-            );
+            assert!(player_info_constructor.is_ok());
         });
     }
 
-    #[test]
-    fn player_info_python_string() {
-        let player_info = PlayerInfo {
+    fn default_player_info() -> PlayerInfo {
+        PlayerInfo {
             client_id: 2,
-            name: "UnknownPlayer".into(),
+            name: "UnknownPlayer".to_string(),
             connection_state: clientState_t::CS_ACTIVE as i32,
-            userinfo: "asdf".into(),
+            userinfo: "asdf".to_string(),
             steam_id: 42,
             team: team_t::TEAM_SPECTATOR as i32,
             privileges: privileges_t::PRIV_NONE as i32,
-        };
+        }
+    }
 
+    #[test]
+    fn player_info_python_string() {
         assert_eq!(
-            player_info.__str__(),
+            default_player_info().__str__(),
             "PlayerInfo(client_id=2, name=UnknownPlayer, connection_state=4, userinfo=asdf, \
             steam_id=42, team=3, privileges=0)"
         );
     }
 
     #[test]
     fn player_info_python_repr() {
-        let player_info = PlayerInfo {
-            client_id: 2,
-            name: "UnknownPlayer".into(),
-            connection_state: clientState_t::CS_ACTIVE as i32,
-            userinfo: "asdf".into(),
-            steam_id: 42,
-            team: team_t::TEAM_SPECTATOR as i32,
-            privileges: privileges_t::PRIV_NONE as i32,
-        };
-
         assert_eq!(
-            player_info.__repr__(),
+            default_player_info().__repr__(),
             "PlayerInfo(client_id=2, name=UnknownPlayer, connection_state=4, userinfo=asdf, \
             steam_id=42, team=3, privileges=0)"
         );
     }
 
     #[test]
     #[serial]
     fn player_info_from_existing_game_entity_and_client() {
         let game_entity_from_ctx = MockGameEntity::from_context();
         game_entity_from_ctx.expect().returning(|_| {
             let mut mock_game_entity = MockGameEntity::new();
             mock_game_entity
                 .expect_get_player_name()
-                .returning(|| "UnknownPlayer".into());
+                .returning(|| "UnknownPlayer".to_string());
             mock_game_entity
                 .expect_get_team()
                 .returning(|| team_t::TEAM_SPECTATOR);
             mock_game_entity
                 .expect_get_privileges()
                 .returning(|| privileges_t::PRIV_NONE);
             mock_game_entity
@@ -203,21 +192,10 @@
             mock_client
                 .expect_get_user_info()
                 .returning(|| "asdf".into());
             mock_client.expect_get_steam_id().returning(|| 42);
             mock_client
         });
 
-        assert_eq!(
-            PlayerInfo::from(2),
-            PlayerInfo {
-                client_id: 2,
-                name: "UnknownPlayer".into(),
-                connection_state: clientState_t::CS_ACTIVE as i32,
-                userinfo: "asdf".into(),
-                steam_id: 42,
-                team: team_t::TEAM_SPECTATOR as i32,
-                privileges: privileges_t::PRIV_NONE as i32
-            }
-        );
+        assert_eq!(PlayerInfo::from(2), default_player_info());
     }
 }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/player_state.rs` & `shinqlx-0.5.7/src/ffi/python/player_state.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use super::prelude::*;
 use crate::ffi::c::prelude::*;
 
+use alloc::borrow::Cow;
+
 /// Information about a player's state in the game.
-#[pyclass(frozen)]
-#[pyo3(module = "shinqlx", name = "PlayerState", get_all)]
+#[pyclass(module = "_shinqlx", name = "PlayerState", frozen, get_all, sequence)]
 #[derive(Debug, PartialEq)]
 pub(crate) struct PlayerState {
     /// Whether the player's alive or not.
     pub(crate) is_alive: bool,
     /// The player's position.
     pub(crate) position: Vector3,
     /// The player's velocity.
@@ -23,26 +24,26 @@
     /// The player's weapons.
     pub(crate) weapons: Weapons,
     /// The player's weapon ammo.
     pub(crate) ammo: Weapons,
     ///The player's powerups.
     pub(crate) powerups: Powerups,
     /// The player's holdable item.
-    pub(crate) holdable: Option<String>,
+    pub(crate) holdable: Option<Cow<'static, str>>,
     /// A struct sequence with flight parameters.
     pub(crate) flight: Flight,
     /// Whether the player is currently chatting.
     pub(crate) is_chatting: bool,
     /// Whether the player is frozen(freezetag).
     pub(crate) is_frozen: bool,
 }
 
 #[pymethods]
 impl PlayerState {
-    fn __str__(&self) -> String {
+    fn __str__(&self) -> Cow<str> {
         format!("PlayerState(is_alive={}, position={}, veclocity={}, health={}, armor={}, noclip={}, weapon={}, weapons={}, ammo={}, powerups={}, holdable={}, flight={}, is_chatting={}, is_frozen={})",
                 self.is_alive,
                 self.position.__str__(),
                 self.velocity.__str__(),
                 self.health,
                 self.armor,
                 self.noclip,
@@ -52,18 +53,18 @@
                 self.powerups.__str__(),
                 match self.holdable.as_ref() {
                     Some(value) => value,
                     None => "None",
                 },
                 self.flight.__str__(),
                 self.is_chatting,
-                self.is_frozen)
+                self.is_frozen).into()
     }
 
-    fn __repr__(&self) -> String {
+    fn __repr__(&self) -> Cow<str> {
         format!("PlayerState(is_alive={}, position={}, veclocity={}, health={}, armor={}, noclip={}, weapon={}, weapons={}, ammo={}, powerups={}, holdable={}, flight={}, is_chatting={}, is_frozen={})",
                 self.is_alive,
                 self.position.__str__(),
                 self.velocity.__str__(),
                 self.health,
                 self.armor,
                 self.noclip,
@@ -73,15 +74,15 @@
                 self.powerups.__str__(),
                 match self.holdable.as_ref() {
                     Some(value) => value,
                     None => "None",
                 },
                 self.flight.__str__(),
                 self.is_chatting,
-                self.is_frozen)
+                self.is_frozen).into()
     }
 }
 
 impl From<GameEntity> for PlayerState {
     fn from(game_entity: GameEntity) -> Self {
         let game_client = game_entity.get_game_client().unwrap();
         let position = game_client.get_position();
@@ -114,14 +115,33 @@
 mod player_state_tests {
     use crate::ffi::c::prelude::*;
     use crate::ffi::python::prelude::*;
     use crate::prelude::*;
 
     use pretty_assertions::assert_eq;
 
+    fn default_player_state() -> PlayerState {
+        PlayerState {
+            is_alive: true,
+            position: Vector3(1, 2, 3),
+            velocity: Vector3(4, 5, 6),
+            health: 123,
+            armor: 456,
+            noclip: true,
+            weapon: weapon_t::WP_NAILGUN.into(),
+            weapons: Weapons(1, 1, 1, 0, 0, 0, 1, 1, 1, 0, 0, 0, 1, 1, 1),
+            ammo: Weapons(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15),
+            powerups: Powerups(12, 34, 56, 78, 90, 24),
+            holdable: Some("kamikaze".into()),
+            flight: Flight(12, 34, 56, 78),
+            is_chatting: true,
+            is_frozen: true,
+        }
+    }
+
     #[test]
     #[serial]
     fn player_state_from_game_client() {
         let mut mock_game_entity = MockGameEntity::new();
         mock_game_entity.expect_get_game_client().returning(|| {
             let mut mock_game_client = MockGameClient::new();
             mock_game_client
@@ -158,55 +178,21 @@
             mock_game_client.expect_get_flight_refuel().returning(|| 78);
             mock_game_client.expect_is_chatting().returning(|| true);
             mock_game_client.expect_is_frozen().returning(|| true);
             Ok(mock_game_client)
         });
         mock_game_entity.expect_get_health().returning(|| 123);
 
-        assert_eq!(
-            PlayerState::from(mock_game_entity),
-            PlayerState {
-                is_alive: true,
-                position: Vector3(1, 2, 3),
-                velocity: Vector3(4, 5, 6),
-                health: 123,
-                armor: 456,
-                noclip: true,
-                weapon: weapon_t::WP_NAILGUN.into(),
-                weapons: Weapons(1, 1, 1, 0, 0, 0, 1, 1, 1, 0, 0, 0, 1, 1, 1),
-                ammo: Weapons(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15),
-                powerups: Powerups(12, 34, 56, 78, 90, 24),
-                holdable: Some("kamikaze".into()),
-                flight: Flight(12, 34, 56, 78),
-                is_chatting: true,
-                is_frozen: true,
-            }
-        );
+        assert_eq!(PlayerState::from(mock_game_entity), default_player_state());
     }
 
     #[test]
     fn player_state_to_str() {
-        let player_state = PlayerState {
-            is_alive: true,
-            position: Vector3(1, 2, 3),
-            velocity: Vector3(4, 5, 6),
-            health: 123,
-            armor: 456,
-            noclip: true,
-            weapon: weapon_t::WP_NAILGUN.into(),
-            weapons: Weapons(1, 1, 1, 0, 0, 0, 1, 1, 1, 0, 0, 0, 1, 1, 1),
-            ammo: Weapons(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15),
-            powerups: Powerups(12, 34, 56, 78, 90, 24),
-            holdable: Some("kamikaze".into()),
-            flight: Flight(12, 34, 56, 78),
-            is_chatting: true,
-            is_frozen: true,
-        };
         assert_eq!(
-            player_state.__str__(),
+            default_player_state().__str__(),
             "PlayerState(\
             is_alive=true, \
             position=Vector3(x=1, y=2, z=3), \
             veclocity=Vector3(x=4, y=5, z=6), \
             health=123, \
             armor=456, \
             noclip=true, \
@@ -219,33 +205,21 @@
             is_chatting=true, \
             is_frozen=true)");
     }
 
     #[test]
     fn player_state_to_str_with_no_holdble() {
         let player_state = PlayerState {
-            is_alive: true,
-            position: Vector3(1, 2, 3),
-            velocity: Vector3(4, 5, 6),
-            health: 123,
-            armor: 456,
-            noclip: true,
-            weapon: weapon_t::WP_NAILGUN.into(),
-            weapons: Weapons(1, 1, 1, 0, 0, 0, 1, 1, 1, 0, 0, 0, 1, 1, 1),
-            ammo: Weapons(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15),
-            powerups: Powerups(12, 34, 56, 78, 90, 24),
             holdable: None,
-            flight: Flight(12, 34, 56, 78),
-            is_chatting: true,
-            is_frozen: true,
+            ..default_player_state()
         };
 
         assert_eq!(
-                player_state.__str__(),
-                "PlayerState(\
+            player_state.__str__(),
+            "PlayerState(\
             is_alive=true, \
             position=Vector3(x=1, y=2, z=3), \
             veclocity=Vector3(x=4, y=5, z=6), \
             health=123, \
             armor=456, \
             noclip=true, \
             weapon=11, \
@@ -256,33 +230,16 @@
             flight=Flight(fuel=12, max_fuel=34, thrust=56, refuel=78), \
             is_chatting=true, \
             is_frozen=true)");
     }
 
     #[test]
     fn player_state_repr() {
-        let player_state = PlayerState {
-            is_alive: true,
-            position: Vector3(1, 2, 3),
-            velocity: Vector3(4, 5, 6),
-            health: 123,
-            armor: 456,
-            noclip: true,
-            weapon: weapon_t::WP_NAILGUN.into(),
-            weapons: Weapons(1, 1, 1, 0, 0, 0, 1, 1, 1, 0, 0, 0, 1, 1, 1),
-            ammo: Weapons(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15),
-            powerups: Powerups(12, 34, 56, 78, 90, 24),
-            holdable: Some("kamikaze".into()),
-            flight: Flight(12, 34, 56, 78),
-            is_chatting: true,
-            is_frozen: true,
-        };
-
         assert_eq!(
-                player_state.__repr__(),
+                default_player_state().__repr__(),
                 "PlayerState(\
             is_alive=true, \
             position=Vector3(x=1, y=2, z=3), \
             veclocity=Vector3(x=4, y=5, z=6), \
             health=123, \
             armor=456, \
             noclip=true, \
@@ -295,28 +252,16 @@
             is_chatting=true, \
             is_frozen=true)");
     }
 
     #[test]
     fn player_state_repr_with_no_holdable() {
         let player_state = PlayerState {
-            is_alive: true,
-            position: Vector3(1, 2, 3),
-            velocity: Vector3(4, 5, 6),
-            health: 123,
-            armor: 456,
-            noclip: true,
-            weapon: weapon_t::WP_NAILGUN.into(),
-            weapons: Weapons(1, 1, 1, 0, 0, 0, 1, 1, 1, 0, 0, 0, 1, 1, 1),
-            ammo: Weapons(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15),
-            powerups: Powerups(12, 34, 56, 78, 90, 24),
             holdable: None,
-            flight: Flight(12, 34, 56, 78),
-            is_chatting: true,
-            is_frozen: true,
+            ..default_player_state()
         };
 
         assert_eq!(
                 player_state.__repr__(),
                 "PlayerState(\
             is_alive=true, \
             position=Vector3(x=1, y=2, z=3), \
```

### Comparing `shinqlx-0.5.6/src/ffi/python/player_stats.rs` & `shinqlx-0.5.7/src/ffi/python/player_stats.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use super::prelude::*;
 use crate::ffi::c::prelude::*;
 
+use alloc::borrow::Cow;
+
 /// A player's score and some basic stats.
-#[pyclass(frozen)]
-#[pyo3(module = "shinqlx", name = "PlayerStats", get_all)]
+#[pyclass(module = "_shinqlx", name = "PlayerStats", frozen, get_all, sequence)]
 #[derive(Debug, PartialEq)]
 pub(crate) struct PlayerStats {
     /// The player's primary score.
     pub(crate) score: i32,
     /// The player's number of kills.
     pub(crate) kills: i32,
     /// The player's number of deaths.
@@ -20,22 +21,22 @@
     pub(crate) time: i32,
     /// The player's ping.
     pub(crate) ping: i32,
 }
 
 #[pymethods]
 impl PlayerStats {
-    fn __str__(&self) -> String {
+    fn __str__(&self) -> Cow<str> {
         format!("PlayerStats(score={}, kills={}, deaths={}, damage_dealt={}, damage_taken={}, time={}, ping={})",
-                self.score, self.kills, self.deaths, self.damage_dealt, self.damage_taken, self.time, self.ping)
+                self.score, self.kills, self.deaths, self.damage_dealt, self.damage_taken, self.time, self.ping).into()
     }
 
-    fn __repr__(&self) -> String {
+    fn __repr__(&self) -> Cow<str> {
         format!("PlayerStats(score={}, kills={}, deaths={}, damage_dealt={}, damage_taken={}, time={}, ping={})",
-                self.score, self.kills, self.deaths, self.damage_dealt, self.damage_taken, self.time, self.ping)
+                self.score, self.kills, self.deaths, self.damage_dealt, self.damage_taken, self.time, self.ping).into()
     }
 }
 
 impl From<GameClient> for PlayerStats {
     fn from(game_client: GameClient) -> Self {
         Self {
             score: game_client.get_score(),
@@ -53,42 +54,34 @@
 mod player_stats_tests {
     use super::PlayerStats;
     use crate::ffi::c::prelude::*;
     use crate::prelude::*;
 
     use pretty_assertions::assert_eq;
 
-    #[test]
-    fn player_stats_to_str() {
-        let player_stats = PlayerStats {
+    fn default_player_stats() -> PlayerStats {
+        PlayerStats {
             score: 42,
             kills: 7,
             deaths: 9,
             damage_dealt: 5000,
             damage_taken: 4200,
             time: 123,
             ping: 9,
-        };
+        }
+    }
 
-        assert_eq!(player_stats.__str__(), "PlayerStats(score=42, kills=7, deaths=9, damage_dealt=5000, damage_taken=4200, time=123, ping=9)");
+    #[test]
+    fn player_stats_to_str() {
+        assert_eq!(default_player_stats().__str__(), "PlayerStats(score=42, kills=7, deaths=9, damage_dealt=5000, damage_taken=4200, time=123, ping=9)");
     }
 
     #[test]
     fn player_stats_repr() {
-        let player_stats = PlayerStats {
-            score: 42,
-            kills: 7,
-            deaths: 9,
-            damage_dealt: 5000,
-            damage_taken: 4200,
-            time: 123,
-            ping: 9,
-        };
-
-        assert_eq!(player_stats.__repr__(), "PlayerStats(score=42, kills=7, deaths=9, damage_dealt=5000, damage_taken=4200, time=123, ping=9)");
+        assert_eq!(default_player_stats().__repr__(), "PlayerStats(score=42, kills=7, deaths=9, damage_dealt=5000, damage_taken=4200, time=123, ping=9)");
     }
 
     #[test]
     #[serial]
     fn player_state_from_game_client() {
         let mut mock_game_client = MockGameClient::new();
         mock_game_client.expect_get_score().returning(|| 42);
@@ -99,21 +92,10 @@
             .returning(|| 5000);
         mock_game_client
             .expect_get_damage_taken()
             .returning(|| 4200);
         mock_game_client.expect_get_time_on_team().returning(|| 123);
         mock_game_client.expect_get_ping().returning(|| 9);
 
-        assert_eq!(
-            PlayerStats::from(mock_game_client),
-            PlayerStats {
-                score: 42,
-                kills: 7,
-                deaths: 9,
-                damage_dealt: 5000,
-                damage_taken: 4200,
-                time: 123,
-                ping: 9,
-            }
-        )
+        assert_eq!(PlayerStats::from(mock_game_client), default_player_stats())
     }
 }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/powerups.rs` & `shinqlx-0.5.7/src/ffi/python/powerups.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use super::prelude::*;
 
+use alloc::borrow::Cow;
+
 use pyo3::{basic::CompareOp, exceptions::PyValueError, types::PyTuple};
 
 /// A struct sequence containing all the powerups in the game.
-#[pyclass(frozen)]
-#[pyo3(module = "shinqlx", name = "Powerups", get_all)]
+#[pyclass(module = "_shinqlx", name = "Powerups", frozen, get_all, sequence)]
 #[derive(PartialEq, Eq, Debug, Clone, Copy)]
 pub(crate) struct Powerups(
     #[pyo3(name = "quad")] pub(crate) i32,
     #[pyo3(name = "battlesuit")] pub(crate) i32,
     #[pyo3(name = "haste")] pub(crate) i32,
     #[pyo3(name = "invisibility")] pub(crate) i32,
     #[pyo3(name = "regeneration")] pub(crate) i32,
@@ -26,15 +27,15 @@
         [value.0, value.1, value.2, value.3, value.4, value.5]
     }
 }
 
 #[pymethods]
 impl Powerups {
     #[new]
-    fn py_new(values: &PyTuple) -> PyResult<Self> {
+    fn py_new(values: &Bound<'_, PyTuple>) -> PyResult<Self> {
         if values.len() < 6 {
             return Err(PyValueError::new_err(
                 "tuple did not provide values for all 6 powerups",
             ));
         }
 
         if values.len() > 6 {
@@ -67,22 +68,22 @@
         match op {
             CompareOp::Eq => (self == other).into_py(py),
             CompareOp::Ne => (self != other).into_py(py),
             _ => py.NotImplemented(),
         }
     }
 
-    pub(crate) fn __str__(&self) -> String {
+    pub(crate) fn __str__(&self) -> Cow<str> {
         format!("Powerups(quad={}, battlesuit={}, haste={}, invisibility={}, regeneration={}, invulnerability={})",
-                self.0, self.1, self.2, self.3, self.4, self.5)
+                self.0, self.1, self.2, self.3, self.4, self.5).into()
     }
 
-    fn __repr__(&self) -> String {
+    fn __repr__(&self) -> Cow<str> {
         format!("Powerups(quad={}, battlesuit={}, haste={}, invisibility={}, regeneration={}, invulnerability={})",
-                self.0, self.1, self.2, self.3, self.4, self.5)
+                self.0, self.1, self.2, self.3, self.4, self.5).into()
     }
 }
 
 #[cfg(test)]
 mod powerups_tests {
     use crate::ffi::python::prelude::*;
```

### Comparing `shinqlx-0.5.6/src/ffi/python/vector3.rs` & `shinqlx-0.5.7/src/ffi/python/vector3.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use super::prelude::*;
 
+use alloc::borrow::Cow;
 use core::array;
 use pyo3::{basic::CompareOp, exceptions::PyValueError, types::PyTuple};
 
 #[pyclass]
 struct Vector3Iter {
     iter: array::IntoIter<i32, 3>,
 }
@@ -16,26 +17,26 @@
 
     fn __next__(mut slf: PyRefMut<'_, Self>) -> Option<i32> {
         slf.iter.next()
     }
 }
 
 /// A three-dimensional vector.
-#[pyclass(name = "Vector3", module = "shinqlx", get_all, frozen)]
+#[pyclass(module = "_shinqlx", name = "Vector3", frozen, get_all, sequence)]
 #[derive(PartialEq, Eq, Debug, Clone, Copy, Default)]
 pub(crate) struct Vector3(
     #[pyo3(name = "x")] pub(crate) i32,
     #[pyo3(name = "y")] pub(crate) i32,
     #[pyo3(name = "z")] pub(crate) i32,
 );
 
 #[pymethods]
 impl Vector3 {
     #[new]
-    fn py_new(values: &PyTuple) -> PyResult<Self> {
+    fn py_new(values: &Bound<'_, PyTuple>) -> PyResult<Self> {
         if values.len() < 3 {
             return Err(PyValueError::new_err(
                 "tuple did not provide values for all three dimensions",
             ));
         }
 
         if values.len() > 3 {
@@ -64,28 +65,27 @@
         match op {
             CompareOp::Eq => (self == other).into_py(py),
             CompareOp::Ne => (self != other).into_py(py),
             _ => py.NotImplemented(),
         }
     }
 
-    pub(crate) fn __str__(&self) -> String {
-        format!("Vector3(x={}, y={}, z={})", self.0, self.1, self.2)
+    pub(crate) fn __str__(&self) -> Cow<str> {
+        format!("Vector3(x={}, y={}, z={})", self.0, self.1, self.2).into()
     }
 
-    fn __repr__(&self) -> String {
-        format!("Vector3(x={}, y={}, z={})", self.0, self.1, self.2)
+    fn __repr__(&self) -> Cow<str> {
+        format!("Vector3(x={}, y={}, z={})", self.0, self.1, self.2).into()
     }
 
-    fn __iter__(slf: PyRef<'_, Self>) -> PyResult<Py<Vector3Iter>> {
+    fn __iter__(slf: PyRef<'_, Self>) -> Vector3Iter {
         let iter_array = [slf.0, slf.1, slf.2];
-        let iter = Vector3Iter {
+        Vector3Iter {
             iter: iter_array.into_iter(),
-        };
-        Py::new(slf.py(), iter)
+        }
     }
 }
 
 impl From<(f32, f32, f32)> for Vector3 {
     fn from(value: (f32, f32, f32)) -> Self {
         Self(value.0 as i32, value.1 as i32, value.2 as i32)
     }
```

### Comparing `shinqlx-0.5.6/src/ffi/python/weapons.rs` & `shinqlx-0.5.7/src/ffi/python/weapons.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use super::prelude::*;
 
+use alloc::borrow::Cow;
+
 use pyo3::{basic::CompareOp, exceptions::PyValueError, types::PyTuple};
 
 /// A struct sequence containing all the weapons in the game.
-#[pyclass(frozen)]
-#[pyo3(module = "shinqlx", name = "Weapons", get_all)]
+#[pyclass(module = "_shinqlx", name = "Weapons", frozen, get_all, sequence)]
 #[derive(PartialEq, Eq, Debug, Clone, Copy)]
 pub(crate) struct Weapons(
     #[pyo3(name = "g")] pub(crate) i32,
     #[pyo3(name = "mg")] pub(crate) i32,
     #[pyo3(name = "sg")] pub(crate) i32,
     #[pyo3(name = "gl")] pub(crate) i32,
     #[pyo3(name = "rl")] pub(crate) i32,
@@ -41,15 +42,15 @@
         ]
     }
 }
 
 #[pymethods]
 impl Weapons {
     #[new]
-    fn py_new(values: &PyTuple) -> PyResult<Self> {
+    fn py_new(values: &Bound<'_, PyTuple>) -> PyResult<Self> {
         if values.len() < 15 {
             return Err(PyValueError::new_err(
                 "tuple did not provide values for all 15 weapons",
             ));
         }
 
         if values.len() > 15 {
@@ -82,22 +83,22 @@
         match op {
             CompareOp::Eq => (self == other).into_py(py),
             CompareOp::Ne => (self != other).into_py(py),
             _ => py.NotImplemented(),
         }
     }
 
-    pub(crate) fn __str__(&self) -> String {
+    pub(crate) fn __str__(&self) -> Cow<str> {
         format!("Weapons(g={}, mg={}, sg={}, gl={}, rl={}, lg={}, rg={}, pg={}, bfg={}, gh={}, ng={}, pl={}, cg={}, hmg={}, hands={})",
-                self.0, self.1, self.2, self.3, self.4, self.5, self.5, self.7, self.8, self.9, self.10, self.11, self.12, self.13, self.14)
+                self.0, self.1, self.2, self.3, self.4, self.5, self.5, self.7, self.8, self.9, self.10, self.11, self.12, self.13, self.14).into()
     }
 
-    fn __repr__(&self) -> String {
+    fn __repr__(&self) -> Cow<str> {
         format!("Weapons(g={}, mg={}, sg={}, gl={}, rl={}, lg={}, rg={}, pg={}, bfg={}, gh={}, ng={}, pl={}, cg={}, hmg={}, hands={})",
-                self.0, self.1, self.2, self.3, self.4, self.5, self.5, self.7, self.8, self.9, self.10, self.11, self.12, self.13, self.14)
+                self.0, self.1, self.2, self.3, self.4, self.5, self.5, self.7, self.8, self.9, self.10, self.11, self.12, self.13, self.14).into()
     }
 }
 
 #[cfg(test)]
 mod weapons_tests {
     use crate::ffi::python::prelude::*;
 
@@ -258,14 +259,15 @@
             assert!(
                 ammo_constructor.is_ok(),
                 "{}",
                 ammo_constructor.expect_err("this should not happen")
             );
         });
     }
+
     #[rstest]
     #[cfg_attr(miri, ignore)]
     fn ammo_py_constructor_with_too_few_values(_pyshinqlx_setup: ()) {
         Python::with_gil(|py| {
             let ammo_constructor = py.run_bound(
                 r#"
 import _shinqlx
```

### Comparing `shinqlx-0.5.6/src/hooks.rs` & `shinqlx-0.5.7/src/hooks.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,85 +9,77 @@
 use crate::MAIN_ENGINE;
 
 use core::{
     borrow::BorrowMut,
     ffi::{c_char, c_int, CStr, VaList, VaListImpl},
 };
 
-pub(crate) fn shinqlx_cmd_addcommand(cmd: *const c_char, func: unsafe extern "C" fn()) {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    if !main_engine.is_common_initialized() {
-        if let Err(err) = main_engine.initialize_static() {
-            error!(target: "shinqlx", "{:?}", err);
-            error!(target: "shinqlx", "Static initialization failed. Exiting.");
-            panic!("Static initialization failed. Exiting.");
+pub(crate) extern "C" fn shinqlx_cmd_addcommand(cmd: *const c_char, func: unsafe extern "C" fn()) {
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        if !main_engine.is_common_initialized() {
+            if let Err(err) = main_engine.initialize_static() {
+                error!(target: "shinqlx", "{:?}", err);
+                error!(target: "shinqlx", "Static initialization failed. Exiting.");
+                panic!("Static initialization failed. Exiting.");
+            }
         }
-    }
 
-    let command = unsafe { CStr::from_ptr(cmd) }.to_string_lossy();
-    if !command.is_empty() {
-        main_engine.add_command(&command, func);
-    }
+        let command = unsafe { CStr::from_ptr(cmd) }.to_string_lossy();
+        if !command.is_empty() {
+            main_engine.add_command(&command, func);
+        }
+    });
 }
 
-pub(crate) fn shinqlx_sys_setmoduleoffset(
+pub(crate) extern "C" fn shinqlx_sys_setmoduleoffset(
     module_name: *const c_char,
     offset: unsafe extern "C" fn(),
 ) {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        let converted_module_name = unsafe { CStr::from_ptr(module_name) }.to_string_lossy();
 
-    let converted_module_name = unsafe { CStr::from_ptr(module_name) }.to_string_lossy();
-
-    // We should be getting qagame, but check just in case.
-    if converted_module_name.as_ref() != "qagame" {
-        error!(target: "shinqlx", "Unknown module: {}", converted_module_name);
-    }
+        // We should be getting qagame, but check just in case.
+        if converted_module_name.as_ref() != "qagame" {
+            error!(target: "shinqlx", "Unknown module: {}", converted_module_name);
+        }
 
-    main_engine.set_module_offset(&converted_module_name, offset);
+        main_engine.set_module_offset(&converted_module_name, offset);
 
-    if let Err(err) = main_engine.initialize_vm(offset as usize) {
-        error!(target: "shinqlx", "{:?}", err);
-        error!(target: "shinqlx", "VM could not be initializied. Exiting.");
-        panic!("VM could not be initializied. Exiting.");
-    }
+        if let Err(err) = main_engine.initialize_vm(offset as usize) {
+            error!(target: "shinqlx", "{:?}", err);
+            error!(target: "shinqlx", "VM could not be initializied. Exiting.");
+            panic!("VM could not be initializied. Exiting.");
+        }
+    });
 }
 
 #[cfg_attr(test, allow(dead_code))]
 pub(crate) fn shinqlx_g_initgame(level_time: c_int, random_seed: c_int, restart: c_int) {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine.init_game(level_time, random_seed, restart);
 
-    main_engine.init_game(level_time, random_seed, restart);
+        main_engine.set_tag();
+        main_engine.initialize_cvars();
 
-    main_engine.set_tag();
-    main_engine.initialize_cvars();
-
-    if restart != 0 {
-        new_game_dispatcher(true);
-    }
+        if restart != 0 {
+            new_game_dispatcher(true);
+        }
+    });
 }
 
 #[cfg_attr(test, allow(dead_code))]
 pub(crate) fn shinqlx_g_shutdowngame(restart: c_int) {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    main_engine.unhook_vm(restart != 0);
-    main_engine.shutdown_game(restart);
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine.unhook_vm(restart != 0);
+        main_engine.shutdown_game(restart);
+    });
 }
 
 #[cfg_attr(test, allow(dead_code))]
-pub(crate) fn shinqlx_sv_executeclientcommand(
+pub(crate) extern "C" fn shinqlx_sv_executeclientcommand(
     client: *mut client_t,
     cmd: *const c_char,
     client_ok: qboolean,
 ) {
     let rust_cmd = unsafe { CStr::from_ptr(cmd) }.to_string_lossy();
     shinqlx_execute_client_command(Client::try_from(client).ok(), rust_cmd, client_ok);
 }
@@ -200,37 +192,35 @@
     }
 
     if !passed_on_cmd_str.is_empty() {
         main_engine.send_server_command(client, &passed_on_cmd_str);
     }
 }
 
-pub(crate) fn shinqlx_sv_cliententerworld(client: *mut client_t, cmd: *mut usercmd_t) {
-    let Some(mut safe_client): Option<Client> = client.try_into().ok() else {
-        return;
-    };
-
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
+pub(crate) extern "C" fn shinqlx_sv_cliententerworld(client: *mut client_t, cmd: *mut usercmd_t) {
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        let Some(mut safe_client) = Client::try_from(client).ok() else {
+            return;
+        };
 
-    let state = safe_client.get_state();
+        let state = safe_client.get_state();
 
-    main_engine.client_enter_world(&mut safe_client, cmd);
+        main_engine.client_enter_world(&mut safe_client, cmd);
 
-    // gentity is NULL if map changed.
-    // state is CS_PRIMED only if it's the first time they connect to the server,
-    // otherwise the dispatcher would also go off when a game starts and such.
-    if safe_client.has_gentity() && state == clientState_t::CS_PRIMED {
-        client_loaded_dispatcher(safe_client.get_client_id());
-    }
+        // gentity is NULL if map changed.
+        // state is CS_PRIMED only if it's the first time they connect to the server,
+        // otherwise the dispatcher would also go off when a game starts and such.
+        if safe_client.has_gentity() && state == clientState_t::CS_PRIMED {
+            client_loaded_dispatcher(safe_client.get_client_id());
+        }
+    });
 }
 
 #[cfg_attr(test, allow(dead_code))]
-pub(crate) fn shinqlx_sv_setconfigstring(index: c_int, value: *const c_char) {
+pub(crate) extern "C" fn shinqlx_sv_setconfigstring(index: c_int, value: *const c_char) {
     let safe_value = if !value.is_null() {
         unsafe { CStr::from_ptr(value) }.to_string_lossy()
     } else {
         "".into()
     };
 
     let Ok(ql_index) = u32::try_from(index) else {
@@ -240,46 +230,41 @@
     shinqlx_set_configstring(ql_index, &safe_value);
 }
 
 pub(crate) fn shinqlx_set_configstring<T>(index: T, value: &str)
 where
     T: TryInto<c_int> + Into<u32> + Copy,
 {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    let Ok(c_index) = index.try_into() else {
-        return;
-    };
-
-    // Indices 16 and 66X are spammed a ton every frame for some reason,
-    // so we add some exceptions for those. I don't think we should have any
-    // use for those particular ones anyway. If we don't do this, we get
-    // like a 25% increase in CPU usage on an empty server.
-    if c_index == 16 || (662..670).contains(&c_index) {
-        main_engine.set_configstring(c_index, value.as_ref());
-        return;
-    }
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        index.try_into().iter().for_each(|&c_index| {
+            // Indices 16 and 66X are spammed a ton every frame for some reason,
+            // so we add some exceptions for those. I don't think we should have any
+            // use for those particular ones anyway. If we don't do this, we get
+            // like a 25% increase in CPU usage on an empty server.
+            if c_index == 16 || (662..670).contains(&c_index) {
+                main_engine.set_configstring(c_index, value.as_ref());
+                return;
+            }
 
-    let Some(res) = set_configstring_dispatcher(index.into(), value) else {
-        return;
-    };
-    main_engine.set_configstring(c_index, &res);
+            let Some(res) = set_configstring_dispatcher(index.into(), value) else {
+                return;
+            };
+            main_engine.set_configstring(c_index, &res);
+        })
+    });
 }
 
 #[cfg_attr(test, allow(dead_code))]
-pub(crate) fn shinqlx_sv_dropclient(client: *mut client_t, reason: *const c_char) {
-    let Ok(mut safe_client) = Client::try_from(client) else {
-        return;
-    };
-    shinqlx_drop_client(
-        &mut safe_client,
-        unsafe { CStr::from_ptr(reason) }.to_string_lossy(),
-    );
+pub(crate) extern "C" fn shinqlx_sv_dropclient(client: *mut client_t, reason: *const c_char) {
+    Client::try_from(client).iter_mut().for_each(|safe_client| {
+        shinqlx_drop_client(
+            safe_client,
+            unsafe { CStr::from_ptr(reason) }.to_string_lossy(),
+        );
+    });
 }
 
 pub(crate) fn shinqlx_drop_client<T>(client: &mut Client, reason: T)
 where
     T: AsRef<str>,
 {
     client_disconnect_dispatcher(client.get_client_id(), reason.as_ref());
@@ -314,51 +299,45 @@
     }
 }
 
 pub(crate) fn shinqlx_com_printf<T>(msg: T)
 where
     T: AsRef<str>,
 {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    let Some(_res) = console_print_dispatcher(msg.as_ref()) else {
-        return;
-    };
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        let Some(_) = console_print_dispatcher(msg.as_ref()) else {
+            return;
+        };
 
-    main_engine.com_printf(msg.as_ref());
+        main_engine.com_printf(msg.as_ref());
+    });
 }
 
-pub(crate) fn shinqlx_sv_spawnserver(server: *const c_char, kill_bots: qboolean) {
+pub(crate) extern "C" fn shinqlx_sv_spawnserver(server: *const c_char, kill_bots: qboolean) {
     let server_str = unsafe { CStr::from_ptr(server) }.to_string_lossy();
     if server_str.is_empty() {
         return;
     }
 
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    main_engine.spawn_server(
-        server_str.as_ref(),
-        <qboolean as Into<bool>>::into(kill_bots),
-    );
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine.spawn_server(
+            server_str.as_ref(),
+            <qboolean as Into<bool>>::into(kill_bots),
+        );
 
-    new_game_dispatcher(false);
+        new_game_dispatcher(false);
+    });
 }
 
 pub(crate) fn shinqlx_g_runframe(time: c_int) {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    frame_dispatcher();
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        frame_dispatcher();
 
-    main_engine.run_frame(time);
+        main_engine.run_frame(time);
+    });
 }
 
 static mut CLIENT_CONNECT_BUFFER: [[c_char; MAX_STRING_CHARS as usize]; MAX_CLIENTS as usize] =
     [[0; MAX_STRING_CHARS as usize]; MAX_CLIENTS as usize];
 
 unsafe fn to_return_string(client_id: i32, input: String) -> *const c_char {
     let bytes = input.as_bytes();
@@ -366,15 +345,15 @@
     let len = bytes.len();
     CLIENT_CONNECT_BUFFER[client_id as usize][0..len]
         .fill_with(|| *bytes_iter.next().unwrap() as c_char);
     CLIENT_CONNECT_BUFFER[client_id as usize][len..].fill(0);
     &CLIENT_CONNECT_BUFFER[client_id as usize] as *const c_char
 }
 
-pub(crate) fn shinqlx_client_connect(
+pub(crate) extern "C" fn shinqlx_client_connect(
     client_num: c_int,
     first_time: qboolean,
     is_bot: qboolean,
 ) -> *const c_char {
     let Some(ref main_engine) = *MAIN_ENGINE.load() else {
         return ptr::null();
     };
@@ -391,38 +370,35 @@
         client_num,
         <qboolean as Into<bool>>::into(first_time),
         <qboolean as Into<bool>>::into(is_bot),
     )
 }
 
 #[cfg_attr(test, allow(dead_code))]
-pub(crate) fn shinqlx_clientspawn(ent: *mut gentity_t) {
-    let Some(mut game_entity): Option<GameEntity> = ent.try_into().ok() else {
-        return;
-    };
-
-    shinqlx_client_spawn(&mut game_entity)
+pub(crate) extern "C" fn shinqlx_clientspawn(ent: *mut gentity_t) {
+    GameEntity::try_from(ent)
+        .ok()
+        .iter_mut()
+        .for_each(shinqlx_client_spawn);
 }
 
 #[cfg_attr(test, allow(dead_code))]
 pub(crate) fn shinqlx_client_spawn(game_entity: &mut GameEntity) {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine.client_spawn(game_entity.borrow_mut());
 
-    main_engine.client_spawn(game_entity.borrow_mut());
-
-    // Since we won't ever stop the real function from being called,
-    // we trigger the event after calling the real one. This will allow
-    // us to set weapons and such without it getting overriden later.
-    client_spawn_dispatcher(game_entity.get_entity_id());
+        // Since we won't ever stop the real function from being called,
+        // we trigger the event after calling the real one. This will allow
+        // us to set weapons and such without it getting overriden later.
+        client_spawn_dispatcher(game_entity.get_entity_id());
+    });
 }
 
-pub(crate) fn shinqlx_g_startkamikaze(ent: *mut gentity_t) {
-    let Some(mut game_entity): Option<GameEntity> = ent.try_into().ok() else {
+pub(crate) extern "C" fn shinqlx_g_startkamikaze(ent: *mut gentity_t) {
+    let Some(mut game_entity): Option<GameEntity> = GameEntity::try_from(ent).ok() else {
         return;
     };
 
     let client_id = if let Ok(game_client) = game_entity.get_game_client() {
         game_client.get_client_num()
     } else if let Ok(activator) = game_entity.get_activator() {
         activator.get_owner_num()
@@ -440,79 +416,75 @@
         return;
     }
 
     kamikaze_explode_dispatcher(client_id, game_entity.get_game_client().is_ok())
 }
 
 #[allow(clippy::too_many_arguments)]
-pub(crate) fn shinqlx_g_damage(
+pub(crate) extern "C" fn shinqlx_g_damage(
     target: *mut gentity_t,    // entity that is being damaged
     inflictor: *mut gentity_t, // entity that is causing the damage
     attacker: *mut gentity_t,  // entity that caused the inflictor to damage target
     dir: *mut vec3_t,          // direction of the attack for knockback
     pos: *mut vec3_t,          // point at which the damage is being inflicted, used for headshots
     damage: c_int,             // amount of damage being inflicted
     dflags: c_int,             // these flags are used to control how T_Damage works
     // DAMAGE_RADIUS			damage was indirect (from a nearby explosion)
     // DAMAGE_NO_ARMOR			armor does not protect from this damage
     // DAMAGE_NO_KNOCKBACK		do not affect velocity, just view angles
     // DAMAGE_NO_PROTECTION	kills godmode, armor, everything
     // DAMAGE_NO_TEAM_PROTECTION	kills team mates
     means_of_death: c_int, // means_of_death indicator
 ) {
-    let Some(ref main_engine) = *MAIN_ENGINE.load() else {
-        return;
-    };
-
-    main_engine.register_damage(
-        target,
-        inflictor,
-        attacker,
-        dir,
-        pos,
-        damage,
-        dflags,
-        means_of_death,
-    );
-
-    let Ok(target_entity) = GameEntity::try_from(target) else {
-        return;
-    };
-
-    if attacker.is_null() {
-        damage_dispatcher(
-            target_entity.get_entity_id(),
-            None,
+    MAIN_ENGINE.load().iter().for_each(|main_engine| {
+        main_engine.register_damage(
+            target,
+            inflictor,
+            attacker,
+            dir,
+            pos,
             damage,
             dflags,
             means_of_death,
         );
-        return;
-    }
 
-    match GameEntity::try_from(attacker) {
-        Err(_) => {
-            damage_dispatcher(
-                target_entity.get_entity_id(),
-                None,
-                damage,
-                dflags,
-                means_of_death,
-            );
-        }
-        Ok(attacker_entity) => {
-            damage_dispatcher(
-                target_entity.get_entity_id(),
-                Some(attacker_entity.get_entity_id()),
-                damage,
-                dflags,
-                means_of_death,
-            );
-        }
-    }
+        GameEntity::try_from(target)
+            .iter()
+            .for_each(|target_entity| match attacker.is_null() {
+                true => {
+                    damage_dispatcher(
+                        target_entity.get_entity_id(),
+                        None,
+                        damage,
+                        dflags,
+                        means_of_death,
+                    );
+                }
+                false => match GameEntity::try_from(attacker) {
+                    Err(_) => {
+                        damage_dispatcher(
+                            target_entity.get_entity_id(),
+                            None,
+                            damage,
+                            dflags,
+                            means_of_death,
+                        );
+                    }
+                    Ok(attacker_entity) => {
+                        damage_dispatcher(
+                            target_entity.get_entity_id(),
+                            Some(attacker_entity.get_entity_id()),
+                            damage,
+                            dflags,
+                            means_of_death,
+                        );
+                    }
+                },
+            });
+    });
 }
 
 #[cfg(test)]
 #[cfg_attr(test, mockall::automock)]
 #[allow(dead_code)]
 #[allow(clippy::module_inception)]
 pub(crate) mod hooks {
@@ -837,15 +809,15 @@
         let mut mock_client = MockClient::new();
         mock_client.expect_has_gentity().return_const(true).times(1);
         mock_client.expect_get_client_id().return_const(42).times(1);
         let client_command_ctx = client_command_dispatcher_context();
         client_command_ctx
             .expect()
             .with(predicate::eq(42), predicate::eq("cp asdf".to_string()))
-            .return_const(Some("cp modified".into()))
+            .return_const(Some("cp modified".to_string()))
             .times(1);
 
         shinqlx_execute_client_command(Some(mock_client), "cp asdf", true);
     }
 
     #[test]
     #[serial]
@@ -858,15 +830,15 @@
         let mut mock_client = MockClient::new();
         mock_client.expect_has_gentity().return_const(true).times(1);
         mock_client.expect_get_client_id().return_const(42).times(1);
         let client_command_ctx = client_command_dispatcher_context();
         client_command_ctx
             .expect()
             .with(predicate::eq(42), predicate::eq("cp asdf".to_string()))
-            .return_const(Some("".into()))
+            .return_const(Some("".to_string()))
             .times(1);
 
         shinqlx_execute_client_command(Some(mock_client), "cp asdf", true);
     }
 
     #[test]
     #[serial]
@@ -900,15 +872,15 @@
             .expect_send_server_command()
             .withf(|client, cmd| client.is_none() && cmd == "cp modified")
             .times(1);
         let client_command_ctx = server_command_dispatcher_context();
         client_command_ctx
             .expect()
             .with(predicate::eq(None), predicate::eq("cp asdf".to_string()))
-            .return_const(Some("cp modified".into()))
+            .return_const(Some("cp modified".to_string()))
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
         shinqlx_send_server_command(None, "cp asdf");
     }
 
     #[test]
@@ -970,15 +942,15 @@
         let client_command_ctx = server_command_dispatcher_context();
         client_command_ctx
             .expect()
             .with(
                 predicate::eq(Some(42)),
                 predicate::eq("cp asdf".to_string()),
             )
-            .return_const(Some("cp modified".into()))
+            .return_const(Some("cp modified".to_string()))
             .times(1);
 
         shinqlx_send_server_command(Some(mock_client), "cp asdf");
     }
 
     #[test]
     #[serial]
@@ -993,15 +965,15 @@
         let client_command_ctx = server_command_dispatcher_context();
         client_command_ctx
             .expect()
             .with(
                 predicate::eq(Some(42)),
                 predicate::eq("cp asdf".to_string()),
             )
-            .return_const(Some("".into()))
+            .return_const(Some("".to_string()))
             .times(1);
 
         shinqlx_send_server_command(Some(mock_client), "cp asdf");
     }
 
     #[test]
     #[serial]
@@ -1186,15 +1158,15 @@
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
         let set_configstring_dispatcher_ctx = set_configstring_dispatcher_context();
         set_configstring_dispatcher_ctx
             .expect()
             .with(predicate::eq(42), predicate::eq("some value"))
-            .return_const(Some("other value".into()))
+            .return_const(Some("other value".to_string()))
             .times(1);
 
         shinqlx_set_configstring(42u32, "some value");
     }
 
     #[test]
     #[serial]
@@ -1206,15 +1178,15 @@
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
         let set_configstring_dispatcher_ctx = set_configstring_dispatcher_context();
         set_configstring_dispatcher_ctx
             .expect()
             .with(predicate::eq(42), predicate::eq("some value"))
-            .return_const(Some("some value".into()))
+            .return_const(Some("some value".to_string()))
             .times(1);
 
         shinqlx_set_configstring(42u32, "some value");
     }
 
     #[test]
     #[serial]
@@ -1268,15 +1240,15 @@
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
         let mock_console_print_dispatcher_ctx = console_print_dispatcher_context();
         mock_console_print_dispatcher_ctx
             .expect()
             .with(predicate::eq("Hello World!"))
-            .return_const(Some("Hello you!".into()))
+            .return_const(Some("Hello you!".to_string()))
             .times(1);
 
         shinqlx_com_printf("Hello World!");
     }
 
     #[test]
     #[serial]
@@ -1384,15 +1356,15 @@
         mock_engine.expect_client_connect().times(0);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
         let client_connect_dispatcher_ctx = client_connect_dispatcher_context();
         client_connect_dispatcher_ctx
             .expect()
             .with(predicate::eq(42), predicate::eq(false))
-            .return_const(Some("you are banned from this server".into()))
+            .return_const(Some("you are banned from this server".to_string()))
             .times(1);
 
         let result = shinqlx_client_connect(42, qboolean::qtrue, qboolean::qfalse);
         assert_eq!(
             unsafe { CStr::from_ptr(result) }.to_string_lossy(),
             "you are banned from this server"
         );
@@ -1409,15 +1381,15 @@
             .times(1);
         MAIN_ENGINE.store(Some(mock_engine.into()));
 
         let client_connect_dispatcher_ctx = client_connect_dispatcher_context();
         client_connect_dispatcher_ctx
             .expect()
             .with(predicate::eq(42), predicate::eq(true))
-            .return_const(Some("we don't like bots here".into()))
+            .return_const(Some("we don't like bots here".to_string()))
             .times(1);
 
         shinqlx_client_connect(42, qboolean::qtrue, qboolean::qtrue);
     }
 
     #[test]
     #[serial]
```

### Comparing `shinqlx-0.5.6/src/lib.rs` & `shinqlx-0.5.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/patches.rs` & `shinqlx-0.5.7/src/patches.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/src/quake_live_engine.rs` & `shinqlx-0.5.7/src/quake_live_engine.rs`

 * *Files 14% similar despite different names*

```diff
@@ -60,67 +60,74 @@
 }
 
 #[derive(Debug)]
 struct StaticFunctions {
     #[cfg_attr(test, allow(dead_code))]
     com_printf_orig: extern "C" fn(*const c_char, ...),
     #[cfg_attr(test, allow(dead_code))]
-    cmd_addcommand_orig: fn(*const c_char, unsafe extern "C" fn()),
-    cmd_args_orig: fn() -> *const c_char,
-    cmd_argv_orig: fn(c_int) -> *const c_char,
+    cmd_addcommand_orig: extern "C" fn(*const c_char, unsafe extern "C" fn()),
+    cmd_args_orig: extern "C" fn() -> *const c_char,
+    cmd_argv_orig: extern "C" fn(c_int) -> *const c_char,
     #[allow(dead_code)]
-    cmd_tokenizestring_orig: fn(*const c_char),
+    cmd_tokenizestring_orig: extern "C" fn(*const c_char),
     #[allow(dead_code)]
-    cbuf_executetext_orig: fn(cbufExec_t, *const c_char),
-    cvar_findvar_orig: fn(*const c_char) -> *mut cvar_t,
-    cvar_get_orig: fn(*const c_char, *const c_char, c_int) -> *mut cvar_t,
-    cvar_getlimit_orig:
-        fn(*const c_char, *const c_char, *const c_char, *const c_char, c_int) -> *mut cvar_t,
-    cvar_set2_orig: fn(*const c_char, *const c_char, qboolean) -> *mut cvar_t,
+    cbuf_executetext_orig: extern "C" fn(cbufExec_t, *const c_char),
+    cvar_findvar_orig: extern "C" fn(*const c_char) -> *mut cvar_t,
+    cvar_get_orig: extern "C" fn(*const c_char, *const c_char, c_int) -> *mut cvar_t,
+    cvar_getlimit_orig: extern "C" fn(
+        *const c_char,
+        *const c_char,
+        *const c_char,
+        *const c_char,
+        c_int,
+    ) -> *mut cvar_t,
+    cvar_set2_orig: extern "C" fn(*const c_char, *const c_char, qboolean) -> *mut cvar_t,
     #[cfg_attr(test, allow(dead_code))]
     sv_sendservercommand_orig: extern "C" fn(*mut client_t, *const c_char, ...),
     #[cfg_attr(test, allow(dead_code))]
-    sv_executeclientcommand_orig: fn(*mut client_t, *const c_char, qboolean),
+    sv_executeclientcommand_orig: extern "C" fn(*mut client_t, *const c_char, qboolean),
     #[cfg_attr(test, allow(dead_code))]
-    sv_shutdown_orig: fn(*const c_char),
-    sv_map_f_orig: fn(),
+    sv_shutdown_orig: extern "C" fn(*const c_char),
+    sv_map_f_orig: extern "C" fn(),
     #[cfg_attr(test, allow(dead_code))]
-    sv_cliententerworld_orig: fn(*mut client_t, *mut usercmd_t),
+    sv_cliententerworld_orig: extern "C" fn(*mut client_t, *mut usercmd_t),
     #[cfg_attr(test, allow(dead_code))]
-    sv_setconfigstring_orig: fn(c_int, *const c_char),
-    sv_getconfigstring_orig: fn(c_int, *const c_char, c_int),
+    sv_setconfigstring_orig: extern "C" fn(c_int, *const c_char),
+    sv_getconfigstring_orig: extern "C" fn(c_int, *const c_char, c_int),
     #[cfg_attr(test, allow(dead_code))]
-    sv_dropclient_orig: fn(*mut client_t, *const c_char),
+    sv_dropclient_orig: extern "C" fn(*mut client_t, *const c_char),
     #[cfg_attr(test, allow(dead_code))]
-    sys_setmoduleoffset_orig: fn(*const c_char, unsafe extern "C" fn()),
+    sys_setmoduleoffset_orig: extern "C" fn(*const c_char, unsafe extern "C" fn()),
     #[cfg_attr(test, allow(dead_code))]
-    sv_spawnserver_orig: fn(*const c_char, qboolean),
-    cmd_executestring_orig: fn(*const c_char),
-    cmd_argc_orig: fn() -> c_int,
+    sv_spawnserver_orig: extern "C" fn(*const c_char, qboolean),
+    cmd_executestring_orig: extern "C" fn(*const c_char),
+    cmd_argc_orig: extern "C" fn() -> c_int,
 }
 
 #[derive(Debug)]
 struct StaticDetours {
-    cmd_addcommand_detour: GenericDetour<fn(*const c_char, unsafe extern "C" fn())>,
-    sys_setmoduleoffset_detour: GenericDetour<fn(*const c_char, unsafe extern "C" fn())>,
-    sv_executeclientcommand_detour: GenericDetour<fn(*mut client_t, *const c_char, qboolean)>,
-    sv_cliententerworld_detour: GenericDetour<fn(*mut client_t, *mut usercmd_t)>,
-    sv_setconfgistring_detour: GenericDetour<fn(c_int, *const c_char)>,
+    cmd_addcommand_detour: GenericDetour<extern "C" fn(*const c_char, unsafe extern "C" fn())>,
+    sys_setmoduleoffset_detour: GenericDetour<extern "C" fn(*const c_char, unsafe extern "C" fn())>,
+    sv_executeclientcommand_detour:
+        GenericDetour<extern "C" fn(*mut client_t, *const c_char, qboolean)>,
+    sv_cliententerworld_detour: GenericDetour<extern "C" fn(*mut client_t, *mut usercmd_t)>,
+    sv_setconfgistring_detour: GenericDetour<extern "C" fn(c_int, *const c_char)>,
     #[cfg_attr(test, allow(dead_code))]
-    sv_dropclient_detour: GenericDetour<fn(*mut client_t, *const c_char)>,
-    sv_spawnserver_detour: GenericDetour<fn(*const c_char, qboolean)>,
+    sv_dropclient_detour: GenericDetour<extern "C" fn(*mut client_t, *const c_char)>,
+    sv_spawnserver_detour: GenericDetour<extern "C" fn(*const c_char, qboolean)>,
     sv_sendservercommand_detour: RawDetour,
     com_printf_detour: RawDetour,
 }
 
-type ClientSpawnDetourType = GenericDetour<fn(*mut gentity_t)>;
-type ClientConnectDetourType = GenericDetour<fn(c_int, qboolean, qboolean) -> *const c_char>;
-type GStartKamikazeDetourType = GenericDetour<fn(*mut gentity_t)>;
+type ClientSpawnDetourType = GenericDetour<extern "C" fn(*mut gentity_t)>;
+type ClientConnectDetourType =
+    GenericDetour<extern "C" fn(c_int, qboolean, qboolean) -> *const c_char>;
+type GStartKamikazeDetourType = GenericDetour<extern "C" fn(*mut gentity_t)>;
 type GDamageDetourType = GenericDetour<
-    fn(
+    extern "C" fn(
         *mut gentity_t,
         *mut gentity_t,
         *mut gentity_t,
         *mut vec3_t,
         *mut vec3_t,
         c_int,
         c_int,
@@ -167,26 +174,26 @@
     #[cfg_attr(test, allow(dead_code))]
     pub(crate) fn try_initialize_from(
         &self,
         #[allow(unused_variables)] module_offset: usize,
     ) -> Result<(), QuakeLiveEngineError> {
         #[cfg(not(target_os = "linux"))]
         return Err(QuakeLiveEngineError::ProcessNotFound(
-            "could not find my own process\n".into(),
+            "could not find my own process\n".to_string(),
         ));
         #[cfg(target_os = "linux")]
         {
             let Ok(myself_process) = Process::myself() else {
                 return Err(QuakeLiveEngineError::ProcessNotFound(
-                    "could not find my own process\n".into(),
+                    "could not find my own process\n".to_string(),
                 ));
             };
             let Ok(myself_maps) = myself_process.maps() else {
                 return Err(QuakeLiveEngineError::NoMemoryMappingInformationFound(
-                    "no memory mapping information found\n".into(),
+                    "no memory mapping information found\n".to_string(),
                 ));
             };
             let qagame_maps: Vec<&MemoryMap> = myself_maps
                 .iter()
                 .filter(|mmap| {
                     let MMapPath::Path(path) = &mmap.pathname else {
                         return false;
@@ -300,57 +307,78 @@
         }
 
         unsafe {
             ptr::write(vm_call_table as *mut usize, shinqlx_g_shutdowngame as usize);
         }
 
         let client_connect_orig = self.client_connect_orig.load(Ordering::SeqCst);
-        let client_connect_func = unsafe { mem::transmute(client_connect_orig) };
+        let client_connect_func = unsafe {
+            mem::transmute::<usize, extern "C" fn(c_int, qboolean, qboolean) -> *const c_char>(
+                client_connect_orig,
+            )
+        };
         let client_connect_detour =
             unsafe { ClientConnectDetourType::new(client_connect_func, shinqlx_client_connect) }
                 .map_err(|_| {
                     QuakeLiveEngineError::DetourCouldNotBeCreated(QuakeLiveFunction::ClientConnect)
                 })?;
         unsafe { client_connect_detour.enable() }.map_err(|_| {
             QuakeLiveEngineError::DetourCouldNotBeEnabled(QuakeLiveFunction::ClientConnect)
         })?;
 
         self.client_connect_detour
             .store(Some(client_connect_detour.into()));
 
         let g_start_kamikaze_orig = self.g_start_kamikaze_orig.load(Ordering::SeqCst);
-        let g_start_kamikaze_func = unsafe { mem::transmute(g_start_kamikaze_orig) };
+        let g_start_kamikaze_func = unsafe {
+            mem::transmute::<usize, extern "C" fn(*mut gentity_s)>(g_start_kamikaze_orig)
+        };
         let g_start_kamikaze_detour = unsafe {
             GStartKamikazeDetourType::new(g_start_kamikaze_func, shinqlx_g_startkamikaze)
         }
         .map_err(|_| {
             QuakeLiveEngineError::DetourCouldNotBeCreated(QuakeLiveFunction::G_StartKamikaze)
         })?;
         unsafe { g_start_kamikaze_detour.enable() }.map_err(|_| {
             QuakeLiveEngineError::DetourCouldNotBeEnabled(QuakeLiveFunction::G_StartKamikaze)
         })?;
 
         self.g_start_kamikaze_detour
             .store(Some(g_start_kamikaze_detour.into()));
 
         let client_spawn_orig = self.client_spawn_orig.load(Ordering::SeqCst);
-        let client_spawn_func = unsafe { mem::transmute(client_spawn_orig) };
+        let client_spawn_func =
+            unsafe { mem::transmute::<usize, extern "C" fn(*mut gentity_s)>(client_spawn_orig) };
         let client_spawn_detour =
             unsafe { ClientSpawnDetourType::new(client_spawn_func, shinqlx_clientspawn) }.map_err(
                 |_| QuakeLiveEngineError::DetourCouldNotBeCreated(QuakeLiveFunction::ClientSpawn),
             )?;
         unsafe { client_spawn_detour.enable() }.map_err(|_| {
             QuakeLiveEngineError::DetourCouldNotBeEnabled(QuakeLiveFunction::ClientSpawn)
         })?;
 
         self.client_spawn_detour
             .store(Some(client_spawn_detour.into()));
 
         let g_damage_orig = self.g_damage_orig.load(Ordering::SeqCst);
-        let g_damage_func = unsafe { mem::transmute(g_damage_orig) };
+        let g_damage_func = unsafe {
+            mem::transmute::<
+                usize,
+                extern "C" fn(
+                    *mut gentity_t,
+                    *mut gentity_t,
+                    *mut gentity_t,
+                    *mut vec3_t,
+                    *mut vec3_t,
+                    c_int,
+                    c_int,
+                    c_int,
+                ),
+            >(g_damage_orig)
+        };
         let g_damage_detour = unsafe { GDamageDetourType::new(g_damage_func, shinqlx_g_damage) }
             .map_err(|_| {
                 QuakeLiveEngineError::DetourCouldNotBeCreated(QuakeLiveFunction::G_Damage)
             })?;
         unsafe { g_damage_detour.enable() }.map_err(|_| {
             QuakeLiveEngineError::DetourCouldNotBeEnabled(QuakeLiveFunction::G_Damage)
         })?;
@@ -489,26 +517,26 @@
         }
     }
 
     #[cfg_attr(test, allow(dead_code))]
     pub(crate) fn search_static_functions(&self) -> Result<(), QuakeLiveEngineError> {
         #[cfg(not(target_os = "linux"))]
         return Err(QuakeLiveEngineError::ProcessNotFound(
-            "could not find my own process\n".into(),
+            "could not find my own process\n".to_string(),
         ));
         #[cfg(target_os = "linux")]
         {
             let Ok(myself_process) = Process::myself() else {
                 return Err(QuakeLiveEngineError::ProcessNotFound(
-                    "could not find my own process\n".into(),
+                    "could not find my own process\n".to_string(),
                 ));
             };
             let Ok(myself_maps) = myself_process.maps() else {
                 return Err(QuakeLiveEngineError::NoMemoryMappingInformationFound(
-                    "no memory mapping information found\n".into(),
+                    "no memory mapping information found\n".to_string(),
                 ));
             };
             let qzeroded_maps: Vec<&MemoryMap> = myself_maps
                 .iter()
                 .filter(|mmap| {
                     let MMapPath::Path(path) = &mmap.pathname else {
                         return false;
@@ -517,129 +545,162 @@
                         .is_some_and(|file_name| file_name.to_string_lossy() == QZERODED)
                 })
                 .collect();
 
             if qzeroded_maps.is_empty() {
                 error!(target: "shinqlx", "no memory mapping information for {} found", QZERODED);
                 return Err(QuakeLiveEngineError::NoMemoryMappingInformationFound(
-                    "no memory mapping information found\n".into(),
+                    "no memory mapping information found\n".to_string(),
                 ));
             }
 
             debug!(target: "shinqlx", "Searching for necessary functions...");
             let Some(result) = pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Com_Printf)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::Com_Printf);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Com_Printf,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Com_Printf, result);
-            let com_printf_orig = unsafe { mem::transmute(result) };
+            let com_printf_orig =
+                unsafe { mem::transmute::<usize, extern "C" fn(*const c_char, ...)>(result) };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Cmd_AddCommand)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::Cmd_AddCommand);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Cmd_AddCommand,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Cmd_AddCommand, result);
-            let cmd_addcommand_orig = unsafe { mem::transmute(result) };
+            let cmd_addcommand_orig = unsafe {
+                mem::transmute::<usize, extern "C" fn(*const c_char, unsafe extern "C" fn())>(
+                    result,
+                )
+            };
 
             let Some(result) = pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Cmd_Args)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::Cmd_Args);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Cmd_Args,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Cmd_Args, result);
-            let cmd_args_orig = unsafe { mem::transmute(result) };
+            let cmd_args_orig =
+                unsafe { mem::transmute::<usize, extern "C" fn() -> *const c_char>(result) };
 
             let Some(result) = pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Cmd_Argv)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::Cmd_Argv);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Cmd_Argv,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Cmd_Argv, result);
-            let cmd_argv_orig = unsafe { mem::transmute(result) };
+            let cmd_argv_orig =
+                unsafe { mem::transmute::<usize, extern "C" fn(c_int) -> *const c_char>(result) };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Cmd_Tokenizestring)
             else {
                 error!(target: "shinqlx",
                     "Function {} not found",
                     &QuakeLiveFunction::Cmd_Tokenizestring
                 );
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Cmd_Tokenizestring,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Cmd_Tokenizestring, result);
-            let cmd_tokenizestring_orig = unsafe { mem::transmute(result) };
+            let cmd_tokenizestring_orig =
+                unsafe { mem::transmute::<usize, extern "C" fn(*const c_char)>(result) };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Cbuf_ExecuteText)
             else {
                 error!(target: "shinqlx",
                     "Function {} not found",
                     &QuakeLiveFunction::Cbuf_ExecuteText
                 );
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Cbuf_ExecuteText,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Cbuf_ExecuteText, result);
-            let cbuf_executetext_orig = unsafe { mem::transmute(result) };
+            let cbuf_executetext_orig = unsafe {
+                mem::transmute::<usize, extern "C" fn(cbufExec_t, *const c_char)>(result)
+            };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Cvar_FindVar)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::Cvar_FindVar);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Cvar_FindVar,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Cvar_FindVar, result);
-            let cvar_findvar_orig = unsafe { mem::transmute(result) };
+            let cvar_findvar_orig = unsafe {
+                mem::transmute::<usize, extern "C" fn(*const c_char) -> *mut cvar_t>(result)
+            };
 
             let Some(result) = pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Cvar_Get)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::Cvar_Get);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Cvar_Get,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Cvar_Get, result);
-            let cvar_get_orig = unsafe { mem::transmute(result) };
+            let cvar_get_orig = unsafe {
+                mem::transmute::<
+                    usize,
+                    extern "C" fn(*const c_char, *const c_char, c_int) -> *mut cvar_t,
+                >(result)
+            };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Cvar_GetLimit)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::Cvar_GetLimit);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Cvar_GetLimit,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Cvar_GetLimit, result);
-            let cvar_getlimit_orig = unsafe { mem::transmute(result) };
+            let cvar_getlimit_orig = unsafe {
+                mem::transmute::<
+                    usize,
+                    extern "C" fn(
+                        *const c_char,
+                        *const c_char,
+                        *const c_char,
+                        *const c_char,
+                        c_int,
+                    ) -> *mut cvar_t,
+                >(result)
+            };
 
             let Some(result) = pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Cvar_Set2)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::Cvar_Set2);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Cvar_Set2,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Cvar_Set2, result);
-            let cvar_set2_orig = unsafe { mem::transmute(result) };
+            let cvar_set2_orig = unsafe {
+                mem::transmute::<
+                    usize,
+                    extern "C" fn(*const c_char, *const c_char, qboolean) -> *mut cvar_t,
+                >(result)
+            };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::SV_SendServerCommand)
             else {
                 error!(target: "shinqlx",
                     "Function {} not found",
                     &QuakeLiveFunction::SV_SendServerCommand
@@ -649,15 +710,17 @@
                 ));
             };
             debug!(target: "shinqlx",
                 "{}: {:#X}",
                 &QuakeLiveFunction::SV_SendServerCommand,
                 result
             );
-            let sv_sendservercommand_orig = unsafe { mem::transmute(result) };
+            let sv_sendservercommand_orig = unsafe {
+                mem::transmute::<usize, extern "C" fn(*mut client_t, *const c_char, ...)>(result)
+            };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::SV_ExecuteClientCommand)
             else {
                 error!(target: "shinqlx",
                     "Function {} not found",
                     &QuakeLiveFunction::SV_ExecuteClientCommand
@@ -667,139 +730,158 @@
                 ));
             };
             debug!(target: "shinqlx",
                 "{}: {:#X}",
                 &QuakeLiveFunction::SV_ExecuteClientCommand,
                 result
             );
-            let sv_executeclientcommand_orig = unsafe { mem::transmute(result) };
+            let sv_executeclientcommand_orig = unsafe {
+                mem::transmute::<usize, extern "C" fn(*mut client_t, *const c_char, qboolean)>(
+                    result,
+                )
+            };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::SV_Shutdown)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::SV_Shutdown);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::SV_Shutdown,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::SV_Shutdown, result);
-            let sv_shutdown_orig = unsafe { mem::transmute(result) };
+            let sv_shutdown_orig =
+                unsafe { mem::transmute::<usize, extern "C" fn(*const c_char)>(result) };
 
             let Some(result) = pattern_search_module(&qzeroded_maps, QuakeLiveFunction::SV_Map_f)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::SV_Map_f);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::SV_Map_f,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", QuakeLiveFunction::SV_Map_f, result);
-            let sv_map_f_orig = unsafe { mem::transmute(result) };
+            let sv_map_f_orig = unsafe { mem::transmute::<usize, extern "C" fn()>(result) };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::SV_ClientEnterWorld)
             else {
                 error!(target: "shinqlx",
                     "Function {} not found",
                     &QuakeLiveFunction::SV_ClientEnterWorld
                 );
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::SV_ClientEnterWorld,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::SV_ClientEnterWorld, result);
-            let sv_cliententerworld_orig = unsafe { mem::transmute(result) };
+            let sv_cliententerworld_orig = unsafe {
+                mem::transmute::<usize, extern "C" fn(*mut client_t, *mut usercmd_t)>(result)
+            };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::SV_SetConfigstring)
             else {
                 error!(target: "shinqlx",
                     "Function {} not found",
                     &QuakeLiveFunction::SV_SetConfigstring
                 );
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::SV_SetConfigstring,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::SV_SetConfigstring, result);
-            let sv_setconfigstring_orig = unsafe { mem::transmute(result) };
+            let sv_setconfigstring_orig =
+                unsafe { mem::transmute::<usize, extern "C" fn(c_int, *const c_char)>(result) };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::SV_GetConfigstring)
             else {
                 error!(target: "shinqlx",
                     "Function {} not found",
                     &QuakeLiveFunction::SV_GetConfigstring
                 );
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::SV_GetConfigstring,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::SV_GetConfigstring, result);
-            let sv_getconfigstring_orig = unsafe { mem::transmute(result) };
+            let sv_getconfigstring_orig = unsafe {
+                mem::transmute::<usize, extern "C" fn(c_int, *const c_char, c_int)>(result)
+            };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::SV_DropClient)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::SV_DropClient);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::SV_DropClient,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::SV_DropClient, result);
-            let sv_dropclient_orig = unsafe { mem::transmute(result) };
+            let sv_dropclient_orig = unsafe {
+                mem::transmute::<usize, extern "C" fn(*mut client_t, *const c_char)>(result)
+            };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Sys_SetModuleOffset)
             else {
                 error!(target: "shinqlx",
                     "Function {} not found",
                     &QuakeLiveFunction::Sys_SetModuleOffset
                 );
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Sys_SetModuleOffset,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Sys_SetModuleOffset, result);
-            let sys_setmoduleoffset_orig = unsafe { mem::transmute(result) };
+            let sys_setmoduleoffset_orig = unsafe {
+                mem::transmute::<usize, extern "C" fn(*const c_char, unsafe extern "C" fn())>(
+                    result,
+                )
+            };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::SV_SpawnServer)
             else {
                 error!(target: "shinqlx", "Function {} not found", &QuakeLiveFunction::SV_SpawnServer);
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::SV_SpawnServer,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::SV_SpawnServer, result);
-            let sv_spawnserver_orig = unsafe { mem::transmute(result) };
+            let sv_spawnserver_orig =
+                unsafe { mem::transmute::<usize, extern "C" fn(*const c_char, qboolean)>(result) };
 
             let Some(result) =
                 pattern_search_module(&qzeroded_maps, QuakeLiveFunction::Cmd_ExecuteString)
             else {
                 error!(target: "shinqlx",
                     "Function {} not found",
                     &QuakeLiveFunction::Cmd_ExecuteString
                 );
                 return Err(QuakeLiveEngineError::StaticFunctionNotFound(
                     QuakeLiveFunction::Cmd_ExecuteString,
                 ));
             };
             debug!(target: "shinqlx", "{}: {:#X}", &QuakeLiveFunction::Cmd_ExecuteString, result);
-            let cmd_executestring_orig = unsafe { mem::transmute(result) };
+            let cmd_executestring_orig =
+                unsafe { mem::transmute::<usize, extern "C" fn(*const c_char)>(result) };
 
             // Cmd_Argc is really small, making it hard to search for, so we use a reference to it instead.
             let base_address = unsafe {
                 ptr::read_unaligned(
                     (sv_map_f_orig as usize + OFFSET_CMD_ARGC as usize) as *const i32,
                 )
             };
             #[allow(clippy::fn_to_numeric_cast_with_truncation)]
             let cmd_argc_ptr = base_address + sv_map_f_orig as i32 + OFFSET_CMD_ARGC + 4;
             debug!(target: "shinqlx", "{}: {:#X}", QuakeLiveFunction::Cmd_Argc, cmd_argc_ptr);
-            let cmd_argc_orig = unsafe { mem::transmute(cmd_argc_ptr as u64) };
+            let cmd_argc_orig =
+                unsafe { mem::transmute::<usize, extern "C" fn() -> c_int>(cmd_argc_ptr as usize) };
 
             self.static_functions
                 .set(StaticFunctions {
                     com_printf_orig,
                     cmd_addcommand_orig,
                     cmd_args_orig,
                     cmd_argv_orig,
@@ -934,15 +1016,15 @@
         if sv_tags_string.split(',').any(|x| x == SV_TAGS_PREFIX) {
             return;
         }
 
         let new_tags = if sv_tags_string.len() > 2 {
             format!("{},{}", SV_TAGS_PREFIX, sv_tags_string)
         } else {
-            SV_TAGS_PREFIX.into()
+            SV_TAGS_PREFIX.to_string()
         };
         self.set_cvar_forced("sv_tags", new_tags, false);
     }
 
     // Called after the game is initialized.
     #[cfg_attr(test, allow(dead_code))]
     pub(crate) fn initialize_cvars(&self) {
@@ -1007,453 +1089,507 @@
         if !restart {
             self.vm_functions.unhook();
         }
     }
 
     #[cfg_attr(test, allow(dead_code))]
     fn com_printf_orig(&self) -> Result<extern "C" fn(*const c_char, ...), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Com_Printf,
-            ));
-        };
-        Ok(static_functions.com_printf_orig)
+            )),
+            |static_functions| Ok(static_functions.com_printf_orig),
+        )
     }
 
     #[cfg_attr(test, allow(dead_code))]
     fn cmd_addcommand_orig(
         &self,
-    ) -> Result<fn(*const c_char, unsafe extern "C" fn()), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    ) -> Result<extern "C" fn(*const c_char, unsafe extern "C" fn()), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cmd_AddCommand,
-            ));
-        };
-        Ok(static_functions.cmd_addcommand_orig)
+            )),
+            |static_functions| Ok(static_functions.cmd_addcommand_orig),
+        )
     }
 
-    fn cmd_args_orig(&self) -> Result<fn() -> *const c_char, QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn cmd_args_orig(&self) -> Result<extern "C" fn() -> *const c_char, QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cmd_Args,
-            ));
-        };
-        Ok(static_functions.cmd_args_orig)
+            )),
+            |static_functions| Ok(static_functions.cmd_args_orig),
+        )
     }
 
-    fn cmd_argv_orig(&self) -> Result<fn(c_int) -> *const c_char, QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn cmd_argv_orig(&self) -> Result<extern "C" fn(c_int) -> *const c_char, QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cmd_Argv,
-            ));
-        };
-        Ok(static_functions.cmd_argv_orig)
+            )),
+            |static_functions| Ok(static_functions.cmd_argv_orig),
+        )
     }
 
     #[allow(dead_code)]
-    fn cmd_tokenizestring_orig(&self) -> Result<fn(*const c_char), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn cmd_tokenizestring_orig(
+        &self,
+    ) -> Result<extern "C" fn(*const c_char), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cmd_Tokenizestring,
-            ));
-        };
-        Ok(static_functions.cmd_tokenizestring_orig)
+            )),
+            |static_functions| Ok(static_functions.cmd_tokenizestring_orig),
+        )
     }
 
     #[allow(dead_code)]
-    fn cbuf_executetext_orig(&self) -> Result<fn(cbufExec_t, *const c_char), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn cbuf_executetext_orig(
+        &self,
+    ) -> Result<extern "C" fn(cbufExec_t, *const c_char), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cbuf_ExecuteText,
-            ));
-        };
-        Ok(static_functions.cbuf_executetext_orig)
+            )),
+            |static_functions| Ok(static_functions.cbuf_executetext_orig),
+        )
     }
 
-    fn cvar_findvar_orig(&self) -> Result<fn(*const c_char) -> *mut cvar_t, QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn cvar_findvar_orig(
+        &self,
+    ) -> Result<extern "C" fn(*const c_char) -> *mut cvar_t, QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cvar_FindVar,
-            ));
-        };
-        Ok(static_functions.cvar_findvar_orig)
+            )),
+            |static_functions| Ok(static_functions.cvar_findvar_orig),
+        )
     }
 
     #[allow(clippy::type_complexity)]
     fn cvar_get_orig(
         &self,
-    ) -> Result<fn(*const c_char, *const c_char, c_int) -> *mut cvar_t, QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    ) -> Result<
+        extern "C" fn(*const c_char, *const c_char, c_int) -> *mut cvar_t,
+        QuakeLiveEngineError,
+    > {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cvar_Get,
-            ));
-        };
-        Ok(static_functions.cvar_get_orig)
+            )),
+            |static_functions| Ok(static_functions.cvar_get_orig),
+        )
     }
 
     #[allow(clippy::type_complexity)]
     fn cvar_getlimit_orig(
         &self,
     ) -> Result<
-        fn(*const c_char, *const c_char, *const c_char, *const c_char, c_int) -> *mut cvar_t,
+        extern "C" fn(
+            *const c_char,
+            *const c_char,
+            *const c_char,
+            *const c_char,
+            c_int,
+        ) -> *mut cvar_t,
         QuakeLiveEngineError,
     > {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cvar_GetLimit,
-            ));
-        };
-        Ok(static_functions.cvar_getlimit_orig)
+            )),
+            |static_functions| Ok(static_functions.cvar_getlimit_orig),
+        )
     }
 
     #[allow(clippy::type_complexity)]
     fn cvar_set2_orig(
         &self,
-    ) -> Result<fn(*const c_char, *const c_char, qboolean) -> *mut cvar_t, QuakeLiveEngineError>
-    {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    ) -> Result<
+        extern "C" fn(*const c_char, *const c_char, qboolean) -> *mut cvar_t,
+        QuakeLiveEngineError,
+    > {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cvar_Set2,
-            ));
-        };
-        Ok(static_functions.cvar_set2_orig)
+            )),
+            |static_functions| Ok(static_functions.cvar_set2_orig),
+        )
     }
 
     #[cfg_attr(test, allow(dead_code))]
     fn sv_sendservercommand_orig(
         &self,
     ) -> Result<extern "C" fn(*mut client_t, *const c_char, ...), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::SV_SendServerCommand,
-            ));
-        };
-        Ok(static_functions.sv_sendservercommand_orig)
+            )),
+            |static_functions| Ok(static_functions.sv_sendservercommand_orig),
+        )
     }
 
     #[cfg_attr(test, allow(dead_code))]
     fn sv_executeclientcommand_orig(
         &self,
-    ) -> Result<fn(*mut client_t, *const c_char, qboolean), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    ) -> Result<extern "C" fn(*mut client_t, *const c_char, qboolean), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::SV_ExecuteClientCommand,
-            ));
-        };
-        Ok(static_functions.sv_executeclientcommand_orig)
+            )),
+            |static_functions| Ok(static_functions.sv_executeclientcommand_orig),
+        )
     }
 
     #[cfg_attr(test, allow(dead_code))]
-    pub(crate) fn sv_shutdown_orig(&self) -> Result<fn(*const c_char), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    pub(crate) fn sv_shutdown_orig(
+        &self,
+    ) -> Result<extern "C" fn(*const c_char), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::SV_Shutdown,
-            ));
-        };
-        Ok(static_functions.sv_shutdown_orig)
+            )),
+            |static_functions| Ok(static_functions.sv_shutdown_orig),
+        )
     }
 
     #[allow(dead_code)]
-    fn sv_map_f_orig(&self) -> Result<fn(), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn sv_map_f_orig(&self) -> Result<extern "C" fn(), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::SV_Map_f,
-            ));
-        };
-        Ok(static_functions.sv_map_f_orig)
+            )),
+            |static_functions| Ok(static_functions.sv_map_f_orig),
+        )
     }
 
     #[cfg_attr(test, allow(dead_code))]
     fn sv_cliententerworld_orig(
         &self,
-    ) -> Result<fn(*mut client_t, *mut usercmd_t), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    ) -> Result<extern "C" fn(*mut client_t, *mut usercmd_t), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::SV_ClientEnterWorld,
-            ));
-        };
-        Ok(static_functions.sv_cliententerworld_orig)
+            )),
+            |static_functions| Ok(static_functions.sv_cliententerworld_orig),
+        )
     }
 
     #[cfg_attr(test, allow(dead_code))]
-    fn sv_setconfigstring_orig(&self) -> Result<fn(c_int, *const c_char), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn sv_setconfigstring_orig(
+        &self,
+    ) -> Result<extern "C" fn(c_int, *const c_char), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::SV_SetConfigstring,
-            ));
-        };
-        Ok(static_functions.sv_setconfigstring_orig)
+            )),
+            |static_functions| Ok(static_functions.sv_setconfigstring_orig),
+        )
     }
 
     fn sv_getconfigstring_orig(
         &self,
-    ) -> Result<fn(c_int, *const c_char, c_int), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    ) -> Result<extern "C" fn(c_int, *const c_char, c_int), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::SV_GetConfigstring,
-            ));
-        };
-        Ok(static_functions.sv_getconfigstring_orig)
+            )),
+            |static_functions| Ok(static_functions.sv_getconfigstring_orig),
+        )
     }
 
     #[cfg_attr(test, allow(dead_code))]
-    fn sv_dropclient_orig(&self) -> Result<fn(*mut client_t, *const c_char), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn sv_dropclient_orig(
+        &self,
+    ) -> Result<extern "C" fn(*mut client_t, *const c_char), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::SV_DropClient,
-            ));
-        };
-        Ok(static_functions.sv_dropclient_orig)
+            )),
+            |static_functions| Ok(static_functions.sv_dropclient_orig),
+        )
     }
 
     #[cfg_attr(test, allow(dead_code))]
     fn sys_setmoduleoffset_orig(
         &self,
-    ) -> Result<fn(*const c_char, unsafe extern "C" fn()), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    ) -> Result<extern "C" fn(*const c_char, unsafe extern "C" fn()), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Sys_SetModuleOffset,
-            ));
-        };
-        Ok(static_functions.sys_setmoduleoffset_orig)
+            )),
+            |static_functions| Ok(static_functions.sys_setmoduleoffset_orig),
+        )
     }
 
     #[cfg_attr(test, allow(dead_code))]
-    fn sv_spawnserver_orig(&self) -> Result<fn(*const c_char, qboolean), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn sv_spawnserver_orig(
+        &self,
+    ) -> Result<extern "C" fn(*const c_char, qboolean), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::SV_SpawnServer,
-            ));
-        };
-        Ok(static_functions.sv_spawnserver_orig)
+            )),
+            |static_functions| Ok(static_functions.sv_spawnserver_orig),
+        )
     }
 
-    fn cmd_executestring_orig(&self) -> Result<fn(*const c_char), QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn cmd_executestring_orig(&self) -> Result<extern "C" fn(*const c_char), QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cmd_ExecuteString,
-            ));
-        };
-        Ok(static_functions.cmd_executestring_orig)
+            )),
+            |static_functions| Ok(static_functions.cmd_executestring_orig),
+        )
     }
 
-    fn cmd_argc_orig(&self) -> Result<fn() -> c_int, QuakeLiveEngineError> {
-        let Some(static_functions) = self.static_functions.get() else {
-            return Err(QuakeLiveEngineError::StaticFunctionNotFound(
+    fn cmd_argc_orig(&self) -> Result<extern "C" fn() -> c_int, QuakeLiveEngineError> {
+        self.static_functions.get().map_or(
+            Err(QuakeLiveEngineError::StaticFunctionNotFound(
                 QuakeLiveFunction::Cmd_Argc,
-            ));
-        };
-        Ok(static_functions.cmd_argc_orig)
+            )),
+            |static_functions| Ok(static_functions.cmd_argc_orig),
+        )
     }
 
     fn cmd_addcommand_detour(
         &self,
-    ) -> Result<&GenericDetour<fn(*const c_char, unsafe extern "C" fn())>, QuakeLiveEngineError>
-    {
-        let Some(static_detours) = self.static_detours.get() else {
-            return Err(QuakeLiveEngineError::StaticDetourNotFound(
+    ) -> Result<
+        &GenericDetour<extern "C" fn(*const c_char, unsafe extern "C" fn())>,
+        QuakeLiveEngineError,
+    > {
+        self.static_detours.get().map_or(
+            Err(QuakeLiveEngineError::StaticDetourNotFound(
                 QuakeLiveFunction::Cmd_AddCommand,
-            ));
-        };
-        Ok(&static_detours.cmd_addcommand_detour)
+            )),
+            |static_detours| Ok(&static_detours.cmd_addcommand_detour),
+        )
     }
 
     fn sys_setmoduleoffset_detour(
         &self,
-    ) -> Result<&GenericDetour<fn(*const c_char, unsafe extern "C" fn())>, QuakeLiveEngineError>
-    {
-        let Some(static_detours) = self.static_detours.get() else {
-            return Err(QuakeLiveEngineError::StaticDetourNotFound(
+    ) -> Result<
+        &GenericDetour<extern "C" fn(*const c_char, unsafe extern "C" fn())>,
+        QuakeLiveEngineError,
+    > {
+        self.static_detours.get().map_or(
+            Err(QuakeLiveEngineError::StaticDetourNotFound(
                 QuakeLiveFunction::Sys_SetModuleOffset,
-            ));
-        };
-        Ok(&static_detours.sys_setmoduleoffset_detour)
+            )),
+            |static_detours| Ok(&static_detours.sys_setmoduleoffset_detour),
+        )
     }
 
     #[allow(clippy::type_complexity)]
     fn sv_executeclientcommand_detour(
         &self,
-    ) -> Result<&GenericDetour<fn(*mut client_t, *const c_char, qboolean)>, QuakeLiveEngineError>
-    {
-        let Some(static_detours) = self.static_detours.get() else {
-            return Err(QuakeLiveEngineError::StaticDetourNotFound(
+    ) -> Result<
+        &GenericDetour<extern "C" fn(*mut client_t, *const c_char, qboolean)>,
+        QuakeLiveEngineError,
+    > {
+        self.static_detours.get().map_or(
+            Err(QuakeLiveEngineError::StaticDetourNotFound(
                 QuakeLiveFunction::SV_ExecuteClientCommand,
-            ));
-        };
-        Ok(&static_detours.sv_executeclientcommand_detour)
+            )),
+            |static_detours| Ok(&static_detours.sv_executeclientcommand_detour),
+        )
     }
 
     #[allow(clippy::type_complexity)]
     fn sv_cliententerworld_detour(
         &self,
-    ) -> Result<&GenericDetour<fn(*mut client_t, *mut usercmd_t)>, QuakeLiveEngineError> {
-        let Some(static_detours) = self.static_detours.get() else {
-            return Err(QuakeLiveEngineError::StaticDetourNotFound(
+    ) -> Result<&GenericDetour<extern "C" fn(*mut client_t, *mut usercmd_t)>, QuakeLiveEngineError>
+    {
+        self.static_detours.get().map_or(
+            Err(QuakeLiveEngineError::StaticDetourNotFound(
                 QuakeLiveFunction::SV_ClientEnterWorld,
-            ));
-        };
-        Ok(&static_detours.sv_cliententerworld_detour)
+            )),
+            |static_detours| Ok(&static_detours.sv_cliententerworld_detour),
+        )
     }
 
     #[allow(clippy::type_complexity)]
     fn sv_setconfgistring_detour(
         &self,
-    ) -> Result<&GenericDetour<fn(c_int, *const c_char)>, QuakeLiveEngineError> {
-        let Some(static_detours) = self.static_detours.get() else {
-            return Err(QuakeLiveEngineError::StaticDetourNotFound(
+    ) -> Result<&GenericDetour<extern "C" fn(c_int, *const c_char)>, QuakeLiveEngineError> {
+        self.static_detours.get().map_or(
+            Err(QuakeLiveEngineError::StaticDetourNotFound(
                 QuakeLiveFunction::SV_SetConfigstring,
-            ));
-        };
-        Ok(&static_detours.sv_setconfgistring_detour)
+            )),
+            |static_detours| Ok(&static_detours.sv_setconfgistring_detour),
+        )
     }
 
     #[cfg_attr(test, allow(dead_code))]
     #[allow(clippy::type_complexity)]
     pub(crate) fn sv_dropclient_detour(
         &self,
-    ) -> Result<&GenericDetour<fn(*mut client_t, *const c_char)>, QuakeLiveEngineError> {
-        let Some(static_detours) = self.static_detours.get() else {
-            return Err(QuakeLiveEngineError::StaticDetourNotFound(
+    ) -> Result<&GenericDetour<extern "C" fn(*mut client_t, *const c_char)>, QuakeLiveEngineError>
+    {
+        self.static_detours.get().map_or(
+            Err(QuakeLiveEngineError::StaticDetourNotFound(
                 QuakeLiveFunction::SV_DropClient,
-            ));
-        };
-        Ok(&static_detours.sv_dropclient_detour)
+            )),
+            |static_detours| Ok(&static_detours.sv_dropclient_detour),
+        )
     }
 
     #[allow(clippy::type_complexity)]
     fn sv_spawnserver_detour(
         &self,
-    ) -> Result<&GenericDetour<fn(*const c_char, qboolean)>, QuakeLiveEngineError> {
-        let Some(static_detours) = self.static_detours.get() else {
-            return Err(QuakeLiveEngineError::StaticDetourNotFound(
+    ) -> Result<&GenericDetour<extern "C" fn(*const c_char, qboolean)>, QuakeLiveEngineError> {
+        self.static_detours.get().map_or(
+            Err(QuakeLiveEngineError::StaticDetourNotFound(
                 QuakeLiveFunction::SV_SpawnServer,
-            ));
-        };
-        Ok(&static_detours.sv_spawnserver_detour)
+            )),
+            |static_detours| Ok(&static_detours.sv_spawnserver_detour),
+        )
     }
 
     fn sv_sendservercommand_detour(&self) -> Result<&RawDetour, QuakeLiveEngineError> {
-        let Some(static_detours) = self.static_detours.get() else {
-            return Err(QuakeLiveEngineError::StaticDetourNotFound(
+        self.static_detours.get().map_or(
+            Err(QuakeLiveEngineError::StaticDetourNotFound(
                 QuakeLiveFunction::SV_SendServerCommand,
-            ));
-        };
-        Ok(&static_detours.sv_sendservercommand_detour)
+            )),
+            |static_detours| Ok(&static_detours.sv_sendservercommand_detour),
+        )
     }
 
     fn com_printf_detour(&self) -> Result<&RawDetour, QuakeLiveEngineError> {
-        let Some(static_detours) = self.static_detours.get() else {
-            return Err(QuakeLiveEngineError::StaticDetourNotFound(
+        self.static_detours.get().map_or(
+            Err(QuakeLiveEngineError::StaticDetourNotFound(
                 QuakeLiveFunction::Com_Printf,
-            ));
-        };
-        Ok(&static_detours.com_printf_detour)
+            )),
+            |static_detours| Ok(&static_detours.com_printf_detour),
+        )
     }
 
     pub(crate) fn g_init_game_orig(
         &self,
     ) -> Result<extern "C" fn(c_int, c_int, c_int), QuakeLiveEngineError> {
-        let g_init_game_orig = self.vm_functions.g_init_game_orig.load(Ordering::SeqCst);
-        if g_init_game_orig == 0 {
-            return Err(QuakeLiveEngineError::VmFunctionNotFound(
+        match self.vm_functions.g_init_game_orig.load(Ordering::SeqCst) {
+            0 => Err(QuakeLiveEngineError::VmFunctionNotFound(
                 QuakeLiveFunction::G_InitGame,
-            ));
+            )),
+            g_init_game_orig => {
+                let g_init_game_func = unsafe {
+                    mem::transmute::<usize, extern "C" fn(c_int, c_int, c_int)>(g_init_game_orig)
+                };
+                Ok(g_init_game_func)
+            }
         }
-
-        let g_init_game_func = unsafe { mem::transmute(g_init_game_orig) };
-        Ok(g_init_game_func)
     }
 
     fn g_shutdown_game_orig(&self) -> Result<extern "C" fn(c_int), QuakeLiveEngineError> {
-        let g_shutdown_game_orig = self
+        match self
             .vm_functions
             .g_shutdown_game_orig
-            .load(Ordering::SeqCst);
-        if g_shutdown_game_orig == 0 {
-            return Err(QuakeLiveEngineError::VmFunctionNotFound(
+            .load(Ordering::SeqCst)
+        {
+            0 => Err(QuakeLiveEngineError::VmFunctionNotFound(
                 QuakeLiveFunction::G_ShutdownGame,
-            ));
+            )),
+            g_shutdown_game_orig => {
+                let g_shutdown_game_func =
+                    unsafe { mem::transmute::<usize, extern "C" fn(c_int)>(g_shutdown_game_orig) };
+                Ok(g_shutdown_game_func)
+            }
         }
-
-        let g_shutdown_game_func = unsafe { mem::transmute(g_shutdown_game_orig) };
-        Ok(g_shutdown_game_func)
     }
 
     pub(crate) fn g_run_frame_orig(&self) -> Result<extern "C" fn(c_int), QuakeLiveEngineError> {
-        let g_run_frame_orig = self.vm_functions.g_run_frame_orig.load(Ordering::SeqCst);
-        if g_run_frame_orig == 0 {
-            return Err(QuakeLiveEngineError::VmFunctionNotFound(
+        match self.vm_functions.g_run_frame_orig.load(Ordering::SeqCst) {
+            0 => Err(QuakeLiveEngineError::VmFunctionNotFound(
                 QuakeLiveFunction::G_RunFrame,
-            ));
+            )),
+            g_run_frame_orig => {
+                let g_run_frame_func =
+                    unsafe { mem::transmute::<usize, extern "C" fn(c_int)>(g_run_frame_orig) };
+                Ok(g_run_frame_func)
+            }
         }
-
-        let g_run_frame_func = unsafe { mem::transmute(g_run_frame_orig) };
-        Ok(g_run_frame_func)
     }
 
     fn g_addevent_orig(
         &self,
     ) -> Result<extern "C" fn(*mut gentity_t, entity_event_t, c_int), QuakeLiveEngineError> {
-        let g_addevent_orig = self.vm_functions.g_addevent_orig.load(Ordering::SeqCst);
-        if g_addevent_orig == 0 {
-            return Err(QuakeLiveEngineError::VmFunctionNotFound(
+        match self.vm_functions.g_addevent_orig.load(Ordering::SeqCst) {
+            0 => Err(QuakeLiveEngineError::VmFunctionNotFound(
                 QuakeLiveFunction::G_AddEvent,
-            ));
+            )),
+            g_addevent_orig => {
+                let g_addevent_func = unsafe {
+                    mem::transmute::<usize, extern "C" fn(*mut gentity_t, entity_event_t, c_int)>(
+                        g_addevent_orig,
+                    )
+                };
+                Ok(g_addevent_func)
+            }
         }
-
-        let g_addevent_func = unsafe { mem::transmute(g_addevent_orig) };
-        Ok(g_addevent_func)
     }
 
     pub(crate) fn g_free_entity_orig(
         &self,
     ) -> Result<extern "C" fn(*mut gentity_t), QuakeLiveEngineError> {
-        let g_free_entity_orig = self.vm_functions.g_free_entity_orig.load(Ordering::SeqCst);
-        if g_free_entity_orig == 0 {
-            return Err(QuakeLiveEngineError::VmFunctionNotFound(
+        match self.vm_functions.g_free_entity_orig.load(Ordering::SeqCst) {
+            0 => Err(QuakeLiveEngineError::VmFunctionNotFound(
                 QuakeLiveFunction::G_FreeEntity,
-            ));
+            )),
+            g_free_entity_orig => {
+                let g_free_entity_func = unsafe {
+                    mem::transmute::<usize, extern "C" fn(*mut gentity_t)>(g_free_entity_orig)
+                };
+                Ok(g_free_entity_func)
+            }
         }
-
-        let g_free_entity_func = unsafe { mem::transmute(g_free_entity_orig) };
-        Ok(g_free_entity_func)
     }
 
     #[allow(clippy::type_complexity)]
     pub(crate) fn launch_item_orig(
         &self,
     ) -> Result<
         extern "C" fn(*mut gitem_t, &mut vec3_t, &mut vec3_t) -> *mut gentity_t,
         QuakeLiveEngineError,
     > {
-        let launch_item_orig = self.vm_functions.launch_item_orig.load(Ordering::SeqCst);
-        if launch_item_orig == 0 {
-            return Err(QuakeLiveEngineError::VmFunctionNotFound(
+        match self.vm_functions.launch_item_orig.load(Ordering::SeqCst) {
+            0 => Err(QuakeLiveEngineError::VmFunctionNotFound(
                 QuakeLiveFunction::LaunchItem,
-            ));
+            )),
+            launch_item_orig => {
+                let launch_item_func = unsafe {
+                    mem::transmute::<
+                        usize,
+                        extern "C" fn(*mut gitem_t, &mut vec3_t, &mut vec3_t) -> *mut gentity_t,
+                    >(launch_item_orig)
+                };
+                Ok(launch_item_func)
+            }
         }
-
-        let launch_item_func = unsafe { mem::transmute(launch_item_orig) };
-        Ok(launch_item_func)
     }
 
     #[cfg_attr(test, allow(dead_code))]
     pub(crate) fn touch_item_orig(
         &self,
     ) -> Result<extern "C" fn(*mut gentity_t, *mut gentity_t, *mut trace_t), QuakeLiveEngineError>
     {
-        let touch_item_orig = self.vm_functions.touch_item_orig.load(Ordering::SeqCst);
-        if touch_item_orig == 0 {
-            return Err(QuakeLiveEngineError::VmFunctionNotFound(
+        match self.vm_functions.touch_item_orig.load(Ordering::SeqCst) {
+            0 => Err(QuakeLiveEngineError::VmFunctionNotFound(
                 QuakeLiveFunction::Touch_Item,
-            ));
+            )),
+            touch_item_orig => {
+                let touch_item_func = unsafe {
+                    mem::transmute::<
+                        usize,
+                        extern "C" fn(*mut gentity_t, *mut gentity_t, *mut trace_t),
+                    >(touch_item_orig)
+                };
+                Ok(touch_item_func)
+            }
         }
-
-        let touch_item_func = unsafe { mem::transmute(touch_item_orig) };
-        Ok(touch_item_func)
     }
 }
 
 pub(crate) trait FindCVar<T: AsRef<str>> {
     fn find_cvar(&self, name: T) -> Option<CVar>;
 }
 
@@ -1557,24 +1693,24 @@
 impl<T: AsRef<client_t>> SendServerCommand<T> for QuakeLiveEngine {
     fn send_server_command(&self, client: Option<T>, command: &str) {
         let Ok(c_command) = CString::new(command) else {
             return;
         };
 
         self.sv_sendservercommand_detour()
-            .map(|detour| unsafe { mem::transmute(detour.trampoline()) })
+            .map(|detour| unsafe {
+                mem::transmute::<&(), extern "C" fn(*const client_t, *const c_char, ...)>(
+                    detour.trampoline(),
+                )
+            })
             .iter()
-            .for_each(
-                |original_func: &extern "C" fn(*const client_t, *const c_char, ...)| match &client {
-                    Some(ref safe_client) => {
-                        original_func(safe_client.as_ref(), c_command.as_ptr())
-                    }
-                    None => original_func(ptr::null(), c_command.as_ptr()),
-                },
-            );
+            .for_each(|original_func| match &client {
+                Some(ref safe_client) => original_func(safe_client.as_ref(), c_command.as_ptr()),
+                None => original_func(ptr::null(), c_command.as_ptr()),
+            });
     }
 }
 
 pub(crate) trait ClientEnterWorld<T: AsMut<client_t>> {
     fn client_enter_world(&self, client: T, cmd: *mut usercmd_t);
 }
 
@@ -1608,16 +1744,17 @@
 
 impl ComPrintf for QuakeLiveEngine {
     fn com_printf(&self, msg: &str) {
         let Ok(c_msg) = CString::new(msg) else {
             return;
         };
         self.com_printf_detour().iter().for_each(|detour| {
-            let original_func: extern "C" fn(*const c_char, ...) =
-                unsafe { mem::transmute(detour.trampoline()) };
+            let original_func = unsafe {
+                mem::transmute::<&(), extern "C" fn(*const c_char, ...)>(detour.trampoline())
+            };
             original_func(c_msg.as_ptr())
         });
     }
 }
 
 pub(crate) trait SpawnServer<T: AsRef<str>, U: Into<qboolean>> {
     fn spawn_server(&self, server: T, kill_bots: U);
```

### Comparing `shinqlx-0.5.6/src/quake_live_functions.rs` & `shinqlx-0.5.7/src/quake_live_functions.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/build.rs` & `shinqlx-0.5.7/build.rs`

 * *Files identical despite different names*

### Comparing `shinqlx-0.5.6/PKG-INFO` & `shinqlx-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: shinqlx
-Version: 0.5.6
+Version: 0.5.7
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: setuptools >=61.2
 Requires-Dist: redis >=2.10
```

