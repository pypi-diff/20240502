# Comparing `tmp/esmerald-3.1.2.tar.gz` & `tmp/esmerald-3.1.3.tar.gz`

## Comparing `esmerald-3.1.2.tar` & `esmerald-3.1.3.tar`

### file list

```diff
@@ -1,230 +1,230 @@
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/__main__.py
--rw-r--r--   0        0        0    91447 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/applications.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/concurrency.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/context.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/enums.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/exceptions.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/injector.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/logging.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/param_functions.py
--rw-r--r--   0        0        0    22336 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/params.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/py.typed
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/requests.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/staticfiles.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/testclient.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/types.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/typing.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/websockets.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/enums.py
--rw-r--r--   0        0        0    47597 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/app_template/v1/controllers.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/conf/directives/project_template/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/config/cors.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/config/csrf.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/config/jwt.py
--rw-r--r--   0        0        0    14614 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/config/openapi.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/config/session.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/config/static_files.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/edgy/__init__.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/edgy/base_user.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/edgy/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/mongoz/__init__.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/mongoz/base_user.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/mongoz/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/di/__init__.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/di/provider.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     8906 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/createdeployment.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/shell/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/shell/enums.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/shell/ipython.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/shell/ptpython.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/directives/operations/shell/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/urls/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/core/urls/base.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/datastructures/json.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/datastructures/msgspec.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/app_settings.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/cors.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/https.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/_internal.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/constants.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/docs.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/models.py
--rw-r--r--   0        0        0    20510 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/openapi.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/params.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/utils.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/security/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/security/base.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/security/api_key/__init__.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/security/api_key/base.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/security/http/__init__.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/security/http/base.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/security/oauth2/__init__.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/security/oauth2/base.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/security/openid_connect/__init__.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/openapi/security/openid_connect/base.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/permissions/base.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/protocols/template.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/responses/base.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/responses/json.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/__init__.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/_internal.py
--rw-r--r--   0        0        0    23674 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/base.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/events.py
--rw-r--r--   0        0        0    23680 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/gateways.py
--rw-r--r--   0        0        0   108795 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    72909 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/router.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/views.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/apis/__init__.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/apis/_metaclasses.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/apis/_mixins.py
--rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/apis/base.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/apis/generics.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/apis/views.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/webhooks/__init__.py
--rw-r--r--   0        0        0   106388 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/routing/webhooks/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/transformers/model.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/transformers/signature.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/transformers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/constants.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/helpers.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/inspect.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/models.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/pydantic/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esmerald-3.1.2/esmerald/utils/pydantic/schema.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 esmerald-3.1.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-3.1.2/LICENSE
--rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 esmerald-3.1.2/README.md
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 esmerald-3.1.2/pyproject.toml
--rw-r--r--   0        0        0    22667 2020-02-02 00:00:00.000000 esmerald-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/__main__.py
+-rw-r--r--   0        0        0    91447 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/applications.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/concurrency.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/context.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/enums.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/exceptions.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/injector.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/logging.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/param_functions.py
+-rw-r--r--   0        0        0    22336 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/params.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/py.typed
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/requests.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/testclient.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/types.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/typing.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/websockets.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    47620 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/v1/controllers.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/cors.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/csrf.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/jwt.py
+-rw-r--r--   0        0        0    14614 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/openapi.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/session.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/static_files.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/edgy/__init__.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/edgy/base_user.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/edgy/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/mongoz/__init__.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/mongoz/base_user.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/mongoz/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/di/__init__.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/di/provider.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     8906 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/createdeployment.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/enums.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/urls/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/urls/base.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/msgspec.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/app_settings.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/_internal.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/constants.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/docs.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/models.py
+-rw-r--r--   0        0        0    20526 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/openapi.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/params.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/base.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/api_key/__init__.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/api_key/base.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/http/__init__.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/http/base.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/oauth2/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/oauth2/base.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/openid_connect/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/openid_connect/base.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/template.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/responses/base.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/_internal.py
+-rw-r--r--   0        0        0    23730 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/events.py
+-rw-r--r--   0        0        0    23680 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0   108795 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    72909 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/router.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/views.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/__init__.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/_metaclasses.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/_mixins.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/base.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/generics.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/views.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/webhooks/__init__.py
+-rw-r--r--   0        0        0   106388 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/webhooks/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/constants.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/inspect.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/models.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/pydantic/schema.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 esmerald-3.1.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-3.1.3/LICENSE
+-rw-r--r--   0        0        0    17034 2020-02-02 00:00:00.000000 esmerald-3.1.3/README.md
+-rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 esmerald-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 esmerald-3.1.3/PKG-INFO
```

### Comparing `esmerald-3.1.2/esmerald/__init__.py` & `esmerald-3.1.3/esmerald/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.1.2"
+__version__ = "3.1.3"
 
 
 from lilya import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.context import Context
```

### Comparing `esmerald-3.1.2/esmerald/applications.py` & `esmerald-3.1.3/esmerald/applications.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/backgound.py` & `esmerald-3.1.3/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/context.py` & `esmerald-3.1.3/esmerald/context.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/enums.py` & `esmerald-3.1.3/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/exception_handlers.py` & `esmerald-3.1.3/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/exceptions.py` & `esmerald-3.1.3/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/injector.py` & `esmerald-3.1.3/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/logging.py` & `esmerald-3.1.3/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/params.py` & `esmerald-3.1.3/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/parsers.py` & `esmerald-3.1.3/esmerald/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     """
 
     model_config = ConfigDict(extra="allow")
 
 
 class ArbitraryBaseModel(BaseModel):
     """
-    ArbitratyBaseModel that allows arbitrary_types_allowed to be passed.
+    ArbitraryBaseModel that allows arbitrary_types_allowed to be passed.
     """
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
 class ArbitraryExtraBaseModel(BaseModel):
     model_config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
```

### Comparing `esmerald-3.1.2/esmerald/requests.py` & `esmerald-3.1.3/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/testclient.py` & `esmerald-3.1.3/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/types.py` & `esmerald-3.1.3/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/websockets.py` & `esmerald-3.1.3/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/__init__.py` & `esmerald-3.1.3/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/global_settings.py` & `esmerald-3.1.3/esmerald/conf/global_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 from openapi_schemas_pydantic.v3_1_0 import Contact, License, SecurityScheme
 from pydantic import AnyUrl
 from pydantic_settings import BaseSettings, SettingsConfigDict
 from typing_extensions import Annotated, Doc
 
 from esmerald import __version__
 from esmerald.conf.enums import EnvironmentType
-from esmerald.config import CORSConfig, CSRFConfig, OpenAPIConfig, SessionConfig, StaticFilesConfig
+from esmerald.config import (
+    CORSConfig,
+    CSRFConfig,
+    OpenAPIConfig,
+    SessionConfig,
+    StaticFilesConfig,
+)
 from esmerald.config.asyncexit import AsyncExitConfig
 from esmerald.datastructures import Secret
 from esmerald.interceptors.types import Interceptor
 from esmerald.permissions.types import Permission
 from esmerald.pluggables import Pluggable
 from esmerald.routing import gateways
 from esmerald.types import (
@@ -816,15 +822,15 @@
 
         ```python
         from esmerald import EsmeraldAPISettings
 
 
         class AppSettings(EsmeraldAPISettings):
             @property
-            def template_config(self) -> "TemplateConfig":
+            def template_config(self) -> TemplateConfig:
                 TemplateConfig(directory='templates', engine=MakoTemplateEngine)
         ```
         """
         return None
 
     @property
     def static_files_config(self) -> Optional[StaticFilesConfig]:
```

### Comparing `esmerald-3.1.2/esmerald/conf/directives/app_template/v1/controllers.py-tpl` & `esmerald-3.1.3/esmerald/conf/directives/app_template/v1/controllers.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl` & `esmerald-3.1.3/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl` & `esmerald-3.1.3/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl` & `esmerald-3.1.3/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl` & `esmerald-3.1.3/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl` & `esmerald-3.1.3/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/project_template/.gitignore.e-tpl` & `esmerald-3.1.3/esmerald/conf/directives/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/project_template/Makefile.e-tpl` & `esmerald-3.1.3/esmerald/conf/directives/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/main.py-tpl` & `esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/serve.py-tpl` & `esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/urls.py-tpl` & `esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl` & `esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/config/cors.py` & `esmerald-3.1.3/esmerald/config/cors.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/config/csrf.py` & `esmerald-3.1.3/esmerald/config/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/config/jwt.py` & `esmerald-3.1.3/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/config/openapi.py` & `esmerald-3.1.3/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/config/session.py` & `esmerald-3.1.3/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/config/static_files.py` & `esmerald-3.1.3/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/config/template.py` & `esmerald-3.1.3/esmerald/config/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/contrib/encoding.py` & `esmerald-3.1.3/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/contrib/auth/hashers.py` & `esmerald-3.1.3/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/contrib/auth/common/middleware.py` & `esmerald-3.1.3/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/contrib/auth/edgy/base_user.py` & `esmerald-3.1.3/esmerald/contrib/auth/edgy/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/contrib/auth/edgy/middleware.py` & `esmerald-3.1.3/esmerald/contrib/auth/edgy/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/contrib/auth/mongoz/base_user.py` & `esmerald-3.1.3/esmerald/contrib/auth/mongoz/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/contrib/auth/mongoz/middleware.py` & `esmerald-3.1.3/esmerald/contrib/auth/mongoz/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-3.1.3/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-3.1.3/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/di/provider.py` & `esmerald-3.1.3/esmerald/core/di/provider.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/cli.py` & `esmerald-3.1.3/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/env.py` & `esmerald-3.1.3/esmerald/core/directives/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     path: str
     app: typing.Union[Esmerald, ChildEsmerald]
 
 
 @dataclass
 class DirectiveEnv:
     """
-    Loads an arbitraty application into the object
+    Loads an arbitrary application into the object
     and returns the App.
     """
 
     path: typing.Optional[str] = None
     app: typing.Optional[typing.Union[Esmerald, ChildEsmerald]] = None
     command_path: typing.Optional[str] = None
 
@@ -73,15 +73,17 @@
 
     def _get_folders(self, path: Path) -> typing.List[str]:
         """
         Lists all the folders and checks if there is any file from the DISCOVERY_FILES available
         """
         return [directory.path for directory in os.scandir(path) if directory.is_dir()]
 
-    def _find_app_in_folder(self, path: Path, cwd: Path) -> typing.Union[Scaffold, None]:
+    def _find_app_in_folder(
+        self, path: Path, cwd: Path
+    ) -> typing.Union[Scaffold, None]:
         """
         Iterates inside the folder and looks up to the DISCOVERY_FILES.
         """
         for discovery_file in DISCOVERY_FILES:
             filename = f"{str(path)}/{discovery_file}"
             if not os.path.exists(filename):
                 continue
```

### Comparing `esmerald-3.1.2/esmerald/core/directives/templates.py` & `esmerald-3.1.3/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/utils.py` & `esmerald-3.1.3/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/createapp.py` & `esmerald-3.1.3/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/createdeployment.py` & `esmerald-3.1.3/esmerald/core/directives/operations/createdeployment.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/createproject.py` & `esmerald-3.1.3/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/list.py` & `esmerald-3.1.3/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/run.py` & `esmerald-3.1.3/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/runserver.py` & `esmerald-3.1.3/esmerald/core/directives/operations/runserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,36 +73,39 @@
     """Starts the Esmerald development server.
 
     The --app can be passed in the form of <module>.<submodule>:<app> or be set
     as environment variable ESMERALD_DEFAULT_APP.
 
     Alternatively, if none is passed, Esmerald will perform the application discovery.
 
-    It is strongly advised not to run this command in any pther environment but developmentyping.
-    This was designed to facilitate the development environment and should not be used in pr
+    It is strongly advised not to run this command in any other environment but development.
+    This was designed to facilitate the development environment and should not be used in production.
 
     How to run: `esmerald runserver`
     """
     if getattr(env, "app", None) is None:
         error = (
             "You cannot specify a custom directive without specifying the --app or setting "
             "ESMERALD_DEFAULT_APP environment variable."
         )
         printer.write_error(error)
         sys.exit(1)
 
     try:
         import uvicorn
     except ImportError:
-        raise DirectiveError(detail="Uvicorn needs to be installed to run Esmerald.") from None
+        raise DirectiveError(
+            detail="Uvicorn needs to be installed to run Esmerald."
+        ) from None
 
     app = env.app
     settings = app.settings
     message = terminal.write_info(
-        f"Starting {settings.environment} server @ {host}", colour=OutputColour.BRIGHT_CYAN
+        f"Starting {settings.environment} server @ {host}",
+        colour=OutputColour.BRIGHT_CYAN,
     )
     terminal.rule(message, align="center")
 
     if debug:
         app.debug = debug
 
     uvicorn.run(
```

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/show_urls.py` & `esmerald-3.1.3/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/shell/base.py` & `esmerald-3.1.3/esmerald/core/directives/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/shell/ipython.py` & `esmerald-3.1.3/esmerald/core/directives/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/shell/ptpython.py` & `esmerald-3.1.3/esmerald/core/directives/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/directives/operations/shell/utils.py` & `esmerald-3.1.3/esmerald/core/directives/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/terminal/base.py` & `esmerald-3.1.3/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/terminal/print.py` & `esmerald-3.1.3/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/terminal/terminal.py` & `esmerald-3.1.3/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/core/urls/base.py` & `esmerald-3.1.3/esmerald/core/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/datastructures/__init__.py` & `esmerald-3.1.3/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/datastructures/base.py` & `esmerald-3.1.3/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/datastructures/encoders.py` & `esmerald-3.1.3/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/datastructures/file.py` & `esmerald-3.1.3/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/datastructures/json.py` & `esmerald-3.1.3/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/datastructures/msgspec.py` & `esmerald-3.1.3/esmerald/datastructures/msgspec.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/datastructures/redirect.py` & `esmerald-3.1.3/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/datastructures/stream.py` & `esmerald-3.1.3/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/datastructures/template.py` & `esmerald-3.1.3/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/interceptors/interceptor.py` & `esmerald-3.1.3/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/middleware/__init__.py` & `esmerald-3.1.3/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/middleware/_exception_handlers.py` & `esmerald-3.1.3/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/middleware/app_settings.py` & `esmerald-3.1.3/esmerald/middleware/app_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/middleware/asyncexitstack.py` & `esmerald-3.1.3/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/middleware/authentication.py` & `esmerald-3.1.3/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/middleware/exceptions.py` & `esmerald-3.1.3/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/middleware/settings_middleware.py` & `esmerald-3.1.3/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/_internal.py` & `esmerald-3.1.3/esmerald/openapi/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/datastructures.py` & `esmerald-3.1.3/esmerald/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/docs.py` & `esmerald-3.1.3/esmerald/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/models.py` & `esmerald-3.1.3/esmerald/openapi/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/openapi.py` & `esmerald-3.1.3/esmerald/openapi/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         )
 
         if field_info.description:
             parameter.description = field_info.description
         if field_info.examples is not None:
             parameter.example = json.dumps(field_info.examples)
         if field_info.deprecated:
-            parameter.deprecated = field_info.deprecated
+            parameter.deprecated = field_info.deprecated  # type: ignore
 
         parameters.append(parameter.model_dump(by_alias=True))
     return parameters
 
 
 def get_openapi_operation_request_body(
     *,
```

### Comparing `esmerald-3.1.2/esmerald/openapi/responses.py` & `esmerald-3.1.3/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/utils.py` & `esmerald-3.1.3/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/validation.py` & `esmerald-3.1.3/esmerald/openapi/validation.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/security/base.py` & `esmerald-3.1.3/esmerald/openapi/security/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/security/api_key/base.py` & `esmerald-3.1.3/esmerald/openapi/security/api_key/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/security/http/base.py` & `esmerald-3.1.3/esmerald/openapi/security/http/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/security/oauth2/base.py` & `esmerald-3.1.3/esmerald/openapi/security/oauth2/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/openapi/security/openid_connect/base.py` & `esmerald-3.1.3/esmerald/openapi/security/openid_connect/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/permissions/base.py` & `esmerald-3.1.3/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/permissions/utils.py` & `esmerald-3.1.3/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/pluggables/base.py` & `esmerald-3.1.3/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/protocols/asyncdao.py` & `esmerald-3.1.3/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/protocols/dao.py` & `esmerald-3.1.3/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/protocols/interceptor.py` & `esmerald-3.1.3/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/protocols/template.py` & `esmerald-3.1.3/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/responses/base.py` & `esmerald-3.1.3/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/responses/encoders.py` & `esmerald-3.1.3/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/responses/json.py` & `esmerald-3.1.3/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/responses/template.py` & `esmerald-3.1.3/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/_internal.py` & `esmerald-3.1.3/esmerald/routing/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/base.py` & `esmerald-3.1.3/esmerald/routing/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,18 @@
 from esmerald.enums import MediaType
 from esmerald.exceptions import ImproperlyConfigured
 from esmerald.injector import Inject
 from esmerald.permissions.utils import continue_or_raise_permission_exception
 from esmerald.requests import Request
 from esmerald.responses import JSONResponse, Response
 from esmerald.routing.apis.base import View
-from esmerald.transformers.model import TransformerModel
+from esmerald.transformers.model import (
+    TransformerModel,
+    create_signature as transfomer_create_signature,
+)
 from esmerald.transformers.signature import SignatureFactory
 from esmerald.transformers.utils import get_signature
 from esmerald.typing import Void, VoidType
 from esmerald.utils.constants import DATA, PAYLOAD
 from esmerald.utils.helpers import is_async_callable, is_class_and_subclass
 from esmerald.utils.sync import AsyncCallable
 
@@ -137,15 +140,15 @@
             self.websocket_parameter_model = transformer_model
 
     def create_handler_transformer_model(self) -> "TransformerModel":
         """Method to create a TransformerModel for a given handler."""
         dependencies = self.get_dependencies()
         signature_model = get_signature(self)
 
-        return TransformerModel.create_signature(
+        return transfomer_create_signature(
             signature_model=signature_model,
             dependencies=dependencies,
             path_parameters=self.path_parameters,
         )
 
 
 class BaseResponseHandler:
```

### Comparing `esmerald-3.1.2/esmerald/routing/events.py` & `esmerald-3.1.3/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/gateways.py` & `esmerald-3.1.3/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/handlers.py` & `esmerald-3.1.3/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/router.py` & `esmerald-3.1.3/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/apis/_metaclasses.py` & `esmerald-3.1.3/esmerald/routing/apis/_metaclasses.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/apis/_mixins.py` & `esmerald-3.1.3/esmerald/routing/apis/_mixins.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/apis/base.py` & `esmerald-3.1.3/esmerald/routing/apis/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/apis/generics.py` & `esmerald-3.1.3/esmerald/routing/apis/generics.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/apis/views.py` & `esmerald-3.1.3/esmerald/routing/apis/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/routing/webhooks/handlers.py` & `esmerald-3.1.3/esmerald/routing/webhooks/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/security/jwt/token.py` & `esmerald-3.1.3/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/template/jinja.py` & `esmerald-3.1.3/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/template/mako.py` & `esmerald-3.1.3/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/transformers/datastructures.py` & `esmerald-3.1.3/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/transformers/model.py` & `esmerald-3.1.3/esmerald/transformers/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,204 +71,14 @@
 
     def get_query_params(self) -> Set[ParamSetting]:
         return self.query_params
 
     def get_header_params(self) -> Set[ParamSetting]:
         return self.headers
 
-    @classmethod
-    def dependency_tree(cls, key: str, dependencies: "Dependencies") -> Dependency:
-        inject = dependencies[key]
-        dependency_keys = [
-            key for key in get_signature(inject).model_fields if key in dependencies
-        ]
-        return Dependency(
-            key=key,
-            inject=inject,
-            dependencies=[
-                cls.dependency_tree(key=key, dependencies=dependencies) for key in dependency_keys
-            ],
-        )
-
-    @classmethod
-    def get_parameter_settings(
-        cls,
-        path_parameters: Set[str],
-        dependencies: "Dependencies",
-        signature_fields: Dict[str, FieldInfo],
-    ) -> Tuple[Set[ParamSetting], set]:
-        _dependencies = set()
-
-        for key in dependencies:
-            if key in signature_fields:
-                _dependencies.add(cls.dependency_tree(key=key, dependencies=dependencies))
-
-        ignored_keys = {
-            *RESERVED_KWARGS,
-            *(dependency.key for dependency in _dependencies),
-        }
-
-        parameter_definitions = set()
-        for field_name, model_field in signature_fields.items():
-            if field_name not in ignored_keys:
-                allow_none = getattr(model_field, "allow_none", True)
-                parameter_definitions.add(
-                    create_parameter_setting(
-                        allow_none=allow_none,
-                        field_name=field_name,
-                        field_info=model_field,
-                        path_parameters=path_parameters,
-                    )
-                )
-
-        filtered = [item for item in signature_fields.items() if item[0] not in ignored_keys]
-        for field_name, model_field in filtered:
-            signature_field = model_field
-            allow_none = getattr(signature_field, "allow_none", True)
-            parameter_definitions.add(
-                create_parameter_setting(
-                    allow_none=allow_none,
-                    field_name=field_name,
-                    field_info=signature_field,
-                    path_parameters=path_parameters,
-                )
-            )
-
-        return parameter_definitions, _dependencies
-
-    @classmethod
-    def create_signature(
-        cls,
-        signature_model: Type[SignatureModel],
-        dependencies: "Dependencies",
-        path_parameters: Set[str],
-    ) -> "TransformerModel":
-        cls.validate_kwargs(
-            path_parameters=path_parameters,
-            dependencies=dependencies,
-            model_fields=signature_model.model_fields,
-        )
-
-        reserved_kwargs = set()
-
-        for field_name in signature_model.model_fields:
-            if field_name in RESERVED_KWARGS:
-                reserved_kwargs.add(field_name)
-
-        param_settings, _dependencies = cls.get_parameter_settings(
-            path_parameters=path_parameters,
-            dependencies=dependencies,
-            signature_fields=signature_model.model_fields,
-        )
-
-        path_params = set()
-        for param in param_settings:
-            if param.param_type == ParamType.PATH:
-                path_params.add(param)
-
-        headers = set()
-        for param in param_settings:
-            if param.param_type == ParamType.HEADER:
-                headers.add(param)
-
-        cookies = set()
-        for param in param_settings:
-            if param.param_type == ParamType.COOKIE:
-                cookies.add(param)
-
-        query_params = set()
-        for param in param_settings:
-            if param.param_type == ParamType.QUERY:
-                query_params.add(param)
-
-        query_params_names: Set[ParamSetting] = set()
-
-        form_data = None
-
-        # For the reserved keyword data
-        data_field = signature_model.model_fields.get(DATA) or signature_model.model_fields.get(
-            PAYLOAD
-        )
-        if data_field:
-            extra = getattr(data_field, "json_schema_extra", None) or {}
-            media_type = extra.get("media_type")
-            if media_type in MEDIA_TYPES:
-                form_data = (media_type, data_field)
-
-        (
-            path_params,
-            query_params,
-            cookies,
-            headers,
-            reserved_kwargs,
-        ) = cls.update_parameters(
-            global_dependencies=dependencies,
-            local_dependencies=_dependencies,
-            path_params=path_params,
-            query_params=query_params,
-            cookies=cookies,
-            headers=headers,
-            reserved_kwargs=reserved_kwargs,
-            path_parameters=path_parameters,
-            form_data=form_data,
-        )
-
-        is_optional = False
-        if DATA in reserved_kwargs and PAYLOAD in reserved_kwargs:
-            raise ImproperlyConfigured("Only 'data' or 'payload' must be provided but not both.")
-
-        if DATA in reserved_kwargs:
-            is_optional = is_field_optional(signature_model.model_fields["data"])
-        elif PAYLOAD in reserved_kwargs:
-            is_optional = is_field_optional(signature_model.model_fields["payload"])
-
-        return TransformerModel(
-            form_data=form_data,
-            dependencies=_dependencies,
-            path_params=path_params,
-            query_params=query_params,
-            cookies=cookies,
-            headers=headers,
-            reserved_kwargs=reserved_kwargs,
-            query_param_names=query_params_names,
-            is_optional=is_optional,
-        )
-
-    @classmethod
-    def update_parameters(
-        cls,
-        global_dependencies: "Dependencies",
-        local_dependencies: Set["Dependency"],
-        path_params: Any,
-        query_params: Any,
-        cookies: Any,
-        headers: Any,
-        reserved_kwargs: Any,
-        path_parameters: Any,
-        form_data: Any,
-    ) -> Tuple[Any, Any, Any, Any, Any]:
-        for dependency in local_dependencies:
-            dependency_model = cls.create_signature(
-                signature_model=get_signature(dependency.inject),
-                dependencies=global_dependencies,
-                path_parameters=path_parameters,
-            )
-            path_params = merge_sets(path_params, dependency_model.path_params)
-            query_params = merge_sets(query_params, dependency_model.query_params)
-            cookies = merge_sets(cookies, dependency_model.cookies)
-            headers = merge_sets(headers, dependency_model.headers)
-
-            if DATA in reserved_kwargs and DATA in dependency_model.reserved_kwargs:
-                cls.validate_data(form_data, dependency_model)  # pragma: no cover
-            elif PAYLOAD in reserved_kwargs and PAYLOAD in dependency_model.reserved_kwargs:
-                cls.validate_data(form_data, dependency_model)  # pragma: no cover
-            reserved_kwargs.update(dependency_model.reserved_kwargs)
-
-        return path_params, query_params, cookies, headers, reserved_kwargs
-
     def to_kwargs(
         self,
         connection: Union["WebSocket", "Request"],
         handler: Union["HTTPHandler", "WebSocketHandler"] = None,
     ) -> Any:
         connection_params = {}
         for key, value in connection.query_params.items():
@@ -342,75 +152,14 @@
         if "query" in self.reserved_kwargs:
             reserved_kwargs["query"] = connection_params
         if "state" in self.reserved_kwargs:
             reserved_kwargs["state"] = connection.app.state.copy()  # pragma: no cover
 
         return {**reserved_kwargs, **path_params, **query_params, **headers, **cookies}
 
-    @classmethod
-    def validate_data(
-        cls,
-        form_data: Optional[Tuple[EncodingType, FieldInfo]],
-        dependency_model: "TransformerModel",
-    ) -> None:  # pragma: no cover
-        if form_data and dependency_model.form_data:
-            media_type, _ = form_data
-            dependency_media_type, _ = dependency_model.form_data
-            if media_type != dependency_media_type:
-                raise ImproperlyConfigured(
-                    "Dependencies have incompatible form-data encoding. "
-                    "They should both be the same. Either url-encoded or multi-part."
-                )
-        if (
-            (form_data and not dependency_model.form_data)
-            or not form_data
-            and dependency_model.form_data
-        ):
-            raise ImproperlyConfigured(
-                "Dependencies haev incompativle 'data' kwarg types. "
-                "One expects JSON and the other expects form-data."
-            )
-
-    @classmethod
-    def validate_kwargs(
-        cls,
-        path_parameters: Set[str],
-        dependencies: "Dependencies",
-        model_fields: Dict[str, FieldInfo],
-    ) -> None:  # pragma: no cover
-        keys = set(dependencies.keys())
-        names = set()
-
-        for key, value in model_fields.items():
-            if value.json_schema_extra is not None:
-                extra = cast("Dict[str, Any]", value.json_schema_extra)
-                if (
-                    extra.get(ParamType.QUERY)
-                    or extra.get(ParamType.HEADER)
-                    or extra.get(ParamType.COOKIE)
-                ):
-                    names.add(key)
-
-        for intersect in [
-            path_parameters.intersection(keys)
-            or path_parameters.intersection(names)
-            or keys.intersection(names)
-        ]:
-            if intersect:
-                raise ImproperlyConfigured(
-                    f"Ambiguity in kwarg resolution: {', '.join(intersect)}. "
-                    f"Please make sure to use unique distinct keys for your dependencies and path parameters."
-                )
-
-        reserved_kwargs = {*names, *path_parameters, *keys}.intersection(RESERVED_KWARGS)
-        if reserved_kwargs:
-            raise ImproperlyConfigured(
-                f"Kwargs ({', '.join(RESERVED_KWARGS)}) cannot be used for parameters and/or dependencies."
-            )
-
     async def get_request_data(self, request: "Request") -> Any:
         # Fast exit principle
         if not self.form_data:
             return await request.json()
 
         media_type, field = self.form_data
         form_data = await request.form()
@@ -436,7 +185,402 @@
             kwargs[_dependency.key] = await self.get_dependencies(
                 dependency=_dependency, connection=connection, **kwargs
             )
         dependency_kwargs = signature_model.parse_values_for_connection(
             connection=connection, **kwargs
         )
         return await dependency.inject(**dependency_kwargs)
+
+
+def dependency_tree(key: str, dependencies: "Dependencies") -> Dependency:
+    inject = dependencies[key]
+    dependency_keys = [key for key in get_signature(inject).model_fields if key in dependencies]
+    return Dependency(
+        key=key,
+        inject=inject,
+        dependencies=[
+            dependency_tree(key=key, dependencies=dependencies) for key in dependency_keys
+        ],
+    )
+
+
+def get_parameter_settings(
+    path_parameters: Set[str], dependencies: Dict[str, Any], signature_fields: Dict[str, Any]
+) -> Tuple[Set[ParamSetting], Set["Dependency"]]:
+    """
+    Get parameter settings and dependencies for given inputs.
+
+    Args:
+        path_parameters (set): Set of path parameters.
+        dependencies (dict): Dependency information.
+        signature_fields (dict): Dictionary containing field information.
+
+    Returns:
+        tuple: A tuple containing sets of parameter settings and dependencies.
+    """
+
+    # Set to store dependencies
+    _dependencies: Any = set()
+
+    # Set to store ignored keys
+    ignored_keys = {
+        *RESERVED_KWARGS,
+        *(dependency.key for dependency in _dependencies),
+    }
+
+    # Set to store parameter definitions
+    parameter_definitions = set()
+
+    # Iterate through dependencies to add relevant dependencies
+    for key in dependencies:
+        if key in signature_fields:
+            _dependencies.add(dependency_tree(key=key, dependencies=dependencies))
+
+    # Iterate through signature fields to create parameter settings
+    for field_name, model_field in signature_fields.items():
+        if field_name not in ignored_keys:
+            allow_none = getattr(model_field, "allow_none", True)
+            parameter_definitions.add(
+                create_parameter_setting(
+                    allow_none=allow_none,
+                    field_name=field_name,
+                    field_info=model_field,
+                    path_parameters=path_parameters,
+                )
+            )
+
+    # Filter out ignored keys and create parameter settings
+    filtered = [
+        (field_name, model_field)
+        for field_name, model_field in signature_fields.items()
+        if field_name not in ignored_keys
+    ]
+    for field_name, model_field in filtered:
+        signature_field = model_field
+        allow_none = getattr(signature_field, "allow_none", True)
+        parameter_definitions.add(
+            create_parameter_setting(
+                allow_none=allow_none,
+                field_name=field_name,
+                field_info=signature_field,
+                path_parameters=path_parameters,
+            )
+        )
+
+    return parameter_definitions, _dependencies
+
+
+def _filter_param_settings_by_type(
+    param_settings: Set[ParamSetting], param_type: ParamType
+) -> Set[ParamSetting]:
+    """
+    Filter parameter settings by parameter type.
+
+    Args:
+        param_settings (Set[ParamSetting]): Set of parameter settings.
+        param_type (ParamType): Parameter type to filter.
+
+    Returns:
+        Set[ParamSetting]: Filtered parameter settings.
+    """
+    return {param for param in param_settings if param.param_type == param_type}
+
+
+def _get_form_data(
+    signature_model: Type[SignatureModel],
+) -> Optional[Tuple["EncodingType", "FieldInfo"]]:
+    """
+    Get form data from the signature model.
+
+    Args:
+        signature_model (Type[SignatureModel]): The signature model.
+
+    Returns:
+        Optional[Tuple[str, Any]]: Tuple containing media type and data field, or None.
+    """
+    data_field = signature_model.model_fields.get(DATA) or signature_model.model_fields.get(
+        PAYLOAD
+    )
+    if data_field:
+        extra = getattr(data_field, "json_schema_extra", None) or {}
+        media_type = extra.get("media_type")
+        if media_type in MEDIA_TYPES:
+            return media_type, data_field
+    return None
+
+
+def create_signature(
+    signature_model: Type[SignatureModel],
+    dependencies: "Dependencies",
+    path_parameters: Set[str],
+) -> "TransformerModel":
+    """
+    Create a transformer model based on the signature model.
+
+    Args:
+        signature_model (Type[SignatureModel]): The signature model.
+        dependencies (Dependencies): Dependency information.
+        path_parameters (Set[str]): Set of path parameters.
+
+    Returns:
+        TransformerModel: The created transformer model.
+    """
+    validate_kwargs(
+        path_parameters=path_parameters,
+        dependencies=dependencies,
+        model_fields=signature_model.model_fields,
+    )
+
+    reserved_kwargs = {
+        field_name for field_name in signature_model.model_fields if field_name in RESERVED_KWARGS
+    }
+
+    param_settings, _dependencies = get_parameter_settings(
+        path_parameters=path_parameters,
+        dependencies=dependencies,
+        signature_fields=signature_model.model_fields,
+    )
+
+    path_params = _filter_param_settings_by_type(param_settings, ParamType.PATH)
+    query_params = _filter_param_settings_by_type(param_settings, ParamType.QUERY)
+    cookies = _filter_param_settings_by_type(param_settings, ParamType.COOKIE)
+    headers = _filter_param_settings_by_type(param_settings, ParamType.HEADER)
+
+    form_data: Union[Tuple["EncodingType", "FieldInfo"], None] = _get_form_data(signature_model)
+
+    # Update parameters
+    (
+        path_params,
+        query_params,
+        cookies,
+        headers,
+        reserved_kwargs,
+    ) = update_parameters(
+        global_dependencies=dependencies,
+        local_dependencies=_dependencies,
+        path_params=path_params,
+        query_params=query_params,
+        cookies=cookies,
+        headers=headers,
+        reserved_kwargs=reserved_kwargs,
+        path_parameters=path_parameters,
+        form_data=form_data,
+    )
+
+    is_optional = False
+    if DATA in reserved_kwargs and PAYLOAD in reserved_kwargs:
+        raise ImproperlyConfigured("Only 'data' or 'payload' must be provided but not both.")
+
+    if DATA in reserved_kwargs:
+        is_optional = is_field_optional(signature_model.model_fields["data"])
+    elif PAYLOAD in reserved_kwargs:
+        is_optional = is_field_optional(signature_model.model_fields["payload"])
+
+    query_param_names: Any = set()
+    return TransformerModel(
+        form_data=form_data,
+        dependencies=_dependencies,
+        path_params=path_params,
+        query_params=query_params,
+        cookies=cookies,
+        headers=headers,
+        reserved_kwargs=reserved_kwargs,
+        query_param_names=query_param_names,
+        is_optional=is_optional,
+    )
+
+
+def _update_parameters_with_dependency(
+    dependency: "Dependency",
+    global_dependencies: "Dependencies",
+    path_params: Any,
+    query_params: Any,
+    cookies: Any,
+    headers: Any,
+    reserved_kwargs: Any,
+    path_parameters: Any,
+    form_data: Any,
+) -> Tuple[Any, Any, Any, Any, Any]:
+    """
+    Update parameters based on a dependency.
+
+    Args:
+        dependency (Dependency): The dependency to process.
+        global_dependencies (Dependencies): Global dependency information.
+        path_params (Any): Existing path parameters.
+        query_params (Any): Existing query parameters.
+        cookies (Any): Existing cookies.
+        headers (Any): Existing headers.
+        reserved_kwargs (Any): Existing reserved keywords.
+        path_parameters (Any): Path parameters.
+        form_data (Any): Form data.
+
+    Returns:
+        Tuple[Any, Any, Any, Any, Any]: Updated parameters.
+    """
+    dependency_model = create_signature(
+        signature_model=get_signature(dependency.inject),
+        dependencies=global_dependencies,
+        path_parameters=path_parameters,
+    )
+    path_params = merge_sets(path_params, dependency_model.path_params)
+    query_params = merge_sets(query_params, dependency_model.query_params)
+    cookies = merge_sets(cookies, dependency_model.cookies)
+    headers = merge_sets(headers, dependency_model.headers)
+
+    if DATA in reserved_kwargs and DATA in dependency_model.reserved_kwargs:
+        validate_data(form_data, dependency_model)
+    elif PAYLOAD in reserved_kwargs and PAYLOAD in dependency_model.reserved_kwargs:
+        validate_data(form_data, dependency_model)
+    reserved_kwargs.update(dependency_model.reserved_kwargs)
+
+    return path_params, query_params, cookies, headers, reserved_kwargs
+
+
+def update_parameters(
+    global_dependencies: "Dependencies",
+    local_dependencies: Set["Dependency"],
+    path_params: Any,
+    query_params: Any,
+    cookies: Any,
+    headers: Any,
+    reserved_kwargs: Any,
+    path_parameters: Any,
+    form_data: Any,
+) -> Tuple[Any, Any, Any, Any, Any]:
+    """
+    Update parameters with local dependencies.
+
+    Args:
+        global_dependencies (Dependencies): Global dependency information.
+        local_dependencies (Set[Dependency]): Local dependency set.
+        path_params (Any): Existing path parameters.
+        query_params (Any): Existing query parameters.
+        cookies (Any): Existing cookies.
+        headers (Any): Existing headers.
+        reserved_kwargs (Any): Existing reserved keywords.
+        path_parameters (Any): Path parameters.
+        form_data (Any): Form data.
+
+    Returns:
+        Tuple[Any, Any, Any, Any, Any]: Updated parameters.
+    """
+    for dependency in local_dependencies:
+        path_params, query_params, cookies, headers, reserved_kwargs = (
+            _update_parameters_with_dependency(
+                dependency,
+                global_dependencies,
+                path_params,
+                query_params,
+                cookies,
+                headers,
+                reserved_kwargs,
+                path_parameters,
+                form_data,
+            )
+        )
+
+    return path_params, query_params, cookies, headers, reserved_kwargs
+
+
+def validate_data(
+    form_data: Optional[Tuple[EncodingType, FieldInfo]],
+    dependency_model: "TransformerModel",
+) -> None:  # pragma: no cover
+    if form_data and dependency_model.form_data:
+        media_type, _ = form_data
+        dependency_media_type, _ = dependency_model.form_data
+        if media_type != dependency_media_type:
+            raise ImproperlyConfigured(
+                "Dependencies have incompatible form-data encoding. "
+                "They should both be the same. Either url-encoded or multi-part."
+            )
+    if (
+        (form_data and not dependency_model.form_data)
+        or not form_data
+        and dependency_model.form_data
+    ):
+        raise ImproperlyConfigured(
+            "Dependencies haev incompativle 'data' kwarg types. "
+            "One expects JSON and the other expects form-data."
+        )
+
+
+def _get_names_from_model_fields(model_fields: Dict[str, FieldInfo]) -> Set[str]:
+    """
+    Extract names from model fields.
+
+    Args:
+        model_fields (Dict[str, FieldInfo]): Dictionary of model fields.
+
+    Returns:
+        Set[str]: Set of names extracted from model fields.
+    """
+    names = set()
+    for key, value in model_fields.items():
+        if value.json_schema_extra is not None:
+            extra = cast("Dict[str, Any]", value.json_schema_extra)
+            if (
+                extra.get(ParamType.QUERY)
+                or extra.get(ParamType.HEADER)
+                or extra.get(ParamType.COOKIE)
+            ):
+                names.add(key)
+    return names
+
+
+def _check_ambiguity_in_kwargs(
+    path_parameters: Set[str], dependencies: "Dependencies", model_fields: Dict[str, FieldInfo]
+) -> None:
+    """
+    Check ambiguity in keyword argument resolution.
+
+    Args:
+        path_parameters (Set[str]): Set of path parameters.
+        dependencies (Dependencies): Dependency information.
+        model_fields (Dict[str, FieldInfo]): Dictionary of model fields.
+
+    Raises:
+        ImproperlyConfigured: If ambiguity in keyword argument resolution is detected.
+    """
+    keys = set(dependencies.keys())
+    names = _get_names_from_model_fields(model_fields)
+
+    intersection = (
+        path_parameters.intersection(keys)
+        or path_parameters.intersection(names)
+        or keys.intersection(names)
+    )
+    if intersection:
+        raise ImproperlyConfigured(
+            f"Ambiguity in kwarg resolution: {', '.join(intersection)}. "
+            f"Please make sure to use unique distinct keys for your dependencies and path parameters."
+        )
+
+
+def validate_kwargs(
+    path_parameters: Set[str],
+    dependencies: "Dependencies",
+    model_fields: Dict[str, FieldInfo],
+) -> None:
+    """
+    Validate keyword arguments.
+
+    Args:
+        path_parameters (Set[str]): Set of path parameters.
+        dependencies (Dependencies): Dependency information.
+        model_fields (Dict[str, FieldInfo]): Dictionary of model fields.
+
+    Raises:
+        ImproperlyConfigured: If keyword arguments are invalid.
+    """
+    _check_ambiguity_in_kwargs(path_parameters, dependencies, model_fields)
+
+    reserved_kwargs = {
+        *_get_names_from_model_fields(model_fields),
+        *path_parameters,
+        *dependencies.keys(),
+    }.intersection(RESERVED_KWARGS)
+    if reserved_kwargs:
+        raise ImproperlyConfigured(
+            f"Kwargs ({', '.join(RESERVED_KWARGS)}) cannot be used for parameters and/or dependencies."
+        )
```

### Comparing `esmerald-3.1.2/esmerald/transformers/signature.py` & `esmerald-3.1.3/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/utils/constants.py` & `esmerald-3.1.3/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/utils/dependency.py` & `esmerald-3.1.3/esmerald/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/utils/functional.py` & `esmerald-3.1.3/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/utils/helpers.py` & `esmerald-3.1.3/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/utils/models.py` & `esmerald-3.1.3/esmerald/utils/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/utils/sync.py` & `esmerald-3.1.3/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/esmerald/utils/pydantic/schema.py` & `esmerald-3.1.3/esmerald/utils/pydantic/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/LICENSE` & `esmerald-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.2/README.md` & `esmerald-3.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -181,19 +181,19 @@
 Once the application is up, all the routes are mounted and therefore the url paths are defined.
 Esmerald encourages standard practices and design in mind which means that any application, big or small,
 custom or enterprise, fits within Esmerald ecosystem without scalability issues.
 
 ## Settings
 
 Like every other framework, when starting an application, a lot of [settings](./application/settings.md) can/need to be
-passed to the main object and this can be very dauting and hugly to maintain and see.
+passed to the main object and this can be very dauting and ugly to maintain and see.
 
 Esmerald comes with the
 [settings](./application/settings.md) in mind. A set of defaults that can be overridden by your very own settings
-module but not limited to it as you can still use the classic approach of passing everything into a
+module but not limited to it, as you can still use the classic approach of passing everything into a
 Esmerald instance directly when instantiating.
 
 **Example of classic approach**:
 
 ```python
 from example import ExampleObject
 
@@ -247,15 +247,15 @@
 
 ```python
 
 from esmerald import EsmeraldAPISettings
 from esmerald.conf.enums import EnvironmentType
 
 class Development(EsmeraldAPISettings):
-    app_name: bool = 'My app in dev'
+    app_name: str = 'My app in dev'
     environment: str = EnvironmentType.DEVELOPMENT
 
 ```
 
 **Load the settings into your Esmerald application**:
 
 Assuming your Esmerald app is inside an `src/app.py`.
@@ -481,15 +481,15 @@
 
 app = Esmerald(routes=[Include('src.urls')])
 
 ```
 
 ## Run the application
 
-As mentioned before, we recomment uvicorn for production but it's not mandatory.
+As mentioned before, we recommend uvicorn for production but it's not mandatory.
 
 **Using uvicorn**:
 
 ```shell
 uvicorn src:app --reload
 
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
```

#### html2text {}

```diff
@@ -80,17 +80,17 @@
 hood. The reason behind this decison comes with the fact that performance is
 there and no issues with routing. Once the application is up, all the routes
 are mounted and therefore the url paths are defined. Esmerald encourages
 standard practices and design in mind which means that any application, big or
 small, custom or enterprise, fits within Esmerald ecosystem without scalability
 issues. ## Settings Like every other framework, when starting an application, a
 lot of [settings](./application/settings.md) can/need to be passed to the main
-object and this can be very dauting and hugly to maintain and see. Esmerald
+object and this can be very dauting and ugly to maintain and see. Esmerald
 comes with the [settings](./application/settings.md) in mind. A set of defaults
-that can be overridden by your very own settings module but not limited to it
+that can be overridden by your very own settings module but not limited to it,
 as you can still use the classic approach of passing everything into a Esmerald
 instance directly when instantiating. **Example of classic approach**:
 ```python from example import ExampleObject # ExampleObject is an instance of
 another application # and it serves only for example app = ExampleObject
 (setting_one=..., setting_two=..., setting_three=...) ``` Inspired by the great
 [Django](https://www.djangoproject.com/) and using pydantic, Esmerald has a
 default object ready to be used out-of-the-box. **Esmerald**: ```python from
@@ -106,15 +106,15 @@
 start. ### Custom Settings Separation of settings by enviromment is a must have
 these days and starting with default of Esmerald will not be enough for any
 application. The settings are pydantic standard settings and therefore
 compatible with Esmerald. The system brings some defaults that can be used out-
 of-the-box but it's not mandatory to be used. The environment defaults to
 **production**. ```python from esmerald import EsmeraldAPISettings from
 esmerald.conf.enums import EnvironmentType class Development
-(EsmeraldAPISettings): app_name: bool = 'My app in dev' environment: str =
+(EsmeraldAPISettings): app_name: str = 'My app in dev' environment: str =
 EnvironmentType.DEVELOPMENT ``` **Load the settings into your Esmerald
 application**: Assuming your Esmerald app is inside an `src/app.py`. ```console
 ESMERALD_SETTINGS_MODULE='myapp.settings.Development' python -m src.app.py ```
 ## Gateway, WebSocketGateway and Include Starlette offers the Route classes for
 simple path assignments but this is also very limiting if something more
 complex in mind. Esmerald extends that functionality and adds some `flair` and
 levels up by having the Gateway, WebSocketGateway and Include. Those are
@@ -174,15 +174,15 @@
 Include and Esmerald The `Include` can be very helpful mostly when the goal is
 to avoid a lot of imports and massive list of objects to be passed into one
 single object. This can be particulary useful to make a Esmerald instance.
 **Example**: ```python title='src/urls.py' from esmerald import Include
 route_patterns = [ Include(namespace='myapp.accounts.urls', pattern='my_urls')
 ] ``` ```python title='src/app.py' from esmerald import Esmerald, Include app =
 Esmerald(routes=[Include('src.urls')]) ``` ## Run the application As mentioned
-before, we recomment uvicorn for production but it's not mandatory. **Using
+before, we recommend uvicorn for production but it's not mandatory. **Using
 uvicorn**: ```shell uvicorn src:app --reload INFO: Uvicorn running on http://
 127.0.0.1:8000 (Press CTRL+C to quit) INFO: Started reloader process [28720]
 INFO: Started server process [28722] INFO: Waiting for application startup.
 INFO: Application startup complete. ``` ## Run the application with custom
 settings **Using uvicorn**: ```shell ESMERALD_SETTINGS_MODULE=myapp.AppSettings
 uvicorn src:app --reload INFO: Uvicorn running on http://127.0.0.1:8000 (Press
 CTRL+C to quit) INFO: Started reloader process [28720] INFO: Started server
```

### Comparing `esmerald-3.1.2/pyproject.toml` & `esmerald-3.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -88,76 +88,95 @@
 Homepage = "https://github.com/dymmond/esmerald"
 Documentation = "https://esmerald.dymmond.com/"
 Changelog = "https://esmerald.dymmond.com/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
 Source = "https://github.com/dymmond/esmerald"
 
 [project.optional-dependencies]
-test = [
+test = ["httpx>=0.25.0,<0.30.0"]
+
+dev = [
+    # includes watchfiles
+    "uvicorn[standard]>=0.24.0",
+]
+
+
+templates = ["mako>=1.2.4,<2.0.0"]
+jwt = ["passlib==1.7.4", "python-jose>=3.3.0,<4"]
+encoders = ["ujson>=5.7.0,<6"]
+schedulers = ["asyncz>=0.4.0"]
+
+[tool.hatch.envs.default]
+dependencies = ["ruff", "pre-commit>=2.17.0,<3.0.0", "twine"]
+[tool.hatch.envs.default.scripts]
+clean_pyc = "find . -type f -name \"*.pyc\" -delete"
+clean_pyi = "find . -type f -name \"*.pyi\" -delete"
+clean_pycache = "find . -type d -name \"*__pycache__*\" -delete"
+build_with_check = "hatch build; twine check dist/*"
+lint = "ruff check --fix --line-length 99 esmerald tests docs_src {args}"
+
+
+[tool.hatch.envs.docs]
+dependencies = [
+    "a2wsgi>=1.9.0,<2",
+    "griffe-typingdoc>=0.2.2",
+    "httpx>=0.25.0,<0.30.0",
+    "mike>=2.0.0",
+    "mkautodoc>=0.2.0,<0.3.0",
+    "mkdocs>=1.1.2,<2.0.0",
+    "mkdocs-material>=9.4.4,<10.0.0",
+    "mdx-include>=1.4.2,<2.0.0",
+    "mkdocs-markdownextradata-plugin>=0.2.5,<0.3.0",
+    "mkdocs-meta-descriptions-plugin>=2.3.0",
+    "mkdocstrings[python]>=0.23.0,<0.30.0",
+    "pyyaml>=6.0,<7.0.0",
+]
+[tool.hatch.envs.docs.scripts]
+build = "mkdocs build"
+serve = "mkdocs serve --dev-addr localhost:8000"
+
+
+[tool.hatch.envs.test]
+dependencies = [
     "pytest>=7.1.3,<9.0.0",
     "pytest-cov>=4.1.0,<6.0.0",
     "pytest-asyncio>=0.20.0",
     "mypy==1.9.0",
-    "flake8>=5.0.4",
     "aiofiles>=0.8.0,<24",
     "a2wsgi>=1.9.0,<2",
-    "asyncz>=0.5.0",
+    "asyncz>=0.6.0",
     "anyio[trio]>=3.6.2,<5.0.0",
-    "asyncio[trio]>=3.4.3,<4.0.0",
     "httpx>=0.25.0,<0.30.0",
     "brotli>=1.0.9,<2.0.0",
     "flask>=1.1.2,<4.0.0",
     "freezegun>=1.2.2,<2.0.0",
     "mock==5.1.0",
     "passlib==1.7.4",
     "polyfactory>=2.5.0,<3.0.0",
     "python-jose>=3.3.0,<4",
     "saffier[postgres]>=1.3.7",
     "edgy[postgres]>=0.4.0",
     "mongoz>=0.6.0",
-    "requests>=2.28.2,<3.0.0",
     "ujson>=5.7.0,<6",
 
     # types
     "types-ujson==5.9.0.0",
     "types-orjson==3.6.2",
-]
+    "ipython",
+    "ptpython",
+    "uvicorn",
 
-dev = [
-    "a2wsgi>=1.10.0,<2",
-    "autoflake>=1.4.0",
-    "black==24.3.0",
-    "ipdb",
-    "isort>=5.0.6,<6.0.0",
-    "flake8>=3.8.3,<8.0.0",
-    "uvicorn[standard]>=0.24.0",
-    "pre-commit>=3.0.4,<4.0.0",
-    "ruff>=0.3.0,<1.0.0",
-    "watchfiles>=0.16.1,<0.22.0",
 ]
+[tool.hatch.envs.test.scripts]
 
-doc = [
-    "griffe-typingdoc>=0.2.2",
-    "mike>=2.0.0",
-    "mkautodoc>=0.2.0,<0.3.0",
-    "mkdocs>=1.1.2,<2.0.0",
-    "mkdocs-material>=9.4.4,<10.0.0",
-    "mdx-include>=1.4.2,<2.0.0",
-    "mkdocs-markdownextradata-plugin>=0.2.5,<0.3.0",
-    "mkdocs-meta-descriptions-plugin>=2.3.0",
-    "mkdocstrings[python]>=0.23.0,<0.30.0",
-    "pyyaml>=6.0,<7.0.0",
-]
+# needs docker services running
+test = "ESMERALD_SETTINGS_MODULE='tests.settings.TestSettings' pytest {args}"
+coverage = "ESMERALD_SETTINGS_MODULE='tests.settings.TestSettings' pytest --cov=asyncz --cov=tests --cov-report=term-missing:skip-covered --cov-report=html tests {args}"
+check_types = "mypy -p lilya"
 
-templates = ["mako>=1.2.4,<2.0.0"]
-jwt = ["passlib==1.7.4", "python-jose>=3.3.0,<4"]
-encoders = ["ujson>=5.7.0,<6"]
-schedulers = ["asyncz>=0.4.0"]
-ptpython = ["ptpython>=3.0.23,<4.0.0"]
-ipython = ["ipython>=8.10.0,<9.0.0"]
 
 [tool.hatch.version]
 path = "esmerald/__init__.py"
 
 [project.scripts]
 esmerald = "esmerald.__main__:run_cli"
 
@@ -222,14 +241,15 @@
 
 [[tool.mypy.overrides]]
 module = "docs_src.*"
 ignore_errors = true
 
 [[tool.mypy.overrides]]
 module = [
+    "multipart.*",
     "sqlalchemy.*",
     "sqlalchemy_utils.*",
     "slugify.*",
     "pytz",
     "jose.*",
     "mako.*",
     "passlib.*",
```

### Comparing `esmerald-3.1.2/PKG-INFO` & `esmerald-3.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 330a 4e61 6d65 3a20 6573 6d65  : 2.3.Name: esme
 00000020: 7261 6c64 0a56 6572 7369 6f6e 3a20 332e  rald.Version: 3.
-00000030: 312e 320a 5375 6d6d 6172 793a 2048 6967  1.2.Summary: Hig
+00000030: 312e 330a 5375 6d6d 6172 793a 2048 6967  1.3.Summary: Hig
 00000040: 686c 7920 7363 616c 6162 6c65 2c20 7065  hly scalable, pe
 00000050: 7266 6f72 6d61 6e74 2c20 6561 7379 2074  rformant, easy t
 00000060: 6f20 6c65 6172 6e2c 2065 6173 7920 746f  o learn, easy to
 00000070: 2063 6f64 6520 616e 6420 666f 7220 6576   code and for ev
 00000080: 6572 7920 6170 706c 6963 6174 696f 6e2e  ery application.
 00000090: 0a50 726f 6a65 6374 2d55 524c 3a20 486f  .Project-URL: Ho
 000000a0: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
@@ -159,1259 +159,1105 @@
 000009e0: 302e 302e 370a 5265 7175 6972 6573 2d44  0.0.7.Requires-D
 000009f0: 6973 743a 2072 6963 683c 3134 2e30 2e30  ist: rich<14.0.0
 00000a00: 2c3e 3d31 332e 332e 310a 5265 7175 6972  ,>=13.3.1.Requir
 00000a10: 6573 2d44 6973 743a 2074 7970 696e 672d  es-Dist: typing-
 00000a20: 6578 7465 6e73 696f 6e73 3e3d 342e 3131  extensions>=4.11
 00000a30: 2e30 0a50 726f 7669 6465 732d 4578 7472  .0.Provides-Extr
 00000a40: 613a 2064 6576 0a52 6571 7569 7265 732d  a: dev.Requires-
-00000a50: 4469 7374 3a20 6132 7773 6769 3c32 2c3e  Dist: a2wsgi<2,>
-00000a60: 3d31 2e31 302e 303b 2065 7874 7261 203d  =1.10.0; extra =
-00000a70: 3d20 2764 6576 270a 5265 7175 6972 6573  = 'dev'.Requires
-00000a80: 2d44 6973 743a 2061 7574 6f66 6c61 6b65  -Dist: autoflake
-00000a90: 3e3d 312e 342e 303b 2065 7874 7261 203d  >=1.4.0; extra =
-00000aa0: 3d20 2764 6576 270a 5265 7175 6972 6573  = 'dev'.Requires
-00000ab0: 2d44 6973 743a 2062 6c61 636b 3d3d 3234  -Dist: black==24
-00000ac0: 2e33 2e30 3b20 6578 7472 6120 3d3d 2027  .3.0; extra == '
-00000ad0: 6465 7627 0a52 6571 7569 7265 732d 4469  dev'.Requires-Di
-00000ae0: 7374 3a20 666c 616b 6538 3c38 2e30 2e30  st: flake8<8.0.0
-00000af0: 2c3e 3d33 2e38 2e33 3b20 6578 7472 6120  ,>=3.8.3; extra 
-00000b00: 3d3d 2027 6465 7627 0a52 6571 7569 7265  == 'dev'.Require
-00000b10: 732d 4469 7374 3a20 6970 6462 3b20 6578  s-Dist: ipdb; ex
-00000b20: 7472 6120 3d3d 2027 6465 7627 0a52 6571  tra == 'dev'.Req
-00000b30: 7569 7265 732d 4469 7374 3a20 6973 6f72  uires-Dist: isor
-00000b40: 743c 362e 302e 302c 3e3d 352e 302e 363b  t<6.0.0,>=5.0.6;
-00000b50: 2065 7874 7261 203d 3d20 2764 6576 270a   extra == 'dev'.
-00000b60: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000b70: 7265 2d63 6f6d 6d69 743c 342e 302e 302c  re-commit<4.0.0,
-00000b80: 3e3d 332e 302e 343b 2065 7874 7261 203d  >=3.0.4; extra =
-00000b90: 3d20 2764 6576 270a 5265 7175 6972 6573  = 'dev'.Requires
-00000ba0: 2d44 6973 743a 2072 7566 663c 312e 302e  -Dist: ruff<1.0.
-00000bb0: 302c 3e3d 302e 332e 303b 2065 7874 7261  0,>=0.3.0; extra
-00000bc0: 203d 3d20 2764 6576 270a 5265 7175 6972   == 'dev'.Requir
-00000bd0: 6573 2d44 6973 743a 2075 7669 636f 726e  es-Dist: uvicorn
-00000be0: 5b73 7461 6e64 6172 645d 3e3d 302e 3234  [standard]>=0.24
-00000bf0: 2e30 3b20 6578 7472 6120 3d3d 2027 6465  .0; extra == 'de
-00000c00: 7627 0a52 6571 7569 7265 732d 4469 7374  v'.Requires-Dist
-00000c10: 3a20 7761 7463 6866 696c 6573 3c30 2e32  : watchfiles<0.2
-00000c20: 322e 302c 3e3d 302e 3136 2e31 3b20 6578  2.0,>=0.16.1; ex
-00000c30: 7472 6120 3d3d 2027 6465 7627 0a50 726f  tra == 'dev'.Pro
-00000c40: 7669 6465 732d 4578 7472 613a 2064 6f63  vides-Extra: doc
-00000c50: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000c60: 6772 6966 6665 2d74 7970 696e 6764 6f63  griffe-typingdoc
-00000c70: 3e3d 302e 322e 323b 2065 7874 7261 203d  >=0.2.2; extra =
-00000c80: 3d20 2764 6f63 270a 5265 7175 6972 6573  = 'doc'.Requires
-00000c90: 2d44 6973 743a 206d 6478 2d69 6e63 6c75  -Dist: mdx-inclu
-00000ca0: 6465 3c32 2e30 2e30 2c3e 3d31 2e34 2e32  de<2.0.0,>=1.4.2
-00000cb0: 3b20 6578 7472 6120 3d3d 2027 646f 6327  ; extra == 'doc'
-00000cc0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000cd0: 6d69 6b65 3e3d 322e 302e 303b 2065 7874  mike>=2.0.0; ext
-00000ce0: 7261 203d 3d20 2764 6f63 270a 5265 7175  ra == 'doc'.Requ
-00000cf0: 6972 6573 2d44 6973 743a 206d 6b61 7574  ires-Dist: mkaut
-00000d00: 6f64 6f63 3c30 2e33 2e30 2c3e 3d30 2e32  odoc<0.3.0,>=0.2
-00000d10: 2e30 3b20 6578 7472 6120 3d3d 2027 646f  .0; extra == 'do
-00000d20: 6327 0a52 6571 7569 7265 732d 4469 7374  c'.Requires-Dist
-00000d30: 3a20 6d6b 646f 6373 2d6d 6172 6b64 6f77  : mkdocs-markdow
-00000d40: 6e65 7874 7261 6461 7461 2d70 6c75 6769  nextradata-plugi
-00000d50: 6e3c 302e 332e 302c 3e3d 302e 322e 353b  n<0.3.0,>=0.2.5;
-00000d60: 2065 7874 7261 203d 3d20 2764 6f63 270a   extra == 'doc'.
-00000d70: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
-00000d80: 6b64 6f63 732d 6d61 7465 7269 616c 3c31  kdocs-material<1
-00000d90: 302e 302e 302c 3e3d 392e 342e 343b 2065  0.0.0,>=9.4.4; e
-00000da0: 7874 7261 203d 3d20 2764 6f63 270a 5265  xtra == 'doc'.Re
-00000db0: 7175 6972 6573 2d44 6973 743a 206d 6b64  quires-Dist: mkd
-00000dc0: 6f63 732d 6d65 7461 2d64 6573 6372 6970  ocs-meta-descrip
-00000dd0: 7469 6f6e 732d 706c 7567 696e 3e3d 322e  tions-plugin>=2.
-00000de0: 332e 303b 2065 7874 7261 203d 3d20 2764  3.0; extra == 'd
-00000df0: 6f63 270a 5265 7175 6972 6573 2d44 6973  oc'.Requires-Dis
-00000e00: 743a 206d 6b64 6f63 733c 322e 302e 302c  t: mkdocs<2.0.0,
-00000e10: 3e3d 312e 312e 323b 2065 7874 7261 203d  >=1.1.2; extra =
-00000e20: 3d20 2764 6f63 270a 5265 7175 6972 6573  = 'doc'.Requires
-00000e30: 2d44 6973 743a 206d 6b64 6f63 7374 7269  -Dist: mkdocstri
-00000e40: 6e67 735b 7079 7468 6f6e 5d3c 302e 3330  ngs[python]<0.30
-00000e50: 2e30 2c3e 3d30 2e32 332e 303b 2065 7874  .0,>=0.23.0; ext
-00000e60: 7261 203d 3d20 2764 6f63 270a 5265 7175  ra == 'doc'.Requ
-00000e70: 6972 6573 2d44 6973 743a 2070 7979 616d  ires-Dist: pyyam
-00000e80: 6c3c 372e 302e 302c 3e3d 362e 303b 2065  l<7.0.0,>=6.0; e
-00000e90: 7874 7261 203d 3d20 2764 6f63 270a 5072  xtra == 'doc'.Pr
-00000ea0: 6f76 6964 6573 2d45 7874 7261 3a20 656e  ovides-Extra: en
-00000eb0: 636f 6465 7273 0a52 6571 7569 7265 732d  coders.Requires-
-00000ec0: 4469 7374 3a20 756a 736f 6e3c 362c 3e3d  Dist: ujson<6,>=
-00000ed0: 352e 372e 303b 2065 7874 7261 203d 3d20  5.7.0; extra == 
-00000ee0: 2765 6e63 6f64 6572 7327 0a50 726f 7669  'encoders'.Provi
-00000ef0: 6465 732d 4578 7472 613a 2069 7079 7468  des-Extra: ipyth
-00000f00: 6f6e 0a52 6571 7569 7265 732d 4469 7374  on.Requires-Dist
-00000f10: 3a20 6970 7974 686f 6e3c 392e 302e 302c  : ipython<9.0.0,
-00000f20: 3e3d 382e 3130 2e30 3b20 6578 7472 6120  >=8.10.0; extra 
-00000f30: 3d3d 2027 6970 7974 686f 6e27 0a50 726f  == 'ipython'.Pro
-00000f40: 7669 6465 732d 4578 7472 613a 206a 7774  vides-Extra: jwt
-00000f50: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000f60: 7061 7373 6c69 623d 3d31 2e37 2e34 3b20  passlib==1.7.4; 
-00000f70: 6578 7472 6120 3d3d 2027 6a77 7427 0a52  extra == 'jwt'.R
-00000f80: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000f90: 7468 6f6e 2d6a 6f73 653c 342c 3e3d 332e  thon-jose<4,>=3.
-00000fa0: 332e 303b 2065 7874 7261 203d 3d20 276a  3.0; extra == 'j
-00000fb0: 7774 270a 5072 6f76 6964 6573 2d45 7874  wt'.Provides-Ext
-00000fc0: 7261 3a20 7074 7079 7468 6f6e 0a52 6571  ra: ptpython.Req
-00000fd0: 7569 7265 732d 4469 7374 3a20 7074 7079  uires-Dist: ptpy
-00000fe0: 7468 6f6e 3c34 2e30 2e30 2c3e 3d33 2e30  thon<4.0.0,>=3.0
-00000ff0: 2e32 333b 2065 7874 7261 203d 3d20 2770  .23; extra == 'p
-00001000: 7470 7974 686f 6e27 0a50 726f 7669 6465  tpython'.Provide
-00001010: 732d 4578 7472 613a 2073 6368 6564 756c  s-Extra: schedul
-00001020: 6572 730a 5265 7175 6972 6573 2d44 6973  ers.Requires-Dis
-00001030: 743a 2061 7379 6e63 7a3e 3d30 2e34 2e30  t: asyncz>=0.4.0
-00001040: 3b20 6578 7472 6120 3d3d 2027 7363 6865  ; extra == 'sche
-00001050: 6475 6c65 7273 270a 5072 6f76 6964 6573  dulers'.Provides
-00001060: 2d45 7874 7261 3a20 7465 6d70 6c61 7465  -Extra: template
-00001070: 730a 5265 7175 6972 6573 2d44 6973 743a  s.Requires-Dist:
-00001080: 206d 616b 6f3c 322e 302e 302c 3e3d 312e   mako<2.0.0,>=1.
-00001090: 322e 343b 2065 7874 7261 203d 3d20 2774  2.4; extra == 't
-000010a0: 656d 706c 6174 6573 270a 5072 6f76 6964  emplates'.Provid
-000010b0: 6573 2d45 7874 7261 3a20 7465 7374 0a52  es-Extra: test.R
-000010c0: 6571 7569 7265 732d 4469 7374 3a20 6132  equires-Dist: a2
-000010d0: 7773 6769 3c32 2c3e 3d31 2e39 2e30 3b20  wsgi<2,>=1.9.0; 
-000010e0: 6578 7472 6120 3d3d 2027 7465 7374 270a  extra == 'test'.
-000010f0: 5265 7175 6972 6573 2d44 6973 743a 2061  Requires-Dist: a
-00001100: 696f 6669 6c65 733c 3234 2c3e 3d30 2e38  iofiles<24,>=0.8
-00001110: 2e30 3b20 6578 7472 6120 3d3d 2027 7465  .0; extra == 'te
-00001120: 7374 270a 5265 7175 6972 6573 2d44 6973  st'.Requires-Dis
-00001130: 743a 2061 6e79 696f 5b74 7269 6f5d 3c35  t: anyio[trio]<5
-00001140: 2e30 2e30 2c3e 3d33 2e36 2e32 3b20 6578  .0.0,>=3.6.2; ex
-00001150: 7472 6120 3d3d 2027 7465 7374 270a 5265  tra == 'test'.Re
-00001160: 7175 6972 6573 2d44 6973 743a 2061 7379  quires-Dist: asy
-00001170: 6e63 696f 5b74 7269 6f5d 3c34 2e30 2e30  ncio[trio]<4.0.0
-00001180: 2c3e 3d33 2e34 2e33 3b20 6578 7472 6120  ,>=3.4.3; extra 
-00001190: 3d3d 2027 7465 7374 270a 5265 7175 6972  == 'test'.Requir
-000011a0: 6573 2d44 6973 743a 2061 7379 6e63 7a3e  es-Dist: asyncz>
-000011b0: 3d30 2e35 2e30 3b20 6578 7472 6120 3d3d  =0.5.0; extra ==
-000011c0: 2027 7465 7374 270a 5265 7175 6972 6573   'test'.Requires
-000011d0: 2d44 6973 743a 2062 726f 746c 693c 322e  -Dist: brotli<2.
-000011e0: 302e 302c 3e3d 312e 302e 393b 2065 7874  0.0,>=1.0.9; ext
-000011f0: 7261 203d 3d20 2774 6573 7427 0a52 6571  ra == 'test'.Req
-00001200: 7569 7265 732d 4469 7374 3a20 6564 6779  uires-Dist: edgy
-00001210: 5b70 6f73 7467 7265 735d 3e3d 302e 342e  [postgres]>=0.4.
-00001220: 303b 2065 7874 7261 203d 3d20 2774 6573  0; extra == 'tes
-00001230: 7427 0a52 6571 7569 7265 732d 4469 7374  t'.Requires-Dist
-00001240: 3a20 666c 616b 6538 3e3d 352e 302e 343b  : flake8>=5.0.4;
-00001250: 2065 7874 7261 203d 3d20 2774 6573 7427   extra == 'test'
-00001260: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00001270: 666c 6173 6b3c 342e 302e 302c 3e3d 312e  flask<4.0.0,>=1.
-00001280: 312e 323b 2065 7874 7261 203d 3d20 2774  1.2; extra == 't
-00001290: 6573 7427 0a52 6571 7569 7265 732d 4469  est'.Requires-Di
-000012a0: 7374 3a20 6672 6565 7a65 6775 6e3c 322e  st: freezegun<2.
-000012b0: 302e 302c 3e3d 312e 322e 323b 2065 7874  0.0,>=1.2.2; ext
-000012c0: 7261 203d 3d20 2774 6573 7427 0a52 6571  ra == 'test'.Req
-000012d0: 7569 7265 732d 4469 7374 3a20 6874 7470  uires-Dist: http
-000012e0: 783c 302e 3330 2e30 2c3e 3d30 2e32 352e  x<0.30.0,>=0.25.
-000012f0: 303b 2065 7874 7261 203d 3d20 2774 6573  0; extra == 'tes
-00001300: 7427 0a52 6571 7569 7265 732d 4469 7374  t'.Requires-Dist
-00001310: 3a20 6d6f 636b 3d3d 352e 312e 303b 2065  : mock==5.1.0; e
-00001320: 7874 7261 203d 3d20 2774 6573 7427 0a52  xtra == 'test'.R
-00001330: 6571 7569 7265 732d 4469 7374 3a20 6d6f  equires-Dist: mo
-00001340: 6e67 6f7a 3e3d 302e 362e 303b 2065 7874  ngoz>=0.6.0; ext
-00001350: 7261 203d 3d20 2774 6573 7427 0a52 6571  ra == 'test'.Req
-00001360: 7569 7265 732d 4469 7374 3a20 6d79 7079  uires-Dist: mypy
-00001370: 3d3d 312e 392e 303b 2065 7874 7261 203d  ==1.9.0; extra =
-00001380: 3d20 2774 6573 7427 0a52 6571 7569 7265  = 'test'.Require
-00001390: 732d 4469 7374 3a20 7061 7373 6c69 623d  s-Dist: passlib=
-000013a0: 3d31 2e37 2e34 3b20 6578 7472 6120 3d3d  =1.7.4; extra ==
-000013b0: 2027 7465 7374 270a 5265 7175 6972 6573   'test'.Requires
-000013c0: 2d44 6973 743a 2070 6f6c 7966 6163 746f  -Dist: polyfacto
-000013d0: 7279 3c33 2e30 2e30 2c3e 3d32 2e35 2e30  ry<3.0.0,>=2.5.0
-000013e0: 3b20 6578 7472 6120 3d3d 2027 7465 7374  ; extra == 'test
-000013f0: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
-00001400: 2070 7974 6573 742d 6173 796e 6369 6f3e   pytest-asyncio>
-00001410: 3d30 2e32 302e 303b 2065 7874 7261 203d  =0.20.0; extra =
-00001420: 3d20 2774 6573 7427 0a52 6571 7569 7265  = 'test'.Require
-00001430: 732d 4469 7374 3a20 7079 7465 7374 2d63  s-Dist: pytest-c
-00001440: 6f76 3c36 2e30 2e30 2c3e 3d34 2e31 2e30  ov<6.0.0,>=4.1.0
-00001450: 3b20 6578 7472 6120 3d3d 2027 7465 7374  ; extra == 'test
-00001460: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
-00001470: 2070 7974 6573 743c 392e 302e 302c 3e3d   pytest<9.0.0,>=
-00001480: 372e 312e 333b 2065 7874 7261 203d 3d20  7.1.3; extra == 
-00001490: 2774 6573 7427 0a52 6571 7569 7265 732d  'test'.Requires-
-000014a0: 4469 7374 3a20 7079 7468 6f6e 2d6a 6f73  Dist: python-jos
-000014b0: 653c 342c 3e3d 332e 332e 303b 2065 7874  e<4,>=3.3.0; ext
-000014c0: 7261 203d 3d20 2774 6573 7427 0a52 6571  ra == 'test'.Req
-000014d0: 7569 7265 732d 4469 7374 3a20 7265 7175  uires-Dist: requ
-000014e0: 6573 7473 3c33 2e30 2e30 2c3e 3d32 2e32  ests<3.0.0,>=2.2
-000014f0: 382e 323b 2065 7874 7261 203d 3d20 2774  8.2; extra == 't
-00001500: 6573 7427 0a52 6571 7569 7265 732d 4469  est'.Requires-Di
-00001510: 7374 3a20 7361 6666 6965 725b 706f 7374  st: saffier[post
-00001520: 6772 6573 5d3e 3d31 2e33 2e37 3b20 6578  gres]>=1.3.7; ex
-00001530: 7472 6120 3d3d 2027 7465 7374 270a 5265  tra == 'test'.Re
-00001540: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
-00001550: 6573 2d6f 726a 736f 6e3d 3d33 2e36 2e32  es-orjson==3.6.2
-00001560: 3b20 6578 7472 6120 3d3d 2027 7465 7374  ; extra == 'test
-00001570: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
-00001580: 2074 7970 6573 2d75 6a73 6f6e 3d3d 352e   types-ujson==5.
-00001590: 392e 302e 303b 2065 7874 7261 203d 3d20  9.0.0; extra == 
-000015a0: 2774 6573 7427 0a52 6571 7569 7265 732d  'test'.Requires-
-000015b0: 4469 7374 3a20 756a 736f 6e3c 362c 3e3d  Dist: ujson<6,>=
-000015c0: 352e 372e 303b 2065 7874 7261 203d 3d20  5.7.0; extra == 
-000015d0: 2774 6573 7427 0a44 6573 6372 6970 7469  'test'.Descripti
-000015e0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000015f0: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
-00001600: 2320 4573 6d65 7261 6c64 0a0a 3c70 2061  # Esmerald..<p a
-00001610: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-00001620: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00001630: 2f2f 6573 6d65 7261 6c64 2e64 6576 223e  //esmerald.dev">
-00001640: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001650: 2f2f 7265 732e 636c 6f75 6469 6e61 7279  //res.cloudinary
-00001660: 2e63 6f6d 2f64 796d 6d6f 6e64 2f69 6d61  .com/dymmond/ima
-00001670: 6765 2f75 706c 6f61 642f 7631 3637 3336  ge/upload/v16736
-00001680: 3139 3334 322f 6573 6d65 7261 6c64 2f69  19342/esmerald/i
-00001690: 6d67 2f6c 6f67 6f2d 6772 5f7a 316f 7438  mg/logo-gr_z1ot8
-000016a0: 6f2e 706e 6722 2061 6c74 3d27 4573 6d65  o.png" alt='Esme
-000016b0: 7261 6c64 273e 3c2f 613e 0a3c 2f70 3e0a  rald'></a>.</p>.
-000016c0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-000016d0: 7222 3e0a 2020 2020 3c65 6d3e f09f 9a80  r">.    <em>....
-000016e0: 2048 6967 686c 7920 7363 616c 6162 6c65   Highly scalable
-000016f0: 2c20 7065 7266 6f72 6d61 6e74 2c20 6561  , performant, ea
-00001700: 7379 2074 6f20 6c65 6172 6e2c 2065 6173  sy to learn, eas
-00001710: 7920 746f 2063 6f64 6520 616e 6420 666f  y to code and fo
-00001720: 7220 6576 6572 7920 6170 706c 6963 6174  r every applicat
-00001730: 696f 6e2e 20f0 9f9a 803c 2f65 6d3e 0a3c  ion. ....</em>.<
-00001740: 2f70 3e0a 0a3c 7020 616c 6967 6e3d 2263  /p>..<p align="c
-00001750: 656e 7465 7222 3e0a 3c61 2068 7265 663d  enter">.<a href=
-00001760: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001770: 636f 6d2f 6479 6d6d 6f6e 642f 6573 6d65  com/dymmond/esme
-00001780: 7261 6c64 2f77 6f72 6b66 6c6f 7773 2f54  rald/workflows/T
-00001790: 6573 7425 3230 5375 6974 652f 6261 6467  est%20Suite/badg
-000017a0: 652e 7376 673f 6576 656e 743d 7075 7368  e.svg?event=push
-000017b0: 2662 7261 6e63 683d 6d61 696e 2220 7461  &branch=main" ta
-000017c0: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
-000017d0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-000017e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000017f0: 6479 6d6d 6f6e 642f 6573 6d65 7261 6c64  dymmond/esmerald
-00001800: 2f77 6f72 6b66 6c6f 7773 2f54 6573 7425  /workflows/Test%
-00001810: 3230 5375 6974 652f 6261 6467 652e 7376  20Suite/badge.sv
-00001820: 673f 6576 656e 743d 7075 7368 2662 7261  g?event=push&bra
-00001830: 6e63 683d 6d61 696e 2220 616c 743d 2254  nch=main" alt="T
-00001840: 6573 7420 5375 6974 6522 3e0a 3c2f 613e  est Suite">.</a>
-00001850: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00001860: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00001870: 6563 742f 6573 6d65 7261 6c64 2220 7461  ect/esmerald" ta
-00001880: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
-00001890: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-000018a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000018b0: 2e69 6f2f 7079 7069 2f76 2f65 736d 6572  .io/pypi/v/esmer
-000018c0: 616c 643f 636f 6c6f 723d 2532 3333 3444  ald?color=%2334D
-000018d0: 3035 3826 6c61 6265 6c3d 7079 7069 2532  058&label=pypi%2
-000018e0: 3070 6163 6b61 6765 2220 616c 743d 2250  0package" alt="P
-000018f0: 6163 6b61 6765 2076 6572 7369 6f6e 223e  ackage version">
-00001900: 0a3c 2f61 3e0a 0a3c 6120 6872 6566 3d22  .</a>..<a href="
-00001910: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00001920: 2f70 726f 6a65 6374 2f65 736d 6572 616c  /project/esmeral
-00001930: 6422 2074 6172 6765 743d 225f 626c 616e  d" target="_blan
-00001940: 6b22 3e0a 2020 2020 3c69 6d67 2073 7263  k">.    <img src
-00001950: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00001960: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
-00001970: 7665 7273 696f 6e73 2f65 736d 6572 616c  versions/esmeral
-00001980: 642e 7376 673f 636f 6c6f 723d 2532 3333  d.svg?color=%233
-00001990: 3444 3035 3822 2061 6c74 3d22 5375 7070  4D058" alt="Supp
-000019a0: 6f72 7465 6420 5079 7468 6f6e 2076 6572  orted Python ver
-000019b0: 7369 6f6e 7322 3e0a 3c2f 613e 0a3c 2f70  sions">.</a>.</p
-000019c0: 3e0a 0a2d 2d2d 0a0a 2a2a 446f 6375 6d65  >..---..**Docume
-000019d0: 6e74 6174 696f 6e2a 2a3a 205b 6874 7470  ntation**: [http
-000019e0: 733a 2f2f 6573 6d65 7261 6c64 2e64 6576  s://esmerald.dev
-000019f0: 5d28 6874 7470 733a 2f2f 7777 772e 6573  ](https://www.es
-00001a00: 6d65 7261 6c64 2e64 6576 2920 f09f 939a  merald.dev) ....
-00001a10: 0a0a 2a2a 536f 7572 6365 2043 6f64 652a  ..**Source Code*
-00001a20: 2a3a 205b 6874 7470 733a 2f2f 6769 7468  *: [https://gith
-00001a30: 7562 2e63 6f6d 2f64 796d 6d6f 6e64 2f65  ub.com/dymmond/e
-00001a40: 736d 6572 616c 645d 2868 7474 7073 3a2f  smerald](https:/
-00001a50: 2f67 6974 6875 622e 636f 6d2f 6479 6d6d  /github.com/dymm
-00001a60: 6f6e 642f 6573 6d65 7261 6c64 290a 0a2a  ond/esmerald)..*
-00001a70: 2a54 6865 206f 6666 6963 6961 6c20 7375  *The official su
-00001a80: 7070 6f72 7465 6420 7665 7273 696f 6e20  pported version 
-00001a90: 6973 2061 6c77 6179 7320 7468 6520 6c61  is always the la
-00001aa0: 7465 7374 2072 656c 6561 7365 642a 2a2e  test released**.
-00001ab0: 0a0a 2d2d 2d0a 0a45 736d 6572 616c 6420  ..---..Esmerald 
-00001ac0: 6973 2061 206d 6f64 6572 6e2c 2070 6f77  is a modern, pow
-00001ad0: 6572 6675 6c2c 2066 6c65 7869 626c 652c  erful, flexible,
-00001ae0: 2068 6967 6820 7065 7266 6f72 6d61 6e74   high performant
-00001af0: 2c20 7765 6220 6672 616d 6577 6f72 6b20  , web framework 
-00001b00: 6465 7369 676e 6564 2074 6f20 6275 696c  designed to buil
-00001b10: 6420 6e6f 7420 6f6e 6c79 2041 5049 730a  d not only APIs.
-00001b20: 6275 7420 616c 736f 2066 756c 6c20 7363  but also full sc
-00001b30: 616c 6162 6c65 2061 7070 6c69 6361 7469  alable applicati
-00001b40: 6f6e 7320 6672 6f6d 2074 6865 2073 6d61  ons from the sma
-00001b50: 6c6c 6573 7420 746f 2065 6e74 6572 7072  llest to enterpr
-00001b60: 6973 6520 6c65 7665 6c2e 0a0a 4573 6d65  ise level...Esme
-00001b70: 7261 6c64 2069 7320 6465 7369 676e 6564  rald is designed
-00001b80: 2074 6f20 6275 696c 6420 7769 7468 2070   to build with p
-00001b90: 7974 686f 6e20 332e 382b 2061 6e64 2062  ython 3.8+ and b
-00001ba0: 6173 6564 206f 6e20 7374 616e 6461 7264  ased on standard
-00001bb0: 2070 7974 686f 6e20 7479 7065 2068 696e   python type hin
-00001bc0: 7473 2e20 496e 6974 6961 6c6c 790a 6275  ts. Initially.bu
-00001bd0: 696c 7420 6f6e 2074 6865 2074 6f70 206f  ilt on the top o
-00001be0: 6620 5b53 7461 726c 6574 7465 5d28 6874  f [Starlette](ht
-00001bf0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001c00: 2f65 6e63 6f64 652f 7374 6172 6c65 7474  /encode/starlett
-00001c10: 6529 2061 6e64 206c 6174 6572 206f 6e20  e) and later on 
-00001c20: 6d6f 7665 6420 746f 205b 4c69 6c79 615d  moved to [Lilya]
-00001c30: 2868 7474 7073 3a2f 2f6c 696c 7961 2e64  (https://lilya.d
-00001c40: 6576 2920 616e 6420 5b50 7964 616e 7469  ev) and [Pydanti
-00001c50: 635d 2868 7474 7073 3a2f 2f67 6974 6875  c](https://githu
-00001c60: 622e 636f 6d2f 7361 6d75 656c 636f 6c76  b.com/samuelcolv
-00001c70: 696e 2f70 7964 616e 7469 6329 2f5b 6d73  in/pydantic)/[ms
-00001c80: 6773 7065 635d 2868 7474 7073 3a2f 2f6a  gspec](https://j
-00001c90: 6372 6973 7468 6172 6966 2e63 6f6d 2f6d  cristharif.com/m
-00001ca0: 7367 7370 6563 2f29 2e0a 0a43 6865 636b  sgspec/)...Check
-00001cb0: 206f 7574 2074 6865 205b 4573 6d65 7261   out the [Esmera
-00001cc0: 6c64 2064 6f63 756d 656e 7461 7469 6f6e  ld documentation
-00001cd0: 20f0 9f93 9a5d 2868 7474 7073 3a2f 2f65   ....](https://e
-00001ce0: 736d 6572 616c 642e 6465 7629 0a0a 2a2a  smerald.dev)..**
-00001cf0: 5468 6520 6f66 6669 6369 616c 2073 7570  The official sup
-00001d00: 706f 7274 6564 2076 6572 7369 6f6e 2069  ported version i
-00001d10: 7320 616c 7761 7973 2074 6865 206c 6174  s always the lat
-00001d20: 6573 7420 7265 6c65 6173 6564 2a2a 2e0a  est released**..
-00001d30: 0a23 2320 4d6f 7469 7661 7469 6f6e 0a0a  .## Motivation..
-00001d40: 5468 6572 6520 6172 6520 6772 6561 7420  There are great 
-00001d50: 6672 616d 6577 6f72 6b73 206f 7574 2074  frameworks out t
-00001d60: 6865 7265 206c 696b 6520 4661 7374 4150  here like FastAP
-00001d70: 492c 2053 7461 726c 6974 652c 2046 6c61  I, Starlite, Fla
-00001d80: 6d61 2c20 466c 6173 6b2c 2044 6a61 6e67  ma, Flask, Djang
-00001d90: 6f2e 2e2e 2041 6c6c 206f 6620 7468 656d  o... All of them
-00001da0: 2073 6f6c 7669 6e67 206d 616a 6f72 6974   solving majorit
-00001db0: 790a 6f66 2074 6865 2063 7572 7265 6e74  y.of the current
-00001dc0: 2064 6179 2d74 6f2d 6461 7920 7072 6f62   day-to-day prob
-00001dd0: 6c65 6d73 206f 6620 3939 2520 6f66 2074  lems of 99% of t
-00001de0: 6865 2061 7070 6c69 6361 7469 6f6e 7320  he applications 
-00001df0: 6275 7420 6c65 6176 696e 6720 7468 6520  but leaving the 
-00001e00: 3125 2074 6861 7420 6973 2075 7375 616c  1% that is usual
-00001e10: 6c79 2061 726f 756e 6420 7374 7275 6374  ly around struct
-00001e20: 7572 650a 616e 6420 6465 7369 676e 2f62  ure.and design/b
-00001e30: 7573 696e 6573 7320 7769 7468 6f75 7420  usiness without 
-00001e40: 746f 206d 7563 6820 746f 2064 6f2e 0a0a  to much to do...
-00001e50: 4573 6d65 7261 6c64 2067 6f74 2074 6865  Esmerald got the
-00001e60: 2069 6e73 7069 7261 7469 6f6e 2066 726f   inspiration fro
-00001e70: 6d20 7468 6f73 6520 6772 6561 7420 6672  m those great fr
-00001e80: 616d 6577 6f72 6b73 206f 7574 2074 6865  ameworks out the
-00001e90: 7265 2061 6e64 2077 6173 2062 7569 6c74  re and was built
-00001ea0: 2077 6974 6820 616c 6c20 7468 6520 6b6e   with all the kn
-00001eb0: 6f77 6e20 616d 617a 696e 670a 6665 6174  own amazing.feat
-00001ec0: 7572 6573 2062 7574 2077 6974 6820 6275  ures but with bu
-00001ed0: 7369 6e65 7373 2069 6e20 6d69 6e64 2061  siness in mind a
-00001ee0: 7320 7765 6c6c 2e20 5374 6172 6c69 7465  s well. Starlite
-00001ef0: 2c20 666f 7220 6578 616d 706c 652c 2067  , for example, g
-00001f00: 6176 6520 7468 6520 696e 7370 6972 6174  ave the inspirat
-00001f10: 696f 6e20 666f 7220 7468 6520 7472 616e  ion for the tran
-00001f20: 7366 6f72 6d65 7273 2061 6e64 2066 6f72  sformers and for
-00001f30: 2074 6865 2053 6967 6e61 7475 7265 206d   the Signature m
-00001f40: 6f64 656c 732c 0a73 6f6d 6574 6869 6e67  odels,.something
-00001f50: 2076 6572 7920 7573 6566 756c 2074 6861   very useful tha
-00001f60: 7420 6865 6c70 6564 2045 736d 6572 616c  t helped Esmeral
-00001f70: 6420 696e 7465 6765 7261 7469 6e67 2077  d integerating w
-00001f80: 6974 6820 7079 6461 6e74 6963 2e0a 4661  ith pydantic..Fa
-00001f90: 7374 4150 4920 6761 7665 2074 6865 2069  stAPI gave the i
-00001fa0: 6e73 7069 7261 7469 6f6e 2066 6f72 2041  nspiration for A
-00001fb0: 5049 2064 6573 6967 6e69 6e67 2c20 446a  PI designing, Dj
-00001fc0: 616e 676f 2066 6f72 2074 6865 2070 6572  ango for the per
-00001fd0: 6d69 7373 696f 6e73 2c20 466c 6173 6b20  missions, Flask 
-00001fe0: 666f 7220 7468 6520 7369 6d70 6c69 6369  for the simplici
-00001ff0: 7479 2c20 4e65 7374 4a53 2066 6f72 2074  ty, NestJS for t
-00002000: 6865 0a63 6f6e 7472 6f6c 6c65 7273 2061  he.controllers a
-00002010: 6e64 2074 6865 206c 6973 7420 676f 6573  nd the list goes
-00002020: 206f 6e2e 0a0a 466f 7220 6120 6a6f 6220   on...For a job 
-00002030: 746f 2062 6520 646f 6e65 2070 726f 7065  to be done prope
-00002040: 726c 792c 2075 7375 616c 6c79 2069 7420  rly, usually it 
-00002050: 6973 206e 6576 6572 2064 6f6e 6520 616c  is never done al
-00002060: 6f6e 6520 616e 6420 7468 6572 6520 6973  one and there is
-00002070: 2061 6c77 6179 7320 6120 6472 6976 6572   always a driver
-00002080: 2061 6e64 2069 6e73 7069 7261 7469 6f6e   and inspiration
-00002090: 2074 6f20 6974 2e0a 0a23 2320 5265 7175   to it...## Requ
-000020a0: 6972 656d 656e 7473 0a0a 2a20 7079 7468  irements..* pyth
-000020b0: 6f6e 2033 2e38 2b0a 0a45 736d 6572 616c  on 3.8+..Esmeral
-000020c0: 6420 776f 756c 646e 2774 2062 6520 706f  d wouldn't be po
-000020d0: 7373 6962 6c65 2077 6974 686f 7574 2074  ssible without t
-000020e0: 776f 2063 6f6c 6f73 7361 6c73 3a0a 0a2a  wo colossals:..*
-000020f0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00002100: 2f2f 7777 772e 6c69 6c79 612e 6465 762f  //www.lilya.dev/
-00002110: 2220 636c 6173 733d 2265 7874 6572 6e61  " class="externa
-00002120: 6c2d 6c69 6e6b 2220 7461 7267 6574 3d22  l-link" target="
-00002130: 5f62 6c61 6e6b 223e 5374 6172 6c65 7474  _blank">Starlett
-00002140: 653c 2f61 3e0a 2a20 3c61 2068 7265 663d  e</a>.* <a href=
-00002150: 2268 7474 7073 3a2f 2f70 7964 616e 7469  "https://pydanti
-00002160: 632d 646f 6373 2e68 656c 706d 616e 7561  c-docs.helpmanua
-00002170: 6c2e 696f 2f22 2063 6c61 7373 3d22 6578  l.io/" class="ex
-00002180: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
-00002190: 6765 743d 225f 626c 616e 6b22 3e50 7964  get="_blank">Pyd
-000021a0: 616e 7469 633c 2f61 3e0a 0a23 2320 496e  antic</a>..## In
-000021b0: 7374 616c 6c61 7469 6f6e 0a0a 6060 6073  stallation..```s
-000021c0: 6865 6c6c 0a24 2070 6970 2069 6e73 7461  hell.$ pip insta
-000021d0: 6c6c 2065 736d 6572 616c 640a 6060 600a  ll esmerald.```.
-000021e0: 0a41 6e20 4153 4749 2073 6572 7665 7220  .An ASGI server 
-000021f0: 6973 2061 6c73 6f20 6e65 6564 6564 2074  is also needed t
-00002200: 6f20 7275 6e20 696e 2070 726f 6475 6374  o run in product
-00002210: 696f 6e2c 2077 6520 7265 636f 6d6d 656e  ion, we recommen
-00002220: 6420 5b55 7669 636f 726e 5d28 6874 7470  d [Uvicorn](http
-00002230: 733a 2f2f 7777 772e 7576 6963 6f72 6e2e  s://www.uvicorn.
-00002240: 6f72 6729 2062 7574 2069 7420 6973 2065  org) but it is e
-00002250: 6e74 6972 656c 790a 7570 2074 6f20 796f  ntirely.up to yo
-00002260: 752e 0a0a 6060 6073 6865 6c6c 0a24 2070  u...```shell.$ p
-00002270: 6970 2069 6e73 7461 6c6c 2075 7669 636f  ip install uvico
-00002280: 726e 0a0a 6060 600a 0a49 6620 796f 7520  rn..```..If you 
-00002290: 7761 6e74 2069 6e73 7461 6c6c 2065 736d  want install esm
-000022a0: 6572 616c 6420 7769 7468 2073 7065 6369  erald with speci
-000022b0: 6669 6373 3a0a 0a2a 2a53 7570 706f 7274  fics:..**Support
-000022c0: 2066 6f72 2074 656d 706c 6174 6520 7379   for template sy
-000022d0: 7374 656d 2073 7563 6820 6173 206a 696e  stem such as jin
-000022e0: 6a61 3220 616e 6420 6d61 6b6f 2a2a 3a0a  ja2 and mako**:.
-000022f0: 0a60 6060 7368 656c 6c0a 2420 7069 7020  .```shell.$ pip 
-00002300: 696e 7374 616c 6c20 6573 6d65 7261 6c64  install esmerald
-00002310: 5b74 656d 706c 6174 6573 5d0a 6060 600a  [templates].```.
-00002320: 0a2a 2a53 7570 706f 7274 2066 6f72 2074  .**Support for t
-00002330: 6865 2069 6e74 6572 6e61 6c20 7363 6865  he internal sche
-00002340: 6475 6c65 722a 2a3a 0a0a 6060 6073 6865  duler**:..```she
-00002350: 6c6c 0a24 2070 6970 2069 6e73 7461 6c6c  ll.$ pip install
-00002360: 2065 736d 6572 616c 645b 7363 6865 6475   esmerald[schedu
-00002370: 6c65 7273 5d0a 6060 600a 0a2a 2a53 7570  lers].```..**Sup
-00002380: 706f 7274 2066 6f72 2074 6865 206a 7774  port for the jwt
-00002390: 2075 7365 6420 696e 7465 726e 616c 6c79   used internally
-000023a0: 2062 7920 4573 6d65 7261 6c64 2a2a 3a0a   by Esmerald**:.
-000023b0: 0a60 6060 7368 656c 6c0a 2420 7069 7020  .```shell.$ pip 
-000023c0: 696e 7374 616c 6c20 6573 6d65 7261 6c64  install esmerald
-000023d0: 5b6a 7774 5d0a 6060 600a 0a2a 2a53 7570  [jwt].```..**Sup
-000023e0: 706f 7274 2066 6f72 204f 524a 534f 4e20  port for ORJSON 
-000023f0: 616e 6420 554a 534f 4e2a 2a3a 0a0a 6060  and UJSON**:..``
-00002400: 6073 6865 6c6c 0a24 2070 6970 2069 6e73  `shell.$ pip ins
-00002410: 7461 6c6c 2065 736d 6572 616c 645b 656e  tall esmerald[en
-00002420: 636f 6465 7273 5d0a 6060 600a 0a2a 2a49  coders].```..**I
-00002430: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
-00002440: 6520 7468 6520 6573 6d65 7261 6c64 2074  e the esmerald t
-00002450: 6573 7469 6e67 2063 6c69 656e 742a 2a3a  esting client**:
-00002460: 0a0a 6060 6073 6865 6c6c 0a24 2070 6970  ..```shell.$ pip
-00002470: 2069 6e73 7461 6c6c 2065 736d 6572 616c   install esmeral
-00002480: 645b 7465 7374 5d0a 6060 600a 0a2a 2a49  d[test].```..**I
-00002490: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
-000024a0: 6520 7468 6520 6573 6d65 7261 6c64 2073  e the esmerald s
-000024b0: 6865 6c6c 2a2a 3a0a 0a4d 6f72 6520 5b64  hell**:..More [d
-000024c0: 6574 6169 6c73 5d28 6874 7470 733a 2f2f  etails](https://
-000024d0: 6573 6d65 7261 6c64 2e64 6576 2f64 6972  esmerald.dev/dir
-000024e0: 6563 7469 7665 732f 7368 656c 6c29 2061  ectives/shell) a
-000024f0: 626f 7574 2074 6869 7320 746f 7069 6320  bout this topic 
-00002500: 5b69 6e20 7468 6520 646f 6373 5d28 6874  [in the docs](ht
-00002510: 7470 733a 2f2f 6573 6d65 7261 6c64 2e64  tps://esmerald.d
-00002520: 6576 2f64 6972 6563 7469 7665 732f 7368  ev/directives/sh
-00002530: 656c 6c29 0a0a 6060 6073 6865 6c6c 0a24  ell)..```shell.$
-00002540: 2070 6970 2069 6e73 7461 6c6c 2065 736d   pip install esm
-00002550: 6572 616c 645b 6970 7974 686f 6e5d 2023  erald[ipython] #
-00002560: 2064 6566 6175 6c74 2073 6865 6c6c 0a24   default shell.$
-00002570: 2070 6970 2069 6e73 7461 6c6c 2065 736d   pip install esm
-00002580: 6572 616c 645b 7074 7079 7468 6f6e 5d20  erald[ptpython] 
-00002590: 2320 7074 7079 7468 6f6e 2073 6865 6c6c  # ptpython shell
-000025a0: 0a60 6060 0a0a 2323 2320 5374 6172 7420  .```..### Start 
-000025b0: 6120 7072 6f6a 6563 7420 7573 696e 6720  a project using 
-000025c0: 6469 7265 6374 6976 6573 0a0a 2121 2120  directives..!!! 
-000025d0: 5761 726e 696e 670a 2020 2020 5468 6973  Warning.    This
-000025e0: 2069 7320 666f 7220 6d6f 7265 2061 6476   is for more adv
-000025f0: 616e 6365 6420 7573 6572 7320 7468 6174  anced users that
-00002600: 2061 7265 2061 6c72 6561 6479 2063 6f6d   are already com
-00002610: 666f 7274 6162 6c65 2077 6974 6820 4573  fortable with Es
-00002620: 6d65 7261 6c64 2028 6f72 2050 7974 686f  merald (or Pytho
-00002630: 6e20 696e 2067 656e 6572 616c 290a 2020  n in general).  
-00002640: 2020 6f72 2066 6565 6c20 6c69 6b65 2069    or feel like i
-00002650: 7420 6973 206e 6f74 2061 2070 726f 626c  t is not a probl
-00002660: 656d 2075 7369 6e67 2074 6865 7365 2064  em using these d
-00002670: 6972 6563 7469 7665 732e 2049 6620 796f  irectives. If yo
-00002680: 7520 646f 206e 6f74 2066 6565 6c20 636f  u do not feel co
-00002690: 6d66 6f72 7461 626c 6520 7965 7420 746f  mfortable yet to
-000026a0: 2075 7365 2074 6869 732c 0a20 2020 2070   use this,.    p
-000026b0: 6c65 6173 6520 636f 6e74 696e 7565 2072  lease continue r
-000026c0: 6561 6469 6e67 2074 6865 2064 6f63 756d  eading the docum
-000026d0: 656e 7461 7469 6f6e 2061 6e64 206c 6561  entation and lea
-000026e0: 726e 696e 6720 6d6f 7265 2061 626f 7574  rning more about
-000026f0: 2045 736d 6572 616c 642e 0a0a 4966 2079   Esmerald...If y
-00002700: 6f75 2077 6973 6820 746f 2073 7461 7274  ou wish to start
-00002710: 2061 6e20 4573 6d65 7261 6c64 2070 726f   an Esmerald pro
-00002720: 6a65 6374 2077 6974 6820 6120 6465 6661  ject with a defa
-00002730: 756c 7420 7375 6767 6573 7465 6420 7374  ult suggested st
-00002740: 7275 6374 7572 652e 0a0a 6060 6073 6865  ructure...```she
-00002750: 6c6c 0a65 736d 6572 616c 6420 6372 6561  ll.esmerald crea
-00002760: 7465 7072 6f6a 6563 7420 3c59 4f55 522d  teproject <YOUR-
-00002770: 5052 4f4a 4543 542d 4e41 4d45 3e0a 6060  PROJECT-NAME>.``
-00002780: 600a 0a54 6869 7320 7769 6c6c 2067 656e  `..This will gen
-00002790: 6572 6174 6520 6120 7363 6166 666f 6c64  erate a scaffold
-000027a0: 2066 6f72 2079 6f75 7220 7072 6f6a 6563   for your projec
-000027b0: 7420 7769 7468 2073 6f6d 6520 7072 652d  t with some pre-
-000027c0: 6465 6669 6e65 6420 6669 6c65 7320 696e  defined files in
-000027d0: 2061 2073 696d 706c 6520 6661 7368 696f   a simple fashio
-000027e0: 6e2e 0a54 6869 7320 7769 6c6c 2061 6c73  n..This will als
-000027f0: 6f20 6765 6e65 7261 7465 2061 2066 696c  o generate a fil
-00002800: 6520 666f 7220 7468 6520 7465 7374 7320  e for the tests 
-00002810: 7573 696e 6720 7468 6520 4573 6d65 7261  using the Esmera
-00002820: 6c64 5465 7374 436c 6965 6e74 2c20 736f  ldTestClient, so
-00002830: 206d 616b 6520 7375 7265 2079 6f75 2072   make sure you r
-00002840: 756e 3a0a 0a60 6060 7368 656c 6c0a 2420  un:..```shell.$ 
-00002850: 7069 7020 696e 7374 616c 6c20 6573 6d65  pip install esme
-00002860: 7261 6c64 5b74 6573 745d 0a60 6060 0a0a  rald[test].```..
-00002870: 4f72 2079 6f75 2063 616e 2073 6b69 7020  Or you can skip 
-00002880: 7468 6973 2073 7465 7020 6966 2079 6f75  this step if you
-00002890: 2064 6f6e 2774 2077 616e 7420 746f 2075   don't want to u
-000028a0: 7365 2074 6865 2045 736d 6572 616c 6454  se the EsmeraldT
-000028b0: 6573 7443 6c69 656e 742e 0a0a 596f 7520  estClient...You 
-000028c0: 6361 6e20 6669 6e64 205b 6d6f 7265 2069  can find [more i
-000028d0: 6e66 6f72 6d61 7469 6f6e 5d28 6874 7470  nformation](http
-000028e0: 733a 2f2f 6573 6d65 7261 6c64 2e64 6576  s://esmerald.dev
-000028f0: 2f6d 616e 6167 656d 656e 742f 6469 7265  /management/dire
-00002900: 6374 6976 6573 2920 6162 6f75 7420 7468  ctives) about th
-00002910: 6973 2064 6972 6563 7469 7665 2061 6e64  is directive and
-00002920: 2068 6f77 2074 6f0a 7573 6520 6974 2e0a   how to.use it..
-00002930: 0a23 2320 4b65 7920 4665 6174 7572 6573  .## Key Features
-00002940: 0a0a 2a20 2a2a 466c 7569 6420 616e 6420  ..* **Fluid and 
-00002950: 4661 7374 2a2a 3a20 5468 616e 6b73 2074  Fast**: Thanks t
-00002960: 6f20 5374 6172 6c65 7474 6520 616e 6420  o Starlette and 
-00002970: 5079 6461 6e74 6963 2f6d 7367 7370 6563  Pydantic/msgspec
-00002980: 2e0a 2a20 2a2a 4661 7374 2074 6f20 6465  ..* **Fast to de
-00002990: 7665 6c6f 702a 2a3a 2054 6861 6e6b 7320  velop**: Thanks 
-000029a0: 746f 2074 6865 2073 696d 706c 6963 6974  to the simplicit
-000029b0: 7920 6f66 2064 6573 6967 6e2c 2074 6865  y of design, the
-000029c0: 2064 6576 656c 6f70 6d65 6e74 2074 696d   development tim
-000029d0: 6573 2063 616e 2062 6520 7265 6475 6365  es can be reduce
-000029e0: 6420 6578 706f 6e65 6e74 6961 6c6c 792e  d exponentially.
-000029f0: 0a2a 202a 2a49 6e74 7569 7469 7665 2a2a  .* **Intuitive**
-00002a00: 3a20 4966 2079 6f75 2061 7265 2075 7365  : If you are use
-00002a10: 6420 746f 2074 6865 206f 7468 6572 2066  d to the other f
-00002a20: 7261 6d65 776f 726b 732c 2045 736d 6572  rameworks, Esmer
-00002a30: 616c 6420 6973 2061 206e 6f20 6272 6169  ald is a no brai
-00002a40: 6e65 7220 746f 2064 6576 656c 6f70 2e0a  ner to develop..
-00002a50: 2a20 2a2a 4561 7379 2a2a 3a20 4465 7665  * **Easy**: Deve
-00002a60: 6c6f 7065 6420 7769 7468 2064 6573 6967  loped with desig
-00002a70: 6e20 696e 206d 696e 6420 616e 6420 6561  n in mind and ea
-00002a80: 7379 206c 6561 726e 696e 672e 0a2a 202a  sy learning..* *
-00002a90: 2a53 686f 7274 2a2a 3a20 5769 7468 2074  *Short**: With t
-00002aa0: 6865 204f 4f50 2061 7661 696c 6162 6c65  he OOP available
-00002ab0: 206e 6174 6976 656c 7920 7468 6572 6520   natively there 
-00002ac0: 6973 206e 6f20 6e65 6564 2066 6f72 2063  is no need for c
-00002ad0: 6f64 6520 6475 706c 6963 6174 696f 6e2e  ode duplication.
-00002ae0: 2053 4f4c 4944 2e0a 2a20 2a2a 5265 6164   SOLID..* **Read
-00002af0: 792a 2a3a 2047 6574 2079 6f75 7220 6170  y**: Get your ap
-00002b00: 706c 6963 6174 696f 6e20 7570 2061 6e64  plication up and
-00002b10: 2072 756e 6e69 6e67 2077 6974 6820 7072   running with pr
-00002b20: 6f64 7563 7469 6f6e 2d72 6561 6479 2063  oduction-ready c
-00002b30: 6f64 652e 0a2a 202a 2a4f 4f50 2061 6e64  ode..* **OOP and
-00002b40: 2046 756e 6374 696f 6e61 6c2a 2a3a 2044   Functional**: D
-00002b50: 6573 6967 6e20 4150 4973 2069 6e20 616e  esign APIs in an
-00002b60: 7920 6465 7369 7265 6420 7761 792e 204f  y desired way. O
-00002b70: 4f50 206f 7220 4675 6e63 7469 6f6e 616c  OP or Functional
-00002b80: 2069 7320 6176 6169 6c61 626c 652e 0a2a   is available..*
-00002b90: 202a 2a41 7379 6e63 2061 6e64 2053 796e   **Async and Syn
-00002ba0: 632a 2a3a 2044 6f20 796f 7520 7072 6566  c**: Do you pref
-00002bb0: 6572 2073 796e 6320 6f72 2061 7379 6e63  er sync or async
-00002bc0: 3f20 596f 7520 6361 6e20 6861 7665 2062  ? You can have b
-00002bd0: 6f74 682e 0a2a 202a 2a4d 6964 646c 6577  oth..* **Middlew
-00002be0: 6172 652a 2a3a 2041 7070 6c79 206d 6964  are**: Apply mid
-00002bf0: 646c 6577 6172 6573 206f 6e20 7468 6520  dlewares on the 
-00002c00: 6170 706c 6963 6174 696f 6e20 6c65 7665  application leve
-00002c10: 6c20 6f72 2041 5049 206c 6576 656c 2e0a  l or API level..
-00002c20: 2a20 2a2a 4578 6365 7074 696f 6e20 4861  * **Exception Ha
-00002c30: 6e64 6c65 7273 2a2a 3a20 4170 706c 7920  ndlers**: Apply 
-00002c40: 6578 6365 7074 696f 6e20 6861 6e64 6c65  exception handle
-00002c50: 7273 206f 6e20 616e 7920 6465 7369 7265  rs on any desire
-00002c60: 6420 6c65 7665 6c2e 0a2a 202a 2a50 6572  d level..* **Per
-00002c70: 6d69 7373 696f 6e73 2a2a 3a20 4170 706c  missions**: Appl
-00002c80: 7920 7370 6563 6966 6963 2072 756c 6573  y specific rules
-00002c90: 2061 6e64 2070 6572 6d69 7373 696f 6e73   and permissions
-00002ca0: 206f 6e20 6561 6368 2041 5049 2e0a 2a20   on each API..* 
-00002cb0: 2a2a 496e 7465 7263 6570 746f 7273 2a2a  **Interceptors**
-00002cc0: 3a20 496e 7465 7263 6570 7420 7265 7175  : Intercept requ
-00002cd0: 6573 7473 2061 6e64 2061 6464 206c 6f67  ests and add log
-00002ce0: 6963 2062 6566 6f72 6520 7265 6163 6869  ic before reachi
-00002cf0: 6e67 2074 6865 2065 6e64 706f 696e 742e  ng the endpoint.
-00002d00: 0a2a 202a 2a50 6c75 6767 6162 6c65 732a  .* **Pluggables*
-00002d10: 2a3a 2043 7265 6174 6520 706c 7567 696e  *: Create plugin
-00002d20: 7320 666f 7220 4573 6d65 7261 6c64 2061  s for Esmerald a
-00002d30: 6e64 2068 6f6f 6b20 7468 656d 2069 6e74  nd hook them int
-00002d40: 6f20 616e 7920 6170 706c 6963 6174 696f  o any applicatio
-00002d50: 6e20 616e 642f 6f72 0a64 6973 7472 6962  n and/or.distrib
-00002d60: 7574 6520 7468 656d 2e0a 2a20 2a2a 4441  ute them..* **DA
-00002d70: 4f20 616e 6420 4173 796e 6344 414f 2a2a  O and AsyncDAO**
-00002d80: 3a20 4176 6f69 6420 6461 7461 6261 7365  : Avoid database
-00002d90: 2063 616c 6c73 2064 6972 6563 746c 7920   calls directly 
-00002da0: 6672 6f6d 2074 6865 2041 5049 732e 2055  from the APIs. U
-00002db0: 7365 2062 7573 696e 6573 7320 6f62 6a65  se business obje
-00002dc0: 6374 7320 696e 7374 6561 642e 0a2a 202a  cts instead..* *
-00002dd0: 2a4f 524d 2053 7570 706f 7274 2a2a 3a20  *ORM Support**: 
-00002de0: 4e61 7469 7665 2073 7570 706f 7274 2066  Native support f
-00002df0: 6f72 205b 5361 6666 6965 725d 5b73 6166  or [Saffier][saf
-00002e00: 6669 6572 5f6f 726d 5d20 616e 6420 5b45  fier_orm] and [E
-00002e10: 6467 795d 5b65 6467 795f 6f72 6d5d 2e0a  dgy][edgy_orm]..
-00002e20: 2a20 2a2a 4f44 4d20 5375 7070 6f72 742a  * **ODM Support*
-00002e30: 2a3a 204e 6174 6976 6520 7375 7070 6f72  *: Native suppor
-00002e40: 7420 666f 7220 5b4d 6f6e 676f 7a5d 5b6d  t for [Mongoz][m
-00002e50: 6f6e 676f 7a5f 6f64 6d5d 2e0a 2a20 2a2a  ongoz_odm]..* **
-00002e60: 4150 4956 6965 772a 2a3a 2043 6c61 7373  APIView**: Class
-00002e70: 2042 6173 6564 2065 6e64 706f 696e 7473   Based endpoints
-00002e80: 2066 6f72 2079 6f75 7220 6265 6c6f 7665   for your belove
-00002e90: 6420 4f4f 5020 6465 7369 676e 2e0a 2a20  d OOP design..* 
-00002ea0: 2a2a 4a53 4f4e 2073 6572 6961 6c69 7a61  **JSON serializa
-00002eb0: 7469 6f6e 2f64 6573 6572 6961 6c69 7a61  tion/deserializa
-00002ec0: 7469 6f6e 2a2a 3a20 426f 7468 2055 4a53  tion**: Both UJS
-00002ed0: 4f4e 2061 6e64 204f 524a 4f4e 2073 7570  ON and ORJON sup
-00002ee0: 706f 7274 2e0a 2a20 2a2a 4c69 6665 7370  port..* **Lifesp
-00002ef0: 616e 2a2a 3a20 5375 7070 6f72 7420 666f  an**: Support fo
-00002f00: 7220 7468 6520 6e65 776c 7920 6c69 6665  r the newly life
-00002f10: 7370 616e 2061 6e64 206f 6e5f 7374 6172  span and on_star
-00002f20: 742f 6f6e 5f73 6875 7464 6f77 6e20 6576  t/on_shutdown ev
-00002f30: 656e 7473 2e0a 2a20 2a2a 5363 6865 6475  ents..* **Schedu
-00002f40: 6c65 722a 2a3a 2059 6573 2c20 7468 6174  ler**: Yes, that
-00002f50: 2773 2072 6967 6874 2c20 6974 2063 6f6d  's right, it com
-00002f60: 6573 2077 6974 6820 6120 7363 6865 6475  es with a schedu
-00002f70: 6c65 7220 666f 7220 7468 6f73 6520 6175  ler for those au
-00002f80: 746f 6d61 7465 6420 7461 736b 732e 0a2a  tomated tasks..*
-00002f90: 202a 2a44 6570 656e 6465 6e63 7920 496e   **Dependency In
-00002fa0: 6a65 6374 696f 6e2a 2a3a 204c 696b 6520  jection**: Like 
-00002fb0: 616e 7920 6f74 6865 7220 6772 6561 7420  any other great 
-00002fc0: 6672 616d 6577 6f72 6b20 6f75 7420 7468  framework out th
-00002fd0: 6572 652e 0a2a 202a 2a53 696d 706c 6963  ere..* **Simplic
-00002fe0: 6974 7920 6672 6f6d 2073 6574 7469 6e67  ity from setting
-00002ff0: 732a 2a3a 2059 6573 2c20 7765 2068 6176  s**: Yes, we hav
-00003000: 6520 6120 7761 7920 746f 206d 616b 6520  e a way to make 
-00003010: 7468 6520 636f 6465 2065 7665 6e20 636c  the code even cl
-00003020: 6561 6e65 7220 6279 2069 6e74 726f 6475  eaner by introdu
-00003030: 6369 6e67 2073 6574 7469 6e67 730a 6261  cing settings.ba
-00003040: 7365 6420 7379 7374 656d 732e 0a2a 202a  sed systems..* *
-00003050: 2a6d 7367 7370 6563 2a2a 202d 2053 7570  *msgspec** - Sup
-00003060: 706f 7274 2066 6f72 2060 6d73 6773 7065  port for `msgspe
-00003070: 6360 2e0a 0a23 2320 5265 6c61 7469 6f6e  c`...## Relation
-00003080: 2074 6f20 5374 6172 6c65 7474 6520 616e   to Starlette an
-00003090: 6420 6f74 6865 7220 6672 616d 6577 6f72  d other framewor
-000030a0: 6b73 0a0a 4573 6d65 7261 6c64 2075 7365  ks..Esmerald use
-000030b0: 7320 5374 6172 6c65 7474 6520 756e 6465  s Starlette unde
-000030c0: 7220 7468 6520 686f 6f64 2e20 5468 6520  r the hood. The 
-000030d0: 7265 6173 6f6e 2062 6568 696e 6420 7468  reason behind th
-000030e0: 6973 2064 6563 6973 6f6e 2063 6f6d 6573  is decison comes
-000030f0: 2077 6974 6820 7468 6520 6661 6374 2074   with the fact t
-00003100: 6861 7420 7065 7266 6f72 6d61 6e63 6520  hat performance 
-00003110: 6973 2074 6865 7265 0a61 6e64 206e 6f20  is there.and no 
-00003120: 6973 7375 6573 2077 6974 6820 726f 7574  issues with rout
-00003130: 696e 672e 0a0a 4f6e 6365 2074 6865 2061  ing...Once the a
-00003140: 7070 6c69 6361 7469 6f6e 2069 7320 7570  pplication is up
-00003150: 2c20 616c 6c20 7468 6520 726f 7574 6573  , all the routes
-00003160: 2061 7265 206d 6f75 6e74 6564 2061 6e64   are mounted and
-00003170: 2074 6865 7265 666f 7265 2074 6865 2075   therefore the u
-00003180: 726c 2070 6174 6873 2061 7265 2064 6566  rl paths are def
-00003190: 696e 6564 2e0a 4573 6d65 7261 6c64 2065  ined..Esmerald e
-000031a0: 6e63 6f75 7261 6765 7320 7374 616e 6461  ncourages standa
-000031b0: 7264 2070 7261 6374 6963 6573 2061 6e64  rd practices and
-000031c0: 2064 6573 6967 6e20 696e 206d 696e 6420   design in mind 
-000031d0: 7768 6963 6820 6d65 616e 7320 7468 6174  which means that
-000031e0: 2061 6e79 2061 7070 6c69 6361 7469 6f6e   any application
-000031f0: 2c20 6269 6720 6f72 2073 6d61 6c6c 2c0a  , big or small,.
-00003200: 6375 7374 6f6d 206f 7220 656e 7465 7270  custom or enterp
-00003210: 7269 7365 2c20 6669 7473 2077 6974 6869  rise, fits withi
-00003220: 6e20 4573 6d65 7261 6c64 2065 636f 7379  n Esmerald ecosy
-00003230: 7374 656d 2077 6974 686f 7574 2073 6361  stem without sca
-00003240: 6c61 6269 6c69 7479 2069 7373 7565 732e  lability issues.
-00003250: 0a0a 2323 2053 6574 7469 6e67 730a 0a4c  ..## Settings..L
-00003260: 696b 6520 6576 6572 7920 6f74 6865 7220  ike every other 
-00003270: 6672 616d 6577 6f72 6b2c 2077 6865 6e20  framework, when 
-00003280: 7374 6172 7469 6e67 2061 6e20 6170 706c  starting an appl
-00003290: 6963 6174 696f 6e2c 2061 206c 6f74 206f  ication, a lot o
-000032a0: 6620 5b73 6574 7469 6e67 735d 282e 2f61  f [settings](./a
-000032b0: 7070 6c69 6361 7469 6f6e 2f73 6574 7469  pplication/setti
-000032c0: 6e67 732e 6d64 2920 6361 6e2f 6e65 6564  ngs.md) can/need
-000032d0: 2074 6f20 6265 0a70 6173 7365 6420 746f   to be.passed to
-000032e0: 2074 6865 206d 6169 6e20 6f62 6a65 6374   the main object
-000032f0: 2061 6e64 2074 6869 7320 6361 6e20 6265   and this can be
-00003300: 2076 6572 7920 6461 7574 696e 6720 616e   very dauting an
-00003310: 6420 6875 676c 7920 746f 206d 6169 6e74  d hugly to maint
-00003320: 6169 6e20 616e 6420 7365 652e 0a0a 4573  ain and see...Es
-00003330: 6d65 7261 6c64 2063 6f6d 6573 2077 6974  merald comes wit
-00003340: 6820 7468 650a 5b73 6574 7469 6e67 735d  h the.[settings]
-00003350: 282e 2f61 7070 6c69 6361 7469 6f6e 2f73  (./application/s
-00003360: 6574 7469 6e67 732e 6d64 2920 696e 206d  ettings.md) in m
-00003370: 696e 642e 2041 2073 6574 206f 6620 6465  ind. A set of de
-00003380: 6661 756c 7473 2074 6861 7420 6361 6e20  faults that can 
-00003390: 6265 206f 7665 7272 6964 6465 6e20 6279  be overridden by
-000033a0: 2079 6f75 7220 7665 7279 206f 776e 2073   your very own s
-000033b0: 6574 7469 6e67 730a 6d6f 6475 6c65 2062  ettings.module b
-000033c0: 7574 206e 6f74 206c 696d 6974 6564 2074  ut not limited t
-000033d0: 6f20 6974 2061 7320 796f 7520 6361 6e20  o it as you can 
-000033e0: 7374 696c 6c20 7573 6520 7468 6520 636c  still use the cl
-000033f0: 6173 7369 6320 6170 7072 6f61 6368 206f  assic approach o
-00003400: 6620 7061 7373 696e 6720 6576 6572 7974  f passing everyt
-00003410: 6869 6e67 2069 6e74 6f20 610a 4573 6d65  hing into a.Esme
-00003420: 7261 6c64 2069 6e73 7461 6e63 6520 6469  rald instance di
-00003430: 7265 6374 6c79 2077 6865 6e20 696e 7374  rectly when inst
-00003440: 616e 7469 6174 696e 672e 0a0a 2a2a 4578  antiating...**Ex
-00003450: 616d 706c 6520 6f66 2063 6c61 7373 6963  ample of classic
-00003460: 2061 7070 726f 6163 682a 2a3a 0a0a 6060   approach**:..``
-00003470: 6070 7974 686f 6e0a 6672 6f6d 2065 7861  `python.from exa
-00003480: 6d70 6c65 2069 6d70 6f72 7420 4578 616d  mple import Exam
-00003490: 706c 654f 626a 6563 740a 0a23 2045 7861  pleObject..# Exa
-000034a0: 6d70 6c65 4f62 6a65 6374 2069 7320 616e  mpleObject is an
-000034b0: 2069 6e73 7461 6e63 6520 6f66 2061 6e6f   instance of ano
-000034c0: 7468 6572 2061 7070 6c69 6361 7469 6f6e  ther application
-000034d0: 0a23 2061 6e64 2069 7420 7365 7276 6573  .# and it serves
-000034e0: 206f 6e6c 7920 666f 7220 6578 616d 706c   only for exampl
-000034f0: 650a 0a61 7070 203d 2045 7861 6d70 6c65  e..app = Example
-00003500: 4f62 6a65 6374 2873 6574 7469 6e67 5f6f  Object(setting_o
-00003510: 6e65 3d2e 2e2e 2c20 7365 7474 696e 675f  ne=..., setting_
-00003520: 7477 6f3d 2e2e 2e2c 2073 6574 7469 6e67  two=..., setting
-00003530: 5f74 6872 6565 3d2e 2e2e 290a 0a60 6060  _three=...)..```
-00003540: 0a0a 496e 7370 6972 6564 2062 7920 7468  ..Inspired by th
-00003550: 6520 6772 6561 7420 5b44 6a61 6e67 6f5d  e great [Django]
-00003560: 2868 7474 7073 3a2f 2f77 7777 2e64 6a61  (https://www.dja
-00003570: 6e67 6f70 726f 6a65 6374 2e63 6f6d 2f29  ngoproject.com/)
-00003580: 2061 6e64 2075 7369 6e67 2070 7964 616e   and using pydan
-00003590: 7469 632c 2045 736d 6572 616c 6420 6861  tic, Esmerald ha
-000035a0: 7320 6120 6465 6661 756c 7420 6f62 6a65  s a default obje
-000035b0: 6374 0a72 6561 6479 2074 6f20 6265 2075  ct.ready to be u
-000035c0: 7365 6420 6f75 742d 6f66 2d74 6865 2d62  sed out-of-the-b
-000035d0: 6f78 2e0a 0a2a 2a45 736d 6572 616c 642a  ox...**Esmerald*
-000035e0: 2a3a 0a0a 6060 6070 7974 686f 6e0a 6672  *:..```python.fr
-000035f0: 6f6d 2065 736d 6572 616c 6420 696d 706f  om esmerald impo
-00003600: 7274 2045 736d 6572 616c 640a 0a61 7070  rt Esmerald..app
-00003610: 203d 2045 736d 6572 616c 6428 290a 0a60   = Esmerald()..`
-00003620: 6060 0a0a 416e 6420 7468 6174 2773 2069  ``..And that's i
-00003630: 7421 2041 6c6c 2074 6865 2064 6566 6175  t! All the defau
-00003640: 6c74 2073 6574 7469 6e67 7320 6172 6520  lt settings are 
-00003650: 6c6f 6164 6564 2120 5468 6973 2069 7320  loaded! This is 
-00003660: 7369 6d70 6c65 206f 6620 636f 7572 7365  simple of course
-00003670: 2062 7574 2063 616e 2079 6f75 206f 7665   but can you ove
-00003680: 7272 6964 650a 696e 7369 6465 2074 6865  rride.inside the
-00003690: 206f 626a 6563 7420 6173 2077 656c 6c3f   object as well?
-000036a0: 2059 6573 210a 0a60 6060 7079 7468 6f6e   Yes!..```python
-000036b0: 0a66 726f 6d20 6573 6d65 7261 6c64 2069  .from esmerald i
-000036c0: 6d70 6f72 7420 4573 6d65 7261 6c64 0a0a  mport Esmerald..
-000036d0: 6170 7020 3d20 4573 6d65 7261 6c64 2861  app = Esmerald(a
-000036e0: 7070 5f6e 616d 653d 274d 7920 4170 7027  pp_name='My App'
-000036f0: 2c20 7469 746c 653d 274d 7920 7469 746c  , title='My titl
-00003700: 6527 290a 0a60 6060 0a0a 5361 6d65 2061  e')..```..Same a
-00003710: 7320 7468 6520 636c 6173 7369 6373 2e0a  s the classics..
-00003720: 0a53 6f20 686f 7720 646f 6573 2045 736d  .So how does Esm
-00003730: 6572 616c 6420 6b6e 6f77 2061 626f 7574  erald know about
-00003740: 2074 6865 2064 6566 6175 6c74 2073 6574   the default set
-00003750: 7469 6e67 733f 2045 6e74 6572 7320 5b45  tings? Enters [E
-00003760: 736d 6572 616c 6420 7365 7474 696e 6773  smerald settings
-00003770: 206d 6f64 756c 655d 2823 6573 6d65 7261   module](#esmera
-00003780: 6c64 2d73 6574 7469 6e67 732d 6d6f 6475  ld-settings-modu
-00003790: 6c65 292e 0a0a 2323 2320 4573 6d65 7261  le)...### Esmera
-000037a0: 6c64 2053 6574 7469 6e67 7320 4d6f 6475  ld Settings Modu
-000037b0: 6c65 0a0a 5468 6973 2069 7320 7468 6520  le..This is the 
-000037c0: 7761 7920 4573 6d65 7261 6c64 2064 6566  way Esmerald def
-000037d0: 6175 6c74 7320 7468 6520 7661 6c75 6573  aults the values
-000037e0: 2e20 5768 656e 2073 7461 7274 696e 6720  . When starting 
-000037f0: 616e 2061 7070 6c69 6361 7469 6f6e 2c20  an application, 
-00003800: 7468 6520 7379 7374 656d 206c 6f6f 6b73  the system looks
-00003810: 2066 6f72 2061 0a60 4553 4d45 5241 4c44   for a.`ESMERALD
-00003820: 5f53 4554 5449 4e47 535f 4d4f 4455 4c45  _SETTINGS_MODULE
-00003830: 6020 656e 7669 726f 6e6d 656e 7420 7661  ` environment va
-00003840: 7269 6162 6c65 2e20 4966 206e 6f20 7661  riable. If no va
-00003850: 7269 6162 6c65 2069 7320 7375 7070 6c69  riable is suppli
-00003860: 6564 2074 6865 6e20 7468 6520 7379 7374  ed then the syst
-00003870: 656d 2077 696c 6c20 6465 6661 756c 7420  em will default 
-00003880: 746f 0a60 4573 6d65 7261 6c64 4150 4953  to.`EsmeraldAPIS
-00003890: 6574 7469 6e67 7360 2073 6574 7469 6e67  ettings` setting
-000038a0: 7320 616e 6420 7374 6172 742e 0a0a 2323  s and start...##
-000038b0: 2320 4375 7374 6f6d 2053 6574 7469 6e67  # Custom Setting
-000038c0: 730a 0a53 6570 6172 6174 696f 6e20 6f66  s..Separation of
-000038d0: 2073 6574 7469 6e67 7320 6279 2065 6e76   settings by env
-000038e0: 6972 6f6d 6d65 6e74 2069 7320 6120 6d75  iromment is a mu
-000038f0: 7374 2068 6176 6520 7468 6573 6520 6461  st have these da
-00003900: 7973 2061 6e64 2073 7461 7274 696e 6720  ys and starting 
-00003910: 7769 7468 2064 6566 6175 6c74 206f 6620  with default of 
-00003920: 4573 6d65 7261 6c64 2077 696c 6c20 6e6f  Esmerald will no
-00003930: 7420 6265 0a65 6e6f 7567 6820 666f 7220  t be.enough for 
-00003940: 616e 7920 6170 706c 6963 6174 696f 6e2e  any application.
-00003950: 0a0a 5468 6520 7365 7474 696e 6773 2061  ..The settings a
-00003960: 7265 2070 7964 616e 7469 6320 7374 616e  re pydantic stan
-00003970: 6461 7264 2073 6574 7469 6e67 7320 616e  dard settings an
-00003980: 6420 7468 6572 6566 6f72 6520 636f 6d70  d therefore comp
-00003990: 6174 6962 6c65 2077 6974 6820 4573 6d65  atible with Esme
-000039a0: 7261 6c64 2e0a 5468 6520 7379 7374 656d  rald..The system
-000039b0: 2062 7269 6e67 7320 736f 6d65 2064 6566   brings some def
-000039c0: 6175 6c74 7320 7468 6174 2063 616e 2062  aults that can b
-000039d0: 6520 7573 6564 206f 7574 2d6f 662d 7468  e used out-of-th
-000039e0: 652d 626f 7820 6275 7420 6974 2773 206e  e-box but it's n
-000039f0: 6f74 206d 616e 6461 746f 7279 2074 6f20  ot mandatory to 
-00003a00: 6265 2075 7365 642e 0a54 6865 2065 6e76  be used..The env
-00003a10: 6972 6f6e 6d65 6e74 2064 6566 6175 6c74  ironment default
-00003a20: 7320 746f 202a 2a70 726f 6475 6374 696f  s to **productio
-00003a30: 6e2a 2a2e 0a0a 6060 6070 7974 686f 6e0a  n**...```python.
-00003a40: 0a66 726f 6d20 6573 6d65 7261 6c64 2069  .from esmerald i
-00003a50: 6d70 6f72 7420 4573 6d65 7261 6c64 4150  mport EsmeraldAP
-00003a60: 4953 6574 7469 6e67 730a 6672 6f6d 2065  ISettings.from e
-00003a70: 736d 6572 616c 642e 636f 6e66 2e65 6e75  smerald.conf.enu
-00003a80: 6d73 2069 6d70 6f72 7420 456e 7669 726f  ms import Enviro
-00003a90: 6e6d 656e 7454 7970 650a 0a63 6c61 7373  nmentType..class
-00003aa0: 2044 6576 656c 6f70 6d65 6e74 2845 736d   Development(Esm
-00003ab0: 6572 616c 6441 5049 5365 7474 696e 6773  eraldAPISettings
-00003ac0: 293a 0a20 2020 2061 7070 5f6e 616d 653a  ):.    app_name:
-00003ad0: 2062 6f6f 6c20 3d20 274d 7920 6170 7020   bool = 'My app 
-00003ae0: 696e 2064 6576 270a 2020 2020 656e 7669  in dev'.    envi
-00003af0: 726f 6e6d 656e 743a 2073 7472 203d 2045  ronment: str = E
-00003b00: 6e76 6972 6f6e 6d65 6e74 5479 7065 2e44  nvironmentType.D
-00003b10: 4556 454c 4f50 4d45 4e54 0a0a 6060 600a  EVELOPMENT..```.
-00003b20: 0a2a 2a4c 6f61 6420 7468 6520 7365 7474  .**Load the sett
-00003b30: 696e 6773 2069 6e74 6f20 796f 7572 2045  ings into your E
-00003b40: 736d 6572 616c 6420 6170 706c 6963 6174  smerald applicat
-00003b50: 696f 6e2a 2a3a 0a0a 4173 7375 6d69 6e67  ion**:..Assuming
-00003b60: 2079 6f75 7220 4573 6d65 7261 6c64 2061   your Esmerald a
-00003b70: 7070 2069 7320 696e 7369 6465 2061 6e20  pp is inside an 
-00003b80: 6073 7263 2f61 7070 2e70 7960 2e0a 0a60  `src/app.py`...`
-00003b90: 6060 636f 6e73 6f6c 650a 0a45 534d 4552  ``console..ESMER
-00003ba0: 414c 445f 5345 5454 494e 4753 5f4d 4f44  ALD_SETTINGS_MOD
-00003bb0: 554c 453d 276d 7961 7070 2e73 6574 7469  ULE='myapp.setti
-00003bc0: 6e67 732e 4465 7665 6c6f 706d 656e 7427  ngs.Development'
-00003bd0: 2070 7974 686f 6e20 2d6d 2073 7263 2e61   python -m src.a
-00003be0: 7070 2e70 790a 0a60 6060 0a0a 2323 2047  pp.py..```..## G
-00003bf0: 6174 6577 6179 2c20 5765 6253 6f63 6b65  ateway, WebSocke
-00003c00: 7447 6174 6577 6179 2061 6e64 2049 6e63  tGateway and Inc
-00003c10: 6c75 6465 0a0a 5374 6172 6c65 7474 6520  lude..Starlette 
-00003c20: 6f66 6665 7273 2074 6865 2052 6f75 7465  offers the Route
-00003c30: 2063 6c61 7373 6573 2066 6f72 2073 696d   classes for sim
-00003c40: 706c 6520 7061 7468 2061 7373 6967 6e6d  ple path assignm
-00003c50: 656e 7473 2062 7574 2074 6869 7320 6973  ents but this is
-00003c60: 2061 6c73 6f20 7665 7279 206c 696d 6974   also very limit
-00003c70: 696e 6720 6966 2073 6f6d 6574 6869 6e67  ing if something
-00003c80: 206d 6f72 650a 636f 6d70 6c65 7820 696e   more.complex in
-00003c90: 206d 696e 642e 2045 736d 6572 616c 6420   mind. Esmerald 
-00003ca0: 6578 7465 6e64 7320 7468 6174 2066 756e  extends that fun
-00003cb0: 6374 696f 6e61 6c69 7479 2061 6e64 2061  ctionality and a
-00003cc0: 6464 7320 736f 6d65 2060 666c 6169 7260  dds some `flair`
-00003cd0: 2061 6e64 206c 6576 656c 7320 7570 2062   and levels up b
-00003ce0: 7920 6861 7669 6e67 2074 6865 0a47 6174  y having the.Gat
-00003cf0: 6577 6179 2c20 5765 6253 6f63 6b65 7447  eway, WebSocketG
-00003d00: 6174 6577 6179 2061 6e64 2049 6e63 6c75  ateway and Inclu
-00003d10: 6465 2e0a 0a54 686f 7365 2061 7265 2073  de...Those are s
-00003d20: 7065 6369 616c 206f 626a 6563 7473 2074  pecial objects t
-00003d30: 6861 7420 616c 6c6f 7720 616c 6c20 7468  hat allow all th
-00003d40: 6520 6d61 6769 6320 6f66 2045 736d 6572  e magic of Esmer
-00003d50: 616c 6420 746f 2068 6170 7065 6e2e 0a0a  ald to happen...
-00003d60: 466f 7220 6120 636c 6173 7369 632c 2064  For a classic, d
-00003d70: 6972 6563 742c 206f 6e65 2066 696c 6520  irect, one file 
-00003d80: 7369 6e67 6c65 2061 7070 726f 6163 682e  single approach.
-00003d90: 0a0a 2a2a 496e 2061 206e 7574 7368 656c  ..**In a nutshel
-00003da0: 6c2a 2a3a 0a0a 6060 6070 7974 686f 6e20  l**:..```python 
-00003db0: 7469 746c 653d 2773 7263 2f61 7070 2e70  title='src/app.p
-00003dc0: 7927 0a66 726f 6d20 6573 6d65 7261 6c64  y'.from esmerald
-00003dd0: 2069 6d70 6f72 7420 4573 6d65 7261 6c64   import Esmerald
-00003de0: 2c20 6765 742c 2073 7461 7475 732c 2052  , get, status, R
-00003df0: 6571 7565 7374 2c20 554a 534f 4e52 6573  equest, UJSONRes
-00003e00: 706f 6e73 652c 2047 6174 6577 6179 2c20  ponse, Gateway, 
-00003e10: 5765 6253 6f63 6b65 7447 6174 6577 6179  WebSocketGateway
-00003e20: 2c20 5765 6273 6f63 6b65 740a 0a40 6765  , Websocket..@ge
-00003e30: 7428 7374 6174 7573 5f63 6f64 653d 7374  t(status_code=st
-00003e40: 6174 7573 2e48 5454 505f 3230 305f 4f4b  atus.HTTP_200_OK
-00003e50: 290a 6173 796e 6320 6465 6620 686f 6d65  ).async def home
-00003e60: 2829 202d 3e20 554a 534f 4e52 6573 706f  () -> UJSONRespo
-00003e70: 6e73 653a 0a20 2020 2072 6574 7572 6e20  nse:.    return 
-00003e80: 554a 534f 4e52 6573 706f 6e73 6528 7b0a  UJSONResponse({.
-00003e90: 2020 2020 2020 2020 2264 6574 6169 6c22          "detail"
-00003ea0: 3a20 2248 656c 6c6f 2077 6f72 6c64 220a  : "Hello world".
-00003eb0: 2020 2020 7d29 0a0a 0a40 6765 7428 290a      })...@get().
-00003ec0: 6173 796e 6320 6465 6620 616e 6f74 6865  async def anothe
-00003ed0: 7228 7265 7175 6573 743a 2052 6571 7565  r(request: Reque
-00003ee0: 7374 2920 2d3e 2064 6963 743a 0a20 2020  st) -> dict:.   
-00003ef0: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
-00003f00: 2020 2264 6574 6169 6c22 3a20 2241 6e6f    "detail": "Ano
-00003f10: 7468 6572 2077 6f72 6c64 2122 0a20 2020  ther world!".   
-00003f20: 207d 0a0a 4077 6562 736f 636b 6574 2870   }..@websocket(p
-00003f30: 6174 683d 222f 7b70 6174 685f 7061 7261  ath="/{path_para
-00003f40: 6d3a 7374 727d 2229 0a61 7379 6e63 2064  m:str}").async d
-00003f50: 6566 2077 6f72 6c64 5f73 6f63 6b65 7428  ef world_socket(
-00003f60: 736f 636b 6574 3a20 5765 6273 6f63 6b65  socket: Websocke
-00003f70: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-00003f80: 6177 6169 7420 736f 636b 6574 2e61 6363  await socket.acc
-00003f90: 6570 7428 290a 2020 2020 6d73 6720 3d20  ept().    msg = 
-00003fa0: 6177 6169 7420 736f 636b 6574 2e72 6563  await socket.rec
-00003fb0: 6569 7665 5f6a 736f 6e28 290a 2020 2020  eive_json().    
-00003fc0: 6173 7365 7274 206d 7367 0a20 2020 2061  assert msg.    a
-00003fd0: 7373 6572 7420 736f 636b 6574 0a20 2020  ssert socket.   
-00003fe0: 2061 7761 6974 2073 6f63 6b65 742e 636c   await socket.cl
-00003ff0: 6f73 6528 290a 0a0a 6170 7020 3d20 4573  ose()...app = Es
-00004000: 6d65 7261 6c64 2872 6f75 7465 733d 5b0a  merald(routes=[.
-00004010: 2020 2020 4761 7465 7761 7928 6861 6e64      Gateway(hand
-00004020: 6c65 723d 686f 6d65 292c 0a20 2020 2047  ler=home),.    G
-00004030: 6174 6577 6179 2868 616e 646c 6572 3d61  ateway(handler=a
-00004040: 6e6f 7468 6572 292c 0a20 2020 2057 6562  nother),.    Web
-00004050: 536f 636b 6574 4761 7465 7761 7928 6861  SocketGateway(ha
-00004060: 6e64 6c65 723d 776f 726c 645f 736f 636b  ndler=world_sock
-00004070: 6574 292c 0a5d 290a 0a60 6060 0a0a 2323  et),.])..```..##
-00004080: 2044 6573 6967 6e20 696e 206d 696e 640a   Design in mind.
-00004090: 0a47 6f6f 6420 6465 7369 676e 2069 7320  .Good design is 
-000040a0: 616c 7761 7973 2065 6e63 6f75 7261 6765  always encourage
-000040b0: 6420 616e 6420 4573 6d65 7261 6c64 2061  d and Esmerald a
-000040c0: 6c6c 6f77 7320 636f 6d70 6c65 7820 726f  llows complex ro
-000040d0: 7574 696e 6720 6f6e 2061 6e79 206c 6576  uting on any lev
-000040e0: 656c 2e0a 0a23 2323 2054 6865 2068 616e  el...### The han
-000040f0: 646c 6572 7320 2876 6965 7773 290a 0a60  dlers (views)..`
-00004100: 6060 7079 7468 6f6e 2074 6974 6c65 3d22  ``python title="
-00004110: 6d79 6170 702f 6163 636f 756e 7473 2f76  myapp/accounts/v
-00004120: 6965 7773 2e70 7922 0a66 726f 6d20 6573  iews.py".from es
-00004130: 6d65 7261 6c64 2069 6d70 6f72 7420 6765  merald import ge
-00004140: 742c 2070 6f73 742c 2070 7574 2c20 7374  t, post, put, st
-00004150: 6174 7573 2c20 7765 6273 6f63 6b65 742c  atus, websocket,
-00004160: 2041 5049 5669 6577 2c20 5265 7175 6573   APIView, Reques
-00004170: 742c 204a 534f 4e52 6573 706f 6e73 652c  t, JSONResponse,
-00004180: 2052 6573 706f 6e73 652c 2057 6562 536f   Response, WebSo
-00004190: 636b 6574 0a66 726f 6d20 7079 6461 6e74  cket.from pydant
-000041a0: 6963 2069 6d70 6f72 7420 4261 7365 4d6f  ic import BaseMo
-000041b0: 6465 6c0a 0a0a 636c 6173 7320 5072 6f64  del...class Prod
-000041c0: 7563 7428 4261 7365 4d6f 6465 6c29 3a0a  uct(BaseModel):.
-000041d0: 2020 2020 6e61 6d65 3a20 7374 720a 2020      name: str.  
-000041e0: 2020 736b 753a 2073 7472 0a20 2020 2070    sku: str.    p
-000041f0: 7269 6365 3a20 666c 6f61 740a 0a0a 4070  rice: float...@p
-00004200: 7574 2827 2f70 726f 6475 6374 2f7b 7072  ut('/product/{pr
-00004210: 6f64 7563 745f 6964 7d27 290a 6465 6620  oduct_id}').def 
-00004220: 7570 6461 7465 5f70 726f 6475 6374 2870  update_product(p
-00004230: 726f 6475 6374 5f69 643a 2069 6e74 2c20  roduct_id: int, 
-00004240: 6461 7461 3a20 5072 6f64 7563 7429 202d  data: Product) -
-00004250: 3e20 6469 6374 3a0a 2020 2020 7265 7475  > dict:.    retu
-00004260: 726e 207b 2270 726f 6475 6374 5f69 6422  rn {"product_id"
-00004270: 3a20 7072 6f64 7563 745f 6964 2c20 2270  : product_id, "p
-00004280: 726f 6475 6374 5f6e 616d 6522 3a20 7072  roduct_name": pr
-00004290: 6f64 7563 742e 6e61 6d65 207d 0a0a 0a40  oduct.name }...@
-000042a0: 6765 7428 7374 6174 7573 5f63 6f64 653d  get(status_code=
-000042b0: 7374 6174 7573 2e48 5454 505f 3230 305f  status.HTTP_200_
-000042c0: 4f4b 290a 6173 796e 6320 6465 6620 686f  OK).async def ho
-000042d0: 6d65 2829 202d 3e20 4a53 4f4e 5265 7370  me() -> JSONResp
-000042e0: 6f6e 7365 3a0a 2020 2020 7265 7475 726e  onse:.    return
-000042f0: 204a 534f 4e52 6573 706f 6e73 6528 7b0a   JSONResponse({.
-00004300: 2020 2020 2020 2020 2264 6574 6169 6c22          "detail"
-00004310: 3a20 2248 656c 6c6f 2077 6f72 6c64 220a  : "Hello world".
-00004320: 2020 2020 7d29 0a0a 0a40 6765 7428 290a      })...@get().
-00004330: 6173 796e 6320 6465 6620 616e 6f74 6865  async def anothe
-00004340: 7228 7265 7175 6573 743a 2052 6571 7565  r(request: Reque
-00004350: 7374 2920 2d3e 2064 6963 743a 0a20 2020  st) -> dict:.   
-00004360: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
-00004370: 2020 2264 6574 6169 6c22 3a20 2241 6e6f    "detail": "Ano
-00004380: 7468 6572 2077 6f72 6c64 2122 0a20 2020  ther world!".   
-00004390: 207d 0a0a 0a40 7765 6273 6f63 6b65 7428   }...@websocket(
-000043a0: 7061 7468 3d22 2f7b 7061 7468 5f70 6172  path="/{path_par
-000043b0: 616d 3a73 7472 7d22 290a 6173 796e 6320  am:str}").async 
-000043c0: 6465 6620 776f 726c 645f 736f 636b 6574  def world_socket
-000043d0: 2873 6f63 6b65 743a 2057 6562 736f 636b  (socket: Websock
-000043e0: 6574 2920 2d3e 204e 6f6e 653a 0a20 2020  et) -> None:.   
-000043f0: 2061 7761 6974 2073 6f63 6b65 742e 6163   await socket.ac
-00004400: 6365 7074 2829 0a20 2020 206d 7367 203d  cept().    msg =
-00004410: 2061 7761 6974 2073 6f63 6b65 742e 7265   await socket.re
-00004420: 6365 6976 655f 6a73 6f6e 2829 0a20 2020  ceive_json().   
-00004430: 2061 7373 6572 7420 6d73 670a 2020 2020   assert msg.    
-00004440: 6173 7365 7274 2073 6f63 6b65 740a 2020  assert socket.  
-00004450: 2020 6177 6169 7420 736f 636b 6574 2e63    await socket.c
-00004460: 6c6f 7365 2829 0a0a 0a63 6c61 7373 2057  lose()...class W
-00004470: 6f72 6c64 2841 5049 5669 6577 293a 0a0a  orld(APIView):..
-00004480: 2020 2020 4067 6574 2870 6174 683d 272f      @get(path='/
-00004490: 7b75 726c 7d27 290a 2020 2020 6173 796e  {url}').    asyn
-000044a0: 6320 6465 6620 686f 6d65 2872 6571 7565  c def home(reque
-000044b0: 7374 3a20 5265 7175 6573 742c 2075 726c  st: Request, url
-000044c0: 3a20 7374 7229 202d 3e20 5265 7370 6f6e  : str) -> Respon
-000044d0: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-000044e0: 726e 2052 6573 706f 6e73 6528 6622 5552  rn Response(f"UR
-000044f0: 4c3a 207b 7572 6c7d 2229 0a0a 2020 2020  L: {url}")..    
-00004500: 4070 6f73 7428 7061 7468 3d27 2f7b 7572  @post(path='/{ur
-00004510: 6c7d 272c 2073 7461 7475 735f 636f 6465  l}', status_code
-00004520: 3d73 7461 7475 732e 4854 5450 5f32 3031  =status.HTTP_201
-00004530: 5f43 5245 4154 4544 290a 2020 2020 6173  _CREATED).    as
-00004540: 796e 6320 6465 6620 6d61 7273 2872 6571  ync def mars(req
-00004550: 7565 7374 3a20 5265 7175 6573 742c 2075  uest: Request, u
-00004560: 726c 3a20 7374 7229 202d 3e20 4a53 4f4e  rl: str) -> JSON
-00004570: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
-00004580: 2020 2e2e 2e0a 0a20 2020 2040 7765 6273    .....    @webs
-00004590: 6f63 6b65 7428 7061 7468 3d22 2f7b 7061  ocket(path="/{pa
-000045a0: 7468 5f70 6172 616d 3a73 7472 7d22 290a  th_param:str}").
-000045b0: 2020 2020 6173 796e 6320 6465 6620 706c      async def pl
-000045c0: 7574 6f28 7365 6c66 2c20 736f 636b 6574  uto(self, socket
-000045d0: 3a20 5765 6273 6f63 6b65 7429 202d 3e20  : Websocket) -> 
-000045e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6177  None:.        aw
-000045f0: 6169 7420 736f 636b 6574 2e61 6363 6570  ait socket.accep
-00004600: 7428 290a 2020 2020 2020 2020 6d73 6720  t().        msg 
-00004610: 3d20 6177 6169 7420 736f 636b 6574 2e72  = await socket.r
-00004620: 6563 6569 7665 5f6a 736f 6e28 290a 2020  eceive_json().  
-00004630: 2020 2020 2020 6173 7365 7274 206d 7367        assert msg
-00004640: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00004650: 736f 636b 6574 0a20 2020 2020 2020 2061  socket.        a
-00004660: 7761 6974 2073 6f63 6b65 742e 636c 6f73  wait socket.clos
-00004670: 6528 290a 0a0a 6060 600a 0a49 6620 6120  e()...```..If a 
-00004680: 6070 6174 6860 2069 7320 6e6f 7420 7072  `path` is not pr
-00004690: 6f76 6964 6564 2c20 6465 6661 756c 7473  ovided, defaults
-000046a0: 2074 6f20 602f 602e 0a0a 2323 2320 5468   to `/`...### Th
-000046b0: 6520 6761 7465 7761 7973 2028 7572 6c73  e gateways (urls
-000046c0: 290a 0a60 6060 7079 7468 6f6e 2074 6974  )..```python tit
-000046d0: 6c65 3d22 6d79 6170 702f 6163 636f 756e  le="myapp/accoun
-000046e0: 7473 2f75 726c 732e 7079 220a 6672 6f6d  ts/urls.py".from
-000046f0: 2065 736d 6572 616c 6420 696d 706f 7274   esmerald import
-00004700: 2047 6174 6577 6179 2c20 5765 6253 6f63   Gateway, WebSoc
-00004710: 6b65 7447 6174 6577 6179 0a66 726f 6d20  ketGateway.from 
-00004720: 2e76 6965 7773 2069 6d70 6f72 7420 686f  .views import ho
-00004730: 6d65 2c20 616e 6f74 6865 722c 2077 6f72  me, another, wor
-00004740: 6c64 5f73 6f63 6b65 742c 2057 6f72 6c64  ld_socket, World
-00004750: 0a0a 726f 7574 655f 7061 7474 6572 6e73  ..route_patterns
-00004760: 203d 205b 0a20 2020 2047 6174 6577 6179   = [.    Gateway
-00004770: 2868 616e 646c 6572 3d75 7064 6174 655f  (handler=update_
-00004780: 7072 6f64 7563 7429 2c0a 2020 2020 4761  product),.    Ga
-00004790: 7465 7761 7928 6861 6e64 6c65 723d 686f  teway(handler=ho
-000047a0: 6d65 292c 0a20 2020 2047 6174 6577 6179  me),.    Gateway
-000047b0: 2868 616e 646c 6572 3d61 6e6f 7468 6572  (handler=another
-000047c0: 292c 0a20 2020 2047 6174 6577 6179 2868  ),.    Gateway(h
-000047d0: 616e 646c 6572 3d57 6f72 6c64 292c 0a20  andler=World),. 
-000047e0: 2020 2057 6562 536f 636b 6574 4761 7465     WebSocketGate
-000047f0: 7761 7928 6861 6e64 6c65 723d 776f 726c  way(handler=worl
-00004800: 645f 736f 636b 6574 292c 0a5d 0a0a 6060  d_socket),.]..``
-00004810: 600a 0a49 6620 6120 6070 6174 6860 2069  `..If a `path` i
-00004820: 7320 6e6f 7420 7072 6f76 6964 6564 2c20  s not provided, 
-00004830: 6465 6661 756c 7473 2074 6f20 602f 602e  defaults to `/`.
-00004840: 0a0a 2323 2320 5468 6520 496e 636c 7564  ..### The Includ
-00004850: 650a 0a54 6869 7320 6973 2061 2076 6572  e..This is a ver
-00004860: 7920 7370 6563 6961 6c20 6f62 6a65 6374  y special object
-00004870: 2074 6861 7420 616c 6c6f 7773 2074 6865   that allows the
-00004880: 2069 6d70 6f72 7420 6f66 2061 6e79 2072   import of any r
-00004890: 6f75 7465 2066 726f 6d20 616e 7977 6865  oute from anywhe
-000048a0: 7265 2069 6e20 7468 6520 6170 706c 6963  re in the applic
-000048b0: 6174 696f 6e2e 0a0a 6049 6e63 6c75 6465  ation...`Include
-000048c0: 6020 6163 6365 7074 7320 7468 6520 696d  ` accepts the im
-000048d0: 706f 7274 2076 6961 2060 6e61 6d65 7370  port via `namesp
-000048e0: 6163 6560 206f 7220 7669 6120 6072 6f75  ace` or via `rou
-000048f0: 7465 7360 206c 6973 7420 6275 7420 6e6f  tes` list but no
-00004900: 7420 626f 7468 2e0a 0a57 6865 6e20 7573  t both...When us
-00004910: 696e 6720 6120 606e 616d 6573 7061 6365  ing a `namespace
-00004920: 602c 2074 6865 2060 496e 636c 7564 6560  `, the `Include`
-00004930: 2077 696c 6c20 6c6f 6f6b 2066 6f72 2074   will look for t
-00004940: 6865 2064 6566 6175 6c74 2060 726f 7574  he default `rout
-00004950: 655f 7061 7474 6572 6e73 6020 6f62 6a65  e_patterns` obje
-00004960: 6374 206c 6973 7420 696e 2074 6865 2069  ct list in the i
-00004970: 6d70 6f72 7465 640a 6e61 6d65 7370 6163  mported.namespac
-00004980: 6520 756e 6c65 7373 2061 2064 6966 6665  e unless a diffe
-00004990: 7265 6e74 2060 7061 7474 6572 6e60 2069  rent `pattern` i
-000049a0: 7320 7370 6563 6966 6965 642e 0a0a 5468  s specified...Th
-000049b0: 6520 7061 7474 6572 6e20 6f6e 6c79 2077  e pattern only w
-000049c0: 6f72 6b73 2069 6620 7468 6520 696d 706f  orks if the impo
-000049d0: 7274 7320 6172 6520 646f 6e65 2076 6961  rts are done via
-000049e0: 2060 6e61 6d65 7370 6163 6560 2061 6e64   `namespace` and
-000049f0: 206e 6f74 2076 6961 2060 726f 7574 6573   not via `routes
-00004a00: 602e 0a0a 2a2a 496d 706f 7274 696e 6720  `...**Importing 
-00004a10: 7573 696e 6720 6e61 6d65 7370 6163 652a  using namespace*
-00004a20: 2a3a 0a0a 6060 6070 7974 686f 6e20 7469  *:..```python ti
-00004a30: 746c 653d 276d 7961 7070 2f75 726c 732e  tle='myapp/urls.
-00004a40: 7079 270a 6672 6f6d 2065 736d 6572 616c  py'.from esmeral
-00004a50: 6420 696d 706f 7274 2049 6e63 6c75 6465  d import Include
-00004a60: 0a0a 726f 7574 655f 7061 7474 6572 6e73  ..route_patterns
-00004a70: 203d 205b 0a20 2020 2049 6e63 6c75 6465   = [.    Include
-00004a80: 286e 616d 6573 7061 6365 3d27 6d79 6170  (namespace='myap
-00004a90: 702e 6163 636f 756e 7473 2e75 726c 7327  p.accounts.urls'
-00004aa0: 290a 5d0a 0a60 6060 0a0a 2a2a 496d 706f  ).]..```..**Impo
-00004ab0: 7274 696e 6720 7573 696e 6720 726f 7574  rting using rout
-00004ac0: 6573 2a2a 3a0a 0a60 6060 7079 7468 6f6e  es**:..```python
-00004ad0: 2074 6974 6c65 3d27 7372 632f 6d79 6170   title='src/myap
-00004ae0: 702f 7572 6c73 2e70 7927 0a66 726f 6d20  p/urls.py'.from 
-00004af0: 6573 6d65 7261 6c64 2069 6d70 6f72 7420  esmerald import 
-00004b00: 496e 636c 7564 650a 6672 6f6d 206d 7961  Include.from mya
-00004b10: 7070 2e61 6363 6f75 6e74 7320 696d 706f  pp.accounts impo
-00004b20: 7274 2075 726c 730a 0a72 6f75 7465 5f70  rt urls..route_p
-00004b30: 6174 7465 726e 7320 3d20 5b0a 2020 2020  atterns = [.    
-00004b40: 496e 636c 7564 6528 726f 7574 6573 3d75  Include(routes=u
-00004b50: 726c 732e 726f 7574 655f 7061 7474 6572  rls.route_patter
-00004b60: 6e73 290a 5d0a 0a60 6060 0a0a 4966 2061  ns).]..```..If a
-00004b70: 2060 7061 7468 6020 6973 206e 6f74 2070   `path` is not p
-00004b80: 726f 7669 6465 642c 2064 6566 6175 6c74  rovided, default
-00004b90: 7320 746f 2060 2f60 2e0a 0a23 2323 2320  s to `/`...#### 
-00004ba0: 5573 696e 6720 6120 6469 6666 6572 656e  Using a differen
-00004bb0: 7420 7061 7474 6572 6e0a 0a60 6060 7079  t pattern..```py
-00004bc0: 7468 6f6e 2074 6974 6c65 3d22 7372 632f  thon title="src/
-00004bd0: 6d79 6170 702f 6163 636f 756e 7473 2f75  myapp/accounts/u
-00004be0: 726c 732e 7079 220a 6672 6f6d 2065 736d  rls.py".from esm
-00004bf0: 6572 616c 6420 696d 706f 7274 2047 6174  erald import Gat
-00004c00: 6577 6179 2c20 5765 6253 6f63 6b65 7447  eway, WebSocketG
-00004c10: 6174 6577 6179 0a66 726f 6d20 2e76 6965  ateway.from .vie
-00004c20: 7773 2069 6d70 6f72 7420 686f 6d65 2c20  ws import home, 
-00004c30: 616e 6f74 6865 722c 2077 6f72 6c64 5f73  another, world_s
-00004c40: 6f63 6b65 742c 2057 6f72 6c64 0a0a 6d79  ocket, World..my
-00004c50: 5f75 726c 7320 3d20 5b0a 2020 2020 4761  _urls = [.    Ga
-00004c60: 7465 7761 7928 6861 6e64 6c65 723d 7570  teway(handler=up
-00004c70: 6461 7465 5f70 726f 6475 6374 292c 0a20  date_product),. 
-00004c80: 2020 2047 6174 6577 6179 2868 616e 646c     Gateway(handl
-00004c90: 6572 3d68 6f6d 6529 2c0a 2020 2020 4761  er=home),.    Ga
-00004ca0: 7465 7761 7928 6861 6e64 6c65 723d 616e  teway(handler=an
-00004cb0: 6f74 6865 7229 2c0a 2020 2020 4761 7465  other),.    Gate
-00004cc0: 7761 7928 6861 6e64 6c65 723d 576f 726c  way(handler=Worl
-00004cd0: 6429 2c0a 2020 2020 5765 6253 6f63 6b65  d),.    WebSocke
-00004ce0: 7447 6174 6577 6179 2868 616e 646c 6572  tGateway(handler
-00004cf0: 3d77 6f72 6c64 5f73 6f63 6b65 7429 2c0a  =world_socket),.
-00004d00: 5d0a 0a60 6060 0a0a 2a2a 496d 706f 7274  ]..```..**Import
-00004d10: 696e 6720 7573 696e 6720 6e61 6d65 7370  ing using namesp
-00004d20: 6163 652a 2a3a 0a0a 6060 6070 7974 686f  ace**:..```pytho
-00004d30: 6e20 7469 746c 653d 2773 7263 2f6d 7961  n title='src/mya
-00004d40: 7070 2f75 726c 732e 7079 270a 6672 6f6d  pp/urls.py'.from
-00004d50: 2065 736d 6572 616c 6420 696d 706f 7274   esmerald import
-00004d60: 2049 6e63 6c75 6465 0a0a 726f 7574 655f   Include..route_
-00004d70: 7061 7474 6572 6e73 203d 205b 0a20 2020  patterns = [.   
-00004d80: 2049 6e63 6c75 6465 286e 616d 6573 7061   Include(namespa
-00004d90: 6365 3d27 6d79 6170 702e 6163 636f 756e  ce='myapp.accoun
-00004da0: 7473 2e75 726c 7327 2c20 7061 7474 6572  ts.urls', patter
-00004db0: 6e3d 276d 795f 7572 6c73 2729 0a5d 0a0a  n='my_urls').]..
-00004dc0: 6060 600a 0a23 2320 496e 636c 7564 6520  ```..## Include 
-00004dd0: 616e 6420 4573 6d65 7261 6c64 0a0a 5468  and Esmerald..Th
-00004de0: 6520 6049 6e63 6c75 6465 6020 6361 6e20  e `Include` can 
-00004df0: 6265 2076 6572 7920 6865 6c70 6675 6c20  be very helpful 
-00004e00: 6d6f 7374 6c79 2077 6865 6e20 7468 6520  mostly when the 
-00004e10: 676f 616c 2069 7320 746f 2061 766f 6964  goal is to avoid
-00004e20: 2061 206c 6f74 206f 6620 696d 706f 7274   a lot of import
-00004e30: 7320 616e 6420 6d61 7373 6976 6520 6c69  s and massive li
-00004e40: 7374 0a6f 6620 6f62 6a65 6374 7320 746f  st.of objects to
-00004e50: 2062 6520 7061 7373 6564 2069 6e74 6f20   be passed into 
-00004e60: 6f6e 6520 7369 6e67 6c65 206f 626a 6563  one single objec
-00004e70: 742e 2054 6869 7320 6361 6e20 6265 2070  t. This can be p
-00004e80: 6172 7469 6375 6c61 7279 2075 7365 6675  articulary usefu
-00004e90: 6c20 746f 206d 616b 6520 6120 4573 6d65  l to make a Esme
-00004ea0: 7261 6c64 2069 6e73 7461 6e63 652e 0a0a  rald instance...
-00004eb0: 2a2a 4578 616d 706c 652a 2a3a 0a0a 6060  **Example**:..``
-00004ec0: 6070 7974 686f 6e20 7469 746c 653d 2773  `python title='s
-00004ed0: 7263 2f75 726c 732e 7079 270a 6672 6f6d  rc/urls.py'.from
-00004ee0: 2065 736d 6572 616c 6420 696d 706f 7274   esmerald import
-00004ef0: 2049 6e63 6c75 6465 0a0a 726f 7574 655f   Include..route_
-00004f00: 7061 7474 6572 6e73 203d 205b 0a20 2020  patterns = [.   
-00004f10: 2049 6e63 6c75 6465 286e 616d 6573 7061   Include(namespa
-00004f20: 6365 3d27 6d79 6170 702e 6163 636f 756e  ce='myapp.accoun
-00004f30: 7473 2e75 726c 7327 2c20 7061 7474 6572  ts.urls', patter
-00004f40: 6e3d 276d 795f 7572 6c73 2729 0a5d 0a0a  n='my_urls').]..
-00004f50: 6060 600a 0a60 6060 7079 7468 6f6e 2074  ```..```python t
-00004f60: 6974 6c65 3d27 7372 632f 6170 702e 7079  itle='src/app.py
-00004f70: 270a 6672 6f6d 2065 736d 6572 616c 6420  '.from esmerald 
-00004f80: 696d 706f 7274 2045 736d 6572 616c 642c  import Esmerald,
-00004f90: 2049 6e63 6c75 6465 0a0a 6170 7020 3d20   Include..app = 
-00004fa0: 4573 6d65 7261 6c64 2872 6f75 7465 733d  Esmerald(routes=
-00004fb0: 5b49 6e63 6c75 6465 2827 7372 632e 7572  [Include('src.ur
-00004fc0: 6c73 2729 5d29 0a0a 6060 600a 0a23 2320  ls')])..```..## 
-00004fd0: 5275 6e20 7468 6520 6170 706c 6963 6174  Run the applicat
-00004fe0: 696f 6e0a 0a41 7320 6d65 6e74 696f 6e65  ion..As mentione
-00004ff0: 6420 6265 666f 7265 2c20 7765 2072 6563  d before, we rec
-00005000: 6f6d 6d65 6e74 2075 7669 636f 726e 2066  omment uvicorn f
-00005010: 6f72 2070 726f 6475 6374 696f 6e20 6275  or production bu
-00005020: 7420 6974 2773 206e 6f74 206d 616e 6461  t it's not manda
-00005030: 746f 7279 2e0a 0a2a 2a55 7369 6e67 2075  tory...**Using u
-00005040: 7669 636f 726e 2a2a 3a0a 0a60 6060 7368  vicorn**:..```sh
-00005050: 656c 6c0a 7576 6963 6f72 6e20 7372 633a  ell.uvicorn src:
-00005060: 6170 7020 2d2d 7265 6c6f 6164 0a0a 494e  app --reload..IN
-00005070: 464f 3a20 2020 2020 5576 6963 6f72 6e20  FO:     Uvicorn 
-00005080: 7275 6e6e 696e 6720 6f6e 2068 7474 703a  running on http:
-00005090: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
-000050a0: 2028 5072 6573 7320 4354 524c 2b43 2074   (Press CTRL+C t
-000050b0: 6f20 7175 6974 290a 494e 464f 3a20 2020  o quit).INFO:   
-000050c0: 2020 5374 6172 7465 6420 7265 6c6f 6164    Started reload
-000050d0: 6572 2070 726f 6365 7373 205b 3238 3732  er process [2872
-000050e0: 305d 0a49 4e46 4f3a 2020 2020 2053 7461  0].INFO:     Sta
-000050f0: 7274 6564 2073 6572 7665 7220 7072 6f63  rted server proc
-00005100: 6573 7320 5b32 3837 3232 5d0a 494e 464f  ess [28722].INFO
-00005110: 3a20 2020 2020 5761 6974 696e 6720 666f  :     Waiting fo
-00005120: 7220 6170 706c 6963 6174 696f 6e20 7374  r application st
-00005130: 6172 7475 702e 0a49 4e46 4f3a 2020 2020  artup..INFO:    
-00005140: 2041 7070 6c69 6361 7469 6f6e 2073 7461   Application sta
-00005150: 7274 7570 2063 6f6d 706c 6574 652e 0a60  rtup complete..`
-00005160: 6060 0a0a 2323 2052 756e 2074 6865 2061  ``..## Run the a
-00005170: 7070 6c69 6361 7469 6f6e 2077 6974 6820  pplication with 
-00005180: 6375 7374 6f6d 2073 6574 7469 6e67 730a  custom settings.
-00005190: 0a2a 2a55 7369 6e67 2075 7669 636f 726e  .**Using uvicorn
-000051a0: 2a2a 3a0a 0a60 6060 7368 656c 6c0a 4553  **:..```shell.ES
-000051b0: 4d45 5241 4c44 5f53 4554 5449 4e47 535f  MERALD_SETTINGS_
-000051c0: 4d4f 4455 4c45 3d6d 7961 7070 2e41 7070  MODULE=myapp.App
-000051d0: 5365 7474 696e 6773 2075 7669 636f 726e  Settings uvicorn
-000051e0: 2073 7263 3a61 7070 202d 2d72 656c 6f61   src:app --reloa
-000051f0: 640a 0a49 4e46 4f3a 2020 2020 2055 7669  d..INFO:     Uvi
-00005200: 636f 726e 2072 756e 6e69 6e67 206f 6e20  corn running on 
-00005210: 6874 7470 3a2f 2f31 3237 2e30 2e30 2e31  http://127.0.0.1
-00005220: 3a38 3030 3020 2850 7265 7373 2043 5452  :8000 (Press CTR
-00005230: 4c2b 4320 746f 2071 7569 7429 0a49 4e46  L+C to quit).INF
-00005240: 4f3a 2020 2020 2053 7461 7274 6564 2072  O:     Started r
-00005250: 656c 6f61 6465 7220 7072 6f63 6573 7320  eloader process 
-00005260: 5b32 3837 3230 5d0a 494e 464f 3a20 2020  [28720].INFO:   
-00005270: 2020 5374 6172 7465 6420 7365 7276 6572    Started server
-00005280: 2070 726f 6365 7373 205b 3238 3732 325d   process [28722]
-00005290: 0a49 4e46 4f3a 2020 2020 2057 6169 7469  .INFO:     Waiti
-000052a0: 6e67 2066 6f72 2061 7070 6c69 6361 7469  ng for applicati
-000052b0: 6f6e 2073 7461 7274 7570 2e0a 494e 464f  on startup..INFO
-000052c0: 3a20 2020 2020 4170 706c 6963 6174 696f  :     Applicatio
-000052d0: 6e20 7374 6172 7475 7020 636f 6d70 6c65  n startup comple
-000052e0: 7465 2e0a 6060 600a 0a23 2320 4f70 656e  te..```..## Open
-000052f0: 4150 4920 646f 6375 6d65 6e74 6174 696f  API documentatio
-00005300: 6e0a 0a45 736d 6572 616c 6420 616c 736f  n..Esmerald also
-00005310: 2063 6f6d 6573 2077 6974 6820 4f70 656e   comes with Open
-00005320: 4150 4920 646f 6373 2069 6e74 6567 7261  API docs integra
-00005330: 7465 642e 2046 6f72 2074 686f 7365 2075  ted. For those u
-00005340: 7365 6420 746f 2074 6861 742c 2074 6869  sed to that, thi
-00005350: 7320 6973 2072 6f75 6768 6c79 2074 6865  s is roughly the
-00005360: 2073 616d 6520 616e 6420 746f 206d 616b   same and to mak
-00005370: 6520 6974 0a68 6170 7065 6e2c 2074 6865  e it.happen, the
-00005380: 7265 2077 6572 6520 696e 7370 6972 6174  re were inspirat
-00005390: 696f 6e73 2074 6861 7420 6865 6c70 6564  ions that helped
-000053a0: 2045 736d 6572 616c 6420 6765 7474 696e   Esmerald gettin
-000053b0: 6720 7468 6572 6520 6661 7374 2e0a 0a45  g there fast...E
-000053c0: 736d 6572 616c 6420 7374 6172 7473 2061  smerald starts a
-000053d0: 7574 6f6d 6174 6963 616c 6c79 2074 6865  utomatically the
-000053e0: 204f 7065 6e41 5049 2064 6f63 756d 656e   OpenAPI documen
-000053f0: 7461 7469 6f6e 2062 7920 696e 6a65 6374  tation by inject
-00005400: 696e 6720 7468 6520 4f70 656e 4150 4943  ing the OpenAPIC
-00005410: 6f6e 6669 6720 6465 6661 756c 7420 6672  onfig default fr
-00005420: 6f6d 0a74 6865 2073 6574 7469 6e67 7320  om.the settings 
-00005430: 616e 6420 6d61 6b65 7320 5377 6167 6765  and makes Swagge
-00005440: 722c 2052 6544 6f63 2061 6e20 5374 6f70  r, ReDoc an Stop
-00005450: 6c69 6768 7420 656c 656d 656e 7473 2061  light elements a
-00005460: 7661 696c 6162 6c65 2074 6f20 796f 7520  vailable to you 
-00005470: 6f75 7420 6f66 2074 6865 2062 6f78 2e0a  out of the box..
-00005480: 0a54 6f20 6163 6365 7373 2074 6865 204f  .To access the O
-00005490: 7065 6e41 5049 2c20 7369 6d70 6c79 2073  penAPI, simply s
-000054a0: 7461 7274 2079 6f75 7220 6c6f 6361 6c20  tart your local 
-000054b0: 6465 7665 6c6f 706d 656e 7420 616e 6420  development and 
-000054c0: 6163 6365 7373 3a0a 0a2a 202a 2a53 7761  access:..* **Swa
-000054d0: 6767 6572 2a2a 202d 2060 2f64 6f63 732f  gger** - `/docs/
-000054e0: 7377 6167 6765 7260 2e0a 2a20 2a2a 5265  swagger`..* **Re
-000054f0: 646f 632a 2a20 2d20 602f 646f 6373 2f72  doc** - `/docs/r
-00005500: 6564 6f63 602e 0a2a 202a 2a53 746f 706c  edoc`..* **Stopl
-00005510: 6967 6874 2045 6c65 6d65 6e74 732a 2a20  ight Elements** 
-00005520: 2d20 602f 646f 6373 2f65 6c65 6d65 6e74  - `/docs/element
-00005530: 7360 2e0a 0a54 6865 7265 2061 7265 206d  s`...There are m
-00005540: 6f72 6520 6465 7461 696c 7320 6162 6f75  ore details abou
-00005550: 7420 5b68 6f77 2074 6f20 636f 6e66 6967  t [how to config
-00005560: 7572 6520 7468 6520 4f70 656e 4150 4943  ure the OpenAPIC
-00005570: 6f6e 6669 675d 2868 7474 7073 3a2f 2f65  onfig](https://e
-00005580: 736d 6572 616c 642e 6465 762f 636f 6e66  smerald.dev/conf
-00005590: 6967 7572 6174 696f 6e73 2f6f 7065 6e61  igurations/opena
-000055a0: 7069 2f63 6f6e 6669 6729 0a77 6974 6869  pi/config).withi
-000055b0: 6e20 7468 6520 646f 6375 6d65 6e74 6174  n the documentat
-000055c0: 696f 6e2e 0a0a 5468 6572 6520 6973 2061  ion...There is a
-000055d0: 6c73 6f20 6120 676f 6f64 2065 7870 6c61  lso a good expla
-000055e0: 6e61 7469 6f6e 206f 6e20 686f 7720 746f  nation on how to
-000055f0: 2075 7365 2074 6865 205b 4f70 656e 4150   use the [OpenAP
-00005600: 4952 6573 706f 6e73 655d 2868 7474 7073  IResponse](https
-00005610: 3a2f 2f65 736d 6572 616c 642e 6465 762f  ://esmerald.dev/
-00005620: 7265 7370 6f6e 7365 7323 6f70 656e 6170  responses#openap
-00005630: 692d 7265 7370 6f6e 7365 7329 0a61 7320  i-responses).as 
-00005640: 7765 6c6c 2e0a 0a23 2320 4e6f 7465 730a  well...## Notes.
-00005650: 0a54 6869 7320 6973 206a 7573 7420 6120  .This is just a 
-00005660: 7665 7279 2068 6967 682d 6c65 7665 6c20  very high-level 
-00005670: 6465 6d6f 6e73 7472 6174 696f 6e20 6f66  demonstration of
-00005680: 2068 6f77 2074 6f20 7374 6172 7420 7175   how to start qu
-00005690: 6963 6b6c 7920 616e 6420 7768 6174 2045  ickly and what E
-000056a0: 736d 6572 616c 6420 6361 6e20 646f 2e0a  smerald can do..
-000056b0: 5468 6572 6520 6172 6520 706c 656e 7479  There are plenty
-000056c0: 206d 6f72 6520 7468 696e 6773 2079 6f75   more things you
-000056d0: 2063 616e 2064 6f20 7769 7468 2045 736d   can do with Esm
-000056e0: 6572 616c 642e 2045 6e6a 6f79 2120 f09f  erald. Enjoy! ..
-000056f0: 988a 0a0a 2323 2053 706f 6e73 6f72 730a  ....## Sponsors.
-00005700: 0a43 7572 7265 6e74 6c79 2074 6865 7265  .Currently there
-00005710: 2061 7265 206e 6f20 7370 6f6e 736f 7273   are no sponsors
-00005720: 206f 6620 4573 6d65 7261 6c64 2062 7574   of Esmerald but
-00005730: 2079 6f75 2063 616e 2066 696e 616e 6369   you can financi
-00005740: 616c 6c79 2068 656c 7020 616e 6420 7375  ally help and su
-00005750: 7070 6f72 7420 7468 6520 6175 7468 6f72  pport the author
-00005760: 2074 686f 7567 680a 5b47 6974 4875 6220   though.[GitHub 
-00005770: 7370 6f6e 736f 7273 5d28 6874 7470 733a  sponsors](https:
-00005780: 2f2f 6769 7468 7562 2e63 6f6d 2f73 706f  //github.com/spo
-00005790: 6e73 6f72 732f 7461 7273 696c 2920 616e  nsors/tarsil) an
-000057a0: 6420 6265 636f 6d65 2061 202a 2a53 7065  d become a **Spe
-000057b0: 6369 616c 206f 6e65 2a2a 206f 7220 6120  cial one** or a 
-000057c0: 2a2a 4c65 6765 6e64 2a2a 2e0a 0a5b 7361  **Legend**...[sa
-000057d0: 6666 6965 725f 6f72 6d5d 3a20 6874 7470  ffier_orm]: http
-000057e0: 733a 2f2f 6573 6d65 7261 6c64 2e64 6576  s://esmerald.dev
-000057f0: 2f64 6174 6162 6173 6573 2f73 6166 6669  /databases/saffi
-00005800: 6572 2f6d 6f74 6976 6174 696f 6e0a 5b65  er/motivation.[e
-00005810: 6467 795f 6f72 6d5d 3a20 6874 7470 733a  dgy_orm]: https:
-00005820: 2f2f 6573 6d65 7261 6c64 2e64 6576 2f64  //esmerald.dev/d
-00005830: 6174 6162 6173 6573 2f73 6166 6669 6572  atabases/saffier
-00005840: 2f6d 6f74 6976 6174 696f 6e0a 5b6d 6f6e  /motivation.[mon
-00005850: 676f 7a5f 6f64 6d5d 3a20 6874 7470 733a  goz_odm]: https:
-00005860: 2f2f 6573 6d65 7261 6c64 2e64 6576 2f64  //esmerald.dev/d
-00005870: 6174 6162 6173 6573 2f6d 6f6e 676f 7a2f  atabases/mongoz/
-00005880: 6d6f 7469 7661 7469 6f6e 0a              motivation.
+00000a50: 4469 7374 3a20 7576 6963 6f72 6e5b 7374  Dist: uvicorn[st
+00000a60: 616e 6461 7264 5d3e 3d30 2e32 342e 303b  andard]>=0.24.0;
+00000a70: 2065 7874 7261 203d 3d20 2764 6576 270a   extra == 'dev'.
+00000a80: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000a90: 656e 636f 6465 7273 0a52 6571 7569 7265  encoders.Require
+00000aa0: 732d 4469 7374 3a20 756a 736f 6e3c 362c  s-Dist: ujson<6,
+00000ab0: 3e3d 352e 372e 303b 2065 7874 7261 203d  >=5.7.0; extra =
+00000ac0: 3d20 2765 6e63 6f64 6572 7327 0a50 726f  = 'encoders'.Pro
+00000ad0: 7669 6465 732d 4578 7472 613a 206a 7774  vides-Extra: jwt
+00000ae0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000af0: 7061 7373 6c69 623d 3d31 2e37 2e34 3b20  passlib==1.7.4; 
+00000b00: 6578 7472 6120 3d3d 2027 6a77 7427 0a52  extra == 'jwt'.R
+00000b10: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000b20: 7468 6f6e 2d6a 6f73 653c 342c 3e3d 332e  thon-jose<4,>=3.
+00000b30: 332e 303b 2065 7874 7261 203d 3d20 276a  3.0; extra == 'j
+00000b40: 7774 270a 5072 6f76 6964 6573 2d45 7874  wt'.Provides-Ext
+00000b50: 7261 3a20 7363 6865 6475 6c65 7273 0a52  ra: schedulers.R
+00000b60: 6571 7569 7265 732d 4469 7374 3a20 6173  equires-Dist: as
+00000b70: 796e 637a 3e3d 302e 342e 303b 2065 7874  yncz>=0.4.0; ext
+00000b80: 7261 203d 3d20 2773 6368 6564 756c 6572  ra == 'scheduler
+00000b90: 7327 0a50 726f 7669 6465 732d 4578 7472  s'.Provides-Extr
+00000ba0: 613a 2074 656d 706c 6174 6573 0a52 6571  a: templates.Req
+00000bb0: 7569 7265 732d 4469 7374 3a20 6d61 6b6f  uires-Dist: mako
+00000bc0: 3c32 2e30 2e30 2c3e 3d31 2e32 2e34 3b20  <2.0.0,>=1.2.4; 
+00000bd0: 6578 7472 6120 3d3d 2027 7465 6d70 6c61  extra == 'templa
+00000be0: 7465 7327 0a50 726f 7669 6465 732d 4578  tes'.Provides-Ex
+00000bf0: 7472 613a 2074 6573 740a 5265 7175 6972  tra: test.Requir
+00000c00: 6573 2d44 6973 743a 2068 7474 7078 3c30  es-Dist: httpx<0
+00000c10: 2e33 302e 302c 3e3d 302e 3235 2e30 3b20  .30.0,>=0.25.0; 
+00000c20: 6578 7472 6120 3d3d 2027 7465 7374 270a  extra == 'test'.
+00000c30: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+00000c40: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+00000c50: 6172 6b64 6f77 6e0a 0a23 2045 736d 6572  arkdown..# Esmer
+00000c60: 616c 640a 0a3c 7020 616c 6967 6e3d 2263  ald..<p align="c
+00000c70: 656e 7465 7222 3e0a 2020 3c61 2068 7265  enter">.  <a hre
+00000c80: 663d 2268 7474 7073 3a2f 2f65 736d 6572  f="https://esmer
+00000c90: 616c 642e 6465 7622 3e3c 696d 6720 7372  ald.dev"><img sr
+00000ca0: 633d 2268 7474 7073 3a2f 2f72 6573 2e63  c="https://res.c
+00000cb0: 6c6f 7564 696e 6172 792e 636f 6d2f 6479  loudinary.com/dy
+00000cc0: 6d6d 6f6e 642f 696d 6167 652f 7570 6c6f  mmond/image/uplo
+00000cd0: 6164 2f76 3136 3733 3631 3933 3432 2f65  ad/v1673619342/e
+00000ce0: 736d 6572 616c 642f 696d 672f 6c6f 676f  smerald/img/logo
+00000cf0: 2d67 725f 7a31 6f74 386f 2e70 6e67 2220  -gr_z1ot8o.png" 
+00000d00: 616c 743d 2745 736d 6572 616c 6427 3e3c  alt='Esmerald'><
+00000d10: 2f61 3e0a 3c2f 703e 0a0a 3c70 2061 6c69  /a>.</p>..<p ali
+00000d20: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000d30: 203c 656d 3ef0 9f9a 8020 4869 6768 6c79   <em>.... Highly
+00000d40: 2073 6361 6c61 626c 652c 2070 6572 666f   scalable, perfo
+00000d50: 726d 616e 742c 2065 6173 7920 746f 206c  rmant, easy to l
+00000d60: 6561 726e 2c20 6561 7379 2074 6f20 636f  earn, easy to co
+00000d70: 6465 2061 6e64 2066 6f72 2065 7665 7279  de and for every
+00000d80: 2061 7070 6c69 6361 7469 6f6e 2e20 f09f   application. ..
+00000d90: 9a80 3c2f 656d 3e0a 3c2f 703e 0a0a 3c70  ..</em>.</p>..<p
+00000da0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000db0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000dc0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 796d  //github.com/dym
+00000dd0: 6d6f 6e64 2f65 736d 6572 616c 642f 776f  mond/esmerald/wo
+00000de0: 726b 666c 6f77 732f 5465 7374 2532 3053  rkflows/Test%20S
+00000df0: 7569 7465 2f62 6164 6765 2e73 7667 3f65  uite/badge.svg?e
+00000e00: 7665 6e74 3d70 7573 6826 6272 616e 6368  vent=push&branch
+00000e10: 3d6d 6169 6e22 2074 6172 6765 743d 225f  =main" target="_
+00000e20: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
+00000e30: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000e40: 7468 7562 2e63 6f6d 2f64 796d 6d6f 6e64  thub.com/dymmond
+00000e50: 2f65 736d 6572 616c 642f 776f 726b 666c  /esmerald/workfl
+00000e60: 6f77 732f 5465 7374 2532 3053 7569 7465  ows/Test%20Suite
+00000e70: 2f62 6164 6765 2e73 7667 3f65 7665 6e74  /badge.svg?event
+00000e80: 3d70 7573 6826 6272 616e 6368 3d6d 6169  =push&branch=mai
+00000e90: 6e22 2061 6c74 3d22 5465 7374 2053 7569  n" alt="Test Sui
+00000ea0: 7465 223e 0a3c 2f61 3e0a 0a3c 6120 6872  te">.</a>..<a hr
+00000eb0: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+00000ec0: 2e6f 7267 2f70 726f 6a65 6374 2f65 736d  .org/project/esm
+00000ed0: 6572 616c 6422 2074 6172 6765 743d 225f  erald" target="_
+00000ee0: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
+00000ef0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000f00: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000f10: 692f 762f 6573 6d65 7261 6c64 3f63 6f6c  i/v/esmerald?col
+00000f20: 6f72 3d25 3233 3334 4430 3538 266c 6162  or=%2334D058&lab
+00000f30: 656c 3d70 7970 6925 3230 7061 636b 6167  el=pypi%20packag
+00000f40: 6522 2061 6c74 3d22 5061 636b 6167 6520  e" alt="Package 
+00000f50: 7665 7273 696f 6e22 3e0a 3c2f 613e 0a0a  version">.</a>..
+00000f60: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000f70: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000f80: 742f 6573 6d65 7261 6c64 2220 7461 7267  t/esmerald" targ
+00000f90: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
+00000fa0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000fb0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000fc0: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
+00000fd0: 732f 6573 6d65 7261 6c64 2e73 7667 3f63  s/esmerald.svg?c
+00000fe0: 6f6c 6f72 3d25 3233 3334 4430 3538 2220  olor=%2334D058" 
+00000ff0: 616c 743d 2253 7570 706f 7274 6564 2050  alt="Supported P
+00001000: 7974 686f 6e20 7665 7273 696f 6e73 223e  ython versions">
+00001010: 0a3c 2f61 3e0a 3c2f 703e 0a0a 2d2d 2d0a  .</a>.</p>..---.
+00001020: 0a2a 2a44 6f63 756d 656e 7461 7469 6f6e  .**Documentation
+00001030: 2a2a 3a20 5b68 7474 7073 3a2f 2f65 736d  **: [https://esm
+00001040: 6572 616c 642e 6465 765d 2868 7474 7073  erald.dev](https
+00001050: 3a2f 2f77 7777 2e65 736d 6572 616c 642e  ://www.esmerald.
+00001060: 6465 7629 20f0 9f93 9a0a 0a2a 2a53 6f75  dev) ......**Sou
+00001070: 7263 6520 436f 6465 2a2a 3a20 5b68 7474  rce Code**: [htt
+00001080: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001090: 6479 6d6d 6f6e 642f 6573 6d65 7261 6c64  dymmond/esmerald
+000010a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000010b0: 2e63 6f6d 2f64 796d 6d6f 6e64 2f65 736d  .com/dymmond/esm
+000010c0: 6572 616c 6429 0a0a 2a2a 5468 6520 6f66  erald)..**The of
+000010d0: 6669 6369 616c 2073 7570 706f 7274 6564  ficial supported
+000010e0: 2076 6572 7369 6f6e 2069 7320 616c 7761   version is alwa
+000010f0: 7973 2074 6865 206c 6174 6573 7420 7265  ys the latest re
+00001100: 6c65 6173 6564 2a2a 2e0a 0a2d 2d2d 0a0a  leased**...---..
+00001110: 4573 6d65 7261 6c64 2069 7320 6120 6d6f  Esmerald is a mo
+00001120: 6465 726e 2c20 706f 7765 7266 756c 2c20  dern, powerful, 
+00001130: 666c 6578 6962 6c65 2c20 6869 6768 2070  flexible, high p
+00001140: 6572 666f 726d 616e 742c 2077 6562 2066  erformant, web f
+00001150: 7261 6d65 776f 726b 2064 6573 6967 6e65  ramework designe
+00001160: 6420 746f 2062 7569 6c64 206e 6f74 206f  d to build not o
+00001170: 6e6c 7920 4150 4973 0a62 7574 2061 6c73  nly APIs.but als
+00001180: 6f20 6675 6c6c 2073 6361 6c61 626c 6520  o full scalable 
+00001190: 6170 706c 6963 6174 696f 6e73 2066 726f  applications fro
+000011a0: 6d20 7468 6520 736d 616c 6c65 7374 2074  m the smallest t
+000011b0: 6f20 656e 7465 7270 7269 7365 206c 6576  o enterprise lev
+000011c0: 656c 2e0a 0a45 736d 6572 616c 6420 6973  el...Esmerald is
+000011d0: 2064 6573 6967 6e65 6420 746f 2062 7569   designed to bui
+000011e0: 6c64 2077 6974 6820 7079 7468 6f6e 2033  ld with python 3
+000011f0: 2e38 2b20 616e 6420 6261 7365 6420 6f6e  .8+ and based on
+00001200: 2073 7461 6e64 6172 6420 7079 7468 6f6e   standard python
+00001210: 2074 7970 6520 6869 6e74 732e 2049 6e69   type hints. Ini
+00001220: 7469 616c 6c79 0a62 7569 6c74 206f 6e20  tially.built on 
+00001230: 7468 6520 746f 7020 6f66 205b 5374 6172  the top of [Star
+00001240: 6c65 7474 655d 2868 7474 7073 3a2f 2f67  lette](https://g
+00001250: 6974 6875 622e 636f 6d2f 656e 636f 6465  ithub.com/encode
+00001260: 2f73 7461 726c 6574 7465 2920 616e 6420  /starlette) and 
+00001270: 6c61 7465 7220 6f6e 206d 6f76 6564 2074  later on moved t
+00001280: 6f20 5b4c 696c 7961 5d28 6874 7470 733a  o [Lilya](https:
+00001290: 2f2f 6c69 6c79 612e 6465 7629 2061 6e64  //lilya.dev) and
+000012a0: 205b 5079 6461 6e74 6963 5d28 6874 7470   [Pydantic](http
+000012b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+000012c0: 616d 7565 6c63 6f6c 7669 6e2f 7079 6461  amuelcolvin/pyda
+000012d0: 6e74 6963 292f 5b6d 7367 7370 6563 5d28  ntic)/[msgspec](
+000012e0: 6874 7470 733a 2f2f 6a63 7269 7374 6861  https://jcristha
+000012f0: 7269 662e 636f 6d2f 6d73 6773 7065 632f  rif.com/msgspec/
+00001300: 292e 0a0a 4368 6563 6b20 6f75 7420 7468  )...Check out th
+00001310: 6520 5b45 736d 6572 616c 6420 646f 6375  e [Esmerald docu
+00001320: 6d65 6e74 6174 696f 6e20 f09f 939a 5d28  mentation ....](
+00001330: 6874 7470 733a 2f2f 6573 6d65 7261 6c64  https://esmerald
+00001340: 2e64 6576 290a 0a2a 2a54 6865 206f 6666  .dev)..**The off
+00001350: 6963 6961 6c20 7375 7070 6f72 7465 6420  icial supported 
+00001360: 7665 7273 696f 6e20 6973 2061 6c77 6179  version is alway
+00001370: 7320 7468 6520 6c61 7465 7374 2072 656c  s the latest rel
+00001380: 6561 7365 642a 2a2e 0a0a 2323 204d 6f74  eased**...## Mot
+00001390: 6976 6174 696f 6e0a 0a54 6865 7265 2061  ivation..There a
+000013a0: 7265 2067 7265 6174 2066 7261 6d65 776f  re great framewo
+000013b0: 726b 7320 6f75 7420 7468 6572 6520 6c69  rks out there li
+000013c0: 6b65 2046 6173 7441 5049 2c20 5374 6172  ke FastAPI, Star
+000013d0: 6c69 7465 2c20 466c 616d 612c 2046 6c61  lite, Flama, Fla
+000013e0: 736b 2c20 446a 616e 676f 2e2e 2e20 416c  sk, Django... Al
+000013f0: 6c20 6f66 2074 6865 6d20 736f 6c76 696e  l of them solvin
+00001400: 6720 6d61 6a6f 7269 7479 0a6f 6620 7468  g majority.of th
+00001410: 6520 6375 7272 656e 7420 6461 792d 746f  e current day-to
+00001420: 2d64 6179 2070 726f 626c 656d 7320 6f66  -day problems of
+00001430: 2039 3925 206f 6620 7468 6520 6170 706c   99% of the appl
+00001440: 6963 6174 696f 6e73 2062 7574 206c 6561  ications but lea
+00001450: 7669 6e67 2074 6865 2031 2520 7468 6174  ving the 1% that
+00001460: 2069 7320 7573 7561 6c6c 7920 6172 6f75   is usually arou
+00001470: 6e64 2073 7472 7563 7475 7265 0a61 6e64  nd structure.and
+00001480: 2064 6573 6967 6e2f 6275 7369 6e65 7373   design/business
+00001490: 2077 6974 686f 7574 2074 6f20 6d75 6368   without to much
+000014a0: 2074 6f20 646f 2e0a 0a45 736d 6572 616c   to do...Esmeral
+000014b0: 6420 676f 7420 7468 6520 696e 7370 6972  d got the inspir
+000014c0: 6174 696f 6e20 6672 6f6d 2074 686f 7365  ation from those
+000014d0: 2067 7265 6174 2066 7261 6d65 776f 726b   great framework
+000014e0: 7320 6f75 7420 7468 6572 6520 616e 6420  s out there and 
+000014f0: 7761 7320 6275 696c 7420 7769 7468 2061  was built with a
+00001500: 6c6c 2074 6865 206b 6e6f 776e 2061 6d61  ll the known ama
+00001510: 7a69 6e67 0a66 6561 7475 7265 7320 6275  zing.features bu
+00001520: 7420 7769 7468 2062 7573 696e 6573 7320  t with business 
+00001530: 696e 206d 696e 6420 6173 2077 656c 6c2e  in mind as well.
+00001540: 2053 7461 726c 6974 652c 2066 6f72 2065   Starlite, for e
+00001550: 7861 6d70 6c65 2c20 6761 7665 2074 6865  xample, gave the
+00001560: 2069 6e73 7069 7261 7469 6f6e 2066 6f72   inspiration for
+00001570: 2074 6865 2074 7261 6e73 666f 726d 6572   the transformer
+00001580: 7320 616e 6420 666f 7220 7468 6520 5369  s and for the Si
+00001590: 676e 6174 7572 6520 6d6f 6465 6c73 2c0a  gnature models,.
+000015a0: 736f 6d65 7468 696e 6720 7665 7279 2075  something very u
+000015b0: 7365 6675 6c20 7468 6174 2068 656c 7065  seful that helpe
+000015c0: 6420 4573 6d65 7261 6c64 2069 6e74 6567  d Esmerald integ
+000015d0: 6572 6174 696e 6720 7769 7468 2070 7964  erating with pyd
+000015e0: 616e 7469 632e 0a46 6173 7441 5049 2067  antic..FastAPI g
+000015f0: 6176 6520 7468 6520 696e 7370 6972 6174  ave the inspirat
+00001600: 696f 6e20 666f 7220 4150 4920 6465 7369  ion for API desi
+00001610: 676e 696e 672c 2044 6a61 6e67 6f20 666f  gning, Django fo
+00001620: 7220 7468 6520 7065 726d 6973 7369 6f6e  r the permission
+00001630: 732c 2046 6c61 736b 2066 6f72 2074 6865  s, Flask for the
+00001640: 2073 696d 706c 6963 6974 792c 204e 6573   simplicity, Nes
+00001650: 744a 5320 666f 7220 7468 650a 636f 6e74  tJS for the.cont
+00001660: 726f 6c6c 6572 7320 616e 6420 7468 6520  rollers and the 
+00001670: 6c69 7374 2067 6f65 7320 6f6e 2e0a 0a46  list goes on...F
+00001680: 6f72 2061 206a 6f62 2074 6f20 6265 2064  or a job to be d
+00001690: 6f6e 6520 7072 6f70 6572 6c79 2c20 7573  one properly, us
+000016a0: 7561 6c6c 7920 6974 2069 7320 6e65 7665  ually it is neve
+000016b0: 7220 646f 6e65 2061 6c6f 6e65 2061 6e64  r done alone and
+000016c0: 2074 6865 7265 2069 7320 616c 7761 7973   there is always
+000016d0: 2061 2064 7269 7665 7220 616e 6420 696e   a driver and in
+000016e0: 7370 6972 6174 696f 6e20 746f 2069 742e  spiration to it.
+000016f0: 0a0a 2323 2052 6571 7569 7265 6d65 6e74  ..## Requirement
+00001700: 730a 0a2a 2070 7974 686f 6e20 332e 382b  s..* python 3.8+
+00001710: 0a0a 4573 6d65 7261 6c64 2077 6f75 6c64  ..Esmerald would
+00001720: 6e27 7420 6265 2070 6f73 7369 626c 6520  n't be possible 
+00001730: 7769 7468 6f75 7420 7477 6f20 636f 6c6f  without two colo
+00001740: 7373 616c 733a 0a0a 2a20 3c61 2068 7265  ssals:..* <a hre
+00001750: 663d 2268 7474 7073 3a2f 2f77 7777 2e6c  f="https://www.l
+00001760: 696c 7961 2e64 6576 2f22 2063 6c61 7373  ilya.dev/" class
+00001770: 3d22 6578 7465 726e 616c 2d6c 696e 6b22  ="external-link"
+00001780: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00001790: 3e53 7461 726c 6574 7465 3c2f 613e 0a2a  >Starlette</a>.*
+000017a0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000017b0: 2f2f 7079 6461 6e74 6963 2d64 6f63 732e  //pydantic-docs.
+000017c0: 6865 6c70 6d61 6e75 616c 2e69 6f2f 2220  helpmanual.io/" 
+000017d0: 636c 6173 733d 2265 7874 6572 6e61 6c2d  class="external-
+000017e0: 6c69 6e6b 2220 7461 7267 6574 3d22 5f62  link" target="_b
+000017f0: 6c61 6e6b 223e 5079 6461 6e74 6963 3c2f  lank">Pydantic</
+00001800: 613e 0a0a 2323 2049 6e73 7461 6c6c 6174  a>..## Installat
+00001810: 696f 6e0a 0a60 6060 7368 656c 6c0a 2420  ion..```shell.$ 
+00001820: 7069 7020 696e 7374 616c 6c20 6573 6d65  pip install esme
+00001830: 7261 6c64 0a60 6060 0a0a 416e 2041 5347  rald.```..An ASG
+00001840: 4920 7365 7276 6572 2069 7320 616c 736f  I server is also
+00001850: 206e 6565 6465 6420 746f 2072 756e 2069   needed to run i
+00001860: 6e20 7072 6f64 7563 7469 6f6e 2c20 7765  n production, we
+00001870: 2072 6563 6f6d 6d65 6e64 205b 5576 6963   recommend [Uvic
+00001880: 6f72 6e5d 2868 7474 7073 3a2f 2f77 7777  orn](https://www
+00001890: 2e75 7669 636f 726e 2e6f 7267 2920 6275  .uvicorn.org) bu
+000018a0: 7420 6974 2069 7320 656e 7469 7265 6c79  t it is entirely
+000018b0: 0a75 7020 746f 2079 6f75 2e0a 0a60 6060  .up to you...```
+000018c0: 7368 656c 6c0a 2420 7069 7020 696e 7374  shell.$ pip inst
+000018d0: 616c 6c20 7576 6963 6f72 6e0a 0a60 6060  all uvicorn..```
+000018e0: 0a0a 4966 2079 6f75 2077 616e 7420 696e  ..If you want in
+000018f0: 7374 616c 6c20 6573 6d65 7261 6c64 2077  stall esmerald w
+00001900: 6974 6820 7370 6563 6966 6963 733a 0a0a  ith specifics:..
+00001910: 2a2a 5375 7070 6f72 7420 666f 7220 7465  **Support for te
+00001920: 6d70 6c61 7465 2073 7973 7465 6d20 7375  mplate system su
+00001930: 6368 2061 7320 6a69 6e6a 6132 2061 6e64  ch as jinja2 and
+00001940: 206d 616b 6f2a 2a3a 0a0a 6060 6073 6865   mako**:..```she
+00001950: 6c6c 0a24 2070 6970 2069 6e73 7461 6c6c  ll.$ pip install
+00001960: 2065 736d 6572 616c 645b 7465 6d70 6c61   esmerald[templa
+00001970: 7465 735d 0a60 6060 0a0a 2a2a 5375 7070  tes].```..**Supp
+00001980: 6f72 7420 666f 7220 7468 6520 696e 7465  ort for the inte
+00001990: 726e 616c 2073 6368 6564 756c 6572 2a2a  rnal scheduler**
+000019a0: 3a0a 0a60 6060 7368 656c 6c0a 2420 7069  :..```shell.$ pi
+000019b0: 7020 696e 7374 616c 6c20 6573 6d65 7261  p install esmera
+000019c0: 6c64 5b73 6368 6564 756c 6572 735d 0a60  ld[schedulers].`
+000019d0: 6060 0a0a 2a2a 5375 7070 6f72 7420 666f  ``..**Support fo
+000019e0: 7220 7468 6520 6a77 7420 7573 6564 2069  r the jwt used i
+000019f0: 6e74 6572 6e61 6c6c 7920 6279 2045 736d  nternally by Esm
+00001a00: 6572 616c 642a 2a3a 0a0a 6060 6073 6865  erald**:..```she
+00001a10: 6c6c 0a24 2070 6970 2069 6e73 7461 6c6c  ll.$ pip install
+00001a20: 2065 736d 6572 616c 645b 6a77 745d 0a60   esmerald[jwt].`
+00001a30: 6060 0a0a 2a2a 5375 7070 6f72 7420 666f  ``..**Support fo
+00001a40: 7220 4f52 4a53 4f4e 2061 6e64 2055 4a53  r ORJSON and UJS
+00001a50: 4f4e 2a2a 3a0a 0a60 6060 7368 656c 6c0a  ON**:..```shell.
+00001a60: 2420 7069 7020 696e 7374 616c 6c20 6573  $ pip install es
+00001a70: 6d65 7261 6c64 5b65 6e63 6f64 6572 735d  merald[encoders]
+00001a80: 0a60 6060 0a0a 2a2a 4966 2079 6f75 2077  .```..**If you w
+00001a90: 616e 7420 746f 2075 7365 2074 6865 2065  ant to use the e
+00001aa0: 736d 6572 616c 6420 7465 7374 696e 6720  smerald testing 
+00001ab0: 636c 6965 6e74 2a2a 3a0a 0a60 6060 7368  client**:..```sh
+00001ac0: 656c 6c0a 2420 7069 7020 696e 7374 616c  ell.$ pip instal
+00001ad0: 6c20 6573 6d65 7261 6c64 5b74 6573 745d  l esmerald[test]
+00001ae0: 0a60 6060 0a0a 2a2a 4966 2079 6f75 2077  .```..**If you w
+00001af0: 616e 7420 746f 2075 7365 2074 6865 2065  ant to use the e
+00001b00: 736d 6572 616c 6420 7368 656c 6c2a 2a3a  smerald shell**:
+00001b10: 0a0a 4d6f 7265 205b 6465 7461 696c 735d  ..More [details]
+00001b20: 2868 7474 7073 3a2f 2f65 736d 6572 616c  (https://esmeral
+00001b30: 642e 6465 762f 6469 7265 6374 6976 6573  d.dev/directives
+00001b40: 2f73 6865 6c6c 2920 6162 6f75 7420 7468  /shell) about th
+00001b50: 6973 2074 6f70 6963 205b 696e 2074 6865  is topic [in the
+00001b60: 2064 6f63 735d 2868 7474 7073 3a2f 2f65   docs](https://e
+00001b70: 736d 6572 616c 642e 6465 762f 6469 7265  smerald.dev/dire
+00001b80: 6374 6976 6573 2f73 6865 6c6c 290a 0a60  ctives/shell)..`
+00001b90: 6060 7368 656c 6c0a 2420 7069 7020 696e  ``shell.$ pip in
+00001ba0: 7374 616c 6c20 6573 6d65 7261 6c64 5b69  stall esmerald[i
+00001bb0: 7079 7468 6f6e 5d20 2320 6465 6661 756c  python] # defaul
+00001bc0: 7420 7368 656c 6c0a 2420 7069 7020 696e  t shell.$ pip in
+00001bd0: 7374 616c 6c20 6573 6d65 7261 6c64 5b70  stall esmerald[p
+00001be0: 7470 7974 686f 6e5d 2023 2070 7470 7974  tpython] # ptpyt
+00001bf0: 686f 6e20 7368 656c 6c0a 6060 600a 0a23  hon shell.```..#
+00001c00: 2323 2053 7461 7274 2061 2070 726f 6a65  ## Start a proje
+00001c10: 6374 2075 7369 6e67 2064 6972 6563 7469  ct using directi
+00001c20: 7665 730a 0a21 2121 2057 6172 6e69 6e67  ves..!!! Warning
+00001c30: 0a20 2020 2054 6869 7320 6973 2066 6f72  .    This is for
+00001c40: 206d 6f72 6520 6164 7661 6e63 6564 2075   more advanced u
+00001c50: 7365 7273 2074 6861 7420 6172 6520 616c  sers that are al
+00001c60: 7265 6164 7920 636f 6d66 6f72 7461 626c  ready comfortabl
+00001c70: 6520 7769 7468 2045 736d 6572 616c 6420  e with Esmerald 
+00001c80: 286f 7220 5079 7468 6f6e 2069 6e20 6765  (or Python in ge
+00001c90: 6e65 7261 6c29 0a20 2020 206f 7220 6665  neral).    or fe
+00001ca0: 656c 206c 696b 6520 6974 2069 7320 6e6f  el like it is no
+00001cb0: 7420 6120 7072 6f62 6c65 6d20 7573 696e  t a problem usin
+00001cc0: 6720 7468 6573 6520 6469 7265 6374 6976  g these directiv
+00001cd0: 6573 2e20 4966 2079 6f75 2064 6f20 6e6f  es. If you do no
+00001ce0: 7420 6665 656c 2063 6f6d 666f 7274 6162  t feel comfortab
+00001cf0: 6c65 2079 6574 2074 6f20 7573 6520 7468  le yet to use th
+00001d00: 6973 2c0a 2020 2020 706c 6561 7365 2063  is,.    please c
+00001d10: 6f6e 7469 6e75 6520 7265 6164 696e 6720  ontinue reading 
+00001d20: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00001d30: 6e20 616e 6420 6c65 6172 6e69 6e67 206d  n and learning m
+00001d40: 6f72 6520 6162 6f75 7420 4573 6d65 7261  ore about Esmera
+00001d50: 6c64 2e0a 0a49 6620 796f 7520 7769 7368  ld...If you wish
+00001d60: 2074 6f20 7374 6172 7420 616e 2045 736d   to start an Esm
+00001d70: 6572 616c 6420 7072 6f6a 6563 7420 7769  erald project wi
+00001d80: 7468 2061 2064 6566 6175 6c74 2073 7567  th a default sug
+00001d90: 6765 7374 6564 2073 7472 7563 7475 7265  gested structure
+00001da0: 2e0a 0a60 6060 7368 656c 6c0a 6573 6d65  ...```shell.esme
+00001db0: 7261 6c64 2063 7265 6174 6570 726f 6a65  rald createproje
+00001dc0: 6374 203c 594f 5552 2d50 524f 4a45 4354  ct <YOUR-PROJECT
+00001dd0: 2d4e 414d 453e 0a60 6060 0a0a 5468 6973  -NAME>.```..This
+00001de0: 2077 696c 6c20 6765 6e65 7261 7465 2061   will generate a
+00001df0: 2073 6361 6666 6f6c 6420 666f 7220 796f   scaffold for yo
+00001e00: 7572 2070 726f 6a65 6374 2077 6974 6820  ur project with 
+00001e10: 736f 6d65 2070 7265 2d64 6566 696e 6564  some pre-defined
+00001e20: 2066 696c 6573 2069 6e20 6120 7369 6d70   files in a simp
+00001e30: 6c65 2066 6173 6869 6f6e 2e0a 5468 6973  le fashion..This
+00001e40: 2077 696c 6c20 616c 736f 2067 656e 6572   will also gener
+00001e50: 6174 6520 6120 6669 6c65 2066 6f72 2074  ate a file for t
+00001e60: 6865 2074 6573 7473 2075 7369 6e67 2074  he tests using t
+00001e70: 6865 2045 736d 6572 616c 6454 6573 7443  he EsmeraldTestC
+00001e80: 6c69 656e 742c 2073 6f20 6d61 6b65 2073  lient, so make s
+00001e90: 7572 6520 796f 7520 7275 6e3a 0a0a 6060  ure you run:..``
+00001ea0: 6073 6865 6c6c 0a24 2070 6970 2069 6e73  `shell.$ pip ins
+00001eb0: 7461 6c6c 2065 736d 6572 616c 645b 7465  tall esmerald[te
+00001ec0: 7374 5d0a 6060 600a 0a4f 7220 796f 7520  st].```..Or you 
+00001ed0: 6361 6e20 736b 6970 2074 6869 7320 7374  can skip this st
+00001ee0: 6570 2069 6620 796f 7520 646f 6e27 7420  ep if you don't 
+00001ef0: 7761 6e74 2074 6f20 7573 6520 7468 6520  want to use the 
+00001f00: 4573 6d65 7261 6c64 5465 7374 436c 6965  EsmeraldTestClie
+00001f10: 6e74 2e0a 0a59 6f75 2063 616e 2066 696e  nt...You can fin
+00001f20: 6420 5b6d 6f72 6520 696e 666f 726d 6174  d [more informat
+00001f30: 696f 6e5d 2868 7474 7073 3a2f 2f65 736d  ion](https://esm
+00001f40: 6572 616c 642e 6465 762f 6d61 6e61 6765  erald.dev/manage
+00001f50: 6d65 6e74 2f64 6972 6563 7469 7665 7329  ment/directives)
+00001f60: 2061 626f 7574 2074 6869 7320 6469 7265   about this dire
+00001f70: 6374 6976 6520 616e 6420 686f 7720 746f  ctive and how to
+00001f80: 0a75 7365 2069 742e 0a0a 2323 204b 6579  .use it...## Key
+00001f90: 2046 6561 7475 7265 730a 0a2a 202a 2a46   Features..* **F
+00001fa0: 6c75 6964 2061 6e64 2046 6173 742a 2a3a  luid and Fast**:
+00001fb0: 2054 6861 6e6b 7320 746f 2053 7461 726c   Thanks to Starl
+00001fc0: 6574 7465 2061 6e64 2050 7964 616e 7469  ette and Pydanti
+00001fd0: 632f 6d73 6773 7065 632e 0a2a 202a 2a46  c/msgspec..* **F
+00001fe0: 6173 7420 746f 2064 6576 656c 6f70 2a2a  ast to develop**
+00001ff0: 3a20 5468 616e 6b73 2074 6f20 7468 6520  : Thanks to the 
+00002000: 7369 6d70 6c69 6369 7479 206f 6620 6465  simplicity of de
+00002010: 7369 676e 2c20 7468 6520 6465 7665 6c6f  sign, the develo
+00002020: 706d 656e 7420 7469 6d65 7320 6361 6e20  pment times can 
+00002030: 6265 2072 6564 7563 6564 2065 7870 6f6e  be reduced expon
+00002040: 656e 7469 616c 6c79 2e0a 2a20 2a2a 496e  entially..* **In
+00002050: 7475 6974 6976 652a 2a3a 2049 6620 796f  tuitive**: If yo
+00002060: 7520 6172 6520 7573 6564 2074 6f20 7468  u are used to th
+00002070: 6520 6f74 6865 7220 6672 616d 6577 6f72  e other framewor
+00002080: 6b73 2c20 4573 6d65 7261 6c64 2069 7320  ks, Esmerald is 
+00002090: 6120 6e6f 2062 7261 696e 6572 2074 6f20  a no brainer to 
+000020a0: 6465 7665 6c6f 702e 0a2a 202a 2a45 6173  develop..* **Eas
+000020b0: 792a 2a3a 2044 6576 656c 6f70 6564 2077  y**: Developed w
+000020c0: 6974 6820 6465 7369 676e 2069 6e20 6d69  ith design in mi
+000020d0: 6e64 2061 6e64 2065 6173 7920 6c65 6172  nd and easy lear
+000020e0: 6e69 6e67 2e0a 2a20 2a2a 5368 6f72 742a  ning..* **Short*
+000020f0: 2a3a 2057 6974 6820 7468 6520 4f4f 5020  *: With the OOP 
+00002100: 6176 6169 6c61 626c 6520 6e61 7469 7665  available native
+00002110: 6c79 2074 6865 7265 2069 7320 6e6f 206e  ly there is no n
+00002120: 6565 6420 666f 7220 636f 6465 2064 7570  eed for code dup
+00002130: 6c69 6361 7469 6f6e 2e20 534f 4c49 442e  lication. SOLID.
+00002140: 0a2a 202a 2a52 6561 6479 2a2a 3a20 4765  .* **Ready**: Ge
+00002150: 7420 796f 7572 2061 7070 6c69 6361 7469  t your applicati
+00002160: 6f6e 2075 7020 616e 6420 7275 6e6e 696e  on up and runnin
+00002170: 6720 7769 7468 2070 726f 6475 6374 696f  g with productio
+00002180: 6e2d 7265 6164 7920 636f 6465 2e0a 2a20  n-ready code..* 
+00002190: 2a2a 4f4f 5020 616e 6420 4675 6e63 7469  **OOP and Functi
+000021a0: 6f6e 616c 2a2a 3a20 4465 7369 676e 2041  onal**: Design A
+000021b0: 5049 7320 696e 2061 6e79 2064 6573 6972  PIs in any desir
+000021c0: 6564 2077 6179 2e20 4f4f 5020 6f72 2046  ed way. OOP or F
+000021d0: 756e 6374 696f 6e61 6c20 6973 2061 7661  unctional is ava
+000021e0: 696c 6162 6c65 2e0a 2a20 2a2a 4173 796e  ilable..* **Asyn
+000021f0: 6320 616e 6420 5379 6e63 2a2a 3a20 446f  c and Sync**: Do
+00002200: 2079 6f75 2070 7265 6665 7220 7379 6e63   you prefer sync
+00002210: 206f 7220 6173 796e 633f 2059 6f75 2063   or async? You c
+00002220: 616e 2068 6176 6520 626f 7468 2e0a 2a20  an have both..* 
+00002230: 2a2a 4d69 6464 6c65 7761 7265 2a2a 3a20  **Middleware**: 
+00002240: 4170 706c 7920 6d69 6464 6c65 7761 7265  Apply middleware
+00002250: 7320 6f6e 2074 6865 2061 7070 6c69 6361  s on the applica
+00002260: 7469 6f6e 206c 6576 656c 206f 7220 4150  tion level or AP
+00002270: 4920 6c65 7665 6c2e 0a2a 202a 2a45 7863  I level..* **Exc
+00002280: 6570 7469 6f6e 2048 616e 646c 6572 732a  eption Handlers*
+00002290: 2a3a 2041 7070 6c79 2065 7863 6570 7469  *: Apply excepti
+000022a0: 6f6e 2068 616e 646c 6572 7320 6f6e 2061  on handlers on a
+000022b0: 6e79 2064 6573 6972 6564 206c 6576 656c  ny desired level
+000022c0: 2e0a 2a20 2a2a 5065 726d 6973 7369 6f6e  ..* **Permission
+000022d0: 732a 2a3a 2041 7070 6c79 2073 7065 6369  s**: Apply speci
+000022e0: 6669 6320 7275 6c65 7320 616e 6420 7065  fic rules and pe
+000022f0: 726d 6973 7369 6f6e 7320 6f6e 2065 6163  rmissions on eac
+00002300: 6820 4150 492e 0a2a 202a 2a49 6e74 6572  h API..* **Inter
+00002310: 6365 7074 6f72 732a 2a3a 2049 6e74 6572  ceptors**: Inter
+00002320: 6365 7074 2072 6571 7565 7374 7320 616e  cept requests an
+00002330: 6420 6164 6420 6c6f 6769 6320 6265 666f  d add logic befo
+00002340: 7265 2072 6561 6368 696e 6720 7468 6520  re reaching the 
+00002350: 656e 6470 6f69 6e74 2e0a 2a20 2a2a 506c  endpoint..* **Pl
+00002360: 7567 6761 626c 6573 2a2a 3a20 4372 6561  uggables**: Crea
+00002370: 7465 2070 6c75 6769 6e73 2066 6f72 2045  te plugins for E
+00002380: 736d 6572 616c 6420 616e 6420 686f 6f6b  smerald and hook
+00002390: 2074 6865 6d20 696e 746f 2061 6e79 2061   them into any a
+000023a0: 7070 6c69 6361 7469 6f6e 2061 6e64 2f6f  pplication and/o
+000023b0: 720a 6469 7374 7269 6275 7465 2074 6865  r.distribute the
+000023c0: 6d2e 0a2a 202a 2a44 414f 2061 6e64 2041  m..* **DAO and A
+000023d0: 7379 6e63 4441 4f2a 2a3a 2041 766f 6964  syncDAO**: Avoid
+000023e0: 2064 6174 6162 6173 6520 6361 6c6c 7320   database calls 
+000023f0: 6469 7265 6374 6c79 2066 726f 6d20 7468  directly from th
+00002400: 6520 4150 4973 2e20 5573 6520 6275 7369  e APIs. Use busi
+00002410: 6e65 7373 206f 626a 6563 7473 2069 6e73  ness objects ins
+00002420: 7465 6164 2e0a 2a20 2a2a 4f52 4d20 5375  tead..* **ORM Su
+00002430: 7070 6f72 742a 2a3a 204e 6174 6976 6520  pport**: Native 
+00002440: 7375 7070 6f72 7420 666f 7220 5b53 6166  support for [Saf
+00002450: 6669 6572 5d5b 7361 6666 6965 725f 6f72  fier][saffier_or
+00002460: 6d5d 2061 6e64 205b 4564 6779 5d5b 6564  m] and [Edgy][ed
+00002470: 6779 5f6f 726d 5d2e 0a2a 202a 2a4f 444d  gy_orm]..* **ODM
+00002480: 2053 7570 706f 7274 2a2a 3a20 4e61 7469   Support**: Nati
+00002490: 7665 2073 7570 706f 7274 2066 6f72 205b  ve support for [
+000024a0: 4d6f 6e67 6f7a 5d5b 6d6f 6e67 6f7a 5f6f  Mongoz][mongoz_o
+000024b0: 646d 5d2e 0a2a 202a 2a41 5049 5669 6577  dm]..* **APIView
+000024c0: 2a2a 3a20 436c 6173 7320 4261 7365 6420  **: Class Based 
+000024d0: 656e 6470 6f69 6e74 7320 666f 7220 796f  endpoints for yo
+000024e0: 7572 2062 656c 6f76 6564 204f 4f50 2064  ur beloved OOP d
+000024f0: 6573 6967 6e2e 0a2a 202a 2a4a 534f 4e20  esign..* **JSON 
+00002500: 7365 7269 616c 697a 6174 696f 6e2f 6465  serialization/de
+00002510: 7365 7269 616c 697a 6174 696f 6e2a 2a3a  serialization**:
+00002520: 2042 6f74 6820 554a 534f 4e20 616e 6420   Both UJSON and 
+00002530: 4f52 4a4f 4e20 7375 7070 6f72 742e 0a2a  ORJON support..*
+00002540: 202a 2a4c 6966 6573 7061 6e2a 2a3a 2053   **Lifespan**: S
+00002550: 7570 706f 7274 2066 6f72 2074 6865 206e  upport for the n
+00002560: 6577 6c79 206c 6966 6573 7061 6e20 616e  ewly lifespan an
+00002570: 6420 6f6e 5f73 7461 7274 2f6f 6e5f 7368  d on_start/on_sh
+00002580: 7574 646f 776e 2065 7665 6e74 732e 0a2a  utdown events..*
+00002590: 202a 2a53 6368 6564 756c 6572 2a2a 3a20   **Scheduler**: 
+000025a0: 5965 732c 2074 6861 7427 7320 7269 6768  Yes, that's righ
+000025b0: 742c 2069 7420 636f 6d65 7320 7769 7468  t, it comes with
+000025c0: 2061 2073 6368 6564 756c 6572 2066 6f72   a scheduler for
+000025d0: 2074 686f 7365 2061 7574 6f6d 6174 6564   those automated
+000025e0: 2074 6173 6b73 2e0a 2a20 2a2a 4465 7065   tasks..* **Depe
+000025f0: 6e64 656e 6379 2049 6e6a 6563 7469 6f6e  ndency Injection
+00002600: 2a2a 3a20 4c69 6b65 2061 6e79 206f 7468  **: Like any oth
+00002610: 6572 2067 7265 6174 2066 7261 6d65 776f  er great framewo
+00002620: 726b 206f 7574 2074 6865 7265 2e0a 2a20  rk out there..* 
+00002630: 2a2a 5369 6d70 6c69 6369 7479 2066 726f  **Simplicity fro
+00002640: 6d20 7365 7474 696e 6773 2a2a 3a20 5965  m settings**: Ye
+00002650: 732c 2077 6520 6861 7665 2061 2077 6179  s, we have a way
+00002660: 2074 6f20 6d61 6b65 2074 6865 2063 6f64   to make the cod
+00002670: 6520 6576 656e 2063 6c65 616e 6572 2062  e even cleaner b
+00002680: 7920 696e 7472 6f64 7563 696e 6720 7365  y introducing se
+00002690: 7474 696e 6773 0a62 6173 6564 2073 7973  ttings.based sys
+000026a0: 7465 6d73 2e0a 2a20 2a2a 6d73 6773 7065  tems..* **msgspe
+000026b0: 632a 2a20 2d20 5375 7070 6f72 7420 666f  c** - Support fo
+000026c0: 7220 606d 7367 7370 6563 602e 0a0a 2323  r `msgspec`...##
+000026d0: 2052 656c 6174 696f 6e20 746f 2053 7461   Relation to Sta
+000026e0: 726c 6574 7465 2061 6e64 206f 7468 6572  rlette and other
+000026f0: 2066 7261 6d65 776f 726b 730a 0a45 736d   frameworks..Esm
+00002700: 6572 616c 6420 7573 6573 2053 7461 726c  erald uses Starl
+00002710: 6574 7465 2075 6e64 6572 2074 6865 2068  ette under the h
+00002720: 6f6f 642e 2054 6865 2072 6561 736f 6e20  ood. The reason 
+00002730: 6265 6869 6e64 2074 6869 7320 6465 6369  behind this deci
+00002740: 736f 6e20 636f 6d65 7320 7769 7468 2074  son comes with t
+00002750: 6865 2066 6163 7420 7468 6174 2070 6572  he fact that per
+00002760: 666f 726d 616e 6365 2069 7320 7468 6572  formance is ther
+00002770: 650a 616e 6420 6e6f 2069 7373 7565 7320  e.and no issues 
+00002780: 7769 7468 2072 6f75 7469 6e67 2e0a 0a4f  with routing...O
+00002790: 6e63 6520 7468 6520 6170 706c 6963 6174  nce the applicat
+000027a0: 696f 6e20 6973 2075 702c 2061 6c6c 2074  ion is up, all t
+000027b0: 6865 2072 6f75 7465 7320 6172 6520 6d6f  he routes are mo
+000027c0: 756e 7465 6420 616e 6420 7468 6572 6566  unted and theref
+000027d0: 6f72 6520 7468 6520 7572 6c20 7061 7468  ore the url path
+000027e0: 7320 6172 6520 6465 6669 6e65 642e 0a45  s are defined..E
+000027f0: 736d 6572 616c 6420 656e 636f 7572 6167  smerald encourag
+00002800: 6573 2073 7461 6e64 6172 6420 7072 6163  es standard prac
+00002810: 7469 6365 7320 616e 6420 6465 7369 676e  tices and design
+00002820: 2069 6e20 6d69 6e64 2077 6869 6368 206d   in mind which m
+00002830: 6561 6e73 2074 6861 7420 616e 7920 6170  eans that any ap
+00002840: 706c 6963 6174 696f 6e2c 2062 6967 206f  plication, big o
+00002850: 7220 736d 616c 6c2c 0a63 7573 746f 6d20  r small,.custom 
+00002860: 6f72 2065 6e74 6572 7072 6973 652c 2066  or enterprise, f
+00002870: 6974 7320 7769 7468 696e 2045 736d 6572  its within Esmer
+00002880: 616c 6420 6563 6f73 7973 7465 6d20 7769  ald ecosystem wi
+00002890: 7468 6f75 7420 7363 616c 6162 696c 6974  thout scalabilit
+000028a0: 7920 6973 7375 6573 2e0a 0a23 2320 5365  y issues...## Se
+000028b0: 7474 696e 6773 0a0a 4c69 6b65 2065 7665  ttings..Like eve
+000028c0: 7279 206f 7468 6572 2066 7261 6d65 776f  ry other framewo
+000028d0: 726b 2c20 7768 656e 2073 7461 7274 696e  rk, when startin
+000028e0: 6720 616e 2061 7070 6c69 6361 7469 6f6e  g an application
+000028f0: 2c20 6120 6c6f 7420 6f66 205b 7365 7474  , a lot of [sett
+00002900: 696e 6773 5d28 2e2f 6170 706c 6963 6174  ings](./applicat
+00002910: 696f 6e2f 7365 7474 696e 6773 2e6d 6429  ion/settings.md)
+00002920: 2063 616e 2f6e 6565 6420 746f 2062 650a   can/need to be.
+00002930: 7061 7373 6564 2074 6f20 7468 6520 6d61  passed to the ma
+00002940: 696e 206f 626a 6563 7420 616e 6420 7468  in object and th
+00002950: 6973 2063 616e 2062 6520 7665 7279 2064  is can be very d
+00002960: 6175 7469 6e67 2061 6e64 2075 676c 7920  auting and ugly 
+00002970: 746f 206d 6169 6e74 6169 6e20 616e 6420  to maintain and 
+00002980: 7365 652e 0a0a 4573 6d65 7261 6c64 2063  see...Esmerald c
+00002990: 6f6d 6573 2077 6974 6820 7468 650a 5b73  omes with the.[s
+000029a0: 6574 7469 6e67 735d 282e 2f61 7070 6c69  ettings](./appli
+000029b0: 6361 7469 6f6e 2f73 6574 7469 6e67 732e  cation/settings.
+000029c0: 6d64 2920 696e 206d 696e 642e 2041 2073  md) in mind. A s
+000029d0: 6574 206f 6620 6465 6661 756c 7473 2074  et of defaults t
+000029e0: 6861 7420 6361 6e20 6265 206f 7665 7272  hat can be overr
+000029f0: 6964 6465 6e20 6279 2079 6f75 7220 7665  idden by your ve
+00002a00: 7279 206f 776e 2073 6574 7469 6e67 730a  ry own settings.
+00002a10: 6d6f 6475 6c65 2062 7574 206e 6f74 206c  module but not l
+00002a20: 696d 6974 6564 2074 6f20 6974 2c20 6173  imited to it, as
+00002a30: 2079 6f75 2063 616e 2073 7469 6c6c 2075   you can still u
+00002a40: 7365 2074 6865 2063 6c61 7373 6963 2061  se the classic a
+00002a50: 7070 726f 6163 6820 6f66 2070 6173 7369  pproach of passi
+00002a60: 6e67 2065 7665 7279 7468 696e 6720 696e  ng everything in
+00002a70: 746f 2061 0a45 736d 6572 616c 6420 696e  to a.Esmerald in
+00002a80: 7374 616e 6365 2064 6972 6563 746c 7920  stance directly 
+00002a90: 7768 656e 2069 6e73 7461 6e74 6961 7469  when instantiati
+00002aa0: 6e67 2e0a 0a2a 2a45 7861 6d70 6c65 206f  ng...**Example o
+00002ab0: 6620 636c 6173 7369 6320 6170 7072 6f61  f classic approa
+00002ac0: 6368 2a2a 3a0a 0a60 6060 7079 7468 6f6e  ch**:..```python
+00002ad0: 0a66 726f 6d20 6578 616d 706c 6520 696d  .from example im
+00002ae0: 706f 7274 2045 7861 6d70 6c65 4f62 6a65  port ExampleObje
+00002af0: 6374 0a0a 2320 4578 616d 706c 654f 626a  ct..# ExampleObj
+00002b00: 6563 7420 6973 2061 6e20 696e 7374 616e  ect is an instan
+00002b10: 6365 206f 6620 616e 6f74 6865 7220 6170  ce of another ap
+00002b20: 706c 6963 6174 696f 6e0a 2320 616e 6420  plication.# and 
+00002b30: 6974 2073 6572 7665 7320 6f6e 6c79 2066  it serves only f
+00002b40: 6f72 2065 7861 6d70 6c65 0a0a 6170 7020  or example..app 
+00002b50: 3d20 4578 616d 706c 654f 626a 6563 7428  = ExampleObject(
+00002b60: 7365 7474 696e 675f 6f6e 653d 2e2e 2e2c  setting_one=...,
+00002b70: 2073 6574 7469 6e67 5f74 776f 3d2e 2e2e   setting_two=...
+00002b80: 2c20 7365 7474 696e 675f 7468 7265 653d  , setting_three=
+00002b90: 2e2e 2e29 0a0a 6060 600a 0a49 6e73 7069  ...)..```..Inspi
+00002ba0: 7265 6420 6279 2074 6865 2067 7265 6174  red by the great
+00002bb0: 205b 446a 616e 676f 5d28 6874 7470 733a   [Django](https:
+00002bc0: 2f2f 7777 772e 646a 616e 676f 7072 6f6a  //www.djangoproj
+00002bd0: 6563 742e 636f 6d2f 2920 616e 6420 7573  ect.com/) and us
+00002be0: 696e 6720 7079 6461 6e74 6963 2c20 4573  ing pydantic, Es
+00002bf0: 6d65 7261 6c64 2068 6173 2061 2064 6566  merald has a def
+00002c00: 6175 6c74 206f 626a 6563 740a 7265 6164  ault object.read
+00002c10: 7920 746f 2062 6520 7573 6564 206f 7574  y to be used out
+00002c20: 2d6f 662d 7468 652d 626f 782e 0a0a 2a2a  -of-the-box...**
+00002c30: 4573 6d65 7261 6c64 2a2a 3a0a 0a60 6060  Esmerald**:..```
+00002c40: 7079 7468 6f6e 0a66 726f 6d20 6573 6d65  python.from esme
+00002c50: 7261 6c64 2069 6d70 6f72 7420 4573 6d65  rald import Esme
+00002c60: 7261 6c64 0a0a 6170 7020 3d20 4573 6d65  rald..app = Esme
+00002c70: 7261 6c64 2829 0a0a 6060 600a 0a41 6e64  rald()..```..And
+00002c80: 2074 6861 7427 7320 6974 2120 416c 6c20   that's it! All 
+00002c90: 7468 6520 6465 6661 756c 7420 7365 7474  the default sett
+00002ca0: 696e 6773 2061 7265 206c 6f61 6465 6421  ings are loaded!
+00002cb0: 2054 6869 7320 6973 2073 696d 706c 6520   This is simple 
+00002cc0: 6f66 2063 6f75 7273 6520 6275 7420 6361  of course but ca
+00002cd0: 6e20 796f 7520 6f76 6572 7269 6465 0a69  n you override.i
+00002ce0: 6e73 6964 6520 7468 6520 6f62 6a65 6374  nside the object
+00002cf0: 2061 7320 7765 6c6c 3f20 5965 7321 0a0a   as well? Yes!..
+00002d00: 6060 6070 7974 686f 6e0a 6672 6f6d 2065  ```python.from e
+00002d10: 736d 6572 616c 6420 696d 706f 7274 2045  smerald import E
+00002d20: 736d 6572 616c 640a 0a61 7070 203d 2045  smerald..app = E
+00002d30: 736d 6572 616c 6428 6170 705f 6e61 6d65  smerald(app_name
+00002d40: 3d27 4d79 2041 7070 272c 2074 6974 6c65  ='My App', title
+00002d50: 3d27 4d79 2074 6974 6c65 2729 0a0a 6060  ='My title')..``
+00002d60: 600a 0a53 616d 6520 6173 2074 6865 2063  `..Same as the c
+00002d70: 6c61 7373 6963 732e 0a0a 536f 2068 6f77  lassics...So how
+00002d80: 2064 6f65 7320 4573 6d65 7261 6c64 206b   does Esmerald k
+00002d90: 6e6f 7720 6162 6f75 7420 7468 6520 6465  now about the de
+00002da0: 6661 756c 7420 7365 7474 696e 6773 3f20  fault settings? 
+00002db0: 456e 7465 7273 205b 4573 6d65 7261 6c64  Enters [Esmerald
+00002dc0: 2073 6574 7469 6e67 7320 6d6f 6475 6c65   settings module
+00002dd0: 5d28 2365 736d 6572 616c 642d 7365 7474  ](#esmerald-sett
+00002de0: 696e 6773 2d6d 6f64 756c 6529 2e0a 0a23  ings-module)...#
+00002df0: 2323 2045 736d 6572 616c 6420 5365 7474  ## Esmerald Sett
+00002e00: 696e 6773 204d 6f64 756c 650a 0a54 6869  ings Module..Thi
+00002e10: 7320 6973 2074 6865 2077 6179 2045 736d  s is the way Esm
+00002e20: 6572 616c 6420 6465 6661 756c 7473 2074  erald defaults t
+00002e30: 6865 2076 616c 7565 732e 2057 6865 6e20  he values. When 
+00002e40: 7374 6172 7469 6e67 2061 6e20 6170 706c  starting an appl
+00002e50: 6963 6174 696f 6e2c 2074 6865 2073 7973  ication, the sys
+00002e60: 7465 6d20 6c6f 6f6b 7320 666f 7220 610a  tem looks for a.
+00002e70: 6045 534d 4552 414c 445f 5345 5454 494e  `ESMERALD_SETTIN
+00002e80: 4753 5f4d 4f44 554c 4560 2065 6e76 6972  GS_MODULE` envir
+00002e90: 6f6e 6d65 6e74 2076 6172 6961 626c 652e  onment variable.
+00002ea0: 2049 6620 6e6f 2076 6172 6961 626c 6520   If no variable 
+00002eb0: 6973 2073 7570 706c 6965 6420 7468 656e  is supplied then
+00002ec0: 2074 6865 2073 7973 7465 6d20 7769 6c6c   the system will
+00002ed0: 2064 6566 6175 6c74 2074 6f0a 6045 736d   default to.`Esm
+00002ee0: 6572 616c 6441 5049 5365 7474 696e 6773  eraldAPISettings
+00002ef0: 6020 7365 7474 696e 6773 2061 6e64 2073  ` settings and s
+00002f00: 7461 7274 2e0a 0a23 2323 2043 7573 746f  tart...### Custo
+00002f10: 6d20 5365 7474 696e 6773 0a0a 5365 7061  m Settings..Sepa
+00002f20: 7261 7469 6f6e 206f 6620 7365 7474 696e  ration of settin
+00002f30: 6773 2062 7920 656e 7669 726f 6d6d 656e  gs by envirommen
+00002f40: 7420 6973 2061 206d 7573 7420 6861 7665  t is a must have
+00002f50: 2074 6865 7365 2064 6179 7320 616e 6420   these days and 
+00002f60: 7374 6172 7469 6e67 2077 6974 6820 6465  starting with de
+00002f70: 6661 756c 7420 6f66 2045 736d 6572 616c  fault of Esmeral
+00002f80: 6420 7769 6c6c 206e 6f74 2062 650a 656e  d will not be.en
+00002f90: 6f75 6768 2066 6f72 2061 6e79 2061 7070  ough for any app
+00002fa0: 6c69 6361 7469 6f6e 2e0a 0a54 6865 2073  lication...The s
+00002fb0: 6574 7469 6e67 7320 6172 6520 7079 6461  ettings are pyda
+00002fc0: 6e74 6963 2073 7461 6e64 6172 6420 7365  ntic standard se
+00002fd0: 7474 696e 6773 2061 6e64 2074 6865 7265  ttings and there
+00002fe0: 666f 7265 2063 6f6d 7061 7469 626c 6520  fore compatible 
+00002ff0: 7769 7468 2045 736d 6572 616c 642e 0a54  with Esmerald..T
+00003000: 6865 2073 7973 7465 6d20 6272 696e 6773  he system brings
+00003010: 2073 6f6d 6520 6465 6661 756c 7473 2074   some defaults t
+00003020: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
+00003030: 6f75 742d 6f66 2d74 6865 2d62 6f78 2062  out-of-the-box b
+00003040: 7574 2069 7427 7320 6e6f 7420 6d61 6e64  ut it's not mand
+00003050: 6174 6f72 7920 746f 2062 6520 7573 6564  atory to be used
+00003060: 2e0a 5468 6520 656e 7669 726f 6e6d 656e  ..The environmen
+00003070: 7420 6465 6661 756c 7473 2074 6f20 2a2a  t defaults to **
+00003080: 7072 6f64 7563 7469 6f6e 2a2a 2e0a 0a60  production**...`
+00003090: 6060 7079 7468 6f6e 0a0a 6672 6f6d 2065  ``python..from e
+000030a0: 736d 6572 616c 6420 696d 706f 7274 2045  smerald import E
+000030b0: 736d 6572 616c 6441 5049 5365 7474 696e  smeraldAPISettin
+000030c0: 6773 0a66 726f 6d20 6573 6d65 7261 6c64  gs.from esmerald
+000030d0: 2e63 6f6e 662e 656e 756d 7320 696d 706f  .conf.enums impo
+000030e0: 7274 2045 6e76 6972 6f6e 6d65 6e74 5479  rt EnvironmentTy
+000030f0: 7065 0a0a 636c 6173 7320 4465 7665 6c6f  pe..class Develo
+00003100: 706d 656e 7428 4573 6d65 7261 6c64 4150  pment(EsmeraldAP
+00003110: 4953 6574 7469 6e67 7329 3a0a 2020 2020  ISettings):.    
+00003120: 6170 705f 6e61 6d65 3a20 7374 7220 3d20  app_name: str = 
+00003130: 274d 7920 6170 7020 696e 2064 6576 270a  'My app in dev'.
+00003140: 2020 2020 656e 7669 726f 6e6d 656e 743a      environment:
+00003150: 2073 7472 203d 2045 6e76 6972 6f6e 6d65   str = Environme
+00003160: 6e74 5479 7065 2e44 4556 454c 4f50 4d45  ntType.DEVELOPME
+00003170: 4e54 0a0a 6060 600a 0a2a 2a4c 6f61 6420  NT..```..**Load 
+00003180: 7468 6520 7365 7474 696e 6773 2069 6e74  the settings int
+00003190: 6f20 796f 7572 2045 736d 6572 616c 6420  o your Esmerald 
+000031a0: 6170 706c 6963 6174 696f 6e2a 2a3a 0a0a  application**:..
+000031b0: 4173 7375 6d69 6e67 2079 6f75 7220 4573  Assuming your Es
+000031c0: 6d65 7261 6c64 2061 7070 2069 7320 696e  merald app is in
+000031d0: 7369 6465 2061 6e20 6073 7263 2f61 7070  side an `src/app
+000031e0: 2e70 7960 2e0a 0a60 6060 636f 6e73 6f6c  .py`...```consol
+000031f0: 650a 0a45 534d 4552 414c 445f 5345 5454  e..ESMERALD_SETT
+00003200: 494e 4753 5f4d 4f44 554c 453d 276d 7961  INGS_MODULE='mya
+00003210: 7070 2e73 6574 7469 6e67 732e 4465 7665  pp.settings.Deve
+00003220: 6c6f 706d 656e 7427 2070 7974 686f 6e20  lopment' python 
+00003230: 2d6d 2073 7263 2e61 7070 2e70 790a 0a60  -m src.app.py..`
+00003240: 6060 0a0a 2323 2047 6174 6577 6179 2c20  ``..## Gateway, 
+00003250: 5765 6253 6f63 6b65 7447 6174 6577 6179  WebSocketGateway
+00003260: 2061 6e64 2049 6e63 6c75 6465 0a0a 5374   and Include..St
+00003270: 6172 6c65 7474 6520 6f66 6665 7273 2074  arlette offers t
+00003280: 6865 2052 6f75 7465 2063 6c61 7373 6573  he Route classes
+00003290: 2066 6f72 2073 696d 706c 6520 7061 7468   for simple path
+000032a0: 2061 7373 6967 6e6d 656e 7473 2062 7574   assignments but
+000032b0: 2074 6869 7320 6973 2061 6c73 6f20 7665   this is also ve
+000032c0: 7279 206c 696d 6974 696e 6720 6966 2073  ry limiting if s
+000032d0: 6f6d 6574 6869 6e67 206d 6f72 650a 636f  omething more.co
+000032e0: 6d70 6c65 7820 696e 206d 696e 642e 2045  mplex in mind. E
+000032f0: 736d 6572 616c 6420 6578 7465 6e64 7320  smerald extends 
+00003300: 7468 6174 2066 756e 6374 696f 6e61 6c69  that functionali
+00003310: 7479 2061 6e64 2061 6464 7320 736f 6d65  ty and adds some
+00003320: 2060 666c 6169 7260 2061 6e64 206c 6576   `flair` and lev
+00003330: 656c 7320 7570 2062 7920 6861 7669 6e67  els up by having
+00003340: 2074 6865 0a47 6174 6577 6179 2c20 5765   the.Gateway, We
+00003350: 6253 6f63 6b65 7447 6174 6577 6179 2061  bSocketGateway a
+00003360: 6e64 2049 6e63 6c75 6465 2e0a 0a54 686f  nd Include...Tho
+00003370: 7365 2061 7265 2073 7065 6369 616c 206f  se are special o
+00003380: 626a 6563 7473 2074 6861 7420 616c 6c6f  bjects that allo
+00003390: 7720 616c 6c20 7468 6520 6d61 6769 6320  w all the magic 
+000033a0: 6f66 2045 736d 6572 616c 6420 746f 2068  of Esmerald to h
+000033b0: 6170 7065 6e2e 0a0a 466f 7220 6120 636c  appen...For a cl
+000033c0: 6173 7369 632c 2064 6972 6563 742c 206f  assic, direct, o
+000033d0: 6e65 2066 696c 6520 7369 6e67 6c65 2061  ne file single a
+000033e0: 7070 726f 6163 682e 0a0a 2a2a 496e 2061  pproach...**In a
+000033f0: 206e 7574 7368 656c 6c2a 2a3a 0a0a 6060   nutshell**:..``
+00003400: 6070 7974 686f 6e20 7469 746c 653d 2773  `python title='s
+00003410: 7263 2f61 7070 2e70 7927 0a66 726f 6d20  rc/app.py'.from 
+00003420: 6573 6d65 7261 6c64 2069 6d70 6f72 7420  esmerald import 
+00003430: 4573 6d65 7261 6c64 2c20 6765 742c 2073  Esmerald, get, s
+00003440: 7461 7475 732c 2052 6571 7565 7374 2c20  tatus, Request, 
+00003450: 554a 534f 4e52 6573 706f 6e73 652c 2047  UJSONResponse, G
+00003460: 6174 6577 6179 2c20 5765 6253 6f63 6b65  ateway, WebSocke
+00003470: 7447 6174 6577 6179 2c20 5765 6273 6f63  tGateway, Websoc
+00003480: 6b65 740a 0a40 6765 7428 7374 6174 7573  ket..@get(status
+00003490: 5f63 6f64 653d 7374 6174 7573 2e48 5454  _code=status.HTT
+000034a0: 505f 3230 305f 4f4b 290a 6173 796e 6320  P_200_OK).async 
+000034b0: 6465 6620 686f 6d65 2829 202d 3e20 554a  def home() -> UJ
+000034c0: 534f 4e52 6573 706f 6e73 653a 0a20 2020  SONResponse:.   
+000034d0: 2072 6574 7572 6e20 554a 534f 4e52 6573   return UJSONRes
+000034e0: 706f 6e73 6528 7b0a 2020 2020 2020 2020  ponse({.        
+000034f0: 2264 6574 6169 6c22 3a20 2248 656c 6c6f  "detail": "Hello
+00003500: 2077 6f72 6c64 220a 2020 2020 7d29 0a0a   world".    })..
+00003510: 0a40 6765 7428 290a 6173 796e 6320 6465  .@get().async de
+00003520: 6620 616e 6f74 6865 7228 7265 7175 6573  f another(reques
+00003530: 743a 2052 6571 7565 7374 2920 2d3e 2064  t: Request) -> d
+00003540: 6963 743a 0a20 2020 2072 6574 7572 6e20  ict:.    return 
+00003550: 7b0a 2020 2020 2020 2020 2264 6574 6169  {.        "detai
+00003560: 6c22 3a20 2241 6e6f 7468 6572 2077 6f72  l": "Another wor
+00003570: 6c64 2122 0a20 2020 207d 0a0a 4077 6562  ld!".    }..@web
+00003580: 736f 636b 6574 2870 6174 683d 222f 7b70  socket(path="/{p
+00003590: 6174 685f 7061 7261 6d3a 7374 727d 2229  ath_param:str}")
+000035a0: 0a61 7379 6e63 2064 6566 2077 6f72 6c64  .async def world
+000035b0: 5f73 6f63 6b65 7428 736f 636b 6574 3a20  _socket(socket: 
+000035c0: 5765 6273 6f63 6b65 7429 202d 3e20 4e6f  Websocket) -> No
+000035d0: 6e65 3a0a 2020 2020 6177 6169 7420 736f  ne:.    await so
+000035e0: 636b 6574 2e61 6363 6570 7428 290a 2020  cket.accept().  
+000035f0: 2020 6d73 6720 3d20 6177 6169 7420 736f    msg = await so
+00003600: 636b 6574 2e72 6563 6569 7665 5f6a 736f  cket.receive_jso
+00003610: 6e28 290a 2020 2020 6173 7365 7274 206d  n().    assert m
+00003620: 7367 0a20 2020 2061 7373 6572 7420 736f  sg.    assert so
+00003630: 636b 6574 0a20 2020 2061 7761 6974 2073  cket.    await s
+00003640: 6f63 6b65 742e 636c 6f73 6528 290a 0a0a  ocket.close()...
+00003650: 6170 7020 3d20 4573 6d65 7261 6c64 2872  app = Esmerald(r
+00003660: 6f75 7465 733d 5b0a 2020 2020 4761 7465  outes=[.    Gate
+00003670: 7761 7928 6861 6e64 6c65 723d 686f 6d65  way(handler=home
+00003680: 292c 0a20 2020 2047 6174 6577 6179 2868  ),.    Gateway(h
+00003690: 616e 646c 6572 3d61 6e6f 7468 6572 292c  andler=another),
+000036a0: 0a20 2020 2057 6562 536f 636b 6574 4761  .    WebSocketGa
+000036b0: 7465 7761 7928 6861 6e64 6c65 723d 776f  teway(handler=wo
+000036c0: 726c 645f 736f 636b 6574 292c 0a5d 290a  rld_socket),.]).
+000036d0: 0a60 6060 0a0a 2323 2044 6573 6967 6e20  .```..## Design 
+000036e0: 696e 206d 696e 640a 0a47 6f6f 6420 6465  in mind..Good de
+000036f0: 7369 676e 2069 7320 616c 7761 7973 2065  sign is always e
+00003700: 6e63 6f75 7261 6765 6420 616e 6420 4573  ncouraged and Es
+00003710: 6d65 7261 6c64 2061 6c6c 6f77 7320 636f  merald allows co
+00003720: 6d70 6c65 7820 726f 7574 696e 6720 6f6e  mplex routing on
+00003730: 2061 6e79 206c 6576 656c 2e0a 0a23 2323   any level...###
+00003740: 2054 6865 2068 616e 646c 6572 7320 2876   The handlers (v
+00003750: 6965 7773 290a 0a60 6060 7079 7468 6f6e  iews)..```python
+00003760: 2074 6974 6c65 3d22 6d79 6170 702f 6163   title="myapp/ac
+00003770: 636f 756e 7473 2f76 6965 7773 2e70 7922  counts/views.py"
+00003780: 0a66 726f 6d20 6573 6d65 7261 6c64 2069  .from esmerald i
+00003790: 6d70 6f72 7420 6765 742c 2070 6f73 742c  mport get, post,
+000037a0: 2070 7574 2c20 7374 6174 7573 2c20 7765   put, status, we
+000037b0: 6273 6f63 6b65 742c 2041 5049 5669 6577  bsocket, APIView
+000037c0: 2c20 5265 7175 6573 742c 204a 534f 4e52  , Request, JSONR
+000037d0: 6573 706f 6e73 652c 2052 6573 706f 6e73  esponse, Respons
+000037e0: 652c 2057 6562 536f 636b 6574 0a66 726f  e, WebSocket.fro
+000037f0: 6d20 7079 6461 6e74 6963 2069 6d70 6f72  m pydantic impor
+00003800: 7420 4261 7365 4d6f 6465 6c0a 0a0a 636c  t BaseModel...cl
+00003810: 6173 7320 5072 6f64 7563 7428 4261 7365  ass Product(Base
+00003820: 4d6f 6465 6c29 3a0a 2020 2020 6e61 6d65  Model):.    name
+00003830: 3a20 7374 720a 2020 2020 736b 753a 2073  : str.    sku: s
+00003840: 7472 0a20 2020 2070 7269 6365 3a20 666c  tr.    price: fl
+00003850: 6f61 740a 0a0a 4070 7574 2827 2f70 726f  oat...@put('/pro
+00003860: 6475 6374 2f7b 7072 6f64 7563 745f 6964  duct/{product_id
+00003870: 7d27 290a 6465 6620 7570 6461 7465 5f70  }').def update_p
+00003880: 726f 6475 6374 2870 726f 6475 6374 5f69  roduct(product_i
+00003890: 643a 2069 6e74 2c20 6461 7461 3a20 5072  d: int, data: Pr
+000038a0: 6f64 7563 7429 202d 3e20 6469 6374 3a0a  oduct) -> dict:.
+000038b0: 2020 2020 7265 7475 726e 207b 2270 726f      return {"pro
+000038c0: 6475 6374 5f69 6422 3a20 7072 6f64 7563  duct_id": produc
+000038d0: 745f 6964 2c20 2270 726f 6475 6374 5f6e  t_id, "product_n
+000038e0: 616d 6522 3a20 7072 6f64 7563 742e 6e61  ame": product.na
+000038f0: 6d65 207d 0a0a 0a40 6765 7428 7374 6174  me }...@get(stat
+00003900: 7573 5f63 6f64 653d 7374 6174 7573 2e48  us_code=status.H
+00003910: 5454 505f 3230 305f 4f4b 290a 6173 796e  TTP_200_OK).asyn
+00003920: 6320 6465 6620 686f 6d65 2829 202d 3e20  c def home() -> 
+00003930: 4a53 4f4e 5265 7370 6f6e 7365 3a0a 2020  JSONResponse:.  
+00003940: 2020 7265 7475 726e 204a 534f 4e52 6573    return JSONRes
+00003950: 706f 6e73 6528 7b0a 2020 2020 2020 2020  ponse({.        
+00003960: 2264 6574 6169 6c22 3a20 2248 656c 6c6f  "detail": "Hello
+00003970: 2077 6f72 6c64 220a 2020 2020 7d29 0a0a   world".    })..
+00003980: 0a40 6765 7428 290a 6173 796e 6320 6465  .@get().async de
+00003990: 6620 616e 6f74 6865 7228 7265 7175 6573  f another(reques
+000039a0: 743a 2052 6571 7565 7374 2920 2d3e 2064  t: Request) -> d
+000039b0: 6963 743a 0a20 2020 2072 6574 7572 6e20  ict:.    return 
+000039c0: 7b0a 2020 2020 2020 2020 2264 6574 6169  {.        "detai
+000039d0: 6c22 3a20 2241 6e6f 7468 6572 2077 6f72  l": "Another wor
+000039e0: 6c64 2122 0a20 2020 207d 0a0a 0a40 7765  ld!".    }...@we
+000039f0: 6273 6f63 6b65 7428 7061 7468 3d22 2f7b  bsocket(path="/{
+00003a00: 7061 7468 5f70 6172 616d 3a73 7472 7d22  path_param:str}"
+00003a10: 290a 6173 796e 6320 6465 6620 776f 726c  ).async def worl
+00003a20: 645f 736f 636b 6574 2873 6f63 6b65 743a  d_socket(socket:
+00003a30: 2057 6562 736f 636b 6574 2920 2d3e 204e   Websocket) -> N
+00003a40: 6f6e 653a 0a20 2020 2061 7761 6974 2073  one:.    await s
+00003a50: 6f63 6b65 742e 6163 6365 7074 2829 0a20  ocket.accept(). 
+00003a60: 2020 206d 7367 203d 2061 7761 6974 2073     msg = await s
+00003a70: 6f63 6b65 742e 7265 6365 6976 655f 6a73  ocket.receive_js
+00003a80: 6f6e 2829 0a20 2020 2061 7373 6572 7420  on().    assert 
+00003a90: 6d73 670a 2020 2020 6173 7365 7274 2073  msg.    assert s
+00003aa0: 6f63 6b65 740a 2020 2020 6177 6169 7420  ocket.    await 
+00003ab0: 736f 636b 6574 2e63 6c6f 7365 2829 0a0a  socket.close()..
+00003ac0: 0a63 6c61 7373 2057 6f72 6c64 2841 5049  .class World(API
+00003ad0: 5669 6577 293a 0a0a 2020 2020 4067 6574  View):..    @get
+00003ae0: 2870 6174 683d 272f 7b75 726c 7d27 290a  (path='/{url}').
+00003af0: 2020 2020 6173 796e 6320 6465 6620 686f      async def ho
+00003b00: 6d65 2872 6571 7565 7374 3a20 5265 7175  me(request: Requ
+00003b10: 6573 742c 2075 726c 3a20 7374 7229 202d  est, url: str) -
+00003b20: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
+00003b30: 2020 2020 7265 7475 726e 2052 6573 706f      return Respo
+00003b40: 6e73 6528 6622 5552 4c3a 207b 7572 6c7d  nse(f"URL: {url}
+00003b50: 2229 0a0a 2020 2020 4070 6f73 7428 7061  ")..    @post(pa
+00003b60: 7468 3d27 2f7b 7572 6c7d 272c 2073 7461  th='/{url}', sta
+00003b70: 7475 735f 636f 6465 3d73 7461 7475 732e  tus_code=status.
+00003b80: 4854 5450 5f32 3031 5f43 5245 4154 4544  HTTP_201_CREATED
+00003b90: 290a 2020 2020 6173 796e 6320 6465 6620  ).    async def 
+00003ba0: 6d61 7273 2872 6571 7565 7374 3a20 5265  mars(request: Re
+00003bb0: 7175 6573 742c 2075 726c 3a20 7374 7229  quest, url: str)
+00003bc0: 202d 3e20 4a53 4f4e 5265 7370 6f6e 7365   -> JSONResponse
+00003bd0: 3a0a 2020 2020 2020 2020 2e2e 2e0a 0a20  :.        ..... 
+00003be0: 2020 2040 7765 6273 6f63 6b65 7428 7061     @websocket(pa
+00003bf0: 7468 3d22 2f7b 7061 7468 5f70 6172 616d  th="/{path_param
+00003c00: 3a73 7472 7d22 290a 2020 2020 6173 796e  :str}").    asyn
+00003c10: 6320 6465 6620 706c 7574 6f28 7365 6c66  c def pluto(self
+00003c20: 2c20 736f 636b 6574 3a20 5765 6273 6f63  , socket: Websoc
+00003c30: 6b65 7429 202d 3e20 4e6f 6e65 3a0a 2020  ket) -> None:.  
+00003c40: 2020 2020 2020 6177 6169 7420 736f 636b        await sock
+00003c50: 6574 2e61 6363 6570 7428 290a 2020 2020  et.accept().    
+00003c60: 2020 2020 6d73 6720 3d20 6177 6169 7420      msg = await 
+00003c70: 736f 636b 6574 2e72 6563 6569 7665 5f6a  socket.receive_j
+00003c80: 736f 6e28 290a 2020 2020 2020 2020 6173  son().        as
+00003c90: 7365 7274 206d 7367 0a20 2020 2020 2020  sert msg.       
+00003ca0: 2061 7373 6572 7420 736f 636b 6574 0a20   assert socket. 
+00003cb0: 2020 2020 2020 2061 7761 6974 2073 6f63         await soc
+00003cc0: 6b65 742e 636c 6f73 6528 290a 0a0a 6060  ket.close()...``
+00003cd0: 600a 0a49 6620 6120 6070 6174 6860 2069  `..If a `path` i
+00003ce0: 7320 6e6f 7420 7072 6f76 6964 6564 2c20  s not provided, 
+00003cf0: 6465 6661 756c 7473 2074 6f20 602f 602e  defaults to `/`.
+00003d00: 0a0a 2323 2320 5468 6520 6761 7465 7761  ..### The gatewa
+00003d10: 7973 2028 7572 6c73 290a 0a60 6060 7079  ys (urls)..```py
+00003d20: 7468 6f6e 2074 6974 6c65 3d22 6d79 6170  thon title="myap
+00003d30: 702f 6163 636f 756e 7473 2f75 726c 732e  p/accounts/urls.
+00003d40: 7079 220a 6672 6f6d 2065 736d 6572 616c  py".from esmeral
+00003d50: 6420 696d 706f 7274 2047 6174 6577 6179  d import Gateway
+00003d60: 2c20 5765 6253 6f63 6b65 7447 6174 6577  , WebSocketGatew
+00003d70: 6179 0a66 726f 6d20 2e76 6965 7773 2069  ay.from .views i
+00003d80: 6d70 6f72 7420 686f 6d65 2c20 616e 6f74  mport home, anot
+00003d90: 6865 722c 2077 6f72 6c64 5f73 6f63 6b65  her, world_socke
+00003da0: 742c 2057 6f72 6c64 0a0a 726f 7574 655f  t, World..route_
+00003db0: 7061 7474 6572 6e73 203d 205b 0a20 2020  patterns = [.   
+00003dc0: 2047 6174 6577 6179 2868 616e 646c 6572   Gateway(handler
+00003dd0: 3d75 7064 6174 655f 7072 6f64 7563 7429  =update_product)
+00003de0: 2c0a 2020 2020 4761 7465 7761 7928 6861  ,.    Gateway(ha
+00003df0: 6e64 6c65 723d 686f 6d65 292c 0a20 2020  ndler=home),.   
+00003e00: 2047 6174 6577 6179 2868 616e 646c 6572   Gateway(handler
+00003e10: 3d61 6e6f 7468 6572 292c 0a20 2020 2047  =another),.    G
+00003e20: 6174 6577 6179 2868 616e 646c 6572 3d57  ateway(handler=W
+00003e30: 6f72 6c64 292c 0a20 2020 2057 6562 536f  orld),.    WebSo
+00003e40: 636b 6574 4761 7465 7761 7928 6861 6e64  cketGateway(hand
+00003e50: 6c65 723d 776f 726c 645f 736f 636b 6574  ler=world_socket
+00003e60: 292c 0a5d 0a0a 6060 600a 0a49 6620 6120  ),.]..```..If a 
+00003e70: 6070 6174 6860 2069 7320 6e6f 7420 7072  `path` is not pr
+00003e80: 6f76 6964 6564 2c20 6465 6661 756c 7473  ovided, defaults
+00003e90: 2074 6f20 602f 602e 0a0a 2323 2320 5468   to `/`...### Th
+00003ea0: 6520 496e 636c 7564 650a 0a54 6869 7320  e Include..This 
+00003eb0: 6973 2061 2076 6572 7920 7370 6563 6961  is a very specia
+00003ec0: 6c20 6f62 6a65 6374 2074 6861 7420 616c  l object that al
+00003ed0: 6c6f 7773 2074 6865 2069 6d70 6f72 7420  lows the import 
+00003ee0: 6f66 2061 6e79 2072 6f75 7465 2066 726f  of any route fro
+00003ef0: 6d20 616e 7977 6865 7265 2069 6e20 7468  m anywhere in th
+00003f00: 6520 6170 706c 6963 6174 696f 6e2e 0a0a  e application...
+00003f10: 6049 6e63 6c75 6465 6020 6163 6365 7074  `Include` accept
+00003f20: 7320 7468 6520 696d 706f 7274 2076 6961  s the import via
+00003f30: 2060 6e61 6d65 7370 6163 6560 206f 7220   `namespace` or 
+00003f40: 7669 6120 6072 6f75 7465 7360 206c 6973  via `routes` lis
+00003f50: 7420 6275 7420 6e6f 7420 626f 7468 2e0a  t but not both..
+00003f60: 0a57 6865 6e20 7573 696e 6720 6120 606e  .When using a `n
+00003f70: 616d 6573 7061 6365 602c 2074 6865 2060  amespace`, the `
+00003f80: 496e 636c 7564 6560 2077 696c 6c20 6c6f  Include` will lo
+00003f90: 6f6b 2066 6f72 2074 6865 2064 6566 6175  ok for the defau
+00003fa0: 6c74 2060 726f 7574 655f 7061 7474 6572  lt `route_patter
+00003fb0: 6e73 6020 6f62 6a65 6374 206c 6973 7420  ns` object list 
+00003fc0: 696e 2074 6865 2069 6d70 6f72 7465 640a  in the imported.
+00003fd0: 6e61 6d65 7370 6163 6520 756e 6c65 7373  namespace unless
+00003fe0: 2061 2064 6966 6665 7265 6e74 2060 7061   a different `pa
+00003ff0: 7474 6572 6e60 2069 7320 7370 6563 6966  ttern` is specif
+00004000: 6965 642e 0a0a 5468 6520 7061 7474 6572  ied...The patter
+00004010: 6e20 6f6e 6c79 2077 6f72 6b73 2069 6620  n only works if 
+00004020: 7468 6520 696d 706f 7274 7320 6172 6520  the imports are 
+00004030: 646f 6e65 2076 6961 2060 6e61 6d65 7370  done via `namesp
+00004040: 6163 6560 2061 6e64 206e 6f74 2076 6961  ace` and not via
+00004050: 2060 726f 7574 6573 602e 0a0a 2a2a 496d   `routes`...**Im
+00004060: 706f 7274 696e 6720 7573 696e 6720 6e61  porting using na
+00004070: 6d65 7370 6163 652a 2a3a 0a0a 6060 6070  mespace**:..```p
+00004080: 7974 686f 6e20 7469 746c 653d 276d 7961  ython title='mya
+00004090: 7070 2f75 726c 732e 7079 270a 6672 6f6d  pp/urls.py'.from
+000040a0: 2065 736d 6572 616c 6420 696d 706f 7274   esmerald import
+000040b0: 2049 6e63 6c75 6465 0a0a 726f 7574 655f   Include..route_
+000040c0: 7061 7474 6572 6e73 203d 205b 0a20 2020  patterns = [.   
+000040d0: 2049 6e63 6c75 6465 286e 616d 6573 7061   Include(namespa
+000040e0: 6365 3d27 6d79 6170 702e 6163 636f 756e  ce='myapp.accoun
+000040f0: 7473 2e75 726c 7327 290a 5d0a 0a60 6060  ts.urls').]..```
+00004100: 0a0a 2a2a 496d 706f 7274 696e 6720 7573  ..**Importing us
+00004110: 696e 6720 726f 7574 6573 2a2a 3a0a 0a60  ing routes**:..`
+00004120: 6060 7079 7468 6f6e 2074 6974 6c65 3d27  ``python title='
+00004130: 7372 632f 6d79 6170 702f 7572 6c73 2e70  src/myapp/urls.p
+00004140: 7927 0a66 726f 6d20 6573 6d65 7261 6c64  y'.from esmerald
+00004150: 2069 6d70 6f72 7420 496e 636c 7564 650a   import Include.
+00004160: 6672 6f6d 206d 7961 7070 2e61 6363 6f75  from myapp.accou
+00004170: 6e74 7320 696d 706f 7274 2075 726c 730a  nts import urls.
+00004180: 0a72 6f75 7465 5f70 6174 7465 726e 7320  .route_patterns 
+00004190: 3d20 5b0a 2020 2020 496e 636c 7564 6528  = [.    Include(
+000041a0: 726f 7574 6573 3d75 726c 732e 726f 7574  routes=urls.rout
+000041b0: 655f 7061 7474 6572 6e73 290a 5d0a 0a60  e_patterns).]..`
+000041c0: 6060 0a0a 4966 2061 2060 7061 7468 6020  ``..If a `path` 
+000041d0: 6973 206e 6f74 2070 726f 7669 6465 642c  is not provided,
+000041e0: 2064 6566 6175 6c74 7320 746f 2060 2f60   defaults to `/`
+000041f0: 2e0a 0a23 2323 2320 5573 696e 6720 6120  ...#### Using a 
+00004200: 6469 6666 6572 656e 7420 7061 7474 6572  different patter
+00004210: 6e0a 0a60 6060 7079 7468 6f6e 2074 6974  n..```python tit
+00004220: 6c65 3d22 7372 632f 6d79 6170 702f 6163  le="src/myapp/ac
+00004230: 636f 756e 7473 2f75 726c 732e 7079 220a  counts/urls.py".
+00004240: 6672 6f6d 2065 736d 6572 616c 6420 696d  from esmerald im
+00004250: 706f 7274 2047 6174 6577 6179 2c20 5765  port Gateway, We
+00004260: 6253 6f63 6b65 7447 6174 6577 6179 0a66  bSocketGateway.f
+00004270: 726f 6d20 2e76 6965 7773 2069 6d70 6f72  rom .views impor
+00004280: 7420 686f 6d65 2c20 616e 6f74 6865 722c  t home, another,
+00004290: 2077 6f72 6c64 5f73 6f63 6b65 742c 2057   world_socket, W
+000042a0: 6f72 6c64 0a0a 6d79 5f75 726c 7320 3d20  orld..my_urls = 
+000042b0: 5b0a 2020 2020 4761 7465 7761 7928 6861  [.    Gateway(ha
+000042c0: 6e64 6c65 723d 7570 6461 7465 5f70 726f  ndler=update_pro
+000042d0: 6475 6374 292c 0a20 2020 2047 6174 6577  duct),.    Gatew
+000042e0: 6179 2868 616e 646c 6572 3d68 6f6d 6529  ay(handler=home)
+000042f0: 2c0a 2020 2020 4761 7465 7761 7928 6861  ,.    Gateway(ha
+00004300: 6e64 6c65 723d 616e 6f74 6865 7229 2c0a  ndler=another),.
+00004310: 2020 2020 4761 7465 7761 7928 6861 6e64      Gateway(hand
+00004320: 6c65 723d 576f 726c 6429 2c0a 2020 2020  ler=World),.    
+00004330: 5765 6253 6f63 6b65 7447 6174 6577 6179  WebSocketGateway
+00004340: 2868 616e 646c 6572 3d77 6f72 6c64 5f73  (handler=world_s
+00004350: 6f63 6b65 7429 2c0a 5d0a 0a60 6060 0a0a  ocket),.]..```..
+00004360: 2a2a 496d 706f 7274 696e 6720 7573 696e  **Importing usin
+00004370: 6720 6e61 6d65 7370 6163 652a 2a3a 0a0a  g namespace**:..
+00004380: 6060 6070 7974 686f 6e20 7469 746c 653d  ```python title=
+00004390: 2773 7263 2f6d 7961 7070 2f75 726c 732e  'src/myapp/urls.
+000043a0: 7079 270a 6672 6f6d 2065 736d 6572 616c  py'.from esmeral
+000043b0: 6420 696d 706f 7274 2049 6e63 6c75 6465  d import Include
+000043c0: 0a0a 726f 7574 655f 7061 7474 6572 6e73  ..route_patterns
+000043d0: 203d 205b 0a20 2020 2049 6e63 6c75 6465   = [.    Include
+000043e0: 286e 616d 6573 7061 6365 3d27 6d79 6170  (namespace='myap
+000043f0: 702e 6163 636f 756e 7473 2e75 726c 7327  p.accounts.urls'
+00004400: 2c20 7061 7474 6572 6e3d 276d 795f 7572  , pattern='my_ur
+00004410: 6c73 2729 0a5d 0a0a 6060 600a 0a23 2320  ls').]..```..## 
+00004420: 496e 636c 7564 6520 616e 6420 4573 6d65  Include and Esme
+00004430: 7261 6c64 0a0a 5468 6520 6049 6e63 6c75  rald..The `Inclu
+00004440: 6465 6020 6361 6e20 6265 2076 6572 7920  de` can be very 
+00004450: 6865 6c70 6675 6c20 6d6f 7374 6c79 2077  helpful mostly w
+00004460: 6865 6e20 7468 6520 676f 616c 2069 7320  hen the goal is 
+00004470: 746f 2061 766f 6964 2061 206c 6f74 206f  to avoid a lot o
+00004480: 6620 696d 706f 7274 7320 616e 6420 6d61  f imports and ma
+00004490: 7373 6976 6520 6c69 7374 0a6f 6620 6f62  ssive list.of ob
+000044a0: 6a65 6374 7320 746f 2062 6520 7061 7373  jects to be pass
+000044b0: 6564 2069 6e74 6f20 6f6e 6520 7369 6e67  ed into one sing
+000044c0: 6c65 206f 626a 6563 742e 2054 6869 7320  le object. This 
+000044d0: 6361 6e20 6265 2070 6172 7469 6375 6c61  can be particula
+000044e0: 7279 2075 7365 6675 6c20 746f 206d 616b  ry useful to mak
+000044f0: 6520 6120 4573 6d65 7261 6c64 2069 6e73  e a Esmerald ins
+00004500: 7461 6e63 652e 0a0a 2a2a 4578 616d 706c  tance...**Exampl
+00004510: 652a 2a3a 0a0a 6060 6070 7974 686f 6e20  e**:..```python 
+00004520: 7469 746c 653d 2773 7263 2f75 726c 732e  title='src/urls.
+00004530: 7079 270a 6672 6f6d 2065 736d 6572 616c  py'.from esmeral
+00004540: 6420 696d 706f 7274 2049 6e63 6c75 6465  d import Include
+00004550: 0a0a 726f 7574 655f 7061 7474 6572 6e73  ..route_patterns
+00004560: 203d 205b 0a20 2020 2049 6e63 6c75 6465   = [.    Include
+00004570: 286e 616d 6573 7061 6365 3d27 6d79 6170  (namespace='myap
+00004580: 702e 6163 636f 756e 7473 2e75 726c 7327  p.accounts.urls'
+00004590: 2c20 7061 7474 6572 6e3d 276d 795f 7572  , pattern='my_ur
+000045a0: 6c73 2729 0a5d 0a0a 6060 600a 0a60 6060  ls').]..```..```
+000045b0: 7079 7468 6f6e 2074 6974 6c65 3d27 7372  python title='sr
+000045c0: 632f 6170 702e 7079 270a 6672 6f6d 2065  c/app.py'.from e
+000045d0: 736d 6572 616c 6420 696d 706f 7274 2045  smerald import E
+000045e0: 736d 6572 616c 642c 2049 6e63 6c75 6465  smerald, Include
+000045f0: 0a0a 6170 7020 3d20 4573 6d65 7261 6c64  ..app = Esmerald
+00004600: 2872 6f75 7465 733d 5b49 6e63 6c75 6465  (routes=[Include
+00004610: 2827 7372 632e 7572 6c73 2729 5d29 0a0a  ('src.urls')])..
+00004620: 6060 600a 0a23 2320 5275 6e20 7468 6520  ```..## Run the 
+00004630: 6170 706c 6963 6174 696f 6e0a 0a41 7320  application..As 
+00004640: 6d65 6e74 696f 6e65 6420 6265 666f 7265  mentioned before
+00004650: 2c20 7765 2072 6563 6f6d 6d65 6e64 2075  , we recommend u
+00004660: 7669 636f 726e 2066 6f72 2070 726f 6475  vicorn for produ
+00004670: 6374 696f 6e20 6275 7420 6974 2773 206e  ction but it's n
+00004680: 6f74 206d 616e 6461 746f 7279 2e0a 0a2a  ot mandatory...*
+00004690: 2a55 7369 6e67 2075 7669 636f 726e 2a2a  *Using uvicorn**
+000046a0: 3a0a 0a60 6060 7368 656c 6c0a 7576 6963  :..```shell.uvic
+000046b0: 6f72 6e20 7372 633a 6170 7020 2d2d 7265  orn src:app --re
+000046c0: 6c6f 6164 0a0a 494e 464f 3a20 2020 2020  load..INFO:     
+000046d0: 5576 6963 6f72 6e20 7275 6e6e 696e 6720  Uvicorn running 
+000046e0: 6f6e 2068 7474 703a 2f2f 3132 372e 302e  on http://127.0.
+000046f0: 302e 313a 3830 3030 2028 5072 6573 7320  0.1:8000 (Press 
+00004700: 4354 524c 2b43 2074 6f20 7175 6974 290a  CTRL+C to quit).
+00004710: 494e 464f 3a20 2020 2020 5374 6172 7465  INFO:     Starte
+00004720: 6420 7265 6c6f 6164 6572 2070 726f 6365  d reloader proce
+00004730: 7373 205b 3238 3732 305d 0a49 4e46 4f3a  ss [28720].INFO:
+00004740: 2020 2020 2053 7461 7274 6564 2073 6572       Started ser
+00004750: 7665 7220 7072 6f63 6573 7320 5b32 3837  ver process [287
+00004760: 3232 5d0a 494e 464f 3a20 2020 2020 5761  22].INFO:     Wa
+00004770: 6974 696e 6720 666f 7220 6170 706c 6963  iting for applic
+00004780: 6174 696f 6e20 7374 6172 7475 702e 0a49  ation startup..I
+00004790: 4e46 4f3a 2020 2020 2041 7070 6c69 6361  NFO:     Applica
+000047a0: 7469 6f6e 2073 7461 7274 7570 2063 6f6d  tion startup com
+000047b0: 706c 6574 652e 0a60 6060 0a0a 2323 2052  plete..```..## R
+000047c0: 756e 2074 6865 2061 7070 6c69 6361 7469  un the applicati
+000047d0: 6f6e 2077 6974 6820 6375 7374 6f6d 2073  on with custom s
+000047e0: 6574 7469 6e67 730a 0a2a 2a55 7369 6e67  ettings..**Using
+000047f0: 2075 7669 636f 726e 2a2a 3a0a 0a60 6060   uvicorn**:..```
+00004800: 7368 656c 6c0a 4553 4d45 5241 4c44 5f53  shell.ESMERALD_S
+00004810: 4554 5449 4e47 535f 4d4f 4455 4c45 3d6d  ETTINGS_MODULE=m
+00004820: 7961 7070 2e41 7070 5365 7474 696e 6773  yapp.AppSettings
+00004830: 2075 7669 636f 726e 2073 7263 3a61 7070   uvicorn src:app
+00004840: 202d 2d72 656c 6f61 640a 0a49 4e46 4f3a   --reload..INFO:
+00004850: 2020 2020 2055 7669 636f 726e 2072 756e       Uvicorn run
+00004860: 6e69 6e67 206f 6e20 6874 7470 3a2f 2f31  ning on http://1
+00004870: 3237 2e30 2e30 2e31 3a38 3030 3020 2850  27.0.0.1:8000 (P
+00004880: 7265 7373 2043 5452 4c2b 4320 746f 2071  ress CTRL+C to q
+00004890: 7569 7429 0a49 4e46 4f3a 2020 2020 2053  uit).INFO:     S
+000048a0: 7461 7274 6564 2072 656c 6f61 6465 7220  tarted reloader 
+000048b0: 7072 6f63 6573 7320 5b32 3837 3230 5d0a  process [28720].
+000048c0: 494e 464f 3a20 2020 2020 5374 6172 7465  INFO:     Starte
+000048d0: 6420 7365 7276 6572 2070 726f 6365 7373  d server process
+000048e0: 205b 3238 3732 325d 0a49 4e46 4f3a 2020   [28722].INFO:  
+000048f0: 2020 2057 6169 7469 6e67 2066 6f72 2061     Waiting for a
+00004900: 7070 6c69 6361 7469 6f6e 2073 7461 7274  pplication start
+00004910: 7570 2e0a 494e 464f 3a20 2020 2020 4170  up..INFO:     Ap
+00004920: 706c 6963 6174 696f 6e20 7374 6172 7475  plication startu
+00004930: 7020 636f 6d70 6c65 7465 2e0a 6060 600a  p complete..```.
+00004940: 0a23 2320 4f70 656e 4150 4920 646f 6375  .## OpenAPI docu
+00004950: 6d65 6e74 6174 696f 6e0a 0a45 736d 6572  mentation..Esmer
+00004960: 616c 6420 616c 736f 2063 6f6d 6573 2077  ald also comes w
+00004970: 6974 6820 4f70 656e 4150 4920 646f 6373  ith OpenAPI docs
+00004980: 2069 6e74 6567 7261 7465 642e 2046 6f72   integrated. For
+00004990: 2074 686f 7365 2075 7365 6420 746f 2074   those used to t
+000049a0: 6861 742c 2074 6869 7320 6973 2072 6f75  hat, this is rou
+000049b0: 6768 6c79 2074 6865 2073 616d 6520 616e  ghly the same an
+000049c0: 6420 746f 206d 616b 6520 6974 0a68 6170  d to make it.hap
+000049d0: 7065 6e2c 2074 6865 7265 2077 6572 6520  pen, there were 
+000049e0: 696e 7370 6972 6174 696f 6e73 2074 6861  inspirations tha
+000049f0: 7420 6865 6c70 6564 2045 736d 6572 616c  t helped Esmeral
+00004a00: 6420 6765 7474 696e 6720 7468 6572 6520  d getting there 
+00004a10: 6661 7374 2e0a 0a45 736d 6572 616c 6420  fast...Esmerald 
+00004a20: 7374 6172 7473 2061 7574 6f6d 6174 6963  starts automatic
+00004a30: 616c 6c79 2074 6865 204f 7065 6e41 5049  ally the OpenAPI
+00004a40: 2064 6f63 756d 656e 7461 7469 6f6e 2062   documentation b
+00004a50: 7920 696e 6a65 6374 696e 6720 7468 6520  y injecting the 
+00004a60: 4f70 656e 4150 4943 6f6e 6669 6720 6465  OpenAPIConfig de
+00004a70: 6661 756c 7420 6672 6f6d 0a74 6865 2073  fault from.the s
+00004a80: 6574 7469 6e67 7320 616e 6420 6d61 6b65  ettings and make
+00004a90: 7320 5377 6167 6765 722c 2052 6544 6f63  s Swagger, ReDoc
+00004aa0: 2061 6e20 5374 6f70 6c69 6768 7420 656c   an Stoplight el
+00004ab0: 656d 656e 7473 2061 7661 696c 6162 6c65  ements available
+00004ac0: 2074 6f20 796f 7520 6f75 7420 6f66 2074   to you out of t
+00004ad0: 6865 2062 6f78 2e0a 0a54 6f20 6163 6365  he box...To acce
+00004ae0: 7373 2074 6865 204f 7065 6e41 5049 2c20  ss the OpenAPI, 
+00004af0: 7369 6d70 6c79 2073 7461 7274 2079 6f75  simply start you
+00004b00: 7220 6c6f 6361 6c20 6465 7665 6c6f 706d  r local developm
+00004b10: 656e 7420 616e 6420 6163 6365 7373 3a0a  ent and access:.
+00004b20: 0a2a 202a 2a53 7761 6767 6572 2a2a 202d  .* **Swagger** -
+00004b30: 2060 2f64 6f63 732f 7377 6167 6765 7260   `/docs/swagger`
+00004b40: 2e0a 2a20 2a2a 5265 646f 632a 2a20 2d20  ..* **Redoc** - 
+00004b50: 602f 646f 6373 2f72 6564 6f63 602e 0a2a  `/docs/redoc`..*
+00004b60: 202a 2a53 746f 706c 6967 6874 2045 6c65   **Stoplight Ele
+00004b70: 6d65 6e74 732a 2a20 2d20 602f 646f 6373  ments** - `/docs
+00004b80: 2f65 6c65 6d65 6e74 7360 2e0a 0a54 6865  /elements`...The
+00004b90: 7265 2061 7265 206d 6f72 6520 6465 7461  re are more deta
+00004ba0: 696c 7320 6162 6f75 7420 5b68 6f77 2074  ils about [how t
+00004bb0: 6f20 636f 6e66 6967 7572 6520 7468 6520  o configure the 
+00004bc0: 4f70 656e 4150 4943 6f6e 6669 675d 2868  OpenAPIConfig](h
+00004bd0: 7474 7073 3a2f 2f65 736d 6572 616c 642e  ttps://esmerald.
+00004be0: 6465 762f 636f 6e66 6967 7572 6174 696f  dev/configuratio
+00004bf0: 6e73 2f6f 7065 6e61 7069 2f63 6f6e 6669  ns/openapi/confi
+00004c00: 6729 0a77 6974 6869 6e20 7468 6520 646f  g).within the do
+00004c10: 6375 6d65 6e74 6174 696f 6e2e 0a0a 5468  cumentation...Th
+00004c20: 6572 6520 6973 2061 6c73 6f20 6120 676f  ere is also a go
+00004c30: 6f64 2065 7870 6c61 6e61 7469 6f6e 206f  od explanation o
+00004c40: 6e20 686f 7720 746f 2075 7365 2074 6865  n how to use the
+00004c50: 205b 4f70 656e 4150 4952 6573 706f 6e73   [OpenAPIRespons
+00004c60: 655d 2868 7474 7073 3a2f 2f65 736d 6572  e](https://esmer
+00004c70: 616c 642e 6465 762f 7265 7370 6f6e 7365  ald.dev/response
+00004c80: 7323 6f70 656e 6170 692d 7265 7370 6f6e  s#openapi-respon
+00004c90: 7365 7329 0a61 7320 7765 6c6c 2e0a 0a23  ses).as well...#
+00004ca0: 2320 4e6f 7465 730a 0a54 6869 7320 6973  # Notes..This is
+00004cb0: 206a 7573 7420 6120 7665 7279 2068 6967   just a very hig
+00004cc0: 682d 6c65 7665 6c20 6465 6d6f 6e73 7472  h-level demonstr
+00004cd0: 6174 696f 6e20 6f66 2068 6f77 2074 6f20  ation of how to 
+00004ce0: 7374 6172 7420 7175 6963 6b6c 7920 616e  start quickly an
+00004cf0: 6420 7768 6174 2045 736d 6572 616c 6420  d what Esmerald 
+00004d00: 6361 6e20 646f 2e0a 5468 6572 6520 6172  can do..There ar
+00004d10: 6520 706c 656e 7479 206d 6f72 6520 7468  e plenty more th
+00004d20: 696e 6773 2079 6f75 2063 616e 2064 6f20  ings you can do 
+00004d30: 7769 7468 2045 736d 6572 616c 642e 2045  with Esmerald. E
+00004d40: 6e6a 6f79 2120 f09f 988a 0a0a 2323 2053  njoy! ......## S
+00004d50: 706f 6e73 6f72 730a 0a43 7572 7265 6e74  ponsors..Current
+00004d60: 6c79 2074 6865 7265 2061 7265 206e 6f20  ly there are no 
+00004d70: 7370 6f6e 736f 7273 206f 6620 4573 6d65  sponsors of Esme
+00004d80: 7261 6c64 2062 7574 2079 6f75 2063 616e  rald but you can
+00004d90: 2066 696e 616e 6369 616c 6c79 2068 656c   financially hel
+00004da0: 7020 616e 6420 7375 7070 6f72 7420 7468  p and support th
+00004db0: 6520 6175 7468 6f72 2074 686f 7567 680a  e author though.
+00004dc0: 5b47 6974 4875 6220 7370 6f6e 736f 7273  [GitHub sponsors
+00004dd0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004de0: 2e63 6f6d 2f73 706f 6e73 6f72 732f 7461  .com/sponsors/ta
+00004df0: 7273 696c 2920 616e 6420 6265 636f 6d65  rsil) and become
+00004e00: 2061 202a 2a53 7065 6369 616c 206f 6e65   a **Special one
+00004e10: 2a2a 206f 7220 6120 2a2a 4c65 6765 6e64  ** or a **Legend
+00004e20: 2a2a 2e0a 0a5b 7361 6666 6965 725f 6f72  **...[saffier_or
+00004e30: 6d5d 3a20 6874 7470 733a 2f2f 6573 6d65  m]: https://esme
+00004e40: 7261 6c64 2e64 6576 2f64 6174 6162 6173  rald.dev/databas
+00004e50: 6573 2f73 6166 6669 6572 2f6d 6f74 6976  es/saffier/motiv
+00004e60: 6174 696f 6e0a 5b65 6467 795f 6f72 6d5d  ation.[edgy_orm]
+00004e70: 3a20 6874 7470 733a 2f2f 6573 6d65 7261  : https://esmera
+00004e80: 6c64 2e64 6576 2f64 6174 6162 6173 6573  ld.dev/databases
+00004e90: 2f73 6166 6669 6572 2f6d 6f74 6976 6174  /saffier/motivat
+00004ea0: 696f 6e0a 5b6d 6f6e 676f 7a5f 6f64 6d5d  ion.[mongoz_odm]
+00004eb0: 3a20 6874 7470 733a 2f2f 6573 6d65 7261  : https://esmera
+00004ec0: 6c64 2e64 6576 2f64 6174 6162 6173 6573  ld.dev/databases
+00004ed0: 2f6d 6f6e 676f 7a2f 6d6f 7469 7661 7469  /mongoz/motivati
+00004ee0: 6f6e 0a                                  on.
```

