# Comparing `tmp/enola-0.3.0.tar.gz` & `tmp/enola-0.4.0.tar.gz`

## Comparing `enola-0.3.0.tar` & `enola-0.4.0.tar`

### file list

```diff
@@ -1,616 +1,616 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 enola-0.3.0/.pypirc
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 enola-0.3.0/requirements.txt
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 enola-0.3.0/.vscode/launch.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/pyvenv.cfg
--rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/Scripts/activate
--rwxr-xr-x   0        0        0     1039 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/Scripts/activate.bat
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0   108448 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/Scripts/normalizer.exe
--rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/Scripts/pip.exe
--rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/Scripts/pip3.11.exe
--rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/Scripts/pip3.exe
--rwxr-xr-x   0        0        0   270608 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/Scripts/python.exe
--rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 enola-0.3.0/mi_entorno/Scripts/pythonw.exe
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 enola-0.3.0/src/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/__init__.py
--rw-r--r--   0        0        0    14361 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/agent.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/step.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/connect.py
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/enola_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/__init__.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_common.py
--rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_connection.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_datetime_part.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_error.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_functions.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_http_info.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_logging.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_param.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_response_error.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_response_provider.py
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/huemul_response_to_bloc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/auth/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/auth/auth_model.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/auth/auth_service_bloc.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/auth/auth_service_model.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/common/auth/auth_service_provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/internal/__init__.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/internal/enola_agent.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/internal/enola_agent_bloc.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 enola-0.3.0/src/enola/base/internal/enola_agent_provider.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/pyvenv.cfg
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/INSTALLER
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/LICENSE
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/METADATA
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/WHEEL
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/entry_points.txt
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/INSTALLER
--rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/METADATA
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/RECORD
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/WHEEL
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_elffile.py
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_manylinux.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_musllinux.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/markers.py
--rw-r--r--   0        0        0    32750 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/py.typed
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/specifiers.py
--rw-r--r--   0        0        0    18355 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/tags.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/utils.py
--rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/METADATA
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/WHEEL
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/py.typed
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13839 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23737 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30030 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18440 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28934 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12457 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18607 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    28868 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27475 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17872 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    33084 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    18969 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11642 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    22343 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   278952 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/METADATA
--rw-r--r--   0        0        0    77283 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/top_level.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Scripts/activate
--rwxr-xr-x   0        0        0     1045 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Scripts/activate.bat
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0   108438 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Scripts/pip.exe
--rwxr-xr-x   0        0        0   108438 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Scripts/pip3.12.exe
--rwxr-xr-x   0        0        0   108438 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Scripts/pip3.exe
--rwxr-xr-x   0        0        0   108442 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Scripts/pyproject-build.exe
--rwxr-xr-x   0        0        0   270616 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Scripts/python.exe
--rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 enola-0.3.0/tutorial_env/Scripts/pythonw.exe
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 enola-0.3.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.3.0/LICENSE
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 enola-0.3.0/README.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 enola-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 enola-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 enola-0.4.0/.pypirc
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 enola-0.4.0/requirements.txt
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 enola-0.4.0/.vscode/launch.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/pyvenv.cfg
+-rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/activate
+-rwxr-xr-x   0        0        0     1039 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/activate.bat
+-rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/deactivate.bat
+-rwxr-xr-x   0        0        0   108448 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/normalizer.exe
+-rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/pip.exe
+-rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/pip3.11.exe
+-rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/pip3.exe
+-rwxr-xr-x   0        0        0   270608 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/python.exe
+-rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/pythonw.exe
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 enola-0.4.0/src/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/__init__.py
+-rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/agent.py
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/step.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/connect.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/enola_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/__init__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_common.py
+-rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_connection.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_datetime_part.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_error.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_functions.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_http_info.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_logging.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_param.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_response_error.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_response_provider.py
+-rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_response_to_bloc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/auth/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/auth/auth_model.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/auth/auth_service_bloc.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/auth/auth_service_model.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/auth/auth_service_provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/internal/__init__.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/internal/enola_agent.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/internal/enola_agent_bloc.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/internal/enola_agent_provider.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/pyvenv.cfg
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/METADATA
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/WHEEL
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/INSTALLER
+-rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/METADATA
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/RECORD
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/WHEEL
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_elffile.py
+-rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/markers.py
+-rw-r--r--   0        0        0    32750 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/specifiers.py
+-rw-r--r--   0        0        0    18355 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/tags.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/utils.py
+-rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/METADATA
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13839 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    23737 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30030 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18440 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    28934 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12457 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18607 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    28868 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    27475 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17872 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    33084 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    18969 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11642 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    22343 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   278952 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t32.exe
+-rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/version.py
+-rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w32.exe
+-rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/METADATA
+-rw-r--r--   0        0        0    77283 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/activate
+-rwxr-xr-x   0        0        0     1045 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/activate.bat
+-rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/deactivate.bat
+-rwxr-xr-x   0        0        0   108438 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/pip.exe
+-rwxr-xr-x   0        0        0   108438 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/pip3.12.exe
+-rwxr-xr-x   0        0        0   108438 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/pip3.exe
+-rwxr-xr-x   0        0        0   108442 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/pyproject-build.exe
+-rwxr-xr-x   0        0        0   270616 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/python.exe
+-rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/pythonw.exe
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 enola-0.4.0/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 enola-0.4.0/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 enola-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 enola-0.4.0/PKG-INFO
```

### Comparing `enola-0.3.0/mi_entorno/Scripts/Activate.ps1` & `enola-0.4.0/mi_entorno/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/mi_entorno/Scripts/activate` & `enola-0.4.0/mi_entorno/Scripts/activate`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/mi_entorno/Scripts/activate.bat` & `enola-0.4.0/mi_entorno/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/mi_entorno/Scripts/normalizer.exe` & `enola-0.4.0/mi_entorno/Scripts/normalizer.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/mi_entorno/Scripts/pip.exe` & `enola-0.4.0/mi_entorno/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/mi_entorno/Scripts/pip3.11.exe` & `enola-0.4.0/mi_entorno/Scripts/pip3.11.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/mi_entorno/Scripts/pip3.exe` & `enola-0.4.0/mi_entorno/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/mi_entorno/Scripts/python.exe` & `enola-0.4.0/mi_entorno/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/mi_entorno/Scripts/pythonw.exe` & `enola-0.4.0/mi_entorno/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/test.py` & `enola-0.4.0/src/test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/agent.py` & `enola-0.4.0/src/enola/agent.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,42 +8,49 @@
 from enola.base.common.auth.auth_model import AuthModel
 from enola.base.enola_types import KindType, DataListModel, DataType, ErrOrWarnKind, Info, StepType
 from enola.base.connect import Connect
 from enola.base.enola_types import AgentModel
 from enola.base.internal.enola_agent import create as create_enola_agent
 
 
-def add_one(number):
-    return number + 1
+#def add_one(number):
+#    return number + 1
 
 class Agent:
-    def __init__(self, token, name, app_id=None, user_id=None, session_id=None, channel_id=None, ip=None, code_api=None, isTest=False, enola_id_prev:str = ""):
+    def __init__(self, token, name, app_id=None, user_id=None, session_id=None, channel_id=None, ip=None, code_api=None, isTest=False, message_input: str = "", enola_id_prev:str = "", app_name:str="", user_name:str="", session_name:str="", channel_name:str=""):
         """
         Start agent Execution
 
         token: jwt token, this is used to identify the agent, request from Admin App
         name: name of this execution
+        message_input: message received from user or to explain the execution
         app_id: id of app, this is used to identify the app who is calling
         user_id: id of external user, this is used to identify the user who is calling
         session_id: id of session of user or application, this is used to identify the session who is calling
         channel_id: web, chat, whatsapp, etc, this is used to identify the channel who is calling
         ip: ip of user or application, this is used to identify the ip who is calling
         code_api: code of api, this is used to identify the api who is calling
         isTest: true if this call is for testing purposes
         enola_id_prev: id of previous call, this is used to link agents sequence
         """
         self.name = name
         self.enola_id_prev = enola_id_prev
         self.enola_id = "" #se obtiene al finalizar la ejecución
         self.agent_deploy_id = ""
+        self.message_input = message_input
+        self.message_output = ""
+        self.num_iteratons = 0
         self.hf = HuemulFunctions()
         #Connection data
 
         #decodificar jwt
         try:
+            if token == "":
+                raise Exception("token is empty.")
+            
             decoded = jwt.decode(token, algorithms=['none'], options={'verify_signature': False})
             self.agentDeployId = decoded["sub"]
             self.orgId = decoded["orgId"]
             self.serviceAccountId = decoded["id"]
             self.serviceAccountName = decoded["displayName"]
             self.serviceAccountUrl = decoded["url"]
             
@@ -63,17 +70,21 @@
             print("Invalid Token.")
 
         self.connection = Connect(AuthModel(jwtToken=token, urlService=self.serviceAccountUrl, orgId=self.orgId))
         
 
         #user information
         self.app_id = app_id
+        self.app_name = app_name
         self.user_id = user_id
+        self.user_name = user_name
         self.session_id = session_id
+        self.session_name = session_name
         self.channel_id = channel_id
+        self.channel_name = channel_name
         self.ip = ip
         self.code_api = code_api
 
         #current date
         self.date_start = self.hf.getDateForApi()
         
         #if is empty or not exist assign false
@@ -134,30 +145,36 @@
     def add_warning(self, id: str, message: str, kind: ErrOrWarnKind):
         """
         register warning to agent
         """
         self.first_step.add_warning(id=id, message=message, kind=kind)
 
 
-    def finish_agent(self, successfull: bool):
+    def finish_agent(self, successfull: bool, message_output: str ="", num_iteratons: int = 0):
         """
         register in Enola server
+
         """
         self.date_end = self.hf.getDateForApi()
         self.duration_in_ms = self.hf.getDifMs(self.date_start, self.date_end)
-        self.close_step_others(step=self.first_step, successfull=successfull, others_cost=0, step_id="AGENT")
+        self.first_step.num_iterations  = num_iteratons
+        self.close_step_others(step=self.first_step, successfull=successfull, others_cost=0, step_id="AGENT", message_output=message_output)
 
         #register in server
         print(f'{self.name}: sending to server... ')
         agentModel = AgentModel(
             app_id=self.app_id, 
+            app_name=self.app_name,
             enola_id_prev = self.enola_id_prev,
             user_id=self.user_id, 
+            user_name=self.user_name, 
             session_id=self.session_id, 
-            channel_id=self.channel_id, 
+            session_name=self.session_name,
+            channel_id=self.channel_id,
+            channel_name=self.channel_name,
             ip=self.ip, 
             code_api=self.code_api, 
             isTest=self.isTest, 
             step_list=self.step_list, 
             steps=self.steps
         )
 
@@ -189,137 +206,149 @@
 
         name: name of this step
         """
         #current_step = 
         self.steps += 1
         return Step(name=name)
 
-    def close_step_token(self, step: Step, successfull: bool, token_input_num: int=0, token_output_num: int=0, token_total_num: int=0, token_input_cost: float=0, token_output_cost: float=0, token_total_cost: float=0, enola_id: str="", agent_deploy_id: str="", step_id:str=""):
+    def close_step_token(self, step: Step, successfull: bool, message_output: str ="", token_input_num: int=0, token_output_num: int=0, token_total_num: int=0, token_input_cost: float=0, token_output_cost: float=0, token_total_cost: float=0, enola_id: str="", agent_deploy_id: str="", step_id:str=""):
         """
         close step with token information
         enola_id: If this step was a call to another Enola agent, whether from your own company or another, this is the ID of that agent
         agent_deploy_id: include this if you want to link this step to another agent of another company
         step_id: id of this step, you can use it to link with external calls
+        message_output: message to user or to explain the execution results
         """
         step.enola_id = enola_id
         step.agent_deploy_id = agent_deploy_id
         step.step_id = step_id
+        step.message_output = message_output
         step.stepType = StepType.TOKEN
         step.token.token_input = token_input_num
         step.token.token_output = token_output_num
         step.token.token_total = token_total_num
         step.cost.token_input = token_input_cost
         step.cost.token_output = token_output_cost
         step.cost.token_total = token_total_cost
 
         step.date_end = self.hf.getDateForApi()
         step.duration_in_ms = self.hf.getDifMs(step.date_start, step.date_end)
         step.successfull = successfull
 
         self.step_list.append(step)
 
-    def close_step_video(self, step: Step, successfull: bool, video_num: int=0, video_sec: int=0, video_size: int=0, video_cost: float=0, enola_id_prev: str="", agent_deploy_id: str="", step_id:str=""):
+    def close_step_video(self, step: Step, successfull: bool, message_output: str ="", video_num: int=0, video_sec: int=0, video_size: int=0, video_cost: float=0, enola_id_prev: str="", agent_deploy_id: str="", step_id:str=""):
         """
         close step with video information
 
         enola_id_prev: If this step was a call to another Enola agent, whether from your own company or another, this is the ID of that agent
         agent_deploy_id: include this if you want to link this step to another agent of another company
         step_id: id of this step, you can use it to link with external calls
+        message_output: message to user or to explain the execution results
         """
         step.enola_id_prev = enola_id_prev
         step.agent_deploy_id = agent_deploy_id
         step.step_id = step_id
+        step.message_output = message_output
         step.stepType = StepType.VIDEO
         step.video.num_videos = video_num
         step.video.sec_videos = video_sec
         step.video.size_videos = video_size
         step.cost.videos = video_cost
         step.date_end = self.hf.getDateForApi()
         step.duration_in_ms = self.hf.getDifMs(step.date_start, step.date_end)
         step.successfull = successfull
 
         self.step_list.append(step)
         
-    def close_step_audio(self, step: Step, successfull: bool, audio_num:int = 0, audio_sec:int = 0, audio_size:int = 0, audio_cost: float=0, enola_id_prev: str="", agent_deploy_id: str="", step_id:str=""):
+    def close_step_audio(self, step: Step, successfull: bool, message_output: str ="", audio_num:int = 0, audio_sec:int = 0, audio_size:int = 0, audio_cost: float=0, enola_id_prev: str="", agent_deploy_id: str="", step_id:str=""):
         """
         close step with audio information
 
         enola_id_prev: If this step was a call to another Enola agent, whether from your own company or another, this is the ID of that agent
         agent_deploy_id: include this if you want to link this step to another agent of another company
         step_id: id of this step, you can use it to link with external calls
+        message_output: message to user or to explain the execution results
         """
         step.enola_id_prev = enola_id_prev
         step.agent_deploy_id = agent_deploy_id
         step.step_id = step_id
+        step.message_output = message_output
         step.stepType = StepType.AUDIO
         step.audio.num_audio = audio_num
         step.audio.sec_audio = audio_sec
         step.audio.size_audio = audio_size
         step.cost.audio = audio_cost
         step.date_end = self.hf.getDateForApi()
         step.duration_in_ms = self.hf.getDifMs(step.date_start, step.date_end)
         step.successfull = successfull
 
         self.step_list.append(step)
 
-    def close_step_image(self, step: Step, successfull: bool, image_num:int = 0, image_size:int = 0, image_cost: float = 0, enola_id_prev3: str="", agent_deploy_id: str="", step_id:str=""):
+    def close_step_image(self, step: Step, successfull: bool, message_output: str ="", image_num:int = 0, image_size:int = 0, image_cost: float = 0, enola_id_prev: str="", agent_deploy_id: str="", step_id:str=""):
         """
         close step with image information
 
         enola_id_prev: If this step was a call to another Enola agent, whether from your own company or another, this is the ID of that agent
         agent_deploy_id: include this if you want to link this step to another agent of another company
         step_id: id of this step, you can use it to link with external calls
+        message_output: message to user or to explain the execution results
         """
         step.enola_id_prev = enola_id_prev
         step.agent_deploy_id = agent_deploy_id
         step.step_id = step_id
+        step.message_output = message_output
         step.stepType = StepType.IMAGE
         step.image.num_images = image_num
         step.image.size_images = image_size
         step.cost.images = image_cost
         step.date_end = self.hf.getDateForApi()
         step.duration_in_ms = self.hf.getDifMs(step.date_start, step.date_end)
         step.successfull = successfull
 
         self.step_list.append(step)
 
-    def close_step_doc(self, step: Step, successfull: bool, doc_num:int=0, doc_pages:int=0, doc_size:int = 0, doc_char:int=0, doc_cost: float=0, enola_id_prev: str="", agent_deploy_id: str="", step_id:str=""):
+    def close_step_doc(self, step: Step, successfull: bool, message_output: str ="", doc_num:int=0, doc_pages:int=0, doc_size:int = 0, doc_char:int=0, doc_cost: float=0, enola_id_prev: str="", agent_deploy_id: str="", step_id:str=""):
         """
         close step with doc information
 
         enola_id_prev: If this step was a call to another Enola agent, whether from your own company or another, this is the ID of that agent
         agent_deploy_id: include this if you want to link this step to another agent of another company
         step_id: id of this step, you can use it to link with external calls
+        message_output: message to user or to explain the execution results
         """
         step.enola_id_prev = enola_id_prev
         step.agent_deploy_id = agent_deploy_id
         step.step_id = step_id
+        step.message_output = message_output
         step.stepType = StepType.DOCUMENT
         step.doc.num_docs = doc_num
         step.doc.num_pages = doc_pages
         step.doc.size_docs = doc_size
         step.doc.num_char = doc_char
         step.cost.docs = doc_cost
         step.date_end = self.hf.getDateForApi()
         step.duration_in_ms = self.hf.getDifMs(step.date_start, step.date_end)
         step.successfull = successfull
 
         self.step_list.append(step)
 
-    def close_step_others(self, step: Step, successfull: bool, others_cost: float=0, enola_id_prev: str="", agent_deploy_id: str="", step_id:str=""):
+    def close_step_others(self, step: Step, successfull: bool, message_output: str ="", others_cost: float=0, enola_id_prev: str="", agent_deploy_id: str="", step_id:str=""):
         """
         close step with others information
 
         enola_id_prev: If this step was a call to another Enola agent, whether from your own company or another, this is the ID of that agent
         agent_deploy_id: include this if you want to link this step to another agent of another company
         step_id: id of this step, you can use it to link with external calls
+        message_output: message to user or to explain the execution results
         """
         step.enola_id_prev = enola_id_prev
         step.agent_deploy_id = agent_deploy_id
         step.step_id = step_id
+        step.message_output = message_output
         step.stepType = StepType.OTHER
         step.cost.others = others_cost
         step.date_end = self.hf.getDateForApi()
         step.duration_in_ms = self.hf.getDifMs(step.date_start, step.date_end)
         step.successfull = successfull
 
         self.step_list.append(step)
```

### Comparing `enola-0.3.0/src/enola/step.py` & `enola-0.4.0/src/enola/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 class Step:
     def __init__(self, name: str):
         self.hf = HuemulFunctions()
         self.name = name
         self.enola_id = ""
         self.agent_deploy_id = ""
         self.step_id = ""
+        self.message_input = ""
+        self.message_output = ""
+        self.num_iterations = 0
         self.step_api_code = ""
         self.step_id_prev = ""
         self.date_start = self.hf.getDateForApi()
         self.date_end = self.date_start
         #self.result_list = []
         self.agent_data_list = [] #only for first step
         self.errOrWarn_list = []
@@ -138,14 +141,18 @@
             "agentExecCostImages": self.cost.images,
             "agentExecCostDocs": self.cost.docs,
             "agentExecCostInfra": self.cost.infra,
             "agentExecCostOthers": self.cost.others,
             "agentExecCostTotal": self.cost.total,
             "agentExecIncomeTotal": self.income_total,
 
+            "agentMessageInput": self.message_input,
+            "agentMessageOutput": self.message_output,
+            "agentExecCliNumIter": self.num_iterations,
+
             "agentData": list(map(lambda x: x.to_json(), self.agent_data_list)),
             "errorOrWarning": list(map(lambda x: x.to_json(), self.errOrWarn_list)),
             "extraInfo": list(map(lambda x: x.to_json(), self.extra_info_list)),
             "fileInfo": list(map(lambda x: x.to_json(), self.file_info_list)),
             "stepApiData": list(map(lambda x: x.to_json(), self.step_api_data_list)),
         }
```

### Comparing `enola-0.3.0/src/enola/base/connect.py` & `enola-0.4.0/src/enola/base/connect.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/enola_types.py` & `enola-0.4.0/src/enola/base/enola_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,33 +155,41 @@
         }
     
 
 class AgentModel:
     """
     AgentModel
     """
-    def __init__(self, app_id: str, user_id: str, session_id: str, channel_id: str, ip: str, code_api: str, isTest: bool, step_list: list, steps: int, enola_id_prev: str):
+    def __init__(self, app_id: str, user_id: str, session_id: str, channel_id: str, ip: str, code_api: str, isTest: bool, step_list: list, steps: int, enola_id_prev: str, app_name: str, user_name: str, session_name: str , channel_name: str):
         self.app_id = app_id
+        self.app_name = app_name
         self.user_id = user_id
+        self.user_name = user_name
         self.session_id = session_id
+        self.session_name = session_name
         self.channel_id = channel_id
+        self.channel_name = channel_name
         self.ip = ip
         self.code_api = code_api
         self.isTest = isTest
         #step_list es una lista, generar un arreglo ejecutando el metodo to_json de cada elemento de la lista con map
         self.step_list = step_list
         self.steps = steps
         self.enola_id_prev = enola_id_prev
 
     def to_json(self):
         return {
             "app_id": self.app_id,
+            "app_name": self.app_name,
             "user_id": self.user_id,
+            "user_name": self.user_name,
             "session_id": self.session_id,
             "channel_id": self.channel_id,
+            "session_name": self.session_name,
+            "channel_name": self.channel_name,
             "ip": self.ip,
             "code_api": self.code_api,
             "isTest": self.isTest,
             "step_list": list(map(lambda x: x.to_json(), self.step_list)),
             "steps": self.steps,
             "enola_id_prev": self.enola_id_prev
         }
```

### Comparing `enola-0.3.0/src/enola/base/common/huemul_common.py` & `enola-0.4.0/src/enola/base/common/huemul_common.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/common/huemul_connection.py` & `enola-0.4.0/src/enola/base/common/huemul_connection.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/common/huemul_error.py` & `enola-0.4.0/src/enola/base/common/huemul_error.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/common/huemul_functions.py` & `enola-0.4.0/src/enola/base/common/huemul_functions.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/common/huemul_logging.py` & `enola-0.4.0/src/enola/base/common/huemul_logging.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/common/huemul_response_provider.py` & `enola-0.4.0/src/enola/base/common/huemul_response_provider.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/common/huemul_response_to_bloc.py` & `enola-0.4.0/src/enola/base/common/huemul_response_to_bloc.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,24 +32,24 @@
         #error detail
         self.errors = []
         #data detail
         self.dataRaw = ""
         #extra info detail
         self.extraInfoRaw = ""
 
-        print("paso 100")
+        #print("paso 100")
         if (len(args) == 1 and "huemulResponseProvider" in args):
-            print("paso 200")
+            #print("paso 200")
             self.fromResponseProvider(args["huemulResponseProvider"])
 
         
 
 
     def fromResponseProvider(self, huemulResponseProvider: HuemulResponseProvider):
-        print("paso 300")
+        #print("paso 300")
         self.data = huemulResponseProvider.dataRaw #huemulResponseProvider.dataRaw
         self.isSuccessful = huemulResponseProvider.isSuccessful
         # status code: 200 OK, 500 error, etc
         self.httpStatusCode = huemulResponseProvider.httpStatusCode
         # text to client
         self.message = huemulResponseProvider.message
         self.startDate = huemulResponseProvider.startDate
@@ -61,24 +61,24 @@
 
         #error detail
         self.errors = huemulResponseProvider.errors
         #data detail
         self.dataRaw = huemulResponseProvider.dataRaw
         #extra info detail
         self.extraInfoRaw = huemulResponseProvider.extraInfoRaw
-        print("paso 400")
+        #print("paso 400")
 
     #
     #analyze error and determine attempts strategy
     # @param result create/get/getAll response (HuemulResponseBloc type)
     # @param attempt attempt number
     # @return Boolean
     #
     def analyzeErrors(self, attempt):
-        print("paso 500")
+        #print("paso 500")
         continueInLoop = True
 
         if (self.isSuccessful):
             #all right, exit
             continueInLoop = False
         elif (attempt < self.connectObject.huemulCommon.getTotalAttempt()):
             #send errors
```

### Comparing `enola-0.3.0/src/enola/base/common/auth/auth_model.py` & `enola-0.4.0/src/enola/base/common/auth/auth_model.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/common/auth/auth_service_bloc.py` & `enola-0.4.0/src/enola/base/common/auth/auth_service_bloc.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/common/auth/auth_service_provider.py` & `enola-0.4.0/src/enola/base/common/auth/auth_service_provider.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/internal/enola_agent.py` & `enola-0.4.0/src/enola/base/internal/enola_agent.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/internal/enola_agent_bloc.py` & `enola-0.4.0/src/enola/base/internal/enola_agent_bloc.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/src/enola/base/internal/enola_agent_provider.py` & `enola-0.4.0/src/enola/base/internal/enola_agent_provider.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/LICENSE` & `enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/METADATA` & `enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/RECORD` & `enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/ansi.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/ansitowin32.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/initialise.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/win32.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/winterm.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/ansi_test.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/ansitowin32_test.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/initialise_test.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/isatty_test.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/utils.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama/tests/winterm_test.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/METADATA` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/RECORD` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt` & `enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_elffile.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_manylinux.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_musllinux.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_parser.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_structures.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/_tokenizer.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/markers.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/metadata.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/requirements.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/specifiers.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/tags.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/utils.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging/version.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging/version.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE.APACHE` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE.BSD` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/METADATA` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/RECORD` & `enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/__main__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/__pip-runner__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/build_env.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cache.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/configuration.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/exceptions.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/pyproject.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/self_outdated_check.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/wheel_builder.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/autocompletion.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/base_command.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/cmdoptions.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/command_context.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/main.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/main_parser.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/parser.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/progress_bars.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/req_command.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/cli/spinners.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/cache.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/check.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/completion.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/configuration.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/debug.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/download.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/freeze.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/hash.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/help.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/index.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/inspect.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/install.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/list.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/search.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/show.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/uninstall.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/commands/wheel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/base.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/installed.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/sdist.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/wheel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/index/collector.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/index/package_finder.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/index/sources.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/locations/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/locations/_distutils.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/locations/_sysconfig.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/locations/base.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/_json.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/base.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/pkg_resources.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/candidate.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/direct_url.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/format_control.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/index.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/installation_report.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/link.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/scheme.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/search_scope.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/selection_prefs.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/target_python.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/models/wheel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/auth.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/cache.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/download.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/lazy_wheel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/session.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/utils.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/network/xmlrpc.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/check.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/freeze.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/prepare.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/wheel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/constructors.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_file.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_install.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_set.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_uninstall.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/base.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/_jaraco_text.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/_log.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/appdirs.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/compat.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/compatibility_tags.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/deprecation.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/egg_link.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/encoding.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/entrypoints.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/filesystem.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/filetypes.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/glibc.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/hashes.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/inject_securetransport.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/logging.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/misc.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/models.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/packaging.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/setuptools_build.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/subprocess.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/temp_dir.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/unpacking.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/urls.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/virtualenv.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/utils/wheel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/bazaar.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/git.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/mercurial.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/subversion.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/versioncontrol.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/six.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/typing_extensions.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/compat.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/cacert.pem` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/core.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/big5freq.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/big5prober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/enums.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/escprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/escsm.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/johabfreq.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/johabprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/macromanprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/ansi.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/initialise.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/win32.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/winterm.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/utils.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/compat.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/database.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/index.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/locators.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/manifest.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/markers.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/metadata.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/resources.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/scripts.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t32.exe` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t64.exe` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/util.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/version.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w32.exe` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w64.exe` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/wheel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/distro.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/codec.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/core.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/idnadata.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/intranges.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/uts46data.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/ext.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/fallback.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/__about__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_manylinux.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_musllinux.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_structures.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/markers.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/requirements.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/specifiers.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/tags.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/utils.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/version.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/__main__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/android.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/api.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/macos.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/unix.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/windows.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/cmdline.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/console.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/filter.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatter.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexer.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/modeline.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/plugin.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/regexopt.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/scanner.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/sphinxext.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/style.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/token.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/unistring.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/util.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/html.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/img.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/other.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/python.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/actions.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/common.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/core.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/helpers.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/results.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/testing.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/unicode.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/util.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/adapters.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/api.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/auth.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/certs.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/compat.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/cookies.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/exceptions.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/help.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/hooks.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/models.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/packages.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/sessions.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/status_codes.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/structures.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/utils.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/providers.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/reporters.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/structs.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/__main__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_cell_widths.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_export_format.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_fileno.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_inspect.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_log_render.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_loop.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_null_file.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_palettes.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_ratio.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_spinners.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_win32_console.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_windows.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_wrap.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/abc.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/align.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/ansi.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/bar.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/box.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/cells.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/color.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/color_triplet.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/columns.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/console.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/constrain.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/containers.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/control.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/default_styles.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/diagnose.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/emoji.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/errors.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/file_proxy.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/filesize.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/highlighter.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/json.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/jupyter.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/layout.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/live.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/live_render.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/logging.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/markup.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/measure.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/padding.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/pager.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/palette.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/panel.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/pretty.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/progress.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/progress_bar.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/prompt.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/protocol.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/repr.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/rule.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/scope.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/screen.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/segment.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/spinner.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/status.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/style.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/styled.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/syntax.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/table.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/terminal_theme.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/text.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/theme.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/traceback.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/tree.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/_utils.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/after.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/before.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/nap.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/retry.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/stop.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/wait.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_parser.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_re.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/_collections.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/connection.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/fields.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/filepost.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/request.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/response.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/request.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/response.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/url.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/labels.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/tests.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/AUTHORS.txt` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/LICENSE.txt` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/METADATA` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/RECORD` & `enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks/_impl.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks/_in_process/__init__.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py` & `enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE` & `enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA` & `enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD` & `enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Scripts/Activate.ps1` & `enola-0.4.0/tutorial_env/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Scripts/activate` & `enola-0.4.0/tutorial_env/Scripts/activate`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Scripts/activate.bat` & `enola-0.4.0/tutorial_env/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Scripts/pip.exe` & `enola-0.4.0/tutorial_env/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Scripts/pip3.12.exe` & `enola-0.4.0/tutorial_env/Scripts/pip3.12.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Scripts/pip3.exe` & `enola-0.4.0/tutorial_env/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Scripts/pyproject-build.exe` & `enola-0.4.0/tutorial_env/Scripts/pyproject-build.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Scripts/python.exe` & `enola-0.4.0/tutorial_env/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/tutorial_env/Scripts/pythonw.exe` & `enola-0.4.0/tutorial_env/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/.gitignore` & `enola-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `enola-0.3.0/README.md` & `enola-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,9 +16,13 @@
 py -m pip install build
 
 twine upload dist/*
 
 --para testing
 py -m twine upload --repository testpypi dist/*
 
---para desarrollo
-py -m twine upload --repository pypi dist/*
+--para producción
+py -m twine upload --repository pypi dist/*
+
+
+
+cuando pide token ingresar __token__
```

### Comparing `enola-0.3.0/pyproject.toml` & `enola-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "enola"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Sebastian Rodriguez Robotham", email="sebastian.rodriguez@huemulsolutions.com" },
   { name="Developer Code", email="developer.code@huemulsolutions.com" },
 ]
 description = "Observability & Governance of Intelligence Agents"
+keywords = ["AI", "Observability", "agent", "Intelligence"]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

