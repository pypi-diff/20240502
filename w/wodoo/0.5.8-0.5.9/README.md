# Comparing `tmp/wodoo-0.5.8.tar.gz` & `tmp/wodoo-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wodoo-0.5.8.tar", last modified: Mon Mar 25 22:57:34 2024, max compression
+gzip compressed data, was "wodoo-0.5.9.tar", last modified: Tue Mar 26 20:47:54 2024, max compression
```

## Comparing `wodoo-0.5.8.tar` & `wodoo-0.5.9.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.323265 wodoo-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-25 22:57:20.000000 wodoo-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-03-25 22:57:34.323265 wodoo-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-03-25 22:57:20.000000 wodoo-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-25 22:57:34.323265 wodoo-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-25 22:57:20.000000 wodoo-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.315265 wodoo-0.5.8/wodoo/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/click_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/click_global_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/config/cicd_network_for_project.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/config/default_network
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/config/template_onlyloop.yml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/config/template_withports.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7012 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/daddy_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/defaults
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.307265 wodoo-0.5.8/wodoo/extra_install/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.307265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/debug.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/interactive.sh
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/config
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa.pub
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/ari_additional_custom.conf.appendix
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/manager_custom.conf.appendix
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/freepbx_chown.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/
--rwxr-xr-x   0 runner    (1001) docker     (127)      349 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/10-freepbx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/10-start
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.319265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/apache2
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/asterisk
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fail2ban
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fop
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbc.ini
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbcinst.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.323265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/08-ssh
--rwxr-xr-x   0 runner    (1001) docker     (127)      567 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb
--rwxr-xr-x   0 runner    (1001) docker     (127)    17011 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx
--rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/13-extra-modules
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/15-permissions
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/16-soundlang
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/20-load-default-extensions
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.311265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.323265 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/authorized_keys
--rwxr-xr-x   0 runner    (1001) docker     (127)      423 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/run_freepbx.sh
--rw-r--r--   0 runner    (1001) docker     (127)    22911 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_clickhelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    36383 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16153 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_control_with_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_db_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_db_snapshots_docker_btrfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_db_snapshots_docker_zfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_db_snapshots_plain_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_linting.py
--rw-r--r--   0 runner    (1001) docker     (127)    52043 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_odoosh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    22027 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_src.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_talk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/lib_turnintodev.py
--rw-r--r--   0 runner    (1001) docker     (127)    57199 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/module_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/myconfigparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/odoo_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25426 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/odoo_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/pudb.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/queue-job-channels.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/robo_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/settings.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.323265 wodoo-0.5.8/wodoo/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/tests/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/tests/gimera.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.323265 wodoo-0.5.8/wodoo/tests/module_respartner_dummyfield1/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/tests/module_respartner_dummyfield1/partnerview.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.323265 wodoo-0.5.8/wodoo/tests/module_respartner_dummyfield2/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/tests/module_respartner_dummyfield2/partnerview.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)      801 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/testzfs.sh
--rw-r--r--   0 runner    (1001) docker     (127)    46362 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-25 22:57:31.000000 wodoo-0.5.8/wodoo/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.323265 wodoo-0.5.8/wodoo/wait/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/wait/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/wait/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/wait/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-25 22:57:20.000000 wodoo-0.5.8/wodoo/wait/tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:57:34.315265 wodoo-0.5.8/wodoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-03-25 22:57:34.000000 wodoo-0.5.8/wodoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-03-25 22:57:34.000000 wodoo-0.5.8/wodoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 22:57:34.000000 wodoo-0.5.8/wodoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-25 22:57:34.000000 wodoo-0.5.8/wodoo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-25 22:57:34.000000 wodoo-0.5.8/wodoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 22:57:34.000000 wodoo-0.5.8/wodoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-26 20:47:36.000000 wodoo-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-03-26 20:47:54.064393 wodoo-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-03-26 20:47:36.000000 wodoo-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-26 20:47:54.068393 wodoo-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-26 20:47:36.000000 wodoo-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.056393 wodoo-0.5.9/wodoo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/click_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/click_global_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.060393 wodoo-0.5.9/wodoo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/config/cicd_network_for_project.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/config/default_network
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/config/template_onlyloop.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/config/template_withports.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7012 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/daddy_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/defaults
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.052393 wodoo-0.5.9/wodoo/extra_install/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.052393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.060393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/debug.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/interactive.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.060393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/config
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa.pub
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.060393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.060393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/ari_additional_custom.conf.appendix
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/manager_custom.conf.appendix
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/freepbx_chown.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      349 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/10-freepbx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/10-start
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/apache2
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/asterisk
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fail2ban
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fop
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbc.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbcinst.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/08-ssh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      567 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17011 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/13-extra-modules
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/15-permissions
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/16-soundlang
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/20-load-default-extensions
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.052393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/authorized_keys
+-rwxr-xr-x   0 runner    (1001) docker     (127)      423 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/run_freepbx.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_clickhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36609 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16153 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_control_with_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_db_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_db_snapshots_docker_btrfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_db_snapshots_docker_zfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_db_snapshots_plain_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52043 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_odoosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22027 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_talk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/lib_turnintodev.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57199 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/module_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/myconfigparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/odoo_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25426 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/odoo_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/pudb.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/queue-job-channels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/robo_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/settings.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/tests/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/tests/gimera.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/tests/module_respartner_dummyfield1/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/tests/module_respartner_dummyfield1/partnerview.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/tests/module_respartner_dummyfield2/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/tests/module_respartner_dummyfield2/partnerview.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      801 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/testzfs.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    46362 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-26 20:47:47.000000 wodoo-0.5.9/wodoo/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.064393 wodoo-0.5.9/wodoo/wait/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/wait/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/wait/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/wait/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-26 20:47:36.000000 wodoo-0.5.9/wodoo/wait/tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:54.060393 wodoo-0.5.9/wodoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-03-26 20:47:53.000000 wodoo-0.5.9/wodoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-03-26 20:47:54.000000 wodoo-0.5.9/wodoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 20:47:53.000000 wodoo-0.5.9/wodoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-26 20:47:53.000000 wodoo-0.5.9/wodoo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-26 20:47:53.000000 wodoo-0.5.9/wodoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 20:47:53.000000 wodoo-0.5.9/wodoo.egg-info/top_level.txt
```

### Comparing `wodoo-0.5.8/LICENSE` & `wodoo-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/PKG-INFO` & `wodoo-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wodoo
-Version: 0.5.8
+Version: 0.5.9
 Summary: Odoo Framework
 Home-page: https://github.com/marcwimmer/wodoo
 Author: Marc-Christian Wimmer
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wodoo-0.5.8/README.md` & `wodoo-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/setup.py` & `wodoo-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/__init__.py` & `wodoo-0.5.9/wodoo/__init__.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/cli.py` & `wodoo-0.5.9/wodoo/cli.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/click_config.py` & `wodoo-0.5.9/wodoo/click_config.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/click_global_commands.py` & `wodoo-0.5.9/wodoo/click_global_commands.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/consts.py` & `wodoo-0.5.9/wodoo/consts.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/daddy_cleanup.py` & `wodoo-0.5.9/wodoo/daddy_cleanup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/defaults` & `wodoo-0.5.9/wodoo/defaults`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings` & `wodoo-0.5.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_backup.py` & `wodoo-0.5.9/wodoo/lib_backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -626,15 +626,18 @@
             # stop the run started postgres container; softly
             subprocess.check_output(["docker", "stop", postgres_name])
             try:
                 subprocess.check_output(["docker", "kill", postgres_name])
             except subprocess.CalledProcessError:
                 # ignore - stopped before
                 pass
-            subprocess.check_output(["docker", "rm", "-f", postgres_name])
+            try:
+                subprocess.check_output(["docker", "rm", "-f", postgres_name])
+            except:
+                pass
 
 
 def _add_cronjob_scripts(config):
     """
     Adds scripts from images/cronjobs/bin to sys path to be executed.
     """
     spec = importlib.util.spec_from_file_location(
```

### Comparing `wodoo-0.5.8/wodoo/lib_clickhelpers.py` & `wodoo-0.5.9/wodoo/lib_clickhelpers.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_composer.py` & `wodoo-0.5.9/wodoo/lib_composer.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,24 +29,28 @@
 from .tools import __running_as_root_or_sudo
 from .tools import _makedirs
 from .tools import __try_to_set_owner
 from .tools import whoami
 from .tools import abort
 from .tools import _get_version
 from .tools import rsync
+from .tools import get_docker_version
 from .cli import cli, pass_config, Commands
 from .lib_clickhelpers import AliasedGroup
 from .odoo_config import MANIFEST
 from .tools import execute_script
 from .tools import ensure_project_name
 
 import inspect
 import os
 from pathlib import Path
-current_dir = Path(os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe()))))
+
+current_dir = Path(
+    os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
+)
 
 
 @cli.group(cls=AliasedGroup)
 @pass_config
 def composer(config):
     pass
 
@@ -227,15 +231,15 @@
     defaults = {
         "config": config,
         "db": db,
         "demo": demo,
         "LOCAL_SETTINGS": "1" if local else "0",
         "CUSTOMS_DIR": config.WORKING_DIR,
         "WODOO_VERSION": _get_version(),
-        "QUEUEJOB_CHANNELS_FILE": config.files['queuejob_channels_file'],
+        "QUEUEJOB_CHANNELS_FILE": config.files["queuejob_channels_file"],
     }
     if devmode:
         defaults["DEVMODE"] = 1
     if demo:
         defaults["ODOO_DEMO"] = 1
     if headless:
         defaults.update(
@@ -639,15 +643,15 @@
 
 def post_process_complete_yaml_config(config, yml):
     """
     This is after calling docker-compose config, which returns the
     complete configuration.
     """
 
-    yml["version"] = config.YAML_VERSION
+    _set_yaml_version(yml, config)
 
     # remove restart policies, if not restart allowed:
     if not config.restart_containers:
         for service in yml["services"]:
             if "restart" in yml["services"][service]:
                 yml["services"][service].pop("restart")
 
@@ -867,14 +871,21 @@
                         src = deepcopy(content["services"][explode])
                         dict_merge(src, content["services"][to_explode])
                     else:
                         src = content["services"][explode]
                     content["services"][to_explode] = src
 
 
+def _set_yaml_version(content, config):
+    if get_docker_version()[0] < 26:
+        content["version"] = config.YAML_VERSION
+    else:
+        content.pop("version", None)
+
+
 def _apply_variables(config, contents, env):
     import yaml
 
     # add static yaml content to each machine
     default_network = yaml.safe_load(config.files["config/default_network"].read_text())
 
     # extract further networks
@@ -885,15 +896,15 @@
         if isinstance(content, str):
             from .tools import abort
 
             abort((f"Invalid content {content}"))
         for networkname, network in content.get("networks", {}).items():
             default_network["networks"][networkname] = network
 
-        content["version"] = config.YAML_VERSION
+        _set_yaml_version(content, config)
 
         # set settings environment and the override settings after that
         __set_environment_in_services(content)
         content["networks"] = copy.deepcopy(default_network["networks"])
 
         content = yaml.dump(content, default_flow_style=False)
         content = __replace_all_envs_in_str(content, env)
@@ -1057,102 +1068,110 @@
             file = config.files["odoo_docker_file"]
             content = file.read_text() + "\n" + appendix
             content = content.replace("${PROJECT_NAME}", config.project_name)
             file.write_text(content)
 
         # include source code
         if not config.SRC_EXTRA:
-            import pudb;pudb.set_trace()
+            import pudb
+
+            pudb.set_trace()
             append_odoo_src(config, config.files["odoo_docker_file"])
 
     else:
         # seems to use images from registry; no build section
         pass
 
 
 def append_odoo_src(config, path):
     content = "ADD {src} /opt/src"
     path.write_text(path.read_text() + "\n" + content)
 
+
 def _complete_setting_name(ctx, param, incomplete):
-    lines = (current_dir / 'settings.txt').read_text().splitlines()
+    lines = (current_dir / "settings.txt").read_text().splitlines()
 
     params = []
     for line in lines:
         if not line.strip():
             continue
         try:
             name, doc = line.replace("\t", " ").split(" ", 1)
         except ValueError:
             name = line
             doc = ""
         name = name.strip()
         doc = doc.strip()
         name = name.split("=")[0]
-        params.append({'name': name, 'doc': doc})
-
+        params.append({"name": name, "doc": doc})
 
-    res = set([x['name'].strip() for x in params])
+    res = set([x["name"].strip() for x in params])
     if incomplete:
         res = list(filter(lambda x: x.lower().startswith(incomplete.lower()), res))
     return sorted(res)
 
+
 @composer.command()
 @pass_config
 @click.pass_context
 @click.argument("name", required=False, shell_complete=_complete_setting_name)
 @click.argument("value", required=False, default="")
 def setting(ctx, config, name, value):
     from .myconfigparser import MyConfigParser
+
     if not name:
         ctx.invoke(show_effective_settings)
         return
     configparser = MyConfigParser(config.files["settings"])
-    if '=' in name:
+    if "=" in name:
         name, value = name.split("=", 1)
     if not value:
         for k in sorted(configparser.keys()):
-            if  name.lower() in k.lower():
+            if name.lower() in k.lower():
                 click.secho(f"{k}={configparser[k]}")
     else:
         update_setting(config, name, value)
-        click.secho(f"{name}={value}", fg='green')
+        click.secho(f"{name}={value}", fg="green")
         ctx.invoke(do_reload)
 
+
 @composer.command()
 @pass_config
 @click.pass_context
 def show_effective_settings(ctx, config):
     from .myconfigparser import MyConfigParser
 
     config = MyConfigParser(config.files["settings"])
     for k in sorted(config.keys()):
         click.echo(f"{k}={config[k]}")
 
+
 @composer.command()
 @click.argument("name", required=False)
 @click.argument("amount", required=False, type=int)
 @pass_config
 @click.pass_context
 def queuejob_channels(ctx, config, name, amount):
     if name and amount is None:
         abort(f"Please define the amount of workers in {name}")
 
     from .myconfigparser import MyConfigParser
+
     file = config.files["queuejob_channels_file"]
     if file.exists():
         content = file.read_text()
     else:
         config = MyConfigParser(config.files["settings"])
-        content = config.get('ODOO_QUEUEJOBS_CHANNELS', "root:1")
+        content = config.get("ODOO_QUEUEJOBS_CHANNELS", "root:1")
 
     channels = content.split(",")
 
     if name:
         channels = list(filter(lambda x: x.strip().split(":")[0] != name, channels))
         channels.append(f"{name}:{amount}")
         file.write_text(",".join(channels))
-        click.secho("Now restart the queuejob container", fg='yellow')
+        click.secho("Now restart the queuejob container", fg="yellow")
     for channel in channels:
-        click.secho(f"{channel}", fg='green')
+        click.secho(f"{channel}", fg="green")
+
 
 Commands.register(do_reload, "reload")
```

### Comparing `wodoo-0.5.8/wodoo/lib_control.py` & `wodoo-0.5.9/wodoo/lib_control.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_control_with_docker.py` & `wodoo-0.5.9/wodoo/lib_control_with_docker.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_db.py` & `wodoo-0.5.9/wodoo/lib_db.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_db_snapshots.py` & `wodoo-0.5.9/wodoo/lib_db_snapshots.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_db_snapshots_docker_btrfs.py` & `wodoo-0.5.9/wodoo/lib_db_snapshots_docker_btrfs.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_db_snapshots_docker_zfs.py` & `wodoo-0.5.9/wodoo/lib_db_snapshots_docker_zfs.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_db_snapshots_plain_postgres.py` & `wodoo-0.5.9/wodoo/lib_db_snapshots_plain_postgres.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_docker_registry.py` & `wodoo-0.5.9/wodoo/lib_docker_registry.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_lang.py` & `wodoo-0.5.9/wodoo/lib_lang.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_linting.py` & `wodoo-0.5.9/wodoo/lib_linting.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_module.py` & `wodoo-0.5.9/wodoo/lib_module.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_setup.py` & `wodoo-0.5.9/wodoo/lib_setup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_src.py` & `wodoo-0.5.9/wodoo/lib_src.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_talk.py` & `wodoo-0.5.9/wodoo/lib_talk.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/lib_turnintodev.py` & `wodoo-0.5.9/wodoo/lib_turnintodev.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/module_tools.py` & `wodoo-0.5.9/wodoo/module_tools.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/myconfigparser.py` & `wodoo-0.5.9/wodoo/myconfigparser.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/odoo_config.py` & `wodoo-0.5.9/wodoo/odoo_config.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/odoo_parser.py` & `wodoo-0.5.9/wodoo/odoo_parser.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/robo_helpers.py` & `wodoo-0.5.9/wodoo/robo_helpers.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/settings.py` & `wodoo-0.5.9/wodoo/settings.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/settings.txt` & `wodoo-0.5.9/wodoo/settings.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/testzfs.sh` & `wodoo-0.5.9/wodoo/testzfs.sh`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/tools.py` & `wodoo-0.5.9/wodoo/tools.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/wait/decorator.py` & `wodoo-0.5.9/wodoo/wait/decorator.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/wait/log.py` & `wodoo-0.5.9/wodoo/wait/log.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo/wait/tcp.py` & `wodoo-0.5.9/wodoo/wait/tcp.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.5.8/wodoo.egg-info/PKG-INFO` & `wodoo-0.5.9/wodoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wodoo
-Version: 0.5.8
+Version: 0.5.9
 Summary: Odoo Framework
 Home-page: https://github.com/marcwimmer/wodoo
 Author: Marc-Christian Wimmer
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wodoo-0.5.8/wodoo.egg-info/SOURCES.txt` & `wodoo-0.5.9/wodoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

