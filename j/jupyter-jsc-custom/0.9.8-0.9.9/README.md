# Comparing `tmp/jupyter_jsc_custom-0.9.8.tar.gz` & `tmp/jupyter_jsc_custom-0.9.9.tar.gz`

## Comparing `jupyter_jsc_custom-0.9.8.tar` & `jupyter_jsc_custom-0.9.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/.gitlab-ci.yml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/_version.py
--rw-r--r--   0        0        0    17043 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/misc.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/incidents.py
--rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/misc.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/refresh_hpc_accounts.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/self_api_handler_oauth.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/slurm_wrapper.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/tunnel_restart.py
--rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/twoFA.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/user_count.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/utils/__init__.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/utils/twoFA_mail.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/utils/twoFA_orm.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/utils/twoFA_unity.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/authenticator/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/authenticator/api_services.py
--rw-r--r--   0        0        0    36649 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/authenticator/oauthenticator.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/handler/__init__.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/handler/page_handlers.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/spawner/__init__.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/spawner/api_notifications_sse.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/spawner/api_options_form.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/spawner/api_spawn_options_update.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/spawner/api_start_server_random_name.py
--rw-r--r--   0        0        0    19453 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/spawner/spawner.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/jsc_custom/spawner/utils.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/LICENSE
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/README.md
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/.gitlab-ci.yml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/_version.py
+-rw-r--r--   0        0        0    16719 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/misc.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/incidents.py
+-rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/misc.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/refresh_hpc_accounts.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/self_api_handler_oauth.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/slurm_wrapper.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/tunnel_restart.py
+-rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/twoFA.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/user_count.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/utils/__init__.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/utils/twoFA_mail.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/utils/twoFA_orm.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/utils/twoFA_unity.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/authenticator/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/authenticator/api_services.py
+-rw-r--r--   0        0        0    36685 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/authenticator/oauthenticator.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/handler/__init__.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/handler/page_handlers.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/spawner/__init__.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/spawner/api_notifications_sse.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/spawner/api_options_form.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/spawner/api_spawn_options_update.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/spawner/api_start_server_random_name.py
+-rw-r--r--   0        0        0    19453 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/spawner/spawner.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/jsc_custom/spawner/utils.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/LICENSE
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/README.md
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 jupyter_jsc_custom-0.9.9/PKG-INFO
```

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/misc.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,20 +259,14 @@
                 update_status_image(system, svc["health"])
             incidents.get(system)["health"] = svc["health"]
 
         config = get_custom_config().get("incidentCheck", {})
         sleep_timer = config.get("interval", 60)
         incidents = _incidents_cache.copy()
 
-        # Update threshold
-        interactive_threshold = config.get("healthThreshold", {}).get("interactive", 40)
-        compute_threshold = config.get("healthThreshold", {}).get("compute", 50)
-        incidents["interactive_threshold"] = interactive_threshold
-        incidents["compute_threshold"] = compute_threshold
-
         api_url = config.get("url", "https://status.jsc.fz-juelich.de/api")
         timeout = config.get("timeout", 5)
         try:
             all_incidents_r = requests.get(f"{api_url}/incidents", timeout=timeout)
             all_incidents_r.raise_for_status()
             all_incidents = all_incidents_r.json()
             for name, id in config["services"].items():
```

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/misc.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/misc.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/refresh_hpc_accounts.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/refresh_hpc_accounts.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/self_api_handler_oauth.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/self_api_handler_oauth.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/slurm_wrapper.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/slurm_wrapper.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/tunnel_restart.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/tunnel_restart.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/twoFA.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/twoFA.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/user_count.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/user_count.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/utils/twoFA_mail.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/utils/twoFA_mail.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/utils/twoFA_orm.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/utils/twoFA_orm.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/apihandler/utils/twoFA_unity.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/apihandler/utils/twoFA_unity.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/authenticator/api_services.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/authenticator/api_services.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/authenticator/oauthenticator.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/authenticator/oauthenticator.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,14 +683,15 @@
                 "authStateKeys",
                 [
                     "services",
                     "userModules",
                     "announcement",
                     "groups",
                     "systems",
+                    "incidentCheck"
                 ],
             )
             for key in custom_config_auth_state_keys:
                 if key in custom_config.keys():
                     authentication["auth_state"]["custom_config"][key] = custom_config[
                         key
                     ]
```

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/handler/page_handlers.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/handler/page_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/spawner/api_notifications_sse.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/spawner/api_notifications_sse.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/spawner/api_options_form.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/spawner/api_options_form.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/spawner/api_spawn_options_update.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/spawner/api_spawn_options_update.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/spawner/api_start_server_random_name.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/spawner/api_start_server_random_name.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/spawner/spawner.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/spawner/spawner.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/jsc_custom/spawner/utils.py` & `jupyter_jsc_custom-0.9.9/jsc_custom/spawner/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/.gitignore` & `jupyter_jsc_custom-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/LICENSE` & `jupyter_jsc_custom-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_jsc_custom-0.9.8/pyproject.toml` & `jupyter_jsc_custom-0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 profile = "black"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/kreuzert/jupyter-jsc-custom"
 
 [tool.tbump.version]
-current = "0.9.8"
+current = "0.9.9"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?P<pre>((a|b|rc)\d+)|)
```

### Comparing `jupyter_jsc_custom-0.9.8/PKG-INFO` & `jupyter_jsc_custom-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-jsc-custom
-Version: 0.9.8
+Version: 0.9.9
 Summary: Helper classes and functions, used for JupyterHubs running at Juelich Supercomputing centre
 Author-email: Tim Kreuzer <t.kreuzer@fz-juelich.de>, Alice Grosch <a.grosch@fz-juelich.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Forschungszentrum Juelich GmbH
         
         Redistribution and use in source and binary forms, with or without
```

