# Comparing `tmp/app_model-0.2.6.tar.gz` & `tmp/app_model-0.2.7.tar.gz`

## Comparing `app_model-0.2.6.tar` & `app_model-0.2.7.tar`

### file list

```diff
@@ -1,83 +1,82 @@
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 app_model-0.2.6/.github_changelog_generator
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 app_model-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 app_model-0.2.6/.readthedocs.yaml
--rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 app_model-0.2.6/CHANGELOG.md
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 app_model-0.2.6/codecov.yml
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 app_model-0.2.6/mkdocs.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 app_model-0.2.6/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 app_model-0.2.6/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 app_model-0.2.6/.github/dependabot.yml
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 app_model-0.2.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 app_model-0.2.6/.github/workflows/cron.yml
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 app_model-0.2.6/demo/keybinding_helper.py
--rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 app_model-0.2.6/demo/model_app.py
--rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 app_model-0.2.6/demo/qapplication.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.2.6/demo/multi_file/__init__.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 app_model-0.2.6/demo/multi_file/__main__.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 app_model-0.2.6/demo/multi_file/actions.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 app_model-0.2.6/demo/multi_file/app.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 app_model-0.2.6/demo/multi_file/constants.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 app_model-0.2.6/demo/multi_file/functions.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 app_model-0.2.6/docs/gen_ref_nav.py
--rw-r--r--   0        0        0     9117 2020-02-02 00:00:00.000000 app_model-0.2.6/docs/getting_started.md
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 app_model-0.2.6/docs/index.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 app_model-0.2.6/docs/my_hooks.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 app_model-0.2.6/docs/css/style.css
--rw-r--r--   0        0        0    44931 2020-02-02 00:00:00.000000 app_model-0.2.6/docs/images/qmainwindow.jpeg
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/__init__.py
--rw-r--r--   0        0        0     9994 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/backends/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/backends/qt/__init__.py
--rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/backends/qt/_qaction.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/backends/qt/_qkeybindingedit.py
--rw-r--r--   0        0        0    16824 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/backends/qt/_qkeymap.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/backends/qt/_qmainwindow.py
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/backends/qt/_qmenu.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/backends/qt/_util.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/expressions/__init__.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/expressions/_context.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/expressions/_context_keys.py
--rw-r--r--   0        0        0    19406 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/expressions/_expressions.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/registries/__init__.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/registries/_commands_reg.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/registries/_keybindings_reg.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/registries/_menus_reg.py
--rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/registries/_register.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/__init__.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_action.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_base.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_command_rule.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_constants.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_icon.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_keybinding_rule.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_menu_rule.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_utils.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_keys/__init__.py
--rw-r--r--   0        0        0    34796 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_keys/_key_codes.py
--rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_keys/_keybindings.py
--rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 app_model-0.2.6/src/app_model/types/_keys/_standard_bindings.py
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/conftest.py
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_actions.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_app.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_command_registry.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_key_codes.py
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_keybindings.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_registries.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_types.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/fixtures/fake_module.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_context/test_context.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_context/test_context_keys.py
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_context/test_expressions.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_qt/__init__.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_qt/test_demos.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_qt/test_qactions.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_qt/test_qkeybindingedit.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_qt/test_qkeymap.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_qt/test_qmainwindow.py
--rw-r--r--   0        0        0     5582 2020-02-02 00:00:00.000000 app_model-0.2.6/tests/test_qt/test_qmenu.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 app_model-0.2.6/.gitignore
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 app_model-0.2.6/LICENSE
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 app_model-0.2.6/README.md
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 app_model-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 app_model-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 app_model-0.2.7/.github_changelog_generator
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 app_model-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 app_model-0.2.7/.readthedocs.yaml
+-rw-r--r--   0        0        0    19619 2020-02-02 00:00:00.000000 app_model-0.2.7/CHANGELOG.md
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 app_model-0.2.7/codecov.yml
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 app_model-0.2.7/mkdocs.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 app_model-0.2.7/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 app_model-0.2.7/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 app_model-0.2.7/.github/dependabot.yml
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 app_model-0.2.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 app_model-0.2.7/demo/keybinding_helper.py
+-rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 app_model-0.2.7/demo/model_app.py
+-rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 app_model-0.2.7/demo/qapplication.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.2.7/demo/multi_file/__init__.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 app_model-0.2.7/demo/multi_file/__main__.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 app_model-0.2.7/demo/multi_file/actions.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 app_model-0.2.7/demo/multi_file/app.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 app_model-0.2.7/demo/multi_file/constants.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 app_model-0.2.7/demo/multi_file/functions.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 app_model-0.2.7/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0     9117 2020-02-02 00:00:00.000000 app_model-0.2.7/docs/getting_started.md
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 app_model-0.2.7/docs/index.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 app_model-0.2.7/docs/my_hooks.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 app_model-0.2.7/docs/css/style.css
+-rw-r--r--   0        0        0    44931 2020-02-02 00:00:00.000000 app_model-0.2.7/docs/images/qmainwindow.jpeg
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/__init__.py
+-rw-r--r--   0        0        0     9994 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/backends/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/backends/qt/__init__.py
+-rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/backends/qt/_qaction.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/backends/qt/_qkeybindingedit.py
+-rw-r--r--   0        0        0    16824 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/backends/qt/_qkeymap.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/backends/qt/_qmainwindow.py
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/backends/qt/_qmenu.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/backends/qt/_util.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/expressions/__init__.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/expressions/_context.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/expressions/_context_keys.py
+-rw-r--r--   0        0        0    19406 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/expressions/_expressions.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/registries/__init__.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/registries/_commands_reg.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/registries/_keybindings_reg.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/registries/_menus_reg.py
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/registries/_register.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/__init__.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_action.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_base.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_command_rule.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_constants.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_icon.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_keybinding_rule.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_menu_rule.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_utils.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_keys/__init__.py
+-rw-r--r--   0        0        0    34796 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_keys/_key_codes.py
+-rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_keys/_keybindings.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 app_model-0.2.7/src/app_model/types/_keys/_standard_bindings.py
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/conftest.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_actions.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_app.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_command_registry.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_key_codes.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_keybindings.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_registries.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_types.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/fixtures/fake_module.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_context/test_context.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_context/test_context_keys.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_context/test_expressions.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_qt/__init__.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_qt/test_demos.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_qt/test_qactions.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_qt/test_qkeybindingedit.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_qt/test_qkeymap.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_qt/test_qmainwindow.py
+-rw-r--r--   0        0        0     5582 2020-02-02 00:00:00.000000 app_model-0.2.7/tests/test_qt/test_qmenu.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 app_model-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 app_model-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 app_model-0.2.7/README.md
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 app_model-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 app_model-0.2.7/PKG-INFO
```

### Comparing `app_model-0.2.6/.pre-commit-config.yaml` & `app_model-0.2.7/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 ci:
   autoupdate_schedule: monthly
   autofix_commit_msg: "style: [pre-commit.ci] auto fixes [...]"
   autoupdate_commit_msg: "ci: [pre-commit.ci] autoupdate"
 
 repos:
   - repo: https://github.com/crate-ci/typos
-    rev: v1.19.0
+    rev: v1.21.0
     hooks:
       - id: typos
+        args: []
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.3
+    rev: v0.4.3
     hooks:
       - id: ruff
         args: ["--fix", "--unsafe-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.16
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: mypy
         files: "^src/"
         additional_dependencies:
           - pydantic >2
           - pydantic-compat
           - in-n-out
```

### Comparing `app_model-0.2.6/CHANGELOG.md` & `app_model-0.2.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
+## [v0.2.7](https://github.com/pyapp-kit/app-model/tree/v0.2.7) (2024-05-08)
+
+[Full Changelog](https://github.com/pyapp-kit/app-model/compare/v0.2.6...v0.2.7)
+
+**Implemented enhancements:**
+
+- feat: give registries more control over registration of actions [\#194](https://github.com/pyapp-kit/app-model/pull/194) ([tlambert03](https://github.com/tlambert03))
+
 ## [v0.2.6](https://github.com/pyapp-kit/app-model/tree/v0.2.6) (2024-03-25)
 
 [Full Changelog](https://github.com/pyapp-kit/app-model/compare/v0.2.5...v0.2.6)
 
-**Merged pull requests:**
+**Fixed bugs:**
 
 - fix: Do not use lambda in QMenuItemAction.destroyed callback [\#183](https://github.com/pyapp-kit/app-model/pull/183) ([Czaki](https://github.com/Czaki))
 
 ## [v0.2.5](https://github.com/pyapp-kit/app-model/tree/v0.2.5) (2024-03-18)
 
 [Full Changelog](https://github.com/pyapp-kit/app-model/compare/v0.2.4...v0.2.5)
```

### Comparing `app_model-0.2.6/mkdocs.yml` & `app_model-0.2.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/.github/workflows/ci.yml` & `app_model-0.2.7/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -11,62 +11,66 @@
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   test:
-    uses: pyapp-kit/workflows/.github/workflows/test-pyrepo.yml@v1
+    uses: pyapp-kit/workflows/.github/workflows/test-pyrepo.yml@v2
     with:
       os: ${{ matrix.os }}
       python-version: ${{ matrix.python-version }}
       pip-post-installs: ${{ matrix.pydantic }}
       pip-install-pre-release: ${{ github.event_name == 'schedule' }}
-      report-failures: ${{ github.event_name == 'schedule' }}
+      coverage-upload: artifact
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.8", "3.10", "3.12"]
         os: [ubuntu-latest, macos-latest, windows-latest]
         pydantic: [""]
+        exclude:
+          - python-version: "3.8"
+            os: "macos-latest"
         include:
+          - python-version: "3.8"
+            os: "macos-13"
           - python-version: "3.9"
-            os: "macos-latest"
+            os: "macos-13"
           - python-version: "3.11"
             os: "ubuntu-latest"
           - python-version: "3.12"
             os: "ubuntu-latest"
             pydantic: "'pydantic<2'"
           - python-version: "3.8"
             os: "ubuntu-latest"
             pydantic: "'pydantic<2'"
 
   test-qt:
-    uses: pyapp-kit/workflows/.github/workflows/test-pyrepo.yml@v1
+    uses: pyapp-kit/workflows/.github/workflows/test-pyrepo.yml@v2
     with:
       qt: ${{ matrix.qt }}
       os: ${{ matrix.os }}
       python-version: ${{ matrix.python-version }}
       extras: test-qt
       pip-install-pre-release: ${{ github.event_name == 'schedule' }}
-      report-failures: ${{ github.event_name == 'schedule' }}
+      coverage-upload: artifact
     strategy:
       fail-fast: false
       matrix:
         include:
           - python-version: "3.8"
             os: "ubuntu-latest"
             qt: "PyQt5==5.12"
           - python-version: "3.10"
             os: "ubuntu-latest"
             qt: "PyQt5~=5.15.0"
           - python-version: "3.10"
             os: "ubuntu-latest"
             qt: "PySide2~=5.15.0"
-
           - python-version: "3.10"
             os: "ubuntu-latest"
             qt: "PyQt6~=6.2.0"
           - python-version: "3.10"
             os: "ubuntu-latest"
             qt: "PySide6~=6.3.0"
           - python-version: "3.10"
@@ -76,36 +80,42 @@
             os: "ubuntu-latest"
             qt: "PySide6~=6.5.0"
           - python-version: "3.11"
             os: "ubuntu-latest"
             qt: "PySide6~=6.6.0"
           - python-version: "3.11"
             os: "ubuntu-latest"
-            qt: "PyQt6~=6.6.0"
-
+            qt: pyqt6
           - python-version: "3.10"
             os: "windows-latest"
             qt: "PySide2"
           - python-version: "3.9"
-            os: "macos-latest"
+            os: "macos-13"
             qt: "PySide2"
 
+  upload_coverage:
+    if: always()
+    needs: [test, test-qt]
+    uses: pyapp-kit/workflows/.github/workflows/upload-coverage.yml@v2
+    secrets: inherit
+
   test_napari:
-    uses: pyapp-kit/workflows/.github/workflows/test-dependents.yml@v1
+    uses: pyapp-kit/workflows/.github/workflows/test-dependents.yml@v2
     with:
       dependency-repo: napari/napari
       dependency-ref: ${{ matrix.napari-version }}
       dependency-extras: "testing"
       qt: ${{ matrix.qt }}
-      pytest-args: 'napari/_qt napari/_app_model napari/utils/_tests/test_key_bindings.py -k "not async and not qt_dims_2"'
+      pytest-args: 'napari/_qt/_qapp_model napari/_app_model napari/utils/_tests/test_key_bindings.py -k "not async and not qt_dims_2"'
       python-version: "3.10"
+      post-install-cmd: "pip install lxml_html_clean" # fix for napari v0.4.19
     strategy:
       fail-fast: false
       matrix:
-        napari-version: ["", "v0.4.18"]
+        napari-version: ["", "v0.4.19.post1"]
         qt: ["pyqt5", "pyside2"]
 
   check-manifest:
     name: Check Manifest
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
```

### Comparing `app_model-0.2.6/demo/model_app.py` & `app_model-0.2.7/demo/model_app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/demo/qapplication.py` & `app_model-0.2.7/demo/qapplication.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/demo/multi_file/actions.py` & `app_model-0.2.7/demo/multi_file/actions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/demo/multi_file/app.py` & `app_model-0.2.7/demo/multi_file/app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/docs/gen_ref_nav.py` & `app_model-0.2.7/docs/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/docs/getting_started.md` & `app_model-0.2.7/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/docs/index.md` & `app_model-0.2.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/docs/css/style.css` & `app_model-0.2.7/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/docs/images/qmainwindow.jpeg` & `app_model-0.2.7/docs/images/qmainwindow.jpeg`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/_app.py` & `app_model-0.2.7/src/app_model/_app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/backends/qt/__init__.py` & `app_model-0.2.7/src/app_model/backends/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/backends/qt/_qaction.py` & `app_model-0.2.7/src/app_model/backends/qt/_qaction.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/backends/qt/_qkeybindingedit.py` & `app_model-0.2.7/src/app_model/backends/qt/_qkeybindingedit.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/backends/qt/_qkeymap.py` & `app_model-0.2.7/src/app_model/backends/qt/_qkeymap.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/backends/qt/_qmainwindow.py` & `app_model-0.2.7/src/app_model/backends/qt/_qmainwindow.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/backends/qt/_qmenu.py` & `app_model-0.2.7/src/app_model/backends/qt/_qmenu.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/backends/qt/_util.py` & `app_model-0.2.7/src/app_model/backends/qt/_util.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/expressions/__init__.py` & `app_model-0.2.7/src/app_model/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/expressions/_context.py` & `app_model-0.2.7/src/app_model/expressions/_context.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/expressions/_context_keys.py` & `app_model-0.2.7/src/app_model/expressions/_context_keys.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/expressions/_expressions.py` & `app_model-0.2.7/src/app_model/expressions/_expressions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/registries/_commands_reg.py` & `app_model-0.2.7/src/app_model/registries/_commands_reg.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,147 @@
 from __future__ import annotations
 
 from concurrent.futures import Future, ThreadPoolExecutor
-from functools import cached_property
 from typing import TYPE_CHECKING, Any, Callable, Generic, Iterator, TypeVar, cast
 
 from in_n_out import Store
 from psygnal import Signal
 
 # maintain runtime compatibility with older typing_extensions
 if TYPE_CHECKING:
     from typing_extensions import ParamSpec
 
-    from app_model.types import DisposeCallable
+    from app_model.types import Action, DisposeCallable
 
     P = ParamSpec("P")
 else:
     try:
         from typing_extensions import ParamSpec
 
         P = ParamSpec("P")
     except ImportError:
         P = TypeVar("P")
 
 
 R = TypeVar("R")
 
 
-class _RegisteredCommand(Generic[P, R]):
+class RegisteredCommand(Generic[P, R]):
     """Small object to represent a command in the CommandsRegistry.
 
-    Only used internally by the CommandsRegistry.
+    Used internally by the CommandsRegistry.
+
     This helper class allows us to cache the dependency-injected variant of the
-    command. As usual with `cached_property`, the cache can be cleard by deleting
-    the attribute: `del cmd.run_injected`
+    command, so that type resolution and dependency injection is performed only
+    once.
     """
 
+    __slots__ = (
+        "id",
+        "callback",
+        "title",
+        "_resolved_callback",
+        "_injection_store",
+        "_injected_callback",
+        "_initialized",
+    )
+
     def __init__(
         self,
         id: str,
         callback: Callable[P, R] | str,
         title: str,
         store: Store | None = None,
     ) -> None:
         self.id = id
         self.callback = callback
         self.title = title
-        self._resolved_callback = callback if callable(callback) else None
         self._injection_store: Store = store or Store.get_store()
+        self._resolved_callback = callback if callable(callback) else None
+        self._injected_callback: Callable[P, R] | None = None
+        self._initialized = True
+
+    def __setattr__(self, name: str, value: Any) -> None:
+        """Object is immutable after initialization."""
+        if getattr(self, "_initialized", False):
+            raise AttributeError("RegisteredCommand object is immutable.")
+        super().__setattr__(name, value)
 
     @property
     def resolved_callback(self) -> Callable[P, R]:
+        """Return the resolved command callback.
+
+        This property is cached, so the callback types are only resolved once.
+        """
         if self._resolved_callback is None:
             from app_model.types._utils import import_python_name
 
             try:
-                self._resolved_callback = import_python_name(str(self.callback))
+                cb = import_python_name(str(self.callback))
             except ImportError as e:
-                self._resolved_callback = cast(Callable[P, R], lambda *a, **k: None)
+                object.__setattr__(self, "_resolved_callback", lambda *a, **k: None)
                 raise type(e)(
                     f"Command pointer {self.callback!r} registered for Command "
                     f"{self.id!r} was not importable: {e}"
                 ) from e
 
-            if not callable(self._resolved_callback):
+            if not callable(cb):
                 # don't try to import again, just create a no-op
-                self._resolved_callback = cast(Callable[P, R], lambda *a, **k: None)
+                object.__setattr__(self, "_resolved_callback", lambda *a, **k: None)
                 raise TypeError(
                     f"Command pointer {self.callback!r} registered for Command "
                     f"{self.id!r} did not resolve to a callble object."
                 )
-        return self._resolved_callback
+            object.__setattr__(self, "_resolved_callback", cb)
+        return cast("Callable[P, R]", self._resolved_callback)
 
-    @cached_property
+    @property
     def run_injected(self) -> Callable[P, R]:
-        return self._injection_store.inject(self.resolved_callback, processors=True)
+        """Return the command callback with dependencies injected.
+
+        This property is cached, so the injected version is only created once.
+        """
+        if self._injected_callback is None:
+            cb = self._injection_store.inject(self.resolved_callback, processors=True)
+            object.__setattr__(self, "_injected_callback", cb)
+        return cast("Callable[P, R]", self._injected_callback)
 
 
 class CommandsRegistry:
     """Registry for commands (callable objects)."""
 
     registered = Signal(str)
 
     def __init__(
         self,
         injection_store: Store | None = None,
         raise_synchronous_exceptions: bool = False,
     ) -> None:
-        self._commands: dict[str, _RegisteredCommand] = {}
+        self._commands: dict[str, RegisteredCommand] = {}
         self._injection_store = injection_store
         self._raise_synchronous_exceptions = raise_synchronous_exceptions
 
+    def register_action(self, action: Action) -> DisposeCallable:
+        """Register an Action object.
+
+        This is a convenience method that registers the action's callback
+        with the action's ID and title using `register_command`.
+
+        Parameters
+        ----------
+        action: Action
+            Action to register
+
+        Returns
+        -------
+        DisposeCallable
+            A function that can be called to unregister the action.
+        """
+        return self.register_command(action.id, action.callback, action.title)
+
     def register_command(
         self, id: str, callback: Callable[P, R] | str, title: str
     ) -> DisposeCallable:
         """Register a callable as the handler for command `id`.
 
         Parameters
         ----------
@@ -111,37 +159,37 @@
         """
         if id in self._commands:
             raise ValueError(
                 f"Command {id!r} already registered with callback "
                 f"{self._commands[id].callback!r} (new callback: {callback!r})"
             )
 
-        cmd = _RegisteredCommand(id, callback, title, self._injection_store)
+        cmd = RegisteredCommand(id, callback, title, self._injection_store)
         self._commands[id] = cmd
 
         def _dispose() -> None:
             self._commands.pop(id, None)
 
         self.registered.emit(id)
         return _dispose
 
-    def __iter__(self) -> Iterator[tuple[str, _RegisteredCommand]]:
+    def __iter__(self) -> Iterator[tuple[str, RegisteredCommand]]:
         yield from self._commands.items()
 
     def __len__(self) -> int:
         return len(self._commands)
 
     def __contains__(self, id: str) -> bool:
         return id in self._commands
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
         return f"<{name} at {hex(id(self))} ({len(self._commands)} commands)>"
 
-    def __getitem__(self, id: str) -> _RegisteredCommand:
+    def __getitem__(self, id: str) -> RegisteredCommand:
         """Retrieve commands registered under a given ID."""
         if id not in self._commands:
             raise KeyError(f"Command {id!r} not registered")
         return self._commands[id]
 
     def execute_command(
         self,
```

### Comparing `app_model-0.2.6/src/app_model/registries/_keybindings_reg.py` & `app_model-0.2.7/src/app_model/registries/_keybindings_reg.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from app_model.types import KeyBinding
 
 if TYPE_CHECKING:
     from typing import Iterator, TypeVar
 
     from app_model import expressions
-    from app_model.types import DisposeCallable, KeyBindingRule
+    from app_model.types import Action, DisposeCallable, KeyBindingRule
 
     CommandDecorator = Callable[[Callable], Callable]
     CommandCallable = TypeVar("CommandCallable", bound=Callable)
 
 
 class _RegisteredKeyBinding(NamedTuple):
     """Internal object representing a fully registered keybinding."""
@@ -29,14 +29,55 @@
     """Registry for keybindings."""
 
     registered = Signal()
 
     def __init__(self) -> None:
         self._keybindings: list[_RegisteredKeyBinding] = []
 
+    def register_action_keybindings(self, action: Action) -> DisposeCallable | None:
+        """Register all keybindings declared in `action.keybindings`.
+
+        Parameters
+        ----------
+        action : Action
+            The action to register keybindings for.
+
+        Returns
+        -------
+        DisposeCallable | None
+            A function that can be called to unregister the keybindings.  If no
+            keybindings were registered, returns None.
+        """
+        if not (keybindings := action.keybindings):
+            return None
+
+        disposers: list[Callable[[], None]] = []
+        for keyb in keybindings:
+            if action.enablement is not None:
+                kwargs = keyb.model_dump()
+                kwargs["when"] = (
+                    action.enablement
+                    if keyb.when is None
+                    else action.enablement | keyb.when
+                )
+                _keyb = type(keyb)(**kwargs)
+            else:
+                _keyb = keyb
+            if d := self.register_keybinding_rule(action.id, _keyb):
+                disposers.append(d)
+
+        if not disposers:  # pragma: no cover
+            return None
+
+        def _dispose() -> None:
+            for disposer in disposers:
+                disposer()
+
+        return _dispose
+
     def register_keybinding_rule(
         self, id: str, rule: KeyBindingRule
     ) -> DisposeCallable | None:
         """Register a new keybinding rule.
 
         Parameters
         ----------
```

### Comparing `app_model-0.2.6/src/app_model/registries/_menus_reg.py` & `app_model-0.2.7/src/app_model/registries/_menus_reg.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,78 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Callable, Final, Iterable, Iterator, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Final, Iterable, Iterator
 
 from psygnal import Signal
 
 from app_model.types import MenuItem
 
 if TYPE_CHECKING:
-    from app_model.types import DisposeCallable, MenuOrSubmenu
+    from app_model.types import Action, DisposeCallable, MenuOrSubmenu
 
 MenuId = str
 
 
 class MenusRegistry:
     """Registry for menu and submenu items."""
 
     COMMAND_PALETTE_ID: Final = "_command_pallet_"
     menus_changed = Signal(set)
 
     def __init__(self) -> None:
         self._menu_items: dict[MenuId, dict[MenuOrSubmenu, None]] = {}
 
+    def append_action_menus(self, action: Action) -> DisposeCallable | None:
+        """Append all MenuRule items declared in `action.menus`.
+
+        Parameters
+        ----------
+        action : Action
+            The action containing menus to append.
+
+        Returns
+        -------
+        DisposeCallable | None
+            A function that can be called to unregister the menu items. If no
+            menu items were registered, returns `None`.
+        """
+        disposers: list[Callable[[], None]] = []
+        disp1 = self.append_menu_items(
+            (
+                rule.id,
+                MenuItem(
+                    command=action, when=rule.when, group=rule.group, order=rule.order
+                ),
+            )
+            for rule in action.menus or ()
+        )
+        disposers.append(disp1)
+
+        if action.palette:
+            menu_item = MenuItem(command=action, when=action.enablement)
+            disp = self.append_menu_items([(self.COMMAND_PALETTE_ID, menu_item)])
+            disposers.append(disp)
+
+        if not disposers:  # pragma: no cover
+            return None
+
+        def _dispose() -> None:
+            for disposer in disposers:
+                disposer()
+
+        return _dispose
+
     def append_menu_items(
-        self, items: Sequence[tuple[MenuId, MenuOrSubmenu]]
+        self, items: Iterable[tuple[MenuId, MenuOrSubmenu]]
     ) -> DisposeCallable:
         """Append menu items to the registry.
 
         Parameters
         ----------
-        items : Sequence[Tuple[str, MenuOrSubmenu]]
+        items : Iterable[Tuple[str, MenuOrSubmenu]]
             Items to append.
 
         Returns
         -------
         DisposeCallable
             A function that can be called to unregister the menu items.
         """
```

### Comparing `app_model-0.2.6/src/app_model/registries/_register.py` & `app_model-0.2.7/src/app_model/registries/_register.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, overload
 
-from app_model.types import Action, MenuItem
+from app_model.types import Action
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Literal, TypeVar
 
     from app_model import Application, expressions
     from app_model.types import (
         DisposeCallable,
@@ -266,46 +266,22 @@
 
     Helper for `register_action()`.
     """
     from app_model._app import Application
 
     app = app if isinstance(app, Application) else Application.get_or_create(app)
 
-    # command
-    disp_cmd = app.commands.register_command(action.id, action.callback, action.title)
-    disposers = [disp_cmd]
-
-    # menu
-    items = []
-    for rule in action.menus or ():
-        menu_item = MenuItem(
-            command=action, when=rule.when, group=rule.group, order=rule.order
-        )
-        items.append((rule.id, menu_item))
-    disposers.append(app.menus.append_menu_items(items))
-
-    if action.palette:
-        menu_item = MenuItem(command=action, when=action.enablement)
-        disp = app.menus.append_menu_items([(app.menus.COMMAND_PALETTE_ID, menu_item)])
-        disposers.append(disp)
-
-    # keybinding
-    for keyb in action.keybindings or ():
-        if action.enablement is not None:
-            kwargs = keyb.model_dump()
-            kwargs["when"] = (
-                action.enablement
-                if keyb.when is None
-                else action.enablement | keyb.when
-            )
-            _keyb = type(keyb)(**kwargs)
-        else:
-            _keyb = keyb
-        if _d := app.keybindings.register_keybinding_rule(action.id, _keyb):
-            disposers.append(_d)
+    # commands
+    disposers = [app.commands.register_action(action)]
+    # menus
+    if dm := app.menus.append_action_menus(action):
+        disposers.append(dm)
+    # keybindings
+    if dk := app.keybindings.register_action_keybindings(action):
+        disposers.append(dk)
 
     def _dispose() -> None:
         for d in disposers:
             d()
 
     app._disposers.append((action.id, _dispose))
     return _dispose
```

### Comparing `app_model-0.2.6/src/app_model/types/__init__.py` & `app_model-0.2.7/src/app_model/types/__init__.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/types/_action.py` & `app_model-0.2.7/src/app_model/types/_action.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/types/_command_rule.py` & `app_model-0.2.7/src/app_model/types/_command_rule.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/types/_constants.py` & `app_model-0.2.7/src/app_model/types/_constants.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/types/_icon.py` & `app_model-0.2.7/src/app_model/types/_icon.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/types/_keybinding_rule.py` & `app_model-0.2.7/src/app_model/types/_keybinding_rule.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/types/_menu_rule.py` & `app_model-0.2.7/src/app_model/types/_menu_rule.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/types/_utils.py` & `app_model-0.2.7/src/app_model/types/_utils.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/types/_keys/_key_codes.py` & `app_model-0.2.7/src/app_model/types/_keys/_key_codes.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/types/_keys/_keybindings.py` & `app_model-0.2.7/src/app_model/types/_keys/_keybindings.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/src/app_model/types/_keys/_standard_bindings.py` & `app_model-0.2.7/src/app_model/types/_keys/_standard_bindings.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/conftest.py` & `app_model-0.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_actions.py` & `app_model-0.2.7/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_app.py` & `app_model-0.2.7/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_key_codes.py` & `app_model-0.2.7/tests/test_key_codes.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_keybindings.py` & `app_model-0.2.7/tests/test_keybindings.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_registries.py` & `app_model-0.2.7/tests/test_registries.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_types.py` & `app_model-0.2.7/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_context/test_context.py` & `app_model-0.2.7/tests/test_context/test_context.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_context/test_context_keys.py` & `app_model-0.2.7/tests/test_context/test_context_keys.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_context/test_expressions.py` & `app_model-0.2.7/tests/test_context/test_expressions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_qt/test_qactions.py` & `app_model-0.2.7/tests/test_qt/test_qactions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_qt/test_qkeymap.py` & `app_model-0.2.7/tests/test_qt/test_qkeymap.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_qt/test_qmainwindow.py` & `app_model-0.2.7/tests/test_qt/test_qmainwindow.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/tests/test_qt/test_qmenu.py` & `app_model-0.2.7/tests/test_qt/test_qmenu.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/.gitignore` & `app_model-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/LICENSE` & `app_model-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/README.md` & `app_model-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/pyproject.toml` & `app_model-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `app_model-0.2.6/PKG-INFO` & `app_model-0.2.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: app-model
-Version: 0.2.6
+Version: 0.2.7
 Summary: Generic application schema implemented in python
 Project-URL: homepage, https://github.com/pyapp-kit/app-model
 Project-URL: repository, https://github.com/pyapp-kit/app-model
 Author: Talley Lambert
 Author-email: talley.lambert@gmail.com
 License: BSD 3-Clause License
 License-File: LICENSE
@@ -23,20 +23,25 @@
 Requires-Python: >=3.8
 Requires-Dist: in-n-out>=0.1.5
 Requires-Dist: psygnal>=0.3.4
 Requires-Dist: pydantic-compat>=0.1.1
 Requires-Dist: pydantic>=1.8
 Requires-Dist: typing-extensions
 Provides-Extra: dev
-Requires-Dist: app-model[test-qt]; extra == 'dev'
+Requires-Dist: fonticon-fontawesome6; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-qt; extra == 'dev'
+Requires-Dist: pytest>=6.0; extra == 'dev'
+Requires-Dist: qtpy; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
+Requires-Dist: superqt[iconify]; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: griffe-fieldz; extra == 'docs'
 Requires-Dist: griffe==0.36.9; extra == 'docs'
 Requires-Dist: mkdocs-gen-files; extra == 'docs'
 Requires-Dist: mkdocs-literate-nav; extra == 'docs'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'docs'
 Requires-Dist: mkdocs-material==9.4.1; extra == 'docs'
@@ -47,18 +52,20 @@
 Provides-Extra: qt
 Requires-Dist: qtpy; extra == 'qt'
 Requires-Dist: superqt[iconify]; extra == 'qt'
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
 Provides-Extra: test-qt
-Requires-Dist: app-model[qt]; extra == 'test-qt'
-Requires-Dist: app-model[test]; extra == 'test-qt'
 Requires-Dist: fonticon-fontawesome6; extra == 'test-qt'
+Requires-Dist: pytest-cov; extra == 'test-qt'
 Requires-Dist: pytest-qt; extra == 'test-qt'
+Requires-Dist: pytest>=6.0; extra == 'test-qt'
+Requires-Dist: qtpy; extra == 'test-qt'
+Requires-Dist: superqt[iconify]; extra == 'test-qt'
 Description-Content-Type: text/markdown
 
 # app-model
 
 [![License](https://img.shields.io/pypi/l/app-model.svg?color=green)](https://github.com/pyapp-kit/app-model/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/app-model.svg?color=green)](https://pypi.org/project/app-model)
 [![Python Version](https://img.shields.io/pypi/pyversions/app-model.svg?color=green)](https://python.org)
```

