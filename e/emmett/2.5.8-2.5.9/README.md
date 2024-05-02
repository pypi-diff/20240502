# Comparing `tmp/emmett-2.5.8.tar.gz` & `tmp/emmett-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett-2.5.8.tar", max compression
+gzip compressed data, was "emmett-2.5.9.tar", max compression
```

## Comparing `emmett-2.5.8.tar` & `emmett-2.5.9.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0    14193 2024-01-22 00:31:16.675484 emmett-2.5.8/CHANGES.md
--rw-r--r--   0        0        0     2074 2024-01-22 00:31:16.675484 emmett-2.5.8/LICENSE
--rw-r--r--   0        0        0     2925 2024-01-22 00:31:16.675484 emmett-2.5.8/README.md
--rw-r--r--   0        0        0     9917 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/app_and_modules.md
--rw-r--r--   0        0        0    16591 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/auth.md
--rw-r--r--   0        0        0    12150 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/caching.md
--rw-r--r--   0        0        0     2613 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/cli.md
--rw-r--r--   0        0        0     4481 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/debug_and_logging.md
--rw-r--r--   0        0        0     3056 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/deployment.md
--rw-r--r--   0        0        0     5295 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/extensions.md
--rw-r--r--   0        0        0     5174 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/foreword.md
--rw-r--r--   0        0        0     6493 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/forms.md
--rw-r--r--   0        0        0     2105 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/installation.md
--rw-r--r--   0        0        0     3596 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/languages.md
--rw-r--r--   0        0        0     3087 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/mailer.md
--rw-r--r--   0        0        0     9672 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/orm/advanced.md
--rw-r--r--   0        0        0    12917 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/orm/callbacks.md
--rw-r--r--   0        0        0     7060 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/orm/connecting.md
--rw-r--r--   0        0        0    20808 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/orm/migrations.md
--rw-r--r--   0        0        0    14034 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/orm/models.md
--rw-r--r--   0        0        0    29245 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/orm/operations.md
--rw-r--r--   0        0        0    27472 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/orm/relations.md
--rw-r--r--   0        0        0     5523 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/orm/scopes.md
--rw-r--r--   0        0        0     6732 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/orm/virtuals.md
--rw-r--r--   0        0        0     3172 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/orm.md
--rw-r--r--   0        0        0     4100 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/patterns.md
--rw-r--r--   0        0        0    14161 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/pipeline.md
--rw-r--r--   0        0        0    15916 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/quickstart.md
--rw-r--r--   0        0        0     6082 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/request.md
--rw-r--r--   0        0        0     3378 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/response.md
--rw-r--r--   0        0        0    11727 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/routing.md
--rw-r--r--   0        0        0     2424 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/services.md
--rw-r--r--   0        0        0     4535 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/sessions.md
--rw-r--r--   0        0        0     6405 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/templates.md
--rw-r--r--   0        0        0     6776 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/testing.md
--rw-r--r--   0        0        0      440 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/tree.yml
--rw-r--r--   0        0        0    14840 2024-01-22 00:31:16.675484 emmett-2.5.8/docs/tutorial.md
--rw-r--r--   0        0        0    16597 2024-01-22 00:31:16.679484 emmett-2.5.8/docs/upgrading.md
--rw-r--r--   0        0        0    15878 2024-01-22 00:31:16.679484 emmett-2.5.8/docs/validations.md
--rw-r--r--   0        0        0     2307 2024-01-22 00:31:16.679484 emmett-2.5.8/docs/websocket.md
--rw-r--r--   0        0        0      386 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/__init__.py
--rw-r--r--   0        0        0      248 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/__main__.py
--rw-r--r--   0        0        0       22 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/__version__.py
--rw-r--r--   0        0        0    11242 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/_internal.py
--rw-r--r--   0        0        0     5633 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/_reloader.py
--rw-r--r--   0        0        0      771 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/_shortcuts.py
--rw-r--r--   0        0        0    27001 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/app.py
--rw-r--r--   0        0        0        0 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/asgi/__init__.py
--rw-r--r--   0        0        0    15264 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/asgi/handlers.py
--rw-r--r--   0        0        0      220 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/asgi/helpers.py
--rw-r--r--   0        0        0      533 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/asgi/typing.py
--rw-r--r--   0        0        0     3064 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/asgi/workers.py
--rw-r--r--   0        0        0     8029 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/asgi/wrappers.py
--rw-r--r--   0        0        0        0 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/debug/__init__.py
--rw-r--r--   0        0        0     2437 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/debug/shBrushPython.js
--rw-r--r--   0        0        0     6204 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/debug/shCore.css
--rw-r--r--   0        0        0    16175 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/debug/shCore.js
--rw-r--r--   0        0        0     2499 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/debug/shTheme.css
--rw-r--r--   0        0        0      647 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/debug/view.css
--rw-r--r--   0        0        0     4626 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/debug/view.html
--rw-r--r--   0        0        0     1630 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/helpers.js
--rw-r--r--   0        0        0    89476 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/jquery.min.js
--rw-r--r--   0        0        0   137986 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/assets/jquery.min.map
--rw-r--r--   0        0        0    18871 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/cache.py
--rw-r--r--   0        0        0    15318 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/cli.py
--rw-r--r--   0        0        0     2547 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/ctx.py
--rw-r--r--   0        0        0     8165 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/datastructures.py
--rw-r--r--   0        0        0     5076 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/debug.py
--rw-r--r--   0        0        0     3201 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/extensions.py
--rw-r--r--   0        0        0    26116 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/forms.py
--rw-r--r--   0        0        0     3095 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/helpers.py
--rw-r--r--   0        0        0     6435 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/html.py
--rw-r--r--   0        0        0    10834 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/http.py
--rw-r--r--   0        0        0        0 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/language/__init__.py
--rw-r--r--   0        0        0     1096 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/language/helpers.py
--rw-r--r--   0        0        0      933 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/language/translator.py
--rw-r--r--   0        0        0        0 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/libs/__init__.py
--rw-r--r--   0        0        0    25207 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/libs/contenttype.py
--rw-r--r--   0        0        0     3915 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/libs/portalocker.py
--rw-r--r--   0        0        0      925 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/locals.py
--rw-r--r--   0        0        0     3084 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/logger.py
--rw-r--r--   0        0        0      478 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/orm/__init__.py
--rw-r--r--   0        0        0     2373 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/orm/_patches.py
--rw-r--r--   0        0        0    12979 2024-01-22 00:31:16.679484 emmett-2.5.8/emmett/orm/adapters.py
--rw-r--r--   0        0        0     3224 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/apis.py
--rw-r--r--   0        0        0     8857 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/base.py
--rw-r--r--   0        0        0    12058 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/connection.py
--rw-r--r--   0        0        0       80 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/engines/__init__.py
--rw-r--r--   0        0        0     5577 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/engines/postgres.py
--rw-r--r--   0        0        0     1191 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/engines/sqlite.py
--rw-r--r--   0        0        0      605 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/errors.py
--rw-r--r--   0        0        0     1677 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/geo.py
--rw-r--r--   0        0        0    18102 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/helpers.py
--rw-r--r--   0        0        0       62 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/__init__.py
--rw-r--r--   0        0        0     2892 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/base.py
--rw-r--r--   0        0        0    15289 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/commands.py
--rw-r--r--   0        0        0    14381 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/engine.py
--rw-r--r--   0        0        0     1058 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/exceptions.py
--rw-r--r--   0        0        0    21829 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/generation.py
--rw-r--r--   0        0        0     3636 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/helpers.py
--rw-r--r--   0        0        0      491 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/migration.tmpl
--rw-r--r--   0        0        0    23246 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/operations.py
--rw-r--r--   0        0        0    14902 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/revisions.py
--rw-r--r--   0        0        0    12034 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/scripts.py
--rw-r--r--   0        0        0     1150 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/migrations/utils.py
--rw-r--r--   0        0        0    46828 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/models.py
--rw-r--r--   0        0        0    57286 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/objects.py
--rw-r--r--   0        0        0     4208 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/transactions.py
--rw-r--r--   0        0        0      978 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/orm/wrappers.py
--rw-r--r--   0        0        0      917 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/parsers.py
--rw-r--r--   0        0        0    12040 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/pipeline.py
--rw-r--r--   0        0        0        0 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/routing/__init__.py
--rw-r--r--   0        0        0     5303 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/routing/dispatchers.py
--rw-r--r--   0        0        0     4112 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/routing/response.py
--rw-r--r--   0        0        0    11518 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/routing/router.py
--rw-r--r--   0        0        0     8479 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/routing/routes.py
--rw-r--r--   0        0        0     7026 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/routing/rules.py
--rw-r--r--   0        0        0     9704 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/routing/urls.py
--rw-r--r--   0        0        0        0 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/rsgi/__init__.py
--rw-r--r--   0        0        0     9973 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/rsgi/handlers.py
--rw-r--r--   0        0        0      878 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/rsgi/helpers.py
--rw-r--r--   0        0        0     4338 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/rsgi/wrappers.py
--rw-r--r--   0        0        0     5490 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/security.py
--rw-r--r--   0        0        0     2207 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/serializers.py
--rw-r--r--   0        0        0     1050 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/server.py
--rw-r--r--   0        0        0    11649 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/sessions.py
--rw-r--r--   0        0        0        0 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/templating/__init__.py
--rw-r--r--   0        0        0     1843 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/templating/lexers.py
--rw-r--r--   0        0        0     1957 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/templating/templater.py
--rw-r--r--   0        0        0       37 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/testing/__init__.py
--rw-r--r--   0        0        0    11877 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/testing/client.py
--rw-r--r--   0        0        0    10674 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/testing/env.py
--rw-r--r--   0        0        0    12272 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/testing/helpers.py
--rw-r--r--   0        0        0    15936 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/testing/urls.py
--rw-r--r--   0        0        0      125 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/tools/__init__.py
--rw-r--r--   0        0        0       52 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/tools/auth/__init__.py
--rw-r--r--   0        0        0     9232 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/tools/auth/apis.py
--rw-r--r--   0        0        0    19190 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/tools/auth/exposer.py
--rw-r--r--   0        0        0    14033 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/tools/auth/ext.py
--rw-r--r--   0        0        0     5270 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/tools/auth/forms.py
--rw-r--r--   0        0        0     7485 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/tools/auth/models.py
--rw-r--r--   0        0        0     1417 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/tools/decorators.py
--rw-r--r--   0        0        0    10953 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/tools/mailer.py
--rw-r--r--   0        0        0     1565 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/tools/service.py
--rw-r--r--   0        0        0      355 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/typing.py
--rw-r--r--   0        0        0     5357 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/utils.py
--rw-r--r--   0        0        0    11554 2024-01-22 00:31:16.683483 emmett-2.5.8/emmett/validators/__init__.py
--rw-r--r--   0        0        0     7636 2024-01-22 00:31:16.687483 emmett-2.5.8/emmett/validators/basic.py
--rw-r--r--   0        0        0    31120 2024-01-22 00:31:16.687483 emmett-2.5.8/emmett/validators/consist.py
--rw-r--r--   0        0        0    19038 2024-01-22 00:31:16.687483 emmett-2.5.8/emmett/validators/helpers.py
--rw-r--r--   0        0        0     7367 2024-01-22 00:31:16.687483 emmett-2.5.8/emmett/validators/inside.py
--rw-r--r--   0        0        0     4614 2024-01-22 00:31:16.687483 emmett-2.5.8/emmett/validators/process.py
--rw-r--r--   0        0        0     2190 2024-01-22 00:31:16.687483 emmett-2.5.8/emmett/wrappers/__init__.py
--rw-r--r--   0        0        0     2886 2024-01-22 00:31:16.687483 emmett-2.5.8/emmett/wrappers/helpers.py
--rw-r--r--   0        0        0     4269 2024-01-22 00:31:16.687483 emmett-2.5.8/emmett/wrappers/request.py
--rw-r--r--   0        0        0     1525 2024-01-22 00:31:16.687483 emmett-2.5.8/emmett/wrappers/response.py
--rw-r--r--   0        0        0     1062 2024-01-22 00:31:16.687483 emmett-2.5.8/emmett/wrappers/websocket.py
--rw-r--r--   0        0        0     2165 2024-01-22 00:31:16.687483 emmett-2.5.8/pyproject.toml
--rw-r--r--   0        0        0     1524 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/helpers.py
--rw-r--r--   0        0        0       46 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/languages/de.json
--rw-r--r--   0        0        0       49 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/languages/it.json
--rw-r--r--   0        0        0       69 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/languages/ru.json
--rw-r--r--   0        0        0      134 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/templates/auth/auth.html
--rw-r--r--   0        0        0      479 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/templates/layout.html
--rw-r--r--   0        0        0      153 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/templates/test.html
--rw-r--r--   0        0        0     8027 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_auth.py
--rw-r--r--   0        0        0     4658 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_cache.py
--rw-r--r--   0        0        0     1415 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_http.py
--rw-r--r--   0        0        0      861 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_logger.py
--rw-r--r--   0        0        0    11854 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_mailer.py
--rw-r--r--   0        0        0     8618 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_migrations.py
--rw-r--r--   0        0        0    33038 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_orm.py
--rw-r--r--   0        0        0      853 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_orm_connections.py
--rw-r--r--   0        0        0    10074 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_orm_gis.py
--rw-r--r--   0        0        0    22722 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_orm_pks.py
--rw-r--r--   0        0        0     9863 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_orm_row.py
--rw-r--r--   0        0        0     2958 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_orm_transactions.py
--rw-r--r--   0        0        0    22478 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_pipeline.py
--rw-r--r--   0        0        0     8659 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_routing.py
--rw-r--r--   0        0        0     1475 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_session.py
--rw-r--r--   0        0        0     2705 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_templates.py
--rw-r--r--   0        0        0      622 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_translator.py
--rw-r--r--   0        0        0     2045 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_utils.py
--rw-r--r--   0        0        0    18633 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_validators.py
--rw-r--r--   0        0        0      822 2024-01-22 00:31:16.687483 emmett-2.5.8/tests/test_wrappers.py
--rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 emmett-2.5.8/PKG-INFO
+-rw-r--r--   0        0        0    14193 2024-01-28 15:21:40.953985 emmett-2.5.9/CHANGES.md
+-rw-r--r--   0        0        0     2074 2024-01-28 15:21:40.953985 emmett-2.5.9/LICENSE
+-rw-r--r--   0        0        0     2925 2024-01-28 15:21:40.953985 emmett-2.5.9/README.md
+-rw-r--r--   0        0        0     9917 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/app_and_modules.md
+-rw-r--r--   0        0        0    16591 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/auth.md
+-rw-r--r--   0        0        0    12150 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/caching.md
+-rw-r--r--   0        0        0     2613 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/cli.md
+-rw-r--r--   0        0        0     4481 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/debug_and_logging.md
+-rw-r--r--   0        0        0     3056 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/deployment.md
+-rw-r--r--   0        0        0     5295 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/extensions.md
+-rw-r--r--   0        0        0     5174 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/foreword.md
+-rw-r--r--   0        0        0     6493 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/forms.md
+-rw-r--r--   0        0        0     2105 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/installation.md
+-rw-r--r--   0        0        0     3596 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/languages.md
+-rw-r--r--   0        0        0     3087 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/mailer.md
+-rw-r--r--   0        0        0     9672 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/orm/advanced.md
+-rw-r--r--   0        0        0    12917 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/orm/callbacks.md
+-rw-r--r--   0        0        0     7060 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/orm/connecting.md
+-rw-r--r--   0        0        0    20808 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/orm/migrations.md
+-rw-r--r--   0        0        0    14034 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/orm/models.md
+-rw-r--r--   0        0        0    29245 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/orm/operations.md
+-rw-r--r--   0        0        0    27472 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/orm/relations.md
+-rw-r--r--   0        0        0     5523 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/orm/scopes.md
+-rw-r--r--   0        0        0     6732 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/orm/virtuals.md
+-rw-r--r--   0        0        0     3172 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/orm.md
+-rw-r--r--   0        0        0     4100 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/patterns.md
+-rw-r--r--   0        0        0    14161 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/pipeline.md
+-rw-r--r--   0        0        0    15916 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/quickstart.md
+-rw-r--r--   0        0        0     6082 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/request.md
+-rw-r--r--   0        0        0     3378 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/response.md
+-rw-r--r--   0        0        0    11727 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/routing.md
+-rw-r--r--   0        0        0     2424 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/services.md
+-rw-r--r--   0        0        0     4535 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/sessions.md
+-rw-r--r--   0        0        0     6405 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/templates.md
+-rw-r--r--   0        0        0     6776 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/testing.md
+-rw-r--r--   0        0        0      440 2024-01-28 15:21:40.953985 emmett-2.5.9/docs/tree.yml
+-rw-r--r--   0        0        0    14840 2024-01-28 15:21:40.957985 emmett-2.5.9/docs/tutorial.md
+-rw-r--r--   0        0        0    16597 2024-01-28 15:21:40.957985 emmett-2.5.9/docs/upgrading.md
+-rw-r--r--   0        0        0    15878 2024-01-28 15:21:40.957985 emmett-2.5.9/docs/validations.md
+-rw-r--r--   0        0        0     2307 2024-01-28 15:21:40.957985 emmett-2.5.9/docs/websocket.md
+-rw-r--r--   0        0        0      386 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/__init__.py
+-rw-r--r--   0        0        0      219 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/__main__.py
+-rw-r--r--   0        0        0       22 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/__version__.py
+-rw-r--r--   0        0        0    11242 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/_internal.py
+-rw-r--r--   0        0        0     5633 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/_reloader.py
+-rw-r--r--   0        0        0      771 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/_shortcuts.py
+-rw-r--r--   0        0        0    27001 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/app.py
+-rw-r--r--   0        0        0        0 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/asgi/__init__.py
+-rw-r--r--   0        0        0    15264 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/asgi/handlers.py
+-rw-r--r--   0        0        0      220 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/asgi/helpers.py
+-rw-r--r--   0        0        0      533 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/asgi/typing.py
+-rw-r--r--   0        0        0     3064 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/asgi/workers.py
+-rw-r--r--   0        0        0     8029 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/asgi/wrappers.py
+-rw-r--r--   0        0        0        0 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/debug/__init__.py
+-rw-r--r--   0        0        0     2437 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/debug/shBrushPython.js
+-rw-r--r--   0        0        0     6204 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/debug/shCore.css
+-rw-r--r--   0        0        0    16175 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/debug/shCore.js
+-rw-r--r--   0        0        0     2499 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/debug/shTheme.css
+-rw-r--r--   0        0        0      647 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/debug/view.css
+-rw-r--r--   0        0        0     4626 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/debug/view.html
+-rw-r--r--   0        0        0     1630 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/helpers.js
+-rw-r--r--   0        0        0    89476 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/jquery.min.js
+-rw-r--r--   0        0        0   137986 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/assets/jquery.min.map
+-rw-r--r--   0        0        0    18871 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/cache.py
+-rw-r--r--   0        0        0    15318 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/cli.py
+-rw-r--r--   0        0        0     2547 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/ctx.py
+-rw-r--r--   0        0        0     8165 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/datastructures.py
+-rw-r--r--   0        0        0     5076 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/debug.py
+-rw-r--r--   0        0        0     3201 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/extensions.py
+-rw-r--r--   0        0        0    26116 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/forms.py
+-rw-r--r--   0        0        0     3095 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/helpers.py
+-rw-r--r--   0        0        0     6435 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/html.py
+-rw-r--r--   0        0        0    10842 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/http.py
+-rw-r--r--   0        0        0        0 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/language/__init__.py
+-rw-r--r--   0        0        0     1096 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/language/helpers.py
+-rw-r--r--   0        0        0      933 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/language/translator.py
+-rw-r--r--   0        0        0        0 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/libs/__init__.py
+-rw-r--r--   0        0        0    25207 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/libs/contenttype.py
+-rw-r--r--   0        0        0     3915 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/libs/portalocker.py
+-rw-r--r--   0        0        0      925 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/locals.py
+-rw-r--r--   0        0        0     3084 2024-01-28 15:21:40.957985 emmett-2.5.9/emmett/logger.py
+-rw-r--r--   0        0        0      478 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/__init__.py
+-rw-r--r--   0        0        0     2373 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/_patches.py
+-rw-r--r--   0        0        0    12979 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/adapters.py
+-rw-r--r--   0        0        0     3224 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/apis.py
+-rw-r--r--   0        0        0     8857 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/base.py
+-rw-r--r--   0        0        0    12058 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/connection.py
+-rw-r--r--   0        0        0       80 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/engines/__init__.py
+-rw-r--r--   0        0        0     5577 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/engines/postgres.py
+-rw-r--r--   0        0        0     1191 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/engines/sqlite.py
+-rw-r--r--   0        0        0      605 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/errors.py
+-rw-r--r--   0        0        0     1677 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/geo.py
+-rw-r--r--   0        0        0    18102 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/helpers.py
+-rw-r--r--   0        0        0       62 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/__init__.py
+-rw-r--r--   0        0        0     2892 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/base.py
+-rw-r--r--   0        0        0    15289 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/commands.py
+-rw-r--r--   0        0        0    14381 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/engine.py
+-rw-r--r--   0        0        0     1058 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/exceptions.py
+-rw-r--r--   0        0        0    21829 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/generation.py
+-rw-r--r--   0        0        0     3636 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/helpers.py
+-rw-r--r--   0        0        0      491 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/migration.tmpl
+-rw-r--r--   0        0        0    23246 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/operations.py
+-rw-r--r--   0        0        0    14902 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/revisions.py
+-rw-r--r--   0        0        0    12034 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/scripts.py
+-rw-r--r--   0        0        0     1150 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/migrations/utils.py
+-rw-r--r--   0        0        0    46828 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/models.py
+-rw-r--r--   0        0        0    57286 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/objects.py
+-rw-r--r--   0        0        0     4208 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/transactions.py
+-rw-r--r--   0        0        0      978 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/orm/wrappers.py
+-rw-r--r--   0        0        0      917 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/parsers.py
+-rw-r--r--   0        0        0    12040 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/pipeline.py
+-rw-r--r--   0        0        0        0 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/routing/__init__.py
+-rw-r--r--   0        0        0     5303 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/routing/dispatchers.py
+-rw-r--r--   0        0        0     4112 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/routing/response.py
+-rw-r--r--   0        0        0    11518 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/routing/router.py
+-rw-r--r--   0        0        0     8479 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/routing/routes.py
+-rw-r--r--   0        0        0     7026 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/routing/rules.py
+-rw-r--r--   0        0        0     9704 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/routing/urls.py
+-rw-r--r--   0        0        0        0 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/rsgi/__init__.py
+-rw-r--r--   0        0        0     9973 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/rsgi/handlers.py
+-rw-r--r--   0        0        0      878 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/rsgi/helpers.py
+-rw-r--r--   0        0        0     4510 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/rsgi/wrappers.py
+-rw-r--r--   0        0        0     5490 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/security.py
+-rw-r--r--   0        0        0     2207 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/serializers.py
+-rw-r--r--   0        0        0     1050 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/server.py
+-rw-r--r--   0        0        0    11649 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/sessions.py
+-rw-r--r--   0        0        0        0 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/templating/__init__.py
+-rw-r--r--   0        0        0     1843 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/templating/lexers.py
+-rw-r--r--   0        0        0     1957 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/templating/templater.py
+-rw-r--r--   0        0        0       37 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/testing/__init__.py
+-rw-r--r--   0        0        0    11877 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/testing/client.py
+-rw-r--r--   0        0        0    10674 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/testing/env.py
+-rw-r--r--   0        0        0    12272 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/testing/helpers.py
+-rw-r--r--   0        0        0    15936 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/testing/urls.py
+-rw-r--r--   0        0        0      125 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/tools/__init__.py
+-rw-r--r--   0        0        0       52 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/tools/auth/__init__.py
+-rw-r--r--   0        0        0     9232 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/tools/auth/apis.py
+-rw-r--r--   0        0        0    19190 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/tools/auth/exposer.py
+-rw-r--r--   0        0        0    14033 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/tools/auth/ext.py
+-rw-r--r--   0        0        0     5270 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/tools/auth/forms.py
+-rw-r--r--   0        0        0     7485 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/tools/auth/models.py
+-rw-r--r--   0        0        0     1417 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/tools/decorators.py
+-rw-r--r--   0        0        0    10953 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/tools/mailer.py
+-rw-r--r--   0        0        0     1565 2024-01-28 15:21:40.961985 emmett-2.5.9/emmett/tools/service.py
+-rw-r--r--   0        0        0      355 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/typing.py
+-rw-r--r--   0        0        0     5357 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/utils.py
+-rw-r--r--   0        0        0    11554 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/validators/__init__.py
+-rw-r--r--   0        0        0     7636 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/validators/basic.py
+-rw-r--r--   0        0        0    31120 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/validators/consist.py
+-rw-r--r--   0        0        0    19038 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/validators/helpers.py
+-rw-r--r--   0        0        0     7367 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/validators/inside.py
+-rw-r--r--   0        0        0     4614 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/validators/process.py
+-rw-r--r--   0        0        0     2190 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/wrappers/__init__.py
+-rw-r--r--   0        0        0     2886 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/wrappers/helpers.py
+-rw-r--r--   0        0        0     4269 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/wrappers/request.py
+-rw-r--r--   0        0        0     1525 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/wrappers/response.py
+-rw-r--r--   0        0        0     1062 2024-01-28 15:21:40.965985 emmett-2.5.9/emmett/wrappers/websocket.py
+-rw-r--r--   0        0        0     2165 2024-01-28 15:21:40.965985 emmett-2.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1524 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/helpers.py
+-rw-r--r--   0        0        0       46 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/languages/de.json
+-rw-r--r--   0        0        0       49 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/languages/it.json
+-rw-r--r--   0        0        0       69 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/languages/ru.json
+-rw-r--r--   0        0        0      134 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/templates/auth/auth.html
+-rw-r--r--   0        0        0      479 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/templates/layout.html
+-rw-r--r--   0        0        0      153 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/templates/test.html
+-rw-r--r--   0        0        0     8027 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_auth.py
+-rw-r--r--   0        0        0     4658 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_cache.py
+-rw-r--r--   0        0        0     1415 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_http.py
+-rw-r--r--   0        0        0      861 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_logger.py
+-rw-r--r--   0        0        0    11854 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_mailer.py
+-rw-r--r--   0        0        0     8618 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_migrations.py
+-rw-r--r--   0        0        0    33038 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_orm.py
+-rw-r--r--   0        0        0      853 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_orm_connections.py
+-rw-r--r--   0        0        0    10074 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_orm_gis.py
+-rw-r--r--   0        0        0    22722 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_orm_pks.py
+-rw-r--r--   0        0        0     9863 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_orm_row.py
+-rw-r--r--   0        0        0     2958 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_orm_transactions.py
+-rw-r--r--   0        0        0    22478 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_pipeline.py
+-rw-r--r--   0        0        0     8659 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_routing.py
+-rw-r--r--   0        0        0     1475 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_session.py
+-rw-r--r--   0        0        0     2705 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_templates.py
+-rw-r--r--   0        0        0      622 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_translator.py
+-rw-r--r--   0        0        0     2045 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_utils.py
+-rw-r--r--   0        0        0    18633 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_validators.py
+-rw-r--r--   0        0        0      822 2024-01-28 15:21:40.965985 emmett-2.5.9/tests/test_wrappers.py
+-rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 emmett-2.5.9/PKG-INFO
```

### Comparing `emmett-2.5.8/CHANGES.md` & `emmett-2.5.9/CHANGES.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/LICENSE` & `emmett-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/README.md` & `emmett-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/app_and_modules.md` & `emmett-2.5.9/docs/app_and_modules.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/auth.md` & `emmett-2.5.9/docs/auth.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/caching.md` & `emmett-2.5.9/docs/caching.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/cli.md` & `emmett-2.5.9/docs/cli.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/debug_and_logging.md` & `emmett-2.5.9/docs/debug_and_logging.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/deployment.md` & `emmett-2.5.9/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/extensions.md` & `emmett-2.5.9/docs/extensions.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/foreword.md` & `emmett-2.5.9/docs/foreword.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/forms.md` & `emmett-2.5.9/docs/forms.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/installation.md` & `emmett-2.5.9/docs/installation.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/languages.md` & `emmett-2.5.9/docs/languages.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/mailer.md` & `emmett-2.5.9/docs/mailer.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/orm/advanced.md` & `emmett-2.5.9/docs/orm/advanced.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/orm/callbacks.md` & `emmett-2.5.9/docs/orm/callbacks.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/orm/connecting.md` & `emmett-2.5.9/docs/orm/connecting.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/orm/migrations.md` & `emmett-2.5.9/docs/orm/migrations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/orm/models.md` & `emmett-2.5.9/docs/orm/models.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/orm/operations.md` & `emmett-2.5.9/docs/orm/operations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/orm/relations.md` & `emmett-2.5.9/docs/orm/relations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/orm/scopes.md` & `emmett-2.5.9/docs/orm/scopes.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/orm/virtuals.md` & `emmett-2.5.9/docs/orm/virtuals.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/orm.md` & `emmett-2.5.9/docs/orm.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/patterns.md` & `emmett-2.5.9/docs/patterns.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/pipeline.md` & `emmett-2.5.9/docs/pipeline.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/quickstart.md` & `emmett-2.5.9/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/request.md` & `emmett-2.5.9/docs/request.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/response.md` & `emmett-2.5.9/docs/response.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/routing.md` & `emmett-2.5.9/docs/routing.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/services.md` & `emmett-2.5.9/docs/services.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/sessions.md` & `emmett-2.5.9/docs/sessions.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/templates.md` & `emmett-2.5.9/docs/templates.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/testing.md` & `emmett-2.5.9/docs/testing.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/tutorial.md` & `emmett-2.5.9/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/upgrading.md` & `emmett-2.5.9/docs/upgrading.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/validations.md` & `emmett-2.5.9/docs/validations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/docs/websocket.md` & `emmett-2.5.9/docs/websocket.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/_internal.py` & `emmett-2.5.9/emmett/_internal.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/_reloader.py` & `emmett-2.5.9/emmett/_reloader.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/_shortcuts.py` & `emmett-2.5.9/emmett/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/app.py` & `emmett-2.5.9/emmett/app.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/asgi/handlers.py` & `emmett-2.5.9/emmett/asgi/handlers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/asgi/typing.py` & `emmett-2.5.9/emmett/asgi/typing.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/asgi/workers.py` & `emmett-2.5.9/emmett/asgi/workers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/asgi/wrappers.py` & `emmett-2.5.9/emmett/asgi/wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/assets/debug/shBrushPython.js` & `emmett-2.5.9/emmett/assets/debug/shBrushPython.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/assets/debug/shCore.css` & `emmett-2.5.9/emmett/assets/debug/shCore.css`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/assets/debug/shCore.js` & `emmett-2.5.9/emmett/assets/debug/shCore.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/assets/debug/shTheme.css` & `emmett-2.5.9/emmett/assets/debug/shTheme.css`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/assets/debug/view.css` & `emmett-2.5.9/emmett/assets/debug/view.css`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/assets/debug/view.html` & `emmett-2.5.9/emmett/assets/debug/view.html`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/assets/helpers.js` & `emmett-2.5.9/emmett/assets/helpers.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/assets/jquery.min.js` & `emmett-2.5.9/emmett/assets/jquery.min.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/assets/jquery.min.map` & `emmett-2.5.9/emmett/assets/jquery.min.map`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/cache.py` & `emmett-2.5.9/emmett/cache.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/cli.py` & `emmett-2.5.9/emmett/cli.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/ctx.py` & `emmett-2.5.9/emmett/ctx.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/datastructures.py` & `emmett-2.5.9/emmett/datastructures.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/debug.py` & `emmett-2.5.9/emmett/debug.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/extensions.py` & `emmett-2.5.9/emmett/extensions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/forms.py` & `emmett-2.5.9/emmett/forms.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/helpers.py` & `emmett-2.5.9/emmett/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/html.py` & `emmett-2.5.9/emmett/html.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/http.py` & `emmett-2.5.9/emmett/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         try:
             stat_data = os.stat(self.file_path)
             if not stat.S_ISREG(stat_data.st_mode):
                 await HTTP(403).send(scope, send)
                 return
             self._headers.update(self._get_stat_headers(stat_data))
             await self._send_headers(send)
-            if 'http.response.pathsend' in scope['extensions']:
+            if 'http.response.pathsend' in scope.get('extensions', {}):
                 await send({
                     'type': 'http.response.pathsend',
                     'path': str(self.file_path)
                 })
             else:
                 await self._send_body(send)
         except IOError as e:
```

### Comparing `emmett-2.5.8/emmett/language/helpers.py` & `emmett-2.5.9/emmett/language/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/language/translator.py` & `emmett-2.5.9/emmett/language/translator.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/libs/contenttype.py` & `emmett-2.5.9/emmett/libs/contenttype.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/libs/portalocker.py` & `emmett-2.5.9/emmett/libs/portalocker.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/locals.py` & `emmett-2.5.9/emmett/locals.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/logger.py` & `emmett-2.5.9/emmett/logger.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/_patches.py` & `emmett-2.5.9/emmett/orm/_patches.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/adapters.py` & `emmett-2.5.9/emmett/orm/adapters.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/apis.py` & `emmett-2.5.9/emmett/orm/apis.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/base.py` & `emmett-2.5.9/emmett/orm/base.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/connection.py` & `emmett-2.5.9/emmett/orm/connection.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/engines/postgres.py` & `emmett-2.5.9/emmett/orm/engines/postgres.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/engines/sqlite.py` & `emmett-2.5.9/emmett/orm/engines/sqlite.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/errors.py` & `emmett-2.5.9/emmett/orm/errors.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/geo.py` & `emmett-2.5.9/emmett/orm/geo.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/helpers.py` & `emmett-2.5.9/emmett/orm/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/migrations/base.py` & `emmett-2.5.9/emmett/orm/migrations/base.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/migrations/commands.py` & `emmett-2.5.9/emmett/orm/migrations/commands.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/migrations/engine.py` & `emmett-2.5.9/emmett/orm/migrations/engine.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/migrations/exceptions.py` & `emmett-2.5.9/emmett/orm/migrations/exceptions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/migrations/generation.py` & `emmett-2.5.9/emmett/orm/migrations/generation.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/migrations/helpers.py` & `emmett-2.5.9/emmett/orm/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/migrations/operations.py` & `emmett-2.5.9/emmett/orm/migrations/operations.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/migrations/revisions.py` & `emmett-2.5.9/emmett/orm/migrations/revisions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/migrations/scripts.py` & `emmett-2.5.9/emmett/orm/migrations/scripts.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/migrations/utils.py` & `emmett-2.5.9/emmett/orm/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/models.py` & `emmett-2.5.9/emmett/orm/models.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/objects.py` & `emmett-2.5.9/emmett/orm/objects.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/transactions.py` & `emmett-2.5.9/emmett/orm/transactions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/orm/wrappers.py` & `emmett-2.5.9/emmett/orm/wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/parsers.py` & `emmett-2.5.9/emmett/parsers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/pipeline.py` & `emmett-2.5.9/emmett/pipeline.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/routing/dispatchers.py` & `emmett-2.5.9/emmett/routing/dispatchers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/routing/response.py` & `emmett-2.5.9/emmett/routing/response.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/routing/router.py` & `emmett-2.5.9/emmett/routing/router.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/routing/routes.py` & `emmett-2.5.9/emmett/routing/routes.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/routing/rules.py` & `emmett-2.5.9/emmett/routing/rules.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/routing/urls.py` & `emmett-2.5.9/emmett/routing/urls.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/rsgi/handlers.py` & `emmett-2.5.9/emmett/rsgi/handlers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/rsgi/helpers.py` & `emmett-2.5.9/emmett/rsgi/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/rsgi/wrappers.py` & `emmett-2.5.9/emmett/rsgi/wrappers.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,20 @@
         self.path = path
 
     @property
     def headers(self):
         return self._scope.headers
 
     @cachedprop
+    def host(self) -> str:
+        if self._scope.http_version[0] == '1':
+            return self.headers.get('host')
+        return self._scope.authority
+
+    @cachedprop
     def query_params(self) -> sdict[str, Union[str, List[str]]]:
         rv: sdict[str, Any] = sdict()
         for key, values in parse_qs(
             self._scope.query_string, keep_blank_values=True
         ).items():
             if len(values) == 1:
                 rv[key] = values[0]
```

### Comparing `emmett-2.5.8/emmett/security.py` & `emmett-2.5.9/emmett/security.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/serializers.py` & `emmett-2.5.9/emmett/serializers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/server.py` & `emmett-2.5.9/emmett/server.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/sessions.py` & `emmett-2.5.9/emmett/sessions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/templating/lexers.py` & `emmett-2.5.9/emmett/templating/lexers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/templating/templater.py` & `emmett-2.5.9/emmett/templating/templater.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/testing/client.py` & `emmett-2.5.9/emmett/testing/client.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/testing/env.py` & `emmett-2.5.9/emmett/testing/env.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/testing/helpers.py` & `emmett-2.5.9/emmett/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/testing/urls.py` & `emmett-2.5.9/emmett/testing/urls.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/tools/auth/apis.py` & `emmett-2.5.9/emmett/tools/auth/apis.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/tools/auth/exposer.py` & `emmett-2.5.9/emmett/tools/auth/exposer.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/tools/auth/ext.py` & `emmett-2.5.9/emmett/tools/auth/ext.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/tools/auth/forms.py` & `emmett-2.5.9/emmett/tools/auth/forms.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/tools/auth/models.py` & `emmett-2.5.9/emmett/tools/auth/models.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/tools/decorators.py` & `emmett-2.5.9/emmett/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/tools/mailer.py` & `emmett-2.5.9/emmett/tools/mailer.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/tools/service.py` & `emmett-2.5.9/emmett/tools/service.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/utils.py` & `emmett-2.5.9/emmett/utils.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/validators/__init__.py` & `emmett-2.5.9/emmett/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/validators/basic.py` & `emmett-2.5.9/emmett/validators/basic.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/validators/consist.py` & `emmett-2.5.9/emmett/validators/consist.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/validators/helpers.py` & `emmett-2.5.9/emmett/validators/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/validators/inside.py` & `emmett-2.5.9/emmett/validators/inside.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/validators/process.py` & `emmett-2.5.9/emmett/validators/process.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/wrappers/__init__.py` & `emmett-2.5.9/emmett/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/wrappers/helpers.py` & `emmett-2.5.9/emmett/wrappers/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/wrappers/request.py` & `emmett-2.5.9/emmett/wrappers/request.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/wrappers/response.py` & `emmett-2.5.9/emmett/wrappers/response.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/emmett/wrappers/websocket.py` & `emmett-2.5.9/emmett/wrappers/websocket.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/pyproject.toml` & `emmett-2.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "emmett"
 
 [tool.poetry]
 name = "emmett"
-version = "2.5.8"
+version = "2.5.9"
 description = "The web framework for inventors"
 authors = ["Giovanni Barillari <gi0baro@d4net.org>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://emmett.sh"
 repository = "https://github.com/emmett-framework/emmett"
@@ -43,15 +43,15 @@
 
 [tool.poetry.scripts]
 emmett = "emmett.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = ">=6.0"
-granian = "~1.0.0"
+granian = "~1.0.2"
 emmett-crypto = "^0.5"
 pendulum = "~3.0.0"
 pyDAL = "17.3"
 python-rapidjson = "^1.14"
 pyyaml = "^6.0"
 renoir = "^1.6"
 severus = "^1.1"
```

### Comparing `emmett-2.5.8/tests/helpers.py` & `emmett-2.5.9/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_auth.py` & `emmett-2.5.9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_cache.py` & `emmett-2.5.9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_http.py` & `emmett-2.5.9/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_logger.py` & `emmett-2.5.9/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_mailer.py` & `emmett-2.5.9/tests/test_mailer.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_migrations.py` & `emmett-2.5.9/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_orm.py` & `emmett-2.5.9/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_orm_connections.py` & `emmett-2.5.9/tests/test_orm_connections.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_orm_gis.py` & `emmett-2.5.9/tests/test_orm_gis.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_orm_pks.py` & `emmett-2.5.9/tests/test_orm_pks.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_orm_row.py` & `emmett-2.5.9/tests/test_orm_row.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_orm_transactions.py` & `emmett-2.5.9/tests/test_orm_transactions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_pipeline.py` & `emmett-2.5.9/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_routing.py` & `emmett-2.5.9/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_session.py` & `emmett-2.5.9/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_templates.py` & `emmett-2.5.9/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_translator.py` & `emmett-2.5.9/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_utils.py` & `emmett-2.5.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_validators.py` & `emmett-2.5.9/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/tests/test_wrappers.py` & `emmett-2.5.9/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.8/PKG-INFO` & `emmett-2.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett
-Version: 2.5.8
+Version: 2.5.9
 Summary: The web framework for inventors
 Home-page: https://emmett.sh
 License: BSD-3-Clause
 Keywords: web,asyncio
 Author: Giovanni Barillari
 Author-email: gi0baro@d4net.org
 Requires-Python: >=3.8,<4.0
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: orjson
 Provides-Extra: uvicorn
 Requires-Dist: click (>=6.0)
 Requires-Dist: emmett-crypto (>=0.5,<0.6)
-Requires-Dist: granian (>=1.0.0,<1.1.0)
+Requires-Dist: granian (>=1.0.2,<1.1.0)
 Requires-Dist: h11 (>=0.12.0) ; extra == "uvicorn"
 Requires-Dist: httptools (>=0.6.0,<0.7.0) ; (sys_platform != "win32") and (extra == "uvicorn")
 Requires-Dist: orjson (>=3.9,<3.10) ; extra == "orjson"
 Requires-Dist: pendulum (>=3.0.0,<3.1.0)
 Requires-Dist: pyDAL (==17.3)
 Requires-Dist: python-rapidjson (>=1.14,<2.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
```

