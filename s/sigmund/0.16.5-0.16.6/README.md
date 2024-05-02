# Comparing `tmp/sigmund-0.16.5.tar.gz` & `tmp/sigmund-0.16.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmund-0.16.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigmund-0.16.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigmund-0.16.5.tar` & `sigmund-0.16.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    35147 2024-04-30 15:05:06.434642 sigmund-0.16.5/COPYING
--rw-r--r--   0        0        0     1017 2024-04-30 15:05:06.434642 sigmund-0.16.5/pyproject.toml
--rw-r--r--   0        0        0     3037 2024-04-30 15:05:06.434642 sigmund-0.16.5/readme.md
--rw-r--r--   0        0        0      101 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/__init__.py
--rw-r--r--   0        0        0     2746 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/attachments.py
--rw-r--r--   0        0        0     9770 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/config.py
--rw-r--r--   0        0        0        0 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/database/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/database/encryption.py
--rw-r--r--   0        0        0    14378 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/database/manager.py
--rw-r--r--   0        0        0     3213 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/database/models.py
--rw-r--r--   0        0        0     6331 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/documentation.py
--rw-r--r--   0        0        0      389 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/forms.py
--rw-r--r--   0        0        0     2547 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/library.py
--rw-r--r--   0        0        0    10115 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/messages.py
--rw-r--r--   0        0        0     1252 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/__init__.py
--rw-r--r--   0        0        0     5297 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/_anthropic_model.py
--rw-r--r--   0        0        0     4756 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/_base_model.py
--rw-r--r--   0        0        0      379 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/_dummy_model.py
--rw-r--r--   0        0        0     2700 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/_mistral_model.py
--rw-r--r--   0        0        0     3428 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/_openai_model.py
--rw-r--r--   0        0        0     2141 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/prompt.py
--rw-r--r--   0        0        0      160 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/routes/__init__.py
--rw-r--r--   0        0        0     7298 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/routes/api.py
--rw-r--r--   0        0        0     5775 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/routes/app.py
--rw-r--r--   0        0        0     3769 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/routes/google_login.py
--rw-r--r--   0        0        0     7732 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/routes/subscribe.py
--rw-r--r--   0        0        0     1494 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/server.py
--rw-r--r--   0        0        0     9354 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/sigmund.py
--rw-r--r--   0        0        0     4471 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/static/about.md
--rw-r--r--   0        0        0  4708018 2024-04-30 15:05:06.442642 sigmund-0.16.5/sigmund/static/background.png
--rw-r--r--   0        0        0      386 2024-04-30 15:05:06.442642 sigmund-0.16.5/sigmund/static/favicon.svg
--rw-r--r--   0        0        0     1433 2024-04-30 15:05:06.442642 sigmund-0.16.5/sigmund/static/login.md
--rw-r--r--   0        0        0     4976 2024-04-30 15:05:06.442642 sigmund-0.16.5/sigmund/static/pygments.css
--rw-r--r--   0        0        0   708136 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/static/sofa-with-sigmund.png
--rw-r--r--   0        0        0   684883 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/static/sofa.png
--rw-r--r--   0        0        0     3428 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/static/terms.md
--rw-r--r--   0        0        0     1359 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/chat.html
--rw-r--r--   0        0        0      242 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/footer.html
--rw-r--r--   0        0        0      574 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/head.html
--rw-r--r--   0        0        0      244 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/header.html
--rw-r--r--   0        0        0      329 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/info-page.html
--rw-r--r--   0        0        0     3739 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/login.html
--rw-r--r--   0        0        0    10786 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/main.js
--rw-r--r--   0        0        0    12359 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/menu.html
--rw-r--r--   0        0        0       80 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/sign-out.html
--rw-r--r--   0        0        0     6380 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/stylesheet.css.jinja
--rw-r--r--   0        0        0      531 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/subscribe-error.html
--rw-r--r--   0        0        0     1555 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/subscribe-now.html
--rw-r--r--   0        0        0      515 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/subscribe-success.html
--rw-r--r--   0        0        0      265 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/__init__.py
--rw-r--r--   0        0        0     2231 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_base_tool.py
--rw-r--r--   0        0        0     2920 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_download.py
--rw-r--r--   0        0        0     2085 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_execute_code.py
--rw-r--r--   0        0        0     1846 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_read_attachment.py
--rw-r--r--   0        0        0     2076 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_search_documentation.py
--rw-r--r--   0        0        0     1275 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_search_google_scholar.py
--rw-r--r--   0        0        0     4358 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/utils.py
--rw-r--r--   0        0        0     4228 1970-01-01 00:00:00.000000 sigmund-0.16.5/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-01 10:01:59.129593 sigmund-0.16.6/COPYING
+-rw-r--r--   0        0        0     1017 2024-05-01 10:01:59.129593 sigmund-0.16.6/pyproject.toml
+-rw-r--r--   0        0        0     3037 2024-05-01 10:01:59.129593 sigmund-0.16.6/readme.md
+-rw-r--r--   0        0        0      101 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/__init__.py
+-rw-r--r--   0        0        0     2746 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/attachments.py
+-rw-r--r--   0        0        0     9770 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/config.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/database/__init__.py
+-rw-r--r--   0        0        0     1030 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/database/encryption.py
+-rw-r--r--   0        0        0    14378 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/database/manager.py
+-rw-r--r--   0        0        0     3213 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/database/models.py
+-rw-r--r--   0        0        0     6331 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/documentation.py
+-rw-r--r--   0        0        0      389 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/forms.py
+-rw-r--r--   0        0        0     2547 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/library.py
+-rw-r--r--   0        0        0    10115 2024-05-01 10:01:59.129593 sigmund-0.16.6/sigmund/messages.py
+-rw-r--r--   0        0        0     1252 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/model/__init__.py
+-rw-r--r--   0        0        0     5297 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/model/_anthropic_model.py
+-rw-r--r--   0        0        0     4756 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/model/_base_model.py
+-rw-r--r--   0        0        0      379 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/model/_dummy_model.py
+-rw-r--r--   0        0        0     2700 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/model/_mistral_model.py
+-rw-r--r--   0        0        0     3428 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/model/_openai_model.py
+-rw-r--r--   0        0        0     2141 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/prompt.py
+-rw-r--r--   0        0        0      160 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/routes/__init__.py
+-rw-r--r--   0        0        0     7298 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/routes/api.py
+-rw-r--r--   0        0        0     5775 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/routes/app.py
+-rw-r--r--   0        0        0     3769 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/routes/google_login.py
+-rw-r--r--   0        0        0     7733 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/routes/subscribe.py
+-rw-r--r--   0        0        0     1494 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/server.py
+-rw-r--r--   0        0        0     9354 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/sigmund.py
+-rw-r--r--   0        0        0     4471 2024-05-01 10:01:59.133593 sigmund-0.16.6/sigmund/static/about.md
+-rw-r--r--   0        0        0  4708018 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/static/background.png
+-rw-r--r--   0        0        0      386 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/static/favicon.svg
+-rw-r--r--   0        0        0     1433 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/static/login.md
+-rw-r--r--   0        0        0     4976 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/static/pygments.css
+-rw-r--r--   0        0        0   708136 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/static/sofa-with-sigmund.png
+-rw-r--r--   0        0        0   684883 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/static/sofa.png
+-rw-r--r--   0        0        0     3428 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/static/terms.md
+-rw-r--r--   0        0        0     1359 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/templates/chat.html
+-rw-r--r--   0        0        0      242 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/templates/footer.html
+-rw-r--r--   0        0        0      574 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/templates/head.html
+-rw-r--r--   0        0        0      244 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/templates/header.html
+-rw-r--r--   0        0        0      329 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/templates/info-page.html
+-rw-r--r--   0        0        0     3739 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/templates/login.html
+-rw-r--r--   0        0        0    10786 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/templates/main.js
+-rw-r--r--   0        0        0    12359 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/templates/menu.html
+-rw-r--r--   0        0        0       80 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/templates/sign-out.html
+-rw-r--r--   0        0        0     6380 2024-05-01 10:01:59.141594 sigmund-0.16.6/sigmund/templates/stylesheet.css.jinja
+-rw-r--r--   0        0        0      531 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/templates/subscribe-error.html
+-rw-r--r--   0        0        0     1555 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/templates/subscribe-now.html
+-rw-r--r--   0        0        0      515 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/templates/subscribe-success.html
+-rw-r--r--   0        0        0      265 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/tools/__init__.py
+-rw-r--r--   0        0        0     2231 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/tools/_base_tool.py
+-rw-r--r--   0        0        0     2920 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/tools/_download.py
+-rw-r--r--   0        0        0     2085 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/tools/_execute_code.py
+-rw-r--r--   0        0        0     1846 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/tools/_read_attachment.py
+-rw-r--r--   0        0        0     2076 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/tools/_search_documentation.py
+-rw-r--r--   0        0        0     1275 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/tools/_search_google_scholar.py
+-rw-r--r--   0        0        0     4358 2024-05-01 10:01:59.145594 sigmund-0.16.6/sigmund/utils.py
+-rw-r--r--   0        0        0     4228 1970-01-01 00:00:00.000000 sigmund-0.16.6/PKG-INFO
```

### Comparing `sigmund-0.16.5/COPYING` & `sigmund-0.16.6/COPYING`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/pyproject.toml` & `sigmund-0.16.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/readme.md` & `sigmund-0.16.6/readme.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/attachments.py` & `sigmund-0.16.6/sigmund/attachments.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/config.py` & `sigmund-0.16.6/sigmund/config.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/database/encryption.py` & `sigmund-0.16.6/sigmund/database/encryption.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/database/manager.py` & `sigmund-0.16.6/sigmund/database/manager.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/database/models.py` & `sigmund-0.16.6/sigmund/database/models.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/documentation.py` & `sigmund-0.16.6/sigmund/documentation.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/library.py` & `sigmund-0.16.6/sigmund/library.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/messages.py` & `sigmund-0.16.6/sigmund/messages.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/model/__init__.py` & `sigmund-0.16.6/sigmund/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/model/_anthropic_model.py` & `sigmund-0.16.6/sigmund/model/_anthropic_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/model/_base_model.py` & `sigmund-0.16.6/sigmund/model/_base_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/model/_mistral_model.py` & `sigmund-0.16.6/sigmund/model/_mistral_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/model/_openai_model.py` & `sigmund-0.16.6/sigmund/model/_openai_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/prompt.py` & `sigmund-0.16.6/sigmund/prompt.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/routes/api.py` & `sigmund-0.16.6/sigmund/routes/api.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/routes/app.py` & `sigmund-0.16.6/sigmund/routes/app.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/routes/google_login.py` & `sigmund-0.16.6/sigmund/routes/google_login.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/routes/subscribe.py` & `sigmund-0.16.6/sigmund/routes/subscribe.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     to the Stripe customer portal.
     """
     if not config.subscription_required:
         return redirect(url_for('app.chat'), code=303)    
     sigmund = get_sigmund()
     if sigmund.database.check_subscription():
         logger.info(f'redirecting {sigmund.user_id} to customer portal')
-        redirect(url_for('subscribe.customer-portal'), code=303)
+        redirect(url_for('subscribe.customer_portal'), code=303)
     return utils.render('subscribe-now.html', username=sigmund.user_id)
     
     
 @subscribe_blueprint.route('/create-checkout-session')
 @login_required
 def create_checkout_session():
     """Prepares the product for checkout and then redirects to Stripe for the
@@ -171,8 +171,8 @@
                 stripe_customer_id=stripe_customer_id,
                 stripe_subscription_id=stripe_subscription_id)
             logger.info(
                 f'received payment for {database.username} '
                 f'(stripe_customer_id: {stripe_customer_id}, '
                 f'stripe_subscription_id: {stripe_subscription_id})')
     logger.info('webhook successful')
-    return jsonify(success=True), 200
+    return jsonify(success=True), 200
```

### Comparing `sigmund-0.16.5/sigmund/server.py` & `sigmund-0.16.6/sigmund/server.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/sigmund.py` & `sigmund-0.16.6/sigmund/sigmund.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/static/about.md` & `sigmund-0.16.6/sigmund/static/about.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/static/background.png` & `sigmund-0.16.6/sigmund/static/background.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/static/login.md` & `sigmund-0.16.6/sigmund/static/login.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/static/pygments.css` & `sigmund-0.16.6/sigmund/static/pygments.css`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/static/sofa-with-sigmund.png` & `sigmund-0.16.6/sigmund/static/sofa-with-sigmund.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/static/sofa.png` & `sigmund-0.16.6/sigmund/static/sofa.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/static/terms.md` & `sigmund-0.16.6/sigmund/static/terms.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/templates/chat.html` & `sigmund-0.16.6/sigmund/templates/chat.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/templates/head.html` & `sigmund-0.16.6/sigmund/templates/head.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/templates/login.html` & `sigmund-0.16.6/sigmund/templates/login.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/templates/main.js` & `sigmund-0.16.6/sigmund/templates/main.js`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/templates/menu.html` & `sigmund-0.16.6/sigmund/templates/menu.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/templates/stylesheet.css.jinja` & `sigmund-0.16.6/sigmund/templates/stylesheet.css.jinja`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/templates/subscribe-error.html` & `sigmund-0.16.6/sigmund/templates/subscribe-error.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/templates/subscribe-now.html` & `sigmund-0.16.6/sigmund/templates/subscribe-now.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/templates/subscribe-success.html` & `sigmund-0.16.6/sigmund/templates/subscribe-success.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/tools/_base_tool.py` & `sigmund-0.16.6/sigmund/tools/_base_tool.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/tools/_download.py` & `sigmund-0.16.6/sigmund/tools/_download.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/tools/_execute_code.py` & `sigmund-0.16.6/sigmund/tools/_execute_code.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/tools/_read_attachment.py` & `sigmund-0.16.6/sigmund/tools/_read_attachment.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/tools/_search_documentation.py` & `sigmund-0.16.6/sigmund/tools/_search_documentation.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/tools/_search_google_scholar.py` & `sigmund-0.16.6/sigmund/tools/_search_google_scholar.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/sigmund/utils.py` & `sigmund-0.16.6/sigmund/utils.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.5/PKG-INFO` & `sigmund-0.16.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmund
-Version: 0.16.5
+Version: 0.16.6
 Summary: AI-based chatbot that provides sensible answers based on documentation
 Keywords: ai,chatbot,llm
 Author-email: Sebastiaan Mathôt <s.mathot@cogsci.nl>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anthropic
 Requires-Dist: cryptography
```

