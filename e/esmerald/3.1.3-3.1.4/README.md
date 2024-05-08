# Comparing `tmp/esmerald-3.1.3.tar.gz` & `tmp/esmerald-3.1.4.tar.gz`

## Comparing `esmerald-3.1.3.tar` & `esmerald-3.1.4.tar`

### file list

```diff
@@ -1,230 +1,230 @@
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/__main__.py
--rw-r--r--   0        0        0    91447 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/applications.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/concurrency.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/context.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/enums.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/exceptions.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/injector.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/logging.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/param_functions.py
--rw-r--r--   0        0        0    22336 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/params.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/py.typed
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/requests.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/staticfiles.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/testclient.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/types.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/typing.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/websockets.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/enums.py
--rw-r--r--   0        0        0    47620 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/v1/controllers.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/conf/directives/project_template/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/cors.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/csrf.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/jwt.py
--rw-r--r--   0        0        0    14614 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/openapi.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/session.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/static_files.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/edgy/__init__.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/edgy/base_user.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/edgy/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/mongoz/__init__.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/mongoz/base_user.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/mongoz/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/di/__init__.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/di/provider.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     8906 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/createdeployment.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/enums.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/ipython.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/ptpython.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/directives/operations/shell/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/urls/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/core/urls/base.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/json.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/msgspec.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/app_settings.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/cors.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/https.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/_internal.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/constants.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/docs.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/models.py
--rw-r--r--   0        0        0    20526 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/openapi.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/params.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/utils.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/base.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/api_key/__init__.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/api_key/base.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/http/__init__.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/http/base.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/oauth2/__init__.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/oauth2/base.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/openid_connect/__init__.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/openapi/security/openid_connect/base.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/permissions/base.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/protocols/template.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/responses/base.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/responses/json.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/__init__.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/_internal.py
--rw-r--r--   0        0        0    23730 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/base.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/events.py
--rw-r--r--   0        0        0    23680 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/gateways.py
--rw-r--r--   0        0        0   108795 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    72909 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/router.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/views.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/__init__.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/_metaclasses.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/_mixins.py
--rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/base.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/generics.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/apis/views.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/webhooks/__init__.py
--rw-r--r--   0        0        0   106388 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/routing/webhooks/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/model.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/signature.py
--rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/transformers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/constants.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/helpers.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/inspect.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/models.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/pydantic/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esmerald-3.1.3/esmerald/utils/pydantic/schema.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 esmerald-3.1.3/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-3.1.3/LICENSE
--rw-r--r--   0        0        0    17034 2020-02-02 00:00:00.000000 esmerald-3.1.3/README.md
--rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 esmerald-3.1.3/pyproject.toml
--rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 esmerald-3.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/__main__.py
+-rw-r--r--   0        0        0    91447 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/applications.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/concurrency.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/context.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/enums.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/exceptions.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/injector.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/logging.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/param_functions.py
+-rw-r--r--   0        0        0    22336 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/params.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/py.typed
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/requests.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/testclient.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/types.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/typing.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/websockets.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    47620 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/app_template/v1/controllers.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/conf/directives/project_template/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/config/cors.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/config/csrf.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/config/jwt.py
+-rw-r--r--   0        0        0    14614 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/config/openapi.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/config/session.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/config/static_files.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/edgy/__init__.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/edgy/base_user.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/edgy/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/mongoz/__init__.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/mongoz/base_user.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/mongoz/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/di/__init__.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/di/provider.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     8906 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/createdeployment.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/shell/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/shell/enums.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/directives/operations/shell/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/urls/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/core/urls/base.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/datastructures/msgspec.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/app_settings.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/_internal.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/constants.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/docs.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/models.py
+-rw-r--r--   0        0        0    20721 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/openapi.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/params.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/security/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/security/base.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/security/api_key/__init__.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/security/api_key/base.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/security/http/__init__.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/security/http/base.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/security/oauth2/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/security/oauth2/base.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/security/openid_connect/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/openapi/security/openid_connect/base.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/protocols/template.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/responses/base.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/_internal.py
+-rw-r--r--   0        0        0    23730 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/events.py
+-rw-r--r--   0        0        0    23680 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0   108795 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    72909 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/router.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/views.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/apis/__init__.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/apis/_metaclasses.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/apis/_mixins.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/apis/base.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/apis/generics.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/apis/views.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/webhooks/__init__.py
+-rw-r--r--   0        0        0   106388 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/routing/webhooks/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/constants.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/inspect.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/models.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esmerald-3.1.4/esmerald/utils/pydantic/schema.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 esmerald-3.1.4/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-3.1.4/LICENSE
+-rw-r--r--   0        0        0    17034 2020-02-02 00:00:00.000000 esmerald-3.1.4/README.md
+-rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 esmerald-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 esmerald-3.1.4/PKG-INFO
```

### Comparing `esmerald-3.1.3/esmerald/__init__.py` & `esmerald-3.1.4/esmerald/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.1.3"
+__version__ = "3.1.4"
 
 
 from lilya import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.context import Context
```

### Comparing `esmerald-3.1.3/esmerald/applications.py` & `esmerald-3.1.4/esmerald/applications.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/backgound.py` & `esmerald-3.1.4/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/context.py` & `esmerald-3.1.4/esmerald/context.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/enums.py` & `esmerald-3.1.4/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/exception_handlers.py` & `esmerald-3.1.4/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/exceptions.py` & `esmerald-3.1.4/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/injector.py` & `esmerald-3.1.4/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/logging.py` & `esmerald-3.1.4/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/params.py` & `esmerald-3.1.4/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/parsers.py` & `esmerald-3.1.4/esmerald/parsers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/requests.py` & `esmerald-3.1.4/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/testclient.py` & `esmerald-3.1.4/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/types.py` & `esmerald-3.1.4/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/websockets.py` & `esmerald-3.1.4/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/__init__.py` & `esmerald-3.1.4/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/global_settings.py` & `esmerald-3.1.4/esmerald/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/app_template/v1/controllers.py-tpl` & `esmerald-3.1.4/esmerald/conf/directives/app_template/v1/controllers.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl` & `esmerald-3.1.4/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl` & `esmerald-3.1.4/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl` & `esmerald-3.1.4/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl` & `esmerald-3.1.4/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl` & `esmerald-3.1.4/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/project_template/.gitignore.e-tpl` & `esmerald-3.1.4/esmerald/conf/directives/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/project_template/Makefile.e-tpl` & `esmerald-3.1.4/esmerald/conf/directives/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/main.py-tpl` & `esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/serve.py-tpl` & `esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/urls.py-tpl` & `esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl` & `esmerald-3.1.4/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/config/cors.py` & `esmerald-3.1.4/esmerald/config/cors.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/config/csrf.py` & `esmerald-3.1.4/esmerald/config/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/config/jwt.py` & `esmerald-3.1.4/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/config/openapi.py` & `esmerald-3.1.4/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/config/session.py` & `esmerald-3.1.4/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/config/static_files.py` & `esmerald-3.1.4/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/config/template.py` & `esmerald-3.1.4/esmerald/config/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/contrib/encoding.py` & `esmerald-3.1.4/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/contrib/auth/hashers.py` & `esmerald-3.1.4/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/contrib/auth/common/middleware.py` & `esmerald-3.1.4/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/contrib/auth/edgy/base_user.py` & `esmerald-3.1.4/esmerald/contrib/auth/edgy/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/contrib/auth/edgy/middleware.py` & `esmerald-3.1.4/esmerald/contrib/auth/edgy/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/contrib/auth/mongoz/base_user.py` & `esmerald-3.1.4/esmerald/contrib/auth/mongoz/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/contrib/auth/mongoz/middleware.py` & `esmerald-3.1.4/esmerald/contrib/auth/mongoz/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-3.1.4/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-3.1.4/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/di/provider.py` & `esmerald-3.1.4/esmerald/core/di/provider.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/cli.py` & `esmerald-3.1.4/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/env.py` & `esmerald-3.1.4/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/templates.py` & `esmerald-3.1.4/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/utils.py` & `esmerald-3.1.4/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/createapp.py` & `esmerald-3.1.4/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/createdeployment.py` & `esmerald-3.1.4/esmerald/core/directives/operations/createdeployment.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/createproject.py` & `esmerald-3.1.4/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/list.py` & `esmerald-3.1.4/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/run.py` & `esmerald-3.1.4/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/runserver.py` & `esmerald-3.1.4/esmerald/core/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/show_urls.py` & `esmerald-3.1.4/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/shell/base.py` & `esmerald-3.1.4/esmerald/core/directives/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/shell/ipython.py` & `esmerald-3.1.4/esmerald/core/directives/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/shell/ptpython.py` & `esmerald-3.1.4/esmerald/core/directives/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/directives/operations/shell/utils.py` & `esmerald-3.1.4/esmerald/core/directives/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/terminal/base.py` & `esmerald-3.1.4/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/terminal/print.py` & `esmerald-3.1.4/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/terminal/terminal.py` & `esmerald-3.1.4/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/core/urls/base.py` & `esmerald-3.1.4/esmerald/core/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/datastructures/__init__.py` & `esmerald-3.1.4/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/datastructures/base.py` & `esmerald-3.1.4/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/datastructures/encoders.py` & `esmerald-3.1.4/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/datastructures/file.py` & `esmerald-3.1.4/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/datastructures/json.py` & `esmerald-3.1.4/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/datastructures/msgspec.py` & `esmerald-3.1.4/esmerald/datastructures/msgspec.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/datastructures/redirect.py` & `esmerald-3.1.4/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/datastructures/stream.py` & `esmerald-3.1.4/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/datastructures/template.py` & `esmerald-3.1.4/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/interceptors/interceptor.py` & `esmerald-3.1.4/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/middleware/__init__.py` & `esmerald-3.1.4/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/middleware/_exception_handlers.py` & `esmerald-3.1.4/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/middleware/app_settings.py` & `esmerald-3.1.4/esmerald/middleware/app_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/middleware/asyncexitstack.py` & `esmerald-3.1.4/esmerald/middleware/asyncexitstack.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,9 @@
         exception: Optional[Exception] = None
         async with AsyncExitStack() as stack:
             scope[self.config.context_name] = stack
             try:
                 await self.app(scope, receive, send)
             except Exception as e:
                 exception = e
-                raise e
         if exception:
             raise exception
```

### Comparing `esmerald-3.1.3/esmerald/middleware/authentication.py` & `esmerald-3.1.4/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/middleware/exceptions.py` & `esmerald-3.1.4/esmerald/middleware/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from inspect import getmro
-from typing import Any, Callable, Dict, List, Mapping, Optional, Type, Union, cast
+from typing import Any, Callable, Dict, List, Mapping, Optional, Type, Union
 
 from lilya import status
+
 from lilya.exceptions import HTTPException as LilyaException
 from lilya.middleware.exceptions import ExceptionMiddleware as LilyaExceptionMiddleware
 from lilya.responses import Response as LilyaResponse
 from lilya.types import ASGIApp, Receive, Scope, Send
 from pydantic import BaseModel
 
 from esmerald.enums import MediaType, ScopeType
@@ -138,20 +138,18 @@
         )
 
     def get_exception_handler(
         self,
         exception_handlers: ExceptionHandlerMap,
         exc: Exception,
     ) -> Union[ExceptionHandler, None]:
+        status_code = (
+            exc.status_code
+            if isinstance(exc, LilyaException)
+            else status.HTTP_500_INTERNAL_SERVER_ERROR
+        )
         if not exception_handlers:
             return None
 
-        if not isinstance(exc, HTTPException) and exc.__class__ in exception_handlers:
-            return exception_handlers[exc.__class__]
-
-        if isinstance(exc, HTTPException) and exc.__class__ in exception_handlers:
-            return exception_handlers[exc.__class__]
-
-        for klass in getmro(type(exc)):
-            if klass in exception_handlers:
-                return exception_handlers[cast("Type[Exception]", exc)]
-        return None
+        return self.exception_handlers.get(status_code) or self.exception_handlers.get(
+            exc.__class__
+        )
```

### Comparing `esmerald-3.1.3/esmerald/middleware/settings_middleware.py` & `esmerald-3.1.4/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/_internal.py` & `esmerald-3.1.4/esmerald/openapi/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/datastructures.py` & `esmerald-3.1.4/esmerald/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/docs.py` & `esmerald-3.1.4/esmerald/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/models.py` & `esmerald-3.1.4/esmerald/openapi/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/openapi.py` & `esmerald-3.1.4/esmerald/openapi/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import warnings
 from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Union, cast
 
 from lilya._internal._path import clean_path
 from lilya.middleware import DefineMiddleware
 from lilya.routing import BasePath
 from lilya.status import HTTP_422_UNPROCESSABLE_ENTITY
+from lilya.transformers import TRANSFORMER_TYPES
 from orjson import loads
 from pydantic import AnyUrl
 from pydantic.fields import FieldInfo
 from pydantic.json_schema import GenerateJsonSchema, JsonSchemaValue
 from typing_extensions import Literal
 
 from esmerald.enums import MediaType
@@ -42,17 +43,21 @@
 from esmerald.utils.helpers import is_class_and_subclass
 
 
 def get_flat_params(route: Union[router.HTTPHandler, Any]) -> List[Any]:
     """Gets all the neded params of the request and route"""
     path_params = [param.field_info for param in route.transformer.get_path_params()]
     cookie_params = [param.field_info for param in route.transformer.get_cookie_params()]
-    query_params = [param.field_info for param in route.transformer.get_query_params()]
     header_params = [param.field_info for param in route.transformer.get_header_params()]
 
+    query_params = []
+    for param in route.transformer.get_query_params():
+        if param.field_info.annotation.__class__.__name__ in TRANSFORMER_TYPES.keys():
+            query_params.append(param.field_info)
+
     return path_params + query_params + cookie_params + header_params
 
 
 def get_openapi_security_schemes(schemes: Any) -> Tuple[dict, list]:
     """
     Builds the security schemas for OpenAPI.
     """
@@ -177,15 +182,15 @@
         if field_info.description:
             parameter.description = field_info.description
         if field_info.examples is not None:
             parameter.example = json.dumps(field_info.examples)
         if field_info.deprecated:
             parameter.deprecated = field_info.deprecated  # type: ignore
 
-        parameters.append(parameter.model_dump(by_alias=True))
+        parameters.append(parameter.model_dump(by_alias=True, exclude_none=True))
     return parameters
 
 
 def get_openapi_operation_request_body(
     *,
     data_field: Optional[FieldInfo],
     field_mapping: Dict[Tuple[FieldInfo, Literal["validation", "serialization"]], JsonSchemaValue],
```

### Comparing `esmerald-3.1.3/esmerald/openapi/responses.py` & `esmerald-3.1.4/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/utils.py` & `esmerald-3.1.4/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/validation.py` & `esmerald-3.1.4/esmerald/openapi/validation.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/security/base.py` & `esmerald-3.1.4/esmerald/openapi/security/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/security/api_key/base.py` & `esmerald-3.1.4/esmerald/openapi/security/api_key/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/security/http/base.py` & `esmerald-3.1.4/esmerald/openapi/security/http/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/security/oauth2/base.py` & `esmerald-3.1.4/esmerald/openapi/security/oauth2/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/openapi/security/openid_connect/base.py` & `esmerald-3.1.4/esmerald/openapi/security/openid_connect/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/permissions/base.py` & `esmerald-3.1.4/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/permissions/utils.py` & `esmerald-3.1.4/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/pluggables/base.py` & `esmerald-3.1.4/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/protocols/asyncdao.py` & `esmerald-3.1.4/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/protocols/dao.py` & `esmerald-3.1.4/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/protocols/interceptor.py` & `esmerald-3.1.4/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/protocols/template.py` & `esmerald-3.1.4/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/responses/base.py` & `esmerald-3.1.4/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/responses/encoders.py` & `esmerald-3.1.4/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/responses/json.py` & `esmerald-3.1.4/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/responses/template.py` & `esmerald-3.1.4/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/_internal.py` & `esmerald-3.1.4/esmerald/routing/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/base.py` & `esmerald-3.1.4/esmerald/routing/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/events.py` & `esmerald-3.1.4/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/gateways.py` & `esmerald-3.1.4/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/handlers.py` & `esmerald-3.1.4/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/router.py` & `esmerald-3.1.4/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/apis/_metaclasses.py` & `esmerald-3.1.4/esmerald/routing/apis/_metaclasses.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/apis/_mixins.py` & `esmerald-3.1.4/esmerald/routing/apis/_mixins.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/apis/base.py` & `esmerald-3.1.4/esmerald/routing/apis/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/apis/generics.py` & `esmerald-3.1.4/esmerald/routing/apis/generics.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/apis/views.py` & `esmerald-3.1.4/esmerald/routing/apis/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/routing/webhooks/handlers.py` & `esmerald-3.1.4/esmerald/routing/webhooks/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/security/jwt/token.py` & `esmerald-3.1.4/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/template/jinja.py` & `esmerald-3.1.4/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/template/mako.py` & `esmerald-3.1.4/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/transformers/datastructures.py` & `esmerald-3.1.4/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/transformers/model.py` & `esmerald-3.1.4/esmerald/transformers/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/transformers/signature.py` & `esmerald-3.1.4/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/transformers/utils.py` & `esmerald-3.1.4/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/utils/constants.py` & `esmerald-3.1.4/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/utils/dependency.py` & `esmerald-3.1.4/esmerald/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/utils/functional.py` & `esmerald-3.1.4/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/utils/helpers.py` & `esmerald-3.1.4/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/utils/models.py` & `esmerald-3.1.4/esmerald/utils/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/utils/sync.py` & `esmerald-3.1.4/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/esmerald/utils/pydantic/schema.py` & `esmerald-3.1.4/esmerald/utils/pydantic/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/LICENSE` & `esmerald-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/README.md` & `esmerald-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.3/pyproject.toml` & `esmerald-3.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -89,37 +89,41 @@
 Documentation = "https://esmerald.dymmond.com/"
 Changelog = "https://esmerald.dymmond.com/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
 Source = "https://github.com/dymmond/esmerald"
 
 [project.optional-dependencies]
 test = ["httpx>=0.25.0,<0.30.0"]
-
 dev = [
     # includes watchfiles
     "uvicorn[standard]>=0.24.0",
 ]
 
-
 templates = ["mako>=1.2.4,<2.0.0"]
 jwt = ["passlib==1.7.4", "python-jose>=3.3.0,<4"]
 encoders = ["ujson>=5.7.0,<6"]
 schedulers = ["asyncz>=0.4.0"]
+all = ["esmerald[test,dev,templates,jwt,encoders,schedulers]","ipython","ptpython","a2wsgi"]
+
+
 
 [tool.hatch.envs.default]
 dependencies = ["ruff", "pre-commit>=2.17.0,<3.0.0", "twine"]
+
 [tool.hatch.envs.default.scripts]
 clean_pyc = "find . -type f -name \"*.pyc\" -delete"
 clean_pyi = "find . -type f -name \"*.pyi\" -delete"
 clean_pycache = "find . -type d -name \"*__pycache__*\" -delete"
 build_with_check = "hatch build; twine check dist/*"
 lint = "ruff check --fix --line-length 99 esmerald tests docs_src {args}"
 
 
 [tool.hatch.envs.docs]
+detached = true
+skip-install = true
 dependencies = [
     "a2wsgi>=1.9.0,<2",
     "griffe-typingdoc>=0.2.2",
     "httpx>=0.25.0,<0.30.0",
     "mike>=2.0.0",
     "mkautodoc>=0.2.0,<0.3.0",
     "mkdocs>=1.1.2,<2.0.0",
@@ -130,54 +134,50 @@
     "mkdocstrings[python]>=0.23.0,<0.30.0",
     "pyyaml>=6.0,<7.0.0",
 ]
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build"
 serve = "mkdocs serve --dev-addr localhost:8000"
 
-
 [tool.hatch.envs.test]
+features = ["all"]
 dependencies = [
     "pytest>=7.1.3,<9.0.0",
     "pytest-cov>=4.1.0,<6.0.0",
     "pytest-asyncio>=0.20.0",
     "mypy==1.9.0",
-    "aiofiles>=0.8.0,<24",
-    "a2wsgi>=1.9.0,<2",
-    "asyncz>=0.6.0",
     "anyio[trio]>=3.6.2,<5.0.0",
-    "httpx>=0.25.0,<0.30.0",
     "brotli>=1.0.9,<2.0.0",
     "flask>=1.1.2,<4.0.0",
     "freezegun>=1.2.2,<2.0.0",
-    "mock==5.1.0",
-    "passlib==1.7.4",
     "polyfactory>=2.5.0,<3.0.0",
-    "python-jose>=3.3.0,<4",
     "saffier[postgres]>=1.3.7",
     "edgy[postgres]>=0.4.0",
     "mongoz>=0.6.0",
-    "ujson>=5.7.0,<6",
 
     # types
     "types-ujson==5.9.0.0",
     "types-orjson==3.6.2",
-    "ipython",
-    "ptpython",
-    "uvicorn",
-
 ]
 [tool.hatch.envs.test.scripts]
-
 # needs docker services running
 test = "ESMERALD_SETTINGS_MODULE='tests.settings.TestSettings' pytest {args}"
 coverage = "ESMERALD_SETTINGS_MODULE='tests.settings.TestSettings' pytest --cov=asyncz --cov=tests --cov-report=term-missing:skip-covered --cov-report=html tests {args}"
 check_types = "mypy -p lilya"
 
 
+[tool.hatch.envs.hatch-test]
+features = ["all"]
+template = "test"
+installer = "pip"
+
+[tool.hatch.envs.hatch-test.scripts]
+run = "ESMERALD_SETTINGS_MODULE='tests.settings.TestSettings' pytest{env:HATCH_TEST_ARGS:} {args}"
+run-cov = "ESMERALD_SETTINGS_MODULE='tests.settings.TestSettings' coverage run -m pytest{env:HATCH_TEST_ARGS:} {args}"
+
 [tool.hatch.version]
 path = "esmerald/__init__.py"
 
 [project.scripts]
 esmerald = "esmerald.__main__:run_cli"
 
 [tool.ruff.lint.isort]
```

### Comparing `esmerald-3.1.3/PKG-INFO` & `esmerald-3.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esmerald
-Version: 3.1.3
+Version: 3.1.4
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -49,14 +49,25 @@
 Requires-Dist: openapi-schemas-pydantic>=3.0.0
 Requires-Dist: orjson<4.0.0,>=3.8.5
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0
 Requires-Dist: pydantic<3.0.0,>=2.5.3
 Requires-Dist: python-multipart<0.0.10,>=0.0.7
 Requires-Dist: rich<14.0.0,>=13.3.1
 Requires-Dist: typing-extensions>=4.11.0
+Provides-Extra: all
+Requires-Dist: a2wsgi; extra == 'all'
+Requires-Dist: asyncz>=0.4.0; extra == 'all'
+Requires-Dist: httpx<0.30.0,>=0.25.0; extra == 'all'
+Requires-Dist: ipython; extra == 'all'
+Requires-Dist: mako<2.0.0,>=1.2.4; extra == 'all'
+Requires-Dist: passlib==1.7.4; extra == 'all'
+Requires-Dist: ptpython; extra == 'all'
+Requires-Dist: python-jose<4,>=3.3.0; extra == 'all'
+Requires-Dist: ujson<6,>=5.7.0; extra == 'all'
+Requires-Dist: uvicorn[standard]>=0.24.0; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: uvicorn[standard]>=0.24.0; extra == 'dev'
 Provides-Extra: encoders
 Requires-Dist: ujson<6,>=5.7.0; extra == 'encoders'
 Provides-Extra: jwt
 Requires-Dist: passlib==1.7.4; extra == 'jwt'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'jwt'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: esmerald Version: 3.1.3 Summary: Highly scalable,
+Metadata-Version: 2.3 Name: esmerald Version: 3.1.4 Summary: Highly scalable,
 performant, easy to learn, easy to code and for every application. Project-URL:
 Homepage, https://github.com/dymmond/esmerald Project-URL: Documentation,
 https://esmerald.dymmond.com/ Project-URL: Changelog, https://
 esmerald.dymmond.com/release-notes/ Project-URL: Funding, https://github.com/
 sponsors/tarsil Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva
 dymmond.com> License-Expression: MIT License-File: LICENSE Keywords:
@@ -30,22 +30,29 @@
 click<9.0.0,>=8.1.4 Requires-Dist: itsdangerous<3.0.0,>=2.1.2 Requires-Dist:
 jinja2<4.0.0,>=3.1.2 Requires-Dist: lilya>=0.3.3 Requires-Dist:
 loguru<0.8.0,>=0.7.0 Requires-Dist: msgspec<1.0.0,>=0.18.5 Requires-Dist: nest-
 asyncio<2.0.0,>=1.5.8 Requires-Dist: openapi-schemas-pydantic>=3.0.0 Requires-
 Dist: orjson<4.0.0,>=3.8.5 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0
 Requires-Dist: pydantic<3.0.0,>=2.5.3 Requires-Dist: python-
 multipart<0.0.10,>=0.0.7 Requires-Dist: rich<14.0.0,>=13.3.1 Requires-Dist:
-typing-extensions>=4.11.0 Provides-Extra: dev Requires-Dist: uvicorn
-[standard]>=0.24.0; extra == 'dev' Provides-Extra: encoders Requires-Dist:
-ujson<6,>=5.7.0; extra == 'encoders' Provides-Extra: jwt Requires-Dist:
-passlib==1.7.4; extra == 'jwt' Requires-Dist: python-jose<4,>=3.3.0; extra ==
-'jwt' Provides-Extra: schedulers Requires-Dist: asyncz>=0.4.0; extra ==
-'schedulers' Provides-Extra: templates Requires-Dist: mako<2.0.0,>=1.2.4; extra
-== 'templates' Provides-Extra: test Requires-Dist: httpx<0.30.0,>=0.25.0; extra
-== 'test' Description-Content-Type: text/markdown # Esmerald
+typing-extensions>=4.11.0 Provides-Extra: all Requires-Dist: a2wsgi; extra ==
+'all' Requires-Dist: asyncz>=0.4.0; extra == 'all' Requires-Dist:
+httpx<0.30.0,>=0.25.0; extra == 'all' Requires-Dist: ipython; extra == 'all'
+Requires-Dist: mako<2.0.0,>=1.2.4; extra == 'all' Requires-Dist:
+passlib==1.7.4; extra == 'all' Requires-Dist: ptpython; extra == 'all'
+Requires-Dist: python-jose<4,>=3.3.0; extra == 'all' Requires-Dist:
+ujson<6,>=5.7.0; extra == 'all' Requires-Dist: uvicorn[standard]>=0.24.0; extra
+== 'all' Provides-Extra: dev Requires-Dist: uvicorn[standard]>=0.24.0; extra ==
+'dev' Provides-Extra: encoders Requires-Dist: ujson<6,>=5.7.0; extra ==
+'encoders' Provides-Extra: jwt Requires-Dist: passlib==1.7.4; extra == 'jwt'
+Requires-Dist: python-jose<4,>=3.3.0; extra == 'jwt' Provides-Extra: schedulers
+Requires-Dist: asyncz>=0.4.0; extra == 'schedulers' Provides-Extra: templates
+Requires-Dist: mako<2.0.0,>=1.2.4; extra == 'templates' Provides-Extra: test
+Requires-Dist: httpx<0.30.0,>=0.25.0; extra == 'test' Description-Content-Type:
+text/markdown # Esmerald
                                   _[_E_s_m_e_r_a_l_d_]
   ?ð??? HHiigghhllyy ssccaallaabbllee,, ppeerrffoorrmmaanntt,, eeaassyy ttoo lleeaarrnn,, eeaassyy ttoo ccooddee aanndd ffoorr eevveerryy
                                aapppplliiccaattiioonn.. ?ð???
            _[_T_e_s_t_ _S_u_i_t_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
 --- **Documentation**: [https://esmerald.dev](https://www.esmerald.dev) ð
 **Source Code**: [https://github.com/dymmond/esmerald](https://github.com/
 dymmond/esmerald) **The official supported version is always the latest
```

