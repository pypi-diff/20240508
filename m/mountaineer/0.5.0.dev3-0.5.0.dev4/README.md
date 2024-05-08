# Comparing `tmp/mountaineer-0.5.0.dev3.tar.gz` & `tmp/mountaineer-0.5.0.dev4.tar.gz`

## Comparing `mountaineer-0.5.0.dev3.tar` & `mountaineer-0.5.0.dev4.tar`

### file list

```diff
@@ -1,292 +1,292 @@
--rw-r--r--   0     1001      127      269 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src_go/Cargo.toml
--rw-r--r--   0     1001      127     1995 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src_go/build.rs
--rw-r--r--   0     1001      127     4195 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src_go/go/js_build.go
--rw-r--r--   0     1001      127      168 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src_go/go.mod
--rw-r--r--   0     1001      127      376 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src_go/go.sum
--rw-r--r--   0     1001      127     6499 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src_go/src/lib.rs
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.5.0.dev3/Cargo.toml
--rw-r--r--   0     1001      127      133 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.git-blame-ignore-revs
--rw-r--r--   0     1001      127      138 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.gitattributes
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.github/README_SCRIPTS.md
--rw-r--r--   0     1001      127    15100 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.github/poetry.lock
--rw-r--r--   0     1001      127      767 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.github/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.github/scripts/__init__.py
--rw-r--r--   0     1001      127     3032 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.github/scripts/__tests__/test_update_version.py
--rw-r--r--   0     1001      127     2181 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.github/scripts/check_dependencies.py
--rw-r--r--   0     1001      127     3382 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.github/scripts/update_version.py
--rw-r--r--   0     1001      127     1321 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.github/workflows/publish_docs.yml
--rw-r--r--   0     1001      127    20647 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.github/workflows/test.yml
--rw-r--r--   0     1001      127      504 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.github/workflows/validate.yml
--rw-r--r--   0     1001      127     3414 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/.gitignore
--rw-r--r--   0     1001      127     1750 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/Dockerfile
--rw-r--r--   0     1001      127     1079 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/LICENSE
--rw-r--r--   0     1001      127     5159 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/Makefile
--rw-r--r--   0     1001      127    14891 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/README.md
--rw-r--r--   0     1001      127      105 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/benchmarking/README.md
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/benchmarking/benchmarking/__init__.py
--rw-r--r--   0     1001      127      425 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/benchmarking/benchmarking/simple_render.py
--rw-r--r--   0     1001      127   127218 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/benchmarking/poetry.lock
--rw-r--r--   0     1001      127      291 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/benchmarking/pyproject.toml
--rw-r--r--   0     1001      127      850 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/README.md
--rw-r--r--   0     1001      127        1 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/__init__.py
--rw-r--r--   0     1001      127      886 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/app.py
--rw-r--r--   0     1001      127      489 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/cli.py
--rw-r--r--   0     1001      127      111 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/config.py
--rw-r--r--   0     1001      127        1 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/controllers/__init__.py
--rw-r--r--   0     1001      127     1433 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/controllers/complex.py
--rw-r--r--   0     1001      127      581 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/controllers/detail.py
--rw-r--r--   0     1001      127     1658 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/controllers/home.py
--rw-r--r--   0     1001      127      558 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/controllers/root_layout.py
--rw-r--r--   0     1001      127      559 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/controllers/stream.py
--rw-r--r--   0     1001      127       77 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/main.py
--rw-r--r--   0     1001      127      208 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/__init__.py
--rw-r--r--   0     1001      127     2261 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/app/complex/page.tsx
--rw-r--r--   0     1001      127      453 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/app/detail/page.tsx
--rw-r--r--   0     1001      127     2822 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/app/home/page.tsx
--rw-r--r--   0     1001      127      602 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/app/layout.tsx
--rw-r--r--   0     1001      127       59 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/app/main.css
--rw-r--r--   0     1001      127      708 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/app/stream/page.tsx
--rw-r--r--   0     1001      127   125408 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/package-lock.json
--rw-r--r--   0     1001      127      453 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/package.json
--rw-r--r--   0     1001      127       83 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/postcss.config.js
--rw-r--r--   0     1001      127      161 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/tailwind.config.js
--rw-r--r--   0     1001      127   111131 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/poetry.lock
--rw-r--r--   0     1001      127      724 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/ci_webapp/pyproject.toml
--rw-r--r--   0     1001      127     1593 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/README.md
--rw-r--r--   0     1001      127        1 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0     1001      127     1055 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0     1001      127     8021 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0     1001      127      292 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0     1001      127      816 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0     1001      127     4277 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/builder.py
--rw-r--r--   0     1001      127     4656 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/cli.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0     1001      127     1383 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/environments/base.py
--rw-r--r--   0     1001      127     4591 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0     1001      127     1832 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/environments/venv.py
--rw-r--r--   0     1001      127     1336 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/external.py
--rw-r--r--   0     1001      127     1919 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/generation.py
--rw-r--r--   0     1001      127      327 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/io.py
--rw-r--r--   0     1001      127       30 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
--rw-r--r--   0     1001      127      212 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0     1001      127      246 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0     1001      127      162 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0     1001      127      109 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0     1001      127      170 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.env
--rw-r--r--   0     1001      127     3383 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0     1001      127      645 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0     1001      127       17 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0     1001      127      767 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0     1001      127      947 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0     1001      127      282 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0     1001      127      227 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0     1001      127     1702 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0     1001      127     1124 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0     1001      127       84 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0     1001      127      157 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0     1001      127      208 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0     1001      127     1219 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0     1001      127      995 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0     1001      127       95 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0     1001      127      524 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0     1001      127      117 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0     1001      127      195 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0     1001      127      332 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0     1001      127     1493 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0     1001      127    63125 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/poetry.lock
--rw-r--r--   0     1001      127     1318 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/create_mountaineer_app/pyproject.toml
--rw-r--r--   0     1001      127      324 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docker-compose.test.yml
--rw-r--r--   0     1001      127       30 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/.zed/settings.json
--rw-r--r--   0     1001      127      107 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/README.md
--rw-r--r--   0     1001      127       15 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/CNAME
--rw-r--r--   0     1001      127      318 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/actions.md
--rw-r--r--   0     1001      127      454 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/api_exception.md
--rw-r--r--   0     1001      127       99 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/app-controller.md
--rw-r--r--   0     1001      127      281 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/build_plugins/base.md
--rw-r--r--   0     1001      127       57 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/build_plugins/javascript.md
--rw-r--r--   0     1001      127       62 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/build_plugins/postcss.md
--rw-r--r--   0     1001      127      411 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/cli.md
--rw-r--r--   0     1001      127      376 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/config.md
--rw-r--r--   0     1001      127      138 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/controller.md
--rw-r--r--   0     1001      127       67 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/core_dependencies.md
--rw-r--r--   0     1001      127       66 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/database/config.md
--rw-r--r--   0     1001      127       71 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/database/dependencies.md
--rw-r--r--   0     1001      127       80 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/logging.md
--rw-r--r--   0     1001      127      479 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/render.md
--rw-r--r--   0     1001      127      365 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/ssr.md
--rw-r--r--   0     1001      127      299 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/api/watch_server.md
--rw-r--r--   0     1001      127     9375 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/client_actions.md
--rw-r--r--   0     1001      127      753 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/cma.md
--rw-r--r--   0     1001      127     3021 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/database.md
--rw-r--r--   0     1001      127     4690 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/deploy.md
--rw-r--r--   0     1001      127     7698 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/error_handling.md
--rw-r--r--   0     1001      127     1081 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/index.md
--rw-r--r--   0     1001      127     1541 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/internal/core_library.md
--rw-r--r--   0     1001      127     2156 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/links.md
--rw-r--r--   0     1001      127   365251 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/media/final_todo_list.png
--rw-r--r--   0     1001      127   148261 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/media/ide_typehints.png
--rw-r--r--   0     1001      127   545494 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/media/network_debug.png
--rw-r--r--   0     1001      127   346903 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/media/server_side_rendering.png
--rw-r--r--   0     1001      127     2263 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/metadata.md
--rw-r--r--   0     1001      127     2347 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/postcss.md
--rw-r--r--   0     1001      127    12263 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/quickstart.md
--rw-r--r--   0     1001      127     4875 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/static_analysis.md
--rw-r--r--   0     1001      127     2490 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/structure.md
--rw-r--r--   0     1001      127     1219 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127     9401 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/docs/views.md
--rw-r--r--   0     1001      127     1823 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/mkdocs.yml
--rw-r--r--   0     1001      127      109 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/overrides/partials/footer.html
--rw-r--r--   0     1001      127   156250 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/poetry.lock
--rw-r--r--   0     1001      127      500 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/docs_website/pyproject.toml
--rw-r--r--   0     1001      127   675789 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/media/header.png
--rw-r--r--   0     1001      127     1103 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/actions/__init__.py
--rw-r--r--   0     1001      127     8310 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/actions/test_fields.py
--rw-r--r--   0     1001      127     9761 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/actions/test_passthrough_dec.py
--rw-r--r--   0     1001      127     9218 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/actions/test_sideeffect_dec.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/__init__.py
--rw-r--r--   0     1001      127    14334 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/test_build_actions.py
--rw-r--r--   0     1001      127     5031 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/test_build_links.py
--rw-r--r--   0     1001      127    10127 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/test_build_schemas.py
--rw-r--r--   0     1001      127     6322 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/test_builder.py
--rw-r--r--   0     1001      127     4818 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/test_typescript.py
--rw-r--r--   0     1001      127      319 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/common.py
--rw-r--r--   0     1001      127      497 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/conftest.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/database/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/database/dependencies/__init__.py
--rw-r--r--   0     1001      127      208 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/database/dependencies/conftest.py
--rw-r--r--   0     1001      127      801 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/database/dependencies/test_core.py
--rw-r--r--   0     1001      127      627 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/database/test_config.py
--rw-r--r--   0     1001      127      616 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/database/test_sqlmodel.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/dependencies/__init__.py
--rw-r--r--   0     1001      127     2567 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/dependencies/test_base.py
--rw-r--r--   0     1001      127      211 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/fixtures/__init__.py
--rw-r--r--   0     1001      127   571338 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
--rw-r--r--   0     1001      127  1638568 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
--rw-r--r--   0     1001      127   575422 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/js_compiler/__init__.py
--rw-r--r--   0     1001      127     9973 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/js_compiler/test_javascript.py
--rw-r--r--   0     1001      127      808 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/js_compiler/test_postcss.py
--rw-r--r--   0     1001      127     2823 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/js_compiler/test_source_maps.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/__init__.py
--rw-r--r--   0     1001      127     4187 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/conftest.py
--rw-r--r--   0     1001      127     1429 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_actions.py
--rw-r--r--   0     1001      127     5242 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_db_memory_serializer.py
--rw-r--r--   0     1001      127    11405 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_db_serializer.py
--rw-r--r--   0     1001      127     3916 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_generator.py
--rw-r--r--   0     1001      127     2672 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_generics.py
--rw-r--r--   0     1001      127     4496 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_handlers.py
--rw-r--r--   0     1001      127     1236 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_annotation_helpers.py
--rw-r--r--   0     1001      127     9460 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_app.py
--rw-r--r--   0     1001      127      734 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_cache.py
--rw-r--r--   0     1001      127     5304 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_cli.py
--rw-r--r--   0     1001      127     2301 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_compat.py
--rw-r--r--   0     1001      127      494 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_config.py
--rw-r--r--   0     1001      127     6824 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_controller.py
--rw-r--r--   0     1001      127     1126 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_controller_layout.py
--rw-r--r--   0     1001      127     3239 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_cropper.py
--rw-r--r--   0     1001      127     1227 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_exceptions.py
--rw-r--r--   0     1001      127      583 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_generics.py
--rw-r--r--   0     1001      127     1924 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_logging.py
--rw-r--r--   0     1001      127     8494 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_paths.py
--rw-r--r--   0     1001      127     2667 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_ssr.py
--rw-r--r--   0     1001      127     3177 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/__tests__/test_watch.py
--rw-r--r--   0     1001      127      405 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/actions/__init__.py
--rw-r--r--   0     1001      127    13033 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/actions/fields.py
--rw-r--r--   0     1001      127     6847 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/actions/passthrough_dec.py
--rw-r--r--   0     1001      127    12023 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/actions/sideeffect_dec.py
--rw-r--r--   0     1001      127     4671 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/annotation_helpers.py
--rw-r--r--   0     1001      127    22160 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/app.py
--rw-r--r--   0     1001      127     3216 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/cache.py
--rw-r--r--   0     1001      127    19195 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/cli.py
--rw-r--r--   0     1001      127    11390 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/client_builder/build_actions.py
--rw-r--r--   0     1001      127     4002 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/client_builder/build_links.py
--rw-r--r--   0     1001      127    10296 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/client_builder/build_schemas.py
--rw-r--r--   0     1001      127    30715 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/client_builder/builder.py
--rw-r--r--   0     1001      127    11390 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/client_builder/openapi.py
--rw-r--r--   0     1001      127     5629 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/client_builder/typescript.py
--rw-r--r--   0     1001      127     1808 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/compat.py
--rw-r--r--   0     1001      127     2424 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/config.py
--rw-r--r--   0     1001      127      197 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/console.py
--rw-r--r--   0     1001      127       40 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/constants.py
--rw-r--r--   0     1001      127    16758 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/controller.py
--rw-r--r--   0     1001      127      881 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/controller_layout.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/controllers/__init__.py
--rw-r--r--   0     1001      127     1216 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/controllers/exception_controller.py
--rw-r--r--   0     1001      127    10359 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/cropper.py
--rw-r--r--   0     1001      127      327 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/database/__init__.py
--rw-r--r--   0     1001      127     1866 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/database/cli.py
--rw-r--r--   0     1001      127     1822 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/database/config.py
--rw-r--r--   0     1001      127      133 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/database/dependencies/__init__.py
--rw-r--r--   0     1001      127     3188 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/database/dependencies/core.py
--rw-r--r--   0     1001      127     7969 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/database/sqlmodel.py
--rw-r--r--   0     1001      127     8737 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/database/validator.py
--rw-r--r--   0     1001      127      251 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/dependencies/__init__.py
--rw-r--r--   0     1001      127     5122 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/dependencies/base.py
--rw-r--r--   0     1001      127      116 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/dependencies/core/__init__.py
--rw-r--r--   0     1001      127     1069 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/dependencies/core/core.py
--rw-r--r--   0     1001      127     3317 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/exceptions.py
--rw-r--r--   0     1001      127     1740 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/generics.py
--rw-r--r--   0     1001      127     1188 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/io.py
--rw-r--r--   0     1001      127        1 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/js_compiler/__init__.py
--rw-r--r--   0     1001      127     1731 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/js_compiler/base.py
--rw-r--r--   0     1001      127      199 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/js_compiler/exceptions.py
--rw-r--r--   0     1001      127    17413 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/js_compiler/javascript.py
--rw-r--r--   0     1001      127     4163 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/js_compiler/postcss.py
--rw-r--r--   0     1001      127     5614 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/js_compiler/source_maps.py
--rw-r--r--   0     1001      127     2313 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/logging.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/__init__.py
--rw-r--r--   0     1001      127    15430 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/actions.py
--rw-r--r--   0     1001      127     8140 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/cli.py
--rw-r--r--   0     1001      127     2319 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/client_io.py
--rw-r--r--   0     1001      127     8384 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/db_memory_serializer.py
--rw-r--r--   0     1001      127     7801 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/db_serializer.py
--rw-r--r--   0     1001      127     9315 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/db_stubs.py
--rw-r--r--   0     1001      127       85 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/dependency/__init__.py
--rw-r--r--   0     1001      127       47 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/dependency/core/__init__.py
--rw-r--r--   0     1001      127      356 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/dependency/core/core.py
--rw-r--r--   0     1001      127     7765 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/generator.py
--rw-r--r--   0     1001      127     3078 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/generics.py
--rw-r--r--   0     1001      127    22026 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/handlers.py
--rw-r--r--   0     1001      127     1925 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/migration.py
--rw-r--r--   0     1001      127     3491 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/migrations/migrator.py
--rw-r--r--   0     1001      127    13337 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/paths.py
--rw-r--r--   0     1001      127        0 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/py.typed
--rw-r--r--   0     1001      127     5816 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/render.py
--rw-r--r--   0     1001      127     3237 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/ssr.py
--rw-r--r--   0     1001      127      210 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/static/__init__.py
--rw-r--r--   0     1001      127     6711 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/static/api.ts
--rw-r--r--   0     1001      127     3976 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/static/live_reload.ts
--rw-r--r--   0     1001      127      323 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/static/ssr_polyfills.js
--rw-r--r--   0     1001      127     7261 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/test_utilities.py
--rw-r--r--   0     1001      127      213 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/views/__init__.py
--rw-r--r--   0     1001      127      432 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/views/core/exception/page.tsx
--rw-r--r--   0     1001      127      178 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/views/core/layout.tsx
--rw-r--r--   0     1001      127       59 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/views/core/main.css
--rw-r--r--   0     1001      127     1478 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/views/package-lock.json
--rw-r--r--   0     1001      127      257 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/views/package.json
--rw-r--r--   0     1001      127       83 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/views/postcss.config.js
--rw-r--r--   0     1001      127      162 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/views/tailwind.config.js
--rw-r--r--   0     1001      127     8427 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/watch.py
--rw-r--r--   0     1001      127     4062 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/watch_server.py
--rw-r--r--   0     1001      127     1213 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/mountaineer/webservice.py
--rw-r--r--   0     1001      127   129036 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/poetry.lock
--rw-r--r--   0     1001      127   453080 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/benches/fixtures/complex_sourcemap_mapping.txt
--rw-r--r--   0     1001      127   575422 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/benches/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127      322 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/benches/fixtures/ssr_polyfill_archive.js
--rw-r--r--   0     1001      127      899 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/benches/lexers_benchmark.rs
--rw-r--r--   0     1001      127     1089 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/benches/source_map_benchmark.rs
--rw-r--r--   0     1001      127     1595 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/benches/ssr_benchmark.rs
--rw-r--r--   0     1001      127      499 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/errors.rs
--rw-r--r--   0     1001      127     4648 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/lexers.rs
--rw-r--r--   0     1001      127     9118 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/lib.rs
--rw-r--r--   0     1001      127      680 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/logging.rs
--rw-r--r--   0     1001      127    17549 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/source_map.rs
--rw-r--r--   0     1001      127    15113 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/ssr.rs
--rw-r--r--   0     1001      127     3998 2024-05-07 02:12:38.000000 mountaineer-0.5.0.dev3/src/timeout.rs
--rw-r--r--   0     1001      127    32093 2024-05-07 02:12:54.000000 mountaineer-0.5.0.dev3/Cargo.lock
--rw-r--r--   0     1001      127     1624 2024-05-07 02:12:51.000000 mountaineer-0.5.0.dev3/pyproject.toml
--rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.5.0.dev3/PKG-INFO
+-rw-r--r--   0     1001      127      269 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src_go/Cargo.toml
+-rw-r--r--   0     1001      127     1995 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src_go/build.rs
+-rw-r--r--   0     1001      127     4195 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src_go/go/js_build.go
+-rw-r--r--   0     1001      127      168 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src_go/go.mod
+-rw-r--r--   0     1001      127      376 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src_go/go.sum
+-rw-r--r--   0     1001      127     6499 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src_go/src/lib.rs
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.5.0.dev4/Cargo.toml
+-rw-r--r--   0     1001      127      133 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.git-blame-ignore-revs
+-rw-r--r--   0     1001      127      138 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.gitattributes
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.github/README_SCRIPTS.md
+-rw-r--r--   0     1001      127    15100 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.github/poetry.lock
+-rw-r--r--   0     1001      127      767 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.github/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.github/scripts/__init__.py
+-rw-r--r--   0     1001      127     3032 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.github/scripts/__tests__/test_update_version.py
+-rw-r--r--   0     1001      127     2181 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.github/scripts/check_dependencies.py
+-rw-r--r--   0     1001      127     3382 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.github/scripts/update_version.py
+-rw-r--r--   0     1001      127     1321 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.github/workflows/publish_docs.yml
+-rw-r--r--   0     1001      127    20647 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      504 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.github/workflows/validate.yml
+-rw-r--r--   0     1001      127     3414 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/.gitignore
+-rw-r--r--   0     1001      127     1750 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/Dockerfile
+-rw-r--r--   0     1001      127     1079 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/LICENSE
+-rw-r--r--   0     1001      127     5159 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/Makefile
+-rw-r--r--   0     1001      127    14891 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/README.md
+-rw-r--r--   0     1001      127      105 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/benchmarking/README.md
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/benchmarking/benchmarking/__init__.py
+-rw-r--r--   0     1001      127      425 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/benchmarking/benchmarking/simple_render.py
+-rw-r--r--   0     1001      127   127218 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/benchmarking/poetry.lock
+-rw-r--r--   0     1001      127      291 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/benchmarking/pyproject.toml
+-rw-r--r--   0     1001      127      850 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/README.md
+-rw-r--r--   0     1001      127        1 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/__init__.py
+-rw-r--r--   0     1001      127      886 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/app.py
+-rw-r--r--   0     1001      127      603 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/cli.py
+-rw-r--r--   0     1001      127      111 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/config.py
+-rw-r--r--   0     1001      127        1 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/controllers/__init__.py
+-rw-r--r--   0     1001      127     1433 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/controllers/complex.py
+-rw-r--r--   0     1001      127      581 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/controllers/detail.py
+-rw-r--r--   0     1001      127     1658 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/controllers/home.py
+-rw-r--r--   0     1001      127      649 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/controllers/root_layout.py
+-rw-r--r--   0     1001      127      559 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/controllers/stream.py
+-rw-r--r--   0     1001      127       77 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/main.py
+-rw-r--r--   0     1001      127      208 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/__init__.py
+-rw-r--r--   0     1001      127     2261 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/app/complex/page.tsx
+-rw-r--r--   0     1001      127      453 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127     2822 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/app/home/page.tsx
+-rw-r--r--   0     1001      127      645 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/app/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/app/main.css
+-rw-r--r--   0     1001      127      708 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/app/stream/page.tsx
+-rw-r--r--   0     1001      127   125408 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/package-lock.json
+-rw-r--r--   0     1001      127      453 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/package.json
+-rw-r--r--   0     1001      127       83 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/postcss.config.js
+-rw-r--r--   0     1001      127      161 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/tailwind.config.js
+-rw-r--r--   0     1001      127   111131 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/poetry.lock
+-rw-r--r--   0     1001      127      754 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/ci_webapp/pyproject.toml
+-rw-r--r--   0     1001      127     1593 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/README.md
+-rw-r--r--   0     1001      127        1 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0     1001      127     1055 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0     1001      127     8021 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0     1001      127      292 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      816 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0     1001      127     4277 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/builder.py
+-rw-r--r--   0     1001      127     4656 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/cli.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0     1001      127     1383 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/environments/base.py
+-rw-r--r--   0     1001      127     4591 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0     1001      127     1832 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0     1001      127     1336 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/external.py
+-rw-r--r--   0     1001      127     1919 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/generation.py
+-rw-r--r--   0     1001      127      327 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/io.py
+-rw-r--r--   0     1001      127       30 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0     1001      127      212 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0     1001      127      246 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0     1001      127      162 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0     1001      127      109 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0     1001      127      170 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0     1001      127     3383 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0     1001      127      645 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0     1001      127       17 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0     1001      127      767 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0     1001      127      947 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0     1001      127      282 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0     1001      127      227 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0     1001      127     1702 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0     1001      127     1124 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0     1001      127       84 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0     1001      127      157 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0     1001      127      208 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0     1001      127     1219 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127      995 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       95 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0     1001      127      524 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0     1001      127      117 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0     1001      127      195 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0     1001      127      332 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0     1001      127     1493 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0     1001      127    63125 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/poetry.lock
+-rw-r--r--   0     1001      127     1318 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/create_mountaineer_app/pyproject.toml
+-rw-r--r--   0     1001      127      324 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docker-compose.test.yml
+-rw-r--r--   0     1001      127       30 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/.zed/settings.json
+-rw-r--r--   0     1001      127      107 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/README.md
+-rw-r--r--   0     1001      127       15 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/CNAME
+-rw-r--r--   0     1001      127      318 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/actions.md
+-rw-r--r--   0     1001      127      454 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/api_exception.md
+-rw-r--r--   0     1001      127       99 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/app-controller.md
+-rw-r--r--   0     1001      127      281 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/build_plugins/base.md
+-rw-r--r--   0     1001      127       57 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/build_plugins/javascript.md
+-rw-r--r--   0     1001      127       62 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/build_plugins/postcss.md
+-rw-r--r--   0     1001      127      411 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/cli.md
+-rw-r--r--   0     1001      127      376 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/config.md
+-rw-r--r--   0     1001      127      138 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/controller.md
+-rw-r--r--   0     1001      127       67 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/core_dependencies.md
+-rw-r--r--   0     1001      127       66 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/database/config.md
+-rw-r--r--   0     1001      127       71 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/database/dependencies.md
+-rw-r--r--   0     1001      127       80 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/logging.md
+-rw-r--r--   0     1001      127      479 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/render.md
+-rw-r--r--   0     1001      127      365 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/ssr.md
+-rw-r--r--   0     1001      127      299 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/api/watch_server.md
+-rw-r--r--   0     1001      127     9375 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/client_actions.md
+-rw-r--r--   0     1001      127      753 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/cma.md
+-rw-r--r--   0     1001      127     3021 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/database.md
+-rw-r--r--   0     1001      127     4690 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/deploy.md
+-rw-r--r--   0     1001      127     7698 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/error_handling.md
+-rw-r--r--   0     1001      127     1081 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/index.md
+-rw-r--r--   0     1001      127     1541 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/internal/core_library.md
+-rw-r--r--   0     1001      127     2156 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/links.md
+-rw-r--r--   0     1001      127   365251 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/media/final_todo_list.png
+-rw-r--r--   0     1001      127   148261 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/media/ide_typehints.png
+-rw-r--r--   0     1001      127   545494 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/media/network_debug.png
+-rw-r--r--   0     1001      127   346903 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/media/server_side_rendering.png
+-rw-r--r--   0     1001      127     2263 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/metadata.md
+-rw-r--r--   0     1001      127     2347 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/postcss.md
+-rw-r--r--   0     1001      127    12263 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/quickstart.md
+-rw-r--r--   0     1001      127     4875 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/static_analysis.md
+-rw-r--r--   0     1001      127     2490 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/structure.md
+-rw-r--r--   0     1001      127     1219 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127     9534 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/docs/views.md
+-rw-r--r--   0     1001      127     1823 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/mkdocs.yml
+-rw-r--r--   0     1001      127      109 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/overrides/partials/footer.html
+-rw-r--r--   0     1001      127   156250 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/poetry.lock
+-rw-r--r--   0     1001      127      500 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/docs_website/pyproject.toml
+-rw-r--r--   0     1001      127   675789 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/media/header.png
+-rw-r--r--   0     1001      127     1103 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/actions/__init__.py
+-rw-r--r--   0     1001      127     8123 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/actions/test_fields.py
+-rw-r--r--   0     1001      127     9711 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/actions/test_passthrough_dec.py
+-rw-r--r--   0     1001      127     9086 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/actions/test_sideeffect_dec.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/__init__.py
+-rw-r--r--   0     1001      127    14334 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/test_build_actions.py
+-rw-r--r--   0     1001      127     5031 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/test_build_links.py
+-rw-r--r--   0     1001      127    10127 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/test_build_schemas.py
+-rw-r--r--   0     1001      127     6322 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/test_builder.py
+-rw-r--r--   0     1001      127     4818 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/test_typescript.py
+-rw-r--r--   0     1001      127      319 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/common.py
+-rw-r--r--   0     1001      127      497 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/conftest.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/database/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127      208 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/database/dependencies/conftest.py
+-rw-r--r--   0     1001      127      801 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/database/dependencies/test_core.py
+-rw-r--r--   0     1001      127      627 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/database/test_config.py
+-rw-r--r--   0     1001      127      616 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/database/test_sqlmodel.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/dependencies/__init__.py
+-rw-r--r--   0     1001      127     2567 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/dependencies/test_base.py
+-rw-r--r--   0     1001      127      211 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/fixtures/__init__.py
+-rw-r--r--   0     1001      127   571338 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127  1638568 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
+-rw-r--r--   0     1001      127   575422 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     9973 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/js_compiler/test_javascript.py
+-rw-r--r--   0     1001      127      808 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/js_compiler/test_postcss.py
+-rw-r--r--   0     1001      127     2823 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/js_compiler/test_source_maps.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/__init__.py
+-rw-r--r--   0     1001      127     4187 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/conftest.py
+-rw-r--r--   0     1001      127     1429 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_actions.py
+-rw-r--r--   0     1001      127     5242 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_db_memory_serializer.py
+-rw-r--r--   0     1001      127    11405 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_db_serializer.py
+-rw-r--r--   0     1001      127     3916 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_generator.py
+-rw-r--r--   0     1001      127     2672 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_generics.py
+-rw-r--r--   0     1001      127     4496 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_handlers.py
+-rw-r--r--   0     1001      127     1236 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_annotation_helpers.py
+-rw-r--r--   0     1001      127    12749 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_app.py
+-rw-r--r--   0     1001      127      734 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_cache.py
+-rw-r--r--   0     1001      127     5304 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_cli.py
+-rw-r--r--   0     1001      127     2301 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_compat.py
+-rw-r--r--   0     1001      127      494 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_config.py
+-rw-r--r--   0     1001      127     6824 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_controller.py
+-rw-r--r--   0     1001      127     1126 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_controller_layout.py
+-rw-r--r--   0     1001      127     3239 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_cropper.py
+-rw-r--r--   0     1001      127     1227 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_exceptions.py
+-rw-r--r--   0     1001      127      583 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_generics.py
+-rw-r--r--   0     1001      127     1924 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_logging.py
+-rw-r--r--   0     1001      127     8494 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_paths.py
+-rw-r--r--   0     1001      127     2667 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_ssr.py
+-rw-r--r--   0     1001      127     3177 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/__tests__/test_watch.py
+-rw-r--r--   0     1001      127      405 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/actions/__init__.py
+-rw-r--r--   0     1001      127    12444 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/actions/fields.py
+-rw-r--r--   0     1001      127     6841 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/actions/passthrough_dec.py
+-rw-r--r--   0     1001      127    11993 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/actions/sideeffect_dec.py
+-rw-r--r--   0     1001      127     4671 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/annotation_helpers.py
+-rw-r--r--   0     1001      127    28407 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/app.py
+-rw-r--r--   0     1001      127     3216 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/cache.py
+-rw-r--r--   0     1001      127    19195 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/cli.py
+-rw-r--r--   0     1001      127    11390 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/client_builder/build_actions.py
+-rw-r--r--   0     1001      127     4002 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/client_builder/build_links.py
+-rw-r--r--   0     1001      127    10296 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/client_builder/build_schemas.py
+-rw-r--r--   0     1001      127    30695 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/client_builder/builder.py
+-rw-r--r--   0     1001      127    11390 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/client_builder/openapi.py
+-rw-r--r--   0     1001      127     5629 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/client_builder/typescript.py
+-rw-r--r--   0     1001      127     1808 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/compat.py
+-rw-r--r--   0     1001      127     2424 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/config.py
+-rw-r--r--   0     1001      127      197 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/console.py
+-rw-r--r--   0     1001      127       40 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/constants.py
+-rw-r--r--   0     1001      127    16758 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/controller.py
+-rw-r--r--   0     1001      127      881 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/controller_layout.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/controllers/__init__.py
+-rw-r--r--   0     1001      127     1216 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/controllers/exception_controller.py
+-rw-r--r--   0     1001      127    10359 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/cropper.py
+-rw-r--r--   0     1001      127      327 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/database/__init__.py
+-rw-r--r--   0     1001      127     1866 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/database/cli.py
+-rw-r--r--   0     1001      127     1822 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/database/config.py
+-rw-r--r--   0     1001      127      133 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127     3188 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/database/dependencies/core.py
+-rw-r--r--   0     1001      127     7969 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/database/sqlmodel.py
+-rw-r--r--   0     1001      127     8737 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/database/validator.py
+-rw-r--r--   0     1001      127      251 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/dependencies/__init__.py
+-rw-r--r--   0     1001      127     5122 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/dependencies/base.py
+-rw-r--r--   0     1001      127      116 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/dependencies/core/__init__.py
+-rw-r--r--   0     1001      127     1069 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/dependencies/core/core.py
+-rw-r--r--   0     1001      127     3317 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/exceptions.py
+-rw-r--r--   0     1001      127     1740 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/generics.py
+-rw-r--r--   0     1001      127     1188 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/io.py
+-rw-r--r--   0     1001      127        1 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     1731 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/js_compiler/base.py
+-rw-r--r--   0     1001      127      199 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/js_compiler/exceptions.py
+-rw-r--r--   0     1001      127    17413 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/js_compiler/javascript.py
+-rw-r--r--   0     1001      127     4163 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/js_compiler/postcss.py
+-rw-r--r--   0     1001      127     5614 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/js_compiler/source_maps.py
+-rw-r--r--   0     1001      127     2313 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/logging.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/__init__.py
+-rw-r--r--   0     1001      127    15430 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/actions.py
+-rw-r--r--   0     1001      127     8140 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/cli.py
+-rw-r--r--   0     1001      127     2319 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/client_io.py
+-rw-r--r--   0     1001      127     8384 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/db_memory_serializer.py
+-rw-r--r--   0     1001      127     7801 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/db_serializer.py
+-rw-r--r--   0     1001      127     9315 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/db_stubs.py
+-rw-r--r--   0     1001      127       85 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/dependency/__init__.py
+-rw-r--r--   0     1001      127       47 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/dependency/core/__init__.py
+-rw-r--r--   0     1001      127      356 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/dependency/core/core.py
+-rw-r--r--   0     1001      127     7765 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/generator.py
+-rw-r--r--   0     1001      127     3078 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/generics.py
+-rw-r--r--   0     1001      127    22026 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/handlers.py
+-rw-r--r--   0     1001      127     1925 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/migration.py
+-rw-r--r--   0     1001      127     3491 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/migrations/migrator.py
+-rw-r--r--   0     1001      127    13337 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/paths.py
+-rw-r--r--   0     1001      127        0 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/py.typed
+-rw-r--r--   0     1001      127     5816 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/render.py
+-rw-r--r--   0     1001      127     3237 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/ssr.py
+-rw-r--r--   0     1001      127      210 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/static/__init__.py
+-rw-r--r--   0     1001      127     6556 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/static/api.ts
+-rw-r--r--   0     1001      127     3976 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/static/live_reload.ts
+-rw-r--r--   0     1001      127      323 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/static/ssr_polyfills.js
+-rw-r--r--   0     1001      127     7261 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/test_utilities.py
+-rw-r--r--   0     1001      127      213 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/views/__init__.py
+-rw-r--r--   0     1001      127      432 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/views/core/exception/page.tsx
+-rw-r--r--   0     1001      127      178 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/views/core/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/views/core/main.css
+-rw-r--r--   0     1001      127     1478 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/views/package-lock.json
+-rw-r--r--   0     1001      127      257 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/views/package.json
+-rw-r--r--   0     1001      127       83 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/views/postcss.config.js
+-rw-r--r--   0     1001      127      162 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/views/tailwind.config.js
+-rw-r--r--   0     1001      127     8427 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/watch.py
+-rw-r--r--   0     1001      127     4062 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/watch_server.py
+-rw-r--r--   0     1001      127     1213 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/mountaineer/webservice.py
+-rw-r--r--   0     1001      127   129036 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/poetry.lock
+-rw-r--r--   0     1001      127   453080 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/benches/fixtures/complex_sourcemap_mapping.txt
+-rw-r--r--   0     1001      127   575422 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/benches/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127      322 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/benches/fixtures/ssr_polyfill_archive.js
+-rw-r--r--   0     1001      127      899 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/benches/lexers_benchmark.rs
+-rw-r--r--   0     1001      127     1089 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/benches/source_map_benchmark.rs
+-rw-r--r--   0     1001      127     1595 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/benches/ssr_benchmark.rs
+-rw-r--r--   0     1001      127      499 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/errors.rs
+-rw-r--r--   0     1001      127     4648 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/lexers.rs
+-rw-r--r--   0     1001      127     9118 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/lib.rs
+-rw-r--r--   0     1001      127      680 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/logging.rs
+-rw-r--r--   0     1001      127    17549 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/source_map.rs
+-rw-r--r--   0     1001      127    15113 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/ssr.rs
+-rw-r--r--   0     1001      127     3998 2024-05-08 01:56:37.000000 mountaineer-0.5.0.dev4/src/timeout.rs
+-rw-r--r--   0     1001      127    32093 2024-05-08 01:56:54.000000 mountaineer-0.5.0.dev4/Cargo.lock
+-rw-r--r--   0     1001      127     1624 2024-05-08 01:56:50.000000 mountaineer-0.5.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.5.0.dev4/PKG-INFO
```

### Comparing `mountaineer-0.5.0.dev3/src_go/build.rs` & `mountaineer-0.5.0.dev4/src_go/build.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src_go/go/js_build.go` & `mountaineer-0.5.0.dev4/src_go/go/js_build.go`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src_go/src/lib.rs` & `mountaineer-0.5.0.dev4/src_go/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/Cargo.toml` & `mountaineer-0.5.0.dev4/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [[bench]]
 path = "src/benches/lexers_benchmark.rs"
 name = "lexers_benchmark"
 harness = false
 
 [package]
 name = "mountaineer"
-version = "0.5.0-dev3"
+version = "0.5.0-dev4"
 edition = "2021"
 
 [dependencies]
 v8 = "0.89.0"
 deno_core_icudata = "0.73.0"
 lazy_static = "1.4.0"
 serde_json = "1.0"
```

### Comparing `mountaineer-0.5.0.dev3/.github/poetry.lock` & `mountaineer-0.5.0.dev4/.github/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/.github/pyproject.toml` & `mountaineer-0.5.0.dev4/.github/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/.github/scripts/__tests__/test_update_version.py` & `mountaineer-0.5.0.dev4/.github/scripts/__tests__/test_update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/.github/scripts/check_dependencies.py` & `mountaineer-0.5.0.dev4/.github/scripts/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/.github/scripts/update_version.py` & `mountaineer-0.5.0.dev4/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/.github/workflows/publish_docs.yml` & `mountaineer-0.5.0.dev4/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/.github/workflows/test.yml` & `mountaineer-0.5.0.dev4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/.gitignore` & `mountaineer-0.5.0.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/Dockerfile` & `mountaineer-0.5.0.dev4/Dockerfile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/LICENSE` & `mountaineer-0.5.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/Makefile` & `mountaineer-0.5.0.dev4/Makefile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/README.md` & `mountaineer-0.5.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/benchmarking/poetry.lock` & `mountaineer-0.5.0.dev4/benchmarking/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/README.md` & `mountaineer-0.5.0.dev4/ci_webapp/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/app.py` & `mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/controllers/complex.py` & `mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/controllers/complex.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/controllers/detail.py` & `mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/controllers/home.py` & `mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/controllers/stream.py` & `mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/controllers/stream.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/app/complex/page.tsx` & `mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/app/complex/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/app/home/page.tsx` & `mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/app/layout.tsx` & `mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/app/layout.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import { useServer } from "./_server";
 
 const Layout = ({ children }: { children: ReactNode }) => {
   const serverState = useServer();
 
   return (
     <div className="p-6">
-      <h1>Layout State: {serverState.layout_value}</h1>
+      <h1>
+        Layout State: {serverState.layout_value} : {serverState.layout_arg}
+      </h1>
       <div>{children}</div>
       <div>
         <button
           className="rounded-md bg-indigo-500 p-2 text-white"
           onClick={async () => {
             await serverState.increment_layout_value();
           }}
```

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/app/stream/page.tsx` & `mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/app/stream/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/ci_webapp/views/package-lock.json` & `mountaineer-0.5.0.dev4/ci_webapp/ci_webapp/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/poetry.lock` & `mountaineer-0.5.0.dev4/ci_webapp/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/ci_webapp/pyproject.toml` & `mountaineer-0.5.0.dev4/ci_webapp/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 # While in development, link to the local path
 mountaineer = { path = "../", develop = true }
 
 [tool.poetry.scripts]
 runserver = "ci_webapp.cli:runserver"
 watch = "ci_webapp.cli:watch"
+build = "ci_webapp.cli:build"
 
 [tool.poetry.group.dev.dependencies]
 types-setuptools = "^69.0.0.20240125"
 mypy = "^1.8.0"
 ruff = "^0.1.14"
 pyright = "^1.1.352"
```

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/README.md` & `mountaineer-0.5.0.dev4/create_mountaineer_app/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/common.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/builder.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/cli.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/environments/base.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/environments/poetry.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/environments/venv.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/external.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/generation.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/README.md` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml` & `mountaineer-0.5.0.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/poetry.lock` & `mountaineer-0.5.0.dev4/create_mountaineer_app/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/create_mountaineer_app/pyproject.toml` & `mountaineer-0.5.0.dev4/create_mountaineer_app/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/client_actions.md` & `mountaineer-0.5.0.dev4/docs_website/docs/client_actions.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/cma.md` & `mountaineer-0.5.0.dev4/docs_website/docs/cma.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/database.md` & `mountaineer-0.5.0.dev4/docs_website/docs/database.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/deploy.md` & `mountaineer-0.5.0.dev4/docs_website/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/error_handling.md` & `mountaineer-0.5.0.dev4/docs_website/docs/error_handling.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/index.md` & `mountaineer-0.5.0.dev4/docs_website/docs/index.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/internal/core_library.md` & `mountaineer-0.5.0.dev4/docs_website/docs/internal/core_library.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/links.md` & `mountaineer-0.5.0.dev4/docs_website/docs/links.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/media/final_todo_list.png` & `mountaineer-0.5.0.dev4/docs_website/docs/media/final_todo_list.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/media/ide_typehints.png` & `mountaineer-0.5.0.dev4/docs_website/docs/media/ide_typehints.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/media/network_debug.png` & `mountaineer-0.5.0.dev4/docs_website/docs/media/network_debug.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/media/server_side_rendering.png` & `mountaineer-0.5.0.dev4/docs_website/docs/media/server_side_rendering.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/metadata.md` & `mountaineer-0.5.0.dev4/docs_website/docs/metadata.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/postcss.md` & `mountaineer-0.5.0.dev4/docs_website/docs/postcss.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/quickstart.md` & `mountaineer-0.5.0.dev4/docs_website/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/static_analysis.md` & `mountaineer-0.5.0.dev4/docs_website/docs/static_analysis.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/structure.md` & `mountaineer-0.5.0.dev4/docs_website/docs/structure.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/stylesheets/extra.css` & `mountaineer-0.5.0.dev4/docs_website/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/docs/views.md` & `mountaineer-0.5.0.dev4/docs_website/docs/views.md`

 * *Files 5% similar despite different names*

```diff
@@ -235,21 +235,17 @@
 Once your controller is declared, you'll need to mount your layout into the AppController like you do for regular pages.
 
 ```python title="/app.py"
 app_controller = AppController(...)
 app_controller.register(RootLayoutController())
 ```
 
-In general you can implement layout controllers just like you do for pages. But since they're shared across multiple pages there are a few important differences to keep in mind:
+In general you can implement layout controllers just like you do for pages. But since they're shared across multiple child controllers, make sure the keyword arguments you use in your `render` signature don't have any conflicts. Mountaineer will merge these signatures at runtime and check for duplicate keyword names across the layout's child pages. Arguments are allowed to share the same name _and_ type, in which case they will be resolved to the same value. Arguments with conflicting types will raise a `TypeError`.
 
-- Layout controllers will be rendered in an isolated scope. Sideeffects in one layout controller won't affect the others.
-- Dependency injections are similarly isolated. They are run in an isolated, synthetic context and not with the same dependency injection parameters that the page uses.
-- Layout controllers don't modify the page signature. Query params on layouts won't be extracted, for instance.
-
-As long as you write your layout controllers without directly referencing the page that they might be wrapping, which is the case for most layouts, you should be good to go.
+It's also worth noting that layout controllers will resolve their dependencies in the same scope as the page controllers. So if you need database access within your layout, you'll receive the same underlying transaction as the page controller. This makes dependency injection a powerful way to save on resources, but be careful to not treat them as isolated objects.
 
 ## Typescript Configuration
 
 If you want to customize how Mountaineer builds your view files into raw client-side javascript, add a `tsconfig.json` file. The Typescript website includes a [full list](https://www.typescriptlang.org/tsconfig) of the available options here. A good place to start is:
 
 ```json
 {
```

### Comparing `mountaineer-0.5.0.dev3/docs_website/mkdocs.yml` & `mountaineer-0.5.0.dev4/docs_website/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/docs_website/poetry.lock` & `mountaineer-0.5.0.dev4/docs_website/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/media/header.png` & `mountaineer-0.5.0.dev4/media/header.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__init__.py` & `mountaineer-0.5.0.dev4/mountaineer/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/actions/test_fields.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/actions/test_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import AsyncIterator, Iterator, Optional, Type, cast
+from typing import AsyncIterator, Iterator, Optional, Type
 
 import pytest
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel
 from pydantic.fields import FieldInfo
 
 from mountaineer.actions.fields import (
@@ -120,32 +120,27 @@
     expected_passthrough_fields: dict[str, FieldInfo],
 ):
     sample_controller = ExampleController()
     raw_model = fuse_metadata_to_response_typehint(
         metadata, sample_controller, render_model
     )
 
-    assert "ExampleController" in raw_model.model_fields.keys()
-
-    fused_model = cast(
-        BaseModel, raw_model.model_fields["ExampleController"].annotation
-    )
     if expected_sideeffect_fields:
-        assert "sideeffect" in fused_model.model_fields.keys()
-        assert fused_model.model_fields["sideeffect"].annotation
+        assert "sideeffect" in raw_model.model_fields.keys()
+        assert raw_model.model_fields["sideeffect"].annotation
         basic_compare_model_fields(
-            fused_model.model_fields["sideeffect"].annotation.model_fields,
+            raw_model.model_fields["sideeffect"].annotation.model_fields,
             expected_sideeffect_fields,
         )
 
     if expected_passthrough_fields:
-        assert "passthrough" in fused_model.model_fields.keys()
-        assert fused_model.model_fields["passthrough"].annotation
+        assert "passthrough" in raw_model.model_fields.keys()
+        assert raw_model.model_fields["passthrough"].annotation
         basic_compare_model_fields(
-            fused_model.model_fields["passthrough"].annotation.model_fields,
+            raw_model.model_fields["passthrough"].annotation.model_fields,
             expected_passthrough_fields,
         )
 
     assert raw_model.__name__ == expected_model_name
 
 
 class ParentRender(RenderBase):
```

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/actions/test_passthrough_dec.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/actions/test_passthrough_dec.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,19 +96,17 @@
 
     return_value_async = await controller.call_passthrough_async(
         {},
     )
 
     # The response payload should be the same both both sync and async endpoints
     expected_response = {
-        "TestController": {
-            "passthrough": ExamplePassthroughModel(
-                status="success",
-            )
-        }
+        "passthrough": ExamplePassthroughModel(
+            status="success",
+        )
     }
 
     assert return_value_sync == expected_response
     assert return_value_async == expected_response
 
     assert controller.counter == 2
```

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/actions/test_sideeffect_dec.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/actions/test_sideeffect_dec.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,21 +97,19 @@
         return_value_async = await controller.call_sideeffect_async(
             {},
             request=Request({"type": "http"}),  # type: ignore
         )
 
         # The response payload should be the same both both sync and async endpoints
         expected_response = {
-            controller.__class__.__name__: {
-                "sideeffect": ExampleRenderModel(
-                    value_a="Hello",
-                    value_b="World",
-                ),
-                "passthrough": None,
-            }
+            "sideeffect": ExampleRenderModel(
+                value_a="Hello",
+                value_b="World",
+            ),
+            "passthrough": None,
         }
 
         assert return_value_sync == expected_response
         assert return_value_async == expected_response
 
         assert controller.counter == 2
         assert controller.render_counts == 2
@@ -275,18 +273,16 @@
             # From the original view page that is calling this sub-function
             "referer": "http://example.com/test/5/",
         },
     )
     elapsed = (monotonic_ns() - start) / 1e9
     assert response.status_code == 200
     assert response.json() == {
-        "ExampleController": {
-            "sideeffect": {
-                "value_a": "Hello 1229",
-            }
+        "sideeffect": {
+            "value_a": "Hello 1229",
         }
     }
 
     LOGGER.info(f"Use Experimental: {use_experimental}\nElapsed: {elapsed}")
 
     if min_time is not None:
         assert elapsed >= min_time
```

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/test_build_actions.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/test_build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/test_build_links.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/test_build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/test_build_schemas.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/test_build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/test_builder.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/client_builder/test_typescript.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/client_builder/test_typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/database/dependencies/test_core.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/database/dependencies/test_core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/database/test_config.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/database/test_config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/database/test_sqlmodel.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/database/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/dependencies/test_base.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/dependencies/test_base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/fixtures/home_controller_source_map.js.map` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/fixtures/home_controller_source_map.js.map`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/js_compiler/test_javascript.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/js_compiler/test_javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/js_compiler/test_postcss.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/js_compiler/test_postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/js_compiler/test_source_maps.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/js_compiler/test_source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/conftest.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/conftest.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_actions.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_db_memory_serializer.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_db_memory_serializer.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_db_serializer.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_db_serializer.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_generator.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_generator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_generics.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_generics.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/migrations/test_handlers.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/migrations/test_handlers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_annotation_helpers.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_app.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from contextlib import asynccontextmanager
+from inspect import Parameter, signature
 from pathlib import Path
 from unittest.mock import patch
 
 import pytest
-from fastapi import FastAPI
+from fastapi import APIRouter, FastAPI
+from fastapi.routing import APIRoute
 from fastapi.testclient import TestClient
 from pydantic import BaseModel
 
 from mountaineer.actions import passthrough
-from mountaineer.app import AppController
+from mountaineer.app import AppController, ControllerDefinition
 from mountaineer.client_builder.openapi import OpenAPIDefinition
 from mountaineer.config import ConfigBase
 from mountaineer.controller import ControllerBase
 from mountaineer.controller_layout import LayoutControllerBase
 from mountaineer.exceptions import APIException
 
 
@@ -89,15 +91,14 @@
     openapi_spec = app.generate_openapi()
     openapi_definition = OpenAPIDefinition(**openapi_spec)
 
     assert openapi_definition.components.schemas.keys() == {
         "TestExceptionActionResponse",
         "ExampleException",
         "ExampleSubModel",
-        "TestExceptionActionResponseRaw",
     }
 
 
 def test_format_exception_model():
     class ExampleException(APIException):
         status_code = 401
         value: str
@@ -151,15 +152,14 @@
     app.register(ExampleController())
 
     openapi_spec = app.generate_openapi()
     openapi_definition = OpenAPIDefinition(**openapi_spec)
 
     assert openapi_definition.components.schemas.keys() == {
         "TestExceptionActionResponse",
-        "TestExceptionActionResponseRaw",
         "mountaineer.__tests__.test_1.ExampleException",
         "mountaineer.__tests__.test_2.ExampleException",
     }
 
 
 def test_inherit_parent_spec():
     """
@@ -315,7 +315,127 @@
         return ExampleController
 
     app = AppController(view_root=Path(""))
     app.register(make_controller("/example")())
 
     with pytest.raises(ValueError, match="already registered"):
         app.register(make_controller("/example2")())
+
+
+class TargetController(ControllerBase):
+    url = "/target"
+
+    async def render(self) -> None:
+        pass
+
+
+class ReferenceController(ControllerBase):
+    url = "/reference"
+
+    async def render(self) -> None:
+        pass
+
+
+def test_merge_render_signatures():
+    def target_fn(a: int, b: int):
+        pass
+
+    # Partial overlap with (a) and inclusion of a new variable
+    def reference_fn(a: int, c: int):
+        pass
+
+    app = AppController(view_root=Path(""))
+
+    target_definition = ControllerDefinition(
+        controller=TargetController(),
+        router=APIRouter(),
+        view_route=target_fn,
+        url_prefix="/target_prefix",
+        render_router=APIRouter(),
+    )
+    reference_definition = ControllerDefinition(
+        controller=ReferenceController(),
+        router=APIRouter(),
+        view_route=reference_fn,
+        url_prefix="/reference_prefix",
+        render_router=APIRouter(),
+    )
+
+    initial_routes = [
+        route.path for route in app.app.routes if isinstance(route, APIRoute)
+    ]
+    assert initial_routes == []
+
+    app.merge_render_signatures(
+        target_definition, reference_controller=reference_definition
+    )
+
+    assert list(signature(target_definition.view_route).parameters.values()) == [
+        Parameter("a", Parameter.POSITIONAL_OR_KEYWORD, annotation=int),
+        Parameter("b", Parameter.POSITIONAL_OR_KEYWORD, annotation=int),
+        # Items only in the reference function should be included as kwargs
+        Parameter("c", Parameter.KEYWORD_ONLY, annotation=int, default=Parameter.empty),
+    ]
+
+    # After the merging the signature should be updated, and the app controller should
+    # have a new endpoint (since the merging must re-mount)
+    final_routes = [
+        route.path for route in app.app.routes if isinstance(route, APIRoute)
+    ]
+    assert final_routes == ["/target"]
+
+
+def test_merge_render_signatures_conflicting_types():
+    """
+    If the two functions share a parameter, it must be typehinted with the
+    same type in both functions.
+
+    """
+
+    def target_fn(a: int, b: int):
+        pass
+
+    # Partial overlap with (a) and inclusion of a new variable
+    def reference_fn(a: str, c: int):
+        pass
+
+    app = AppController(view_root=Path(""))
+
+    target_definition = ControllerDefinition(
+        controller=TargetController(),
+        router=APIRouter(),
+        view_route=target_fn,
+        url_prefix="/target_prefix",
+        render_router=APIRouter(),
+    )
+    reference_definition = ControllerDefinition(
+        controller=ReferenceController(),
+        router=APIRouter(),
+        view_route=reference_fn,
+        url_prefix="/reference_prefix",
+        render_router=APIRouter(),
+    )
+
+    with pytest.raises(TypeError, match="Conflicting types"):
+        app.merge_render_signatures(
+            target_definition, reference_controller=reference_definition
+        )
+
+
+def test_get_value_mask_for_signature():
+    def target_fn(a: int, b: str):
+        pass
+
+    values = {
+        "a": 1,
+        "b": "test",
+        "c": "other",
+    }
+
+    app = AppController(view_root=Path(""))
+    assert app.get_value_mask_for_signature(
+        signature(target_fn),
+        values,
+    ) == {
+        "a": 1,
+        "b": "test",
+    }
```

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_cache.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_cli.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_compat.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_compat.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_controller.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_controller_layout.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_controller_layout.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_cropper.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_exceptions.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_generics.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_generics.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_logging.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_paths.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_ssr.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/__tests__/test_watch.py` & `mountaineer-0.5.0.dev4/mountaineer/__tests__/test_watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/actions/fields.py` & `mountaineer-0.5.0.dev4/mountaineer/actions/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,32 +229,22 @@
                     for field_name, field_definition in sideeffect_fields.items()
                 },
             ),
             FieldInfo(alias="sideeffect"),
         )
 
     model: Type[BaseModel] = create_model(
-        base_response_name + "Raw",
-        **base_response_params,  # type: ignore
-    )
-
-    # Each action also includes the controller type in the response
-    # signature so the frontend can differentiate between different controllers
-    wrapper_model: Type[BaseModel] = create_model(
         base_response_name,
-        **{controller.__class__.__name__: (model, FieldInfo())},  # type: ignore
+        **base_response_params,  # type: ignore
     )
 
-    return wrapper_model
+    return model
 
 
-def format_final_action_response(
-    controller: "ControllerBase",
-    dict_payload: dict[str, Any],
-):
+def format_final_action_response(dict_payload: dict[str, Any]):
     """
     Wrapper to allow actions to respond with an explicit JSONResponse, or a dictionary. This lets
     both sideeffects and passthrough payloads to inject header metadata that otherwise can't be captured
     in a regular BaseModel.
 
     Since the eventual result of an action is a combined sideeffect+passthrough payload, we need to
     merge the final payload into the explicit response.
@@ -265,27 +255,23 @@
         for key, response in dict_payload.items()
         if isinstance(response, JSONResponse)
     ]
 
     if len(responses) > 1:
         raise ValueError(f"Multiple conflicting responses returned: {responses}")
 
-    # The final transformation should include our controller name
-    # This signals to the frontend which state subset we want to update
-    action_root = controller.__class__.__name__
-
     if len(responses) == 0:
-        return {action_root: dict_payload}
+        return dict_payload
 
     response_key, response = responses[0]
     dict_payload[response_key] = json_loads(response.body)
 
     # Now inject the newly formatted response into the response object
     return JSONResponse(
-        content={action_root: dict_payload},
+        content=dict_payload,
         status_code=response.status_code,
         headers={
             key: value
             for key, value in response.headers.items()
             if key not in {"content-length", "content-type"}
         },
     )
```

### Comparing `mountaineer-0.5.0.dev3/mountaineer/actions/passthrough_dec.py` & `mountaineer-0.5.0.dev4/mountaineer/actions/passthrough_dec.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
                 if raw_response:
                     return response
 
                 if isasyncgen(response):
                     return wrap_passthrough_generator(response)
 
-                return format_final_action_response(self, dict(passthrough=response))
+                return format_final_action_response(dict(passthrough=response))
 
             metadata = init_function_metadata(inner, FunctionActionType.PASSTHROUGH)
             metadata.passthrough_model = passthrough_model
             metadata.exception_models = exception_models
             metadata.is_raw_response = raw_response or False
             metadata.media_type = (
                 STREAM_EVENT_TYPE
```

### Comparing `mountaineer-0.5.0.dev3/mountaineer/actions/sideeffect_dec.py` & `mountaineer-0.5.0.dev4/mountaineer/actions/sideeffect_dec.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,14 @@
                     # referrer can be spoofed, so it assumes that the endpoint also internally validates
                     # the caller has correct permissions to access the data.
                     server_data = render_fn(**values)
                     if isawaitable(server_data):
                         server_data = await server_data
 
                     return format_final_action_response(
-                        self,
                         dict(
                             sideeffect=server_data,
                             passthrough=passthrough_values,
                         ),
                     )
 
             # Update the signature of 'inner' to include 'request: Request'
```

### Comparing `mountaineer-0.5.0.dev3/mountaineer/annotation_helpers.py` & `mountaineer-0.5.0.dev4/mountaineer/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/app.py` & `mountaineer-0.5.0.dev4/mountaineer/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from collections import defaultdict
 from functools import wraps
-from inspect import isawaitable, isclass, signature
+from inspect import Parameter, Signature, isawaitable, isclass, signature
 from pathlib import Path
 from typing import Any, Callable, Type
 
 from fastapi import APIRouter, FastAPI, HTTPException, Request
 from fastapi.openapi.utils import get_openapi
 from fastapi.responses import JSONResponse
+from fastapi.routing import APIRoute
 from fastapi.staticfiles import StaticFiles
 from inflection import underscore
 from pydantic import BaseModel
 from starlette.routing import BaseRoute
 
 from mountaineer.actions import (
     FunctionActionType,
     fuse_metadata_to_response_typehint,
     init_function_metadata,
 )
 from mountaineer.actions.fields import FunctionMetadata
 from mountaineer.annotation_helpers import MountaineerUnsetValue
 from mountaineer.config import ConfigBase
+from mountaineer.console import CONSOLE
 from mountaineer.controller import ControllerBase
 from mountaineer.controller_layout import LayoutControllerBase
-from mountaineer.dependencies.base import get_function_dependencies
 from mountaineer.exceptions import APIException, APIExceptionInternalModelBase
 from mountaineer.js_compiler.base import ClientBuilderBase
 from mountaineer.js_compiler.javascript import JavascriptBundler
 from mountaineer.logging import LOGGER
 from mountaineer.paths import ManagedViewPath, resolve_package_path
 from mountaineer.render import Metadata, RenderBase, RenderNull
 
@@ -207,31 +208,35 @@
                 # to wait until we have registered all of the layout controllers to then register the
                 # page render function - and this would come at the expense of allowing dynamic
                 # registration of page controllers. We would need to "lock" the app controller to know when
                 # we expect to have complete coverage of pages.
                 #
                 # For now we assume that the render method of layouts will specify no URL parameters
                 # and can be leveraged in an isoltaed context.
-                async with get_function_dependencies(
-                    callable=definition.controller.render, url=controller.url
-                ) as values:
-                    server_data = definition.controller.render(**values)
-                    if isawaitable(server_data):
-                        server_data = await server_data
-                    if server_data is None:
-                        server_data = RenderNull()
+                layout_values = self.get_value_mask_for_signature(
+                    signature(definition.controller.render), kwargs
+                )
+                server_data = definition.controller.render(**layout_values)
+                if isawaitable(server_data):
+                    server_data = await server_data
+                if server_data is None:
+                    server_data = RenderNull()
 
                 layout_metadata[definition.controller.__class__.__name__] = server_data
 
             try:
+                render_values = self.get_value_mask_for_signature(
+                    signature(controller.render), kwargs
+                )
                 return await controller._generate_html(
-                    *args,
+                    # *args,
                     global_metadata=self.global_metadata,
                     other_render_contexts=layout_metadata,
-                    **kwargs,
+                    # **kwargs,
+                    **render_values,
                 )
             except Exception as e:
                 # If a user explicitly is raising an APIException, we don't want to log it
                 if not isinstance(e, (APIExceptionInternalModelBase, HTTPException)):
                     # Forward along the exception, just modify it to include
                     # the controller name for additional context
                     LOGGER.error(
@@ -347,20 +352,155 @@
             render_router=view_router,
         )
         controller.definition = controller_definition
 
         self.controllers.append(controller_definition)
         self.controller_names.add(controller_name)
 
+        # Handle the resolution of the full signature of the render function
+        self.greedy_merge_signatures(controller_definition)
+
     async def handle_exception(self, request: Request, exc: APIException):
         return JSONResponse(
             status_code=exc.status_code,
             content=exc.internal_model.model_dump(),
         )
 
+    def greedy_merge_signatures(
+        self,
+        controller_def: ControllerDefinition,
+    ):
+        """
+        As soon as a new controller is mounted, we try to determine whether the new resolution of this
+        controller modifies (or is modified by) existing controllers.
+
+        Specifically:
+
+        - If the new controller is a LayoutController, it might modify controllers that are already
+            mounted. We need to back-fill the relationship between the layout and the controllers.
+        - If the new controller is a standard controller, it might be modified by a LayoutController
+            that is already mounted. We should back-fill in the same way.
+
+        """
+        # Too early in the build lifecycle, hasn't yet built artifacts
+        if not controller_def.controller.build_metadata:
+            CONSOLE.print(
+                "[red]No metadata found for controller on disk. Skipping layout merging until after first build is completed."
+            )
+            return
+
+        # Exclude the self reference
+        other_controllers = [
+            definition
+            for definition in self.controllers
+            if definition is not controller_def
+        ]
+
+        if isinstance(controller_def.controller, LayoutControllerBase):
+            # Go back through the existing controllers and back-fill
+            # the relationship
+            for existing_controller_def in other_controllers:
+                if (
+                    existing_controller_def.controller.build_metadata
+                    and controller_def.controller.build_metadata.view_path
+                    in existing_controller_def.controller.build_metadata.layout_view_paths
+                ):
+                    self.merge_render_signatures(
+                        existing_controller_def,
+                        reference_controller=controller_def,
+                    )
+        else:
+            for candidate_layout_controller in other_controllers:
+                if candidate_layout_controller.controller.build_metadata and (
+                    candidate_layout_controller.controller.build_metadata.view_path
+                    in controller_def.controller.build_metadata.layout_view_paths
+                ):
+                    self.merge_render_signatures(
+                        controller_def,
+                        reference_controller=candidate_layout_controller,
+                    )
+
+    def merge_render_signatures(
+        self,
+        target_controller: ControllerDefinition,
+        *,
+        reference_controller: ControllerDefinition,
+    ):
+        """
+        Collects the signature from the "reference_controller" and replaces the active render endpoint
+        with this new signature. We require all these new parameters to be kwargs so they
+        can be injected into the render function by name alone.
+
+        """
+        reference_signature = signature(reference_controller.view_route)
+        target_signature = signature(target_controller.view_route)
+
+        reference_parameters = reference_signature.parameters.values()
+        target_parameters = list(target_signature.parameters.values())
+
+        # For any additional arguments provided by the reference, inject them into
+        # the target controller
+        # For duplicate ones, the target controller should win
+        for parameter in reference_parameters:
+            if parameter.name not in target_signature.parameters:
+                target_parameters.append(
+                    parameter.replace(
+                        kind=Parameter.KEYWORD_ONLY,
+                    )
+                )
+            else:
+                # We only throw an error if the types are different. If they're the same we assume
+                # that the resolution is intended to be shared.
+                target_annotation_type = target_signature.parameters[
+                    parameter.name
+                ].annotation
+                reference_annotation_type = parameter.annotation
+
+                if target_annotation_type != reference_annotation_type:
+                    raise TypeError(
+                        f"Duplicate parameter {parameter.name} in {target_controller.controller} and {reference_controller.controller}.\n"
+                        f"Conflicting types: {target_annotation_type} vs {reference_annotation_type}"
+                    )
+
+        target_controller.view_route.__signature__ = target_signature.replace(  # type: ignore
+            parameters=target_parameters
+        )
+
+        # Re-mount the controller exactly as it was first mounted
+        if target_controller.render_router:
+            # Clear the previous definition before re-adding it
+            # Both the app route is required (for the actual page resolution) and the render router
+            # (to avoid conflicts in the OpenAPI generation)
+            for route_list in [self.app.routes, target_controller.render_router.routes]:
+                for route in list(route_list):
+                    if (
+                        isinstance(route, APIRoute)
+                        and route.path == target_controller.controller.url
+                        and route.methods == {"GET"}
+                    ):
+                        route_list.remove(route)
+
+            target_controller.render_router.get(target_controller.controller.url)(
+                target_controller.view_route
+            )
+            self.app.include_router(target_controller.render_router)
+
+    def get_value_mask_for_signature(
+        self,
+        signature: Signature,
+        values: dict[str, Any],
+    ):
+        # Assume the values match the parameters specified in the signature
+        passthrough_names = {
+            parameter.name for parameter in signature.parameters.values()
+        }
+        return {
+            name: value for name, value in values.items() if name in passthrough_names
+        }
+
     def generate_openapi(self, routes: list[BaseRoute] | None = None):
         """
         Bundle custom user exceptions in the OpenAPI schema. By default
         endpoints just include the 422 Validation Error, but this allows
         for custom derived user methods.
 
         """
```

### Comparing `mountaineer-0.5.0.dev3/mountaineer/cache.py` & `mountaineer-0.5.0.dev4/mountaineer/cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/cli.py` & `mountaineer-0.5.0.dev4/mountaineer/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/client_builder/build_actions.py` & `mountaineer-0.5.0.dev4/mountaineer/client_builder/build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/client_builder/build_links.py` & `mountaineer-0.5.0.dev4/mountaineer/client_builder/build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/client_builder/build_schemas.py` & `mountaineer-0.5.0.dev4/mountaineer/client_builder/build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/client_builder/builder.py` & `mountaineer-0.5.0.dev4/mountaineer/client_builder/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
                 + "};\n"
                 + "return {\n"
                 + "...serverState,\n"
                 + "linkGenerator: LinkGenerator,\n"
                 + ",\n".join(
                     [
                         (
-                            f"{metadata.function_name}: applySideEffect({metadata.function_name}, setControllerState, '{controller_key}')"
+                            f"{metadata.function_name}: applySideEffect({metadata.function_name}, setControllerState)"
                             if metadata.action_type == FunctionActionType.SIDEEFFECT
                             else f"{metadata.function_name}: {metadata.function_name}"
                         )
                         for metadata in controller_action_metadata
                     ]
                 )
                 + "}\n"
```

### Comparing `mountaineer-0.5.0.dev3/mountaineer/client_builder/openapi.py` & `mountaineer-0.5.0.dev4/mountaineer/client_builder/openapi.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/client_builder/typescript.py` & `mountaineer-0.5.0.dev4/mountaineer/client_builder/typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/compat.py` & `mountaineer-0.5.0.dev4/mountaineer/compat.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/config.py` & `mountaineer-0.5.0.dev4/mountaineer/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/controller.py` & `mountaineer-0.5.0.dev4/mountaineer/controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/controller_layout.py` & `mountaineer-0.5.0.dev4/mountaineer/controller_layout.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/controllers/exception_controller.py` & `mountaineer-0.5.0.dev4/mountaineer/controllers/exception_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/cropper.py` & `mountaineer-0.5.0.dev4/mountaineer/cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/database/cli.py` & `mountaineer-0.5.0.dev4/mountaineer/database/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/database/config.py` & `mountaineer-0.5.0.dev4/mountaineer/database/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/database/dependencies/core.py` & `mountaineer-0.5.0.dev4/mountaineer/database/dependencies/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/database/sqlmodel.py` & `mountaineer-0.5.0.dev4/mountaineer/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/database/validator.py` & `mountaineer-0.5.0.dev4/mountaineer/database/validator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/dependencies/base.py` & `mountaineer-0.5.0.dev4/mountaineer/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/dependencies/core/core.py` & `mountaineer-0.5.0.dev4/mountaineer/dependencies/core/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/exceptions.py` & `mountaineer-0.5.0.dev4/mountaineer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/generics.py` & `mountaineer-0.5.0.dev4/mountaineer/generics.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/io.py` & `mountaineer-0.5.0.dev4/mountaineer/io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/js_compiler/base.py` & `mountaineer-0.5.0.dev4/mountaineer/js_compiler/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/js_compiler/javascript.py` & `mountaineer-0.5.0.dev4/mountaineer/js_compiler/javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/js_compiler/postcss.py` & `mountaineer-0.5.0.dev4/mountaineer/js_compiler/postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/js_compiler/source_maps.py` & `mountaineer-0.5.0.dev4/mountaineer/js_compiler/source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/logging.py` & `mountaineer-0.5.0.dev4/mountaineer/logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/actions.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/cli.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/client_io.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/client_io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/db_memory_serializer.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/db_memory_serializer.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/db_serializer.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/db_serializer.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/db_stubs.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/db_stubs.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/generator.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/generator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/generics.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/generics.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/handlers.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/handlers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/migration.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/migration.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/migrations/migrator.py` & `mountaineer-0.5.0.dev4/mountaineer/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/paths.py` & `mountaineer-0.5.0.dev4/mountaineer/paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/render.py` & `mountaineer-0.5.0.dev4/mountaineer/render.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/ssr.py` & `mountaineer-0.5.0.dev4/mountaineer/ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/static/api.ts` & `mountaineer-0.5.0.dev4/mountaineer/static/api.ts`

 * *Files 3% similar despite different names*

```diff
@@ -147,40 +147,35 @@
         // Yield the line in the requested format.
         yield format === "text" ? line : JSON.parse(line);
       }
     }
   })();
 };
 
-type ApiFunctionReturnType<S, P, K extends PropertyKey> = {
-  // Generic typehint for any key parameter
-  [key in K]: {
-    sideeffect: S;
-    passthrough?: P;
-  };
+type ApiFunctionReturnType<S, P> = {
+  sideeffect: S;
+  passthrough?: P;
 };
 
 export function applySideEffect<
   ARG extends any[],
   S,
   P,
-  K extends PropertyKey,
-  RE extends ApiFunctionReturnType<S, P, K>,
+  RE extends ApiFunctionReturnType<S, P>,
 >(
   apiFunction: (...args: ARG) => Promise<RE>,
   setControllerState: (payload: S) => void,
-  controllerKey: K,
 ): (...args: ARG) => Promise<RE> {
   /*
    * Executes an API server function, triggering any appropriate exceptions.
    * If the fetch succeeds, the sideeffect is applied to the controller state.
    */
   return async (...args: ARG) => {
     const result = await apiFunction(...args);
-    setControllerState(result[controllerKey].sideeffect);
+    setControllerState(result.sideeffect);
     return result;
   };
 }
 
 interface GetLinkParams {
   rawUrl: string;
   queryParameters: Record<string, string>;
```

### Comparing `mountaineer-0.5.0.dev3/mountaineer/static/live_reload.ts` & `mountaineer-0.5.0.dev4/mountaineer/static/live_reload.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/test_utilities.py` & `mountaineer-0.5.0.dev4/mountaineer/test_utilities.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/views/package-lock.json` & `mountaineer-0.5.0.dev4/mountaineer/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/watch.py` & `mountaineer-0.5.0.dev4/mountaineer/watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/watch_server.py` & `mountaineer-0.5.0.dev4/mountaineer/watch_server.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/mountaineer/webservice.py` & `mountaineer-0.5.0.dev4/mountaineer/webservice.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/poetry.lock` & `mountaineer-0.5.0.dev4/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/benches/fixtures/complex_sourcemap_mapping.txt` & `mountaineer-0.5.0.dev4/src/benches/fixtures/complex_sourcemap_mapping.txt`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/benches/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.5.0.dev4/src/benches/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/benches/lexers_benchmark.rs` & `mountaineer-0.5.0.dev4/src/benches/lexers_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/benches/source_map_benchmark.rs` & `mountaineer-0.5.0.dev4/src/benches/source_map_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/benches/ssr_benchmark.rs` & `mountaineer-0.5.0.dev4/src/benches/ssr_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/lexers.rs` & `mountaineer-0.5.0.dev4/src/lexers.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/lib.rs` & `mountaineer-0.5.0.dev4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/logging.rs` & `mountaineer-0.5.0.dev4/src/logging.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/source_map.rs` & `mountaineer-0.5.0.dev4/src/source_map.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/ssr.rs` & `mountaineer-0.5.0.dev4/src/ssr.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/src/timeout.rs` & `mountaineer-0.5.0.dev4/src/timeout.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev3/Cargo.lock` & `mountaineer-0.5.0.dev4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mountaineer"
-version = "0.5.0-dev3"
+version = "0.5.0-dev4"
 dependencies = [
  "criterion",
  "deno_core_icudata",
  "env_logger",
  "lazy_static",
  "libc",
  "log",
```

### Comparing `mountaineer-0.5.0.dev3/pyproject.toml` & `mountaineer-0.5.0.dev4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "mountaineer"
 dependencies = [ "pydantic", "fastapi", "inflection", "click", "uvicorn[standard]", "packaging", "watchdog", "pydantic-settings", "sqlmodel", "asyncpg", "sqlalchemy[asyncio]", "rich",]
 exclude = [ "fixtures", "ci_webapp", "create_mountaineer_app", "media", "docs_website", "benchmarking",]
 
 [tool.poetry]
 name = "mountaineer"
-version = "0.5.0.dev3"
+version = "0.5.0.dev4"
 description = ""
 authors = [ "Pierce Freeman <pierce@freeman.vc>",]
 readme = "README.md"
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
```

### Comparing `mountaineer-0.5.0.dev3/PKG-INFO` & `mountaineer-0.5.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mountaineer
-Version: 0.5.0.dev3
+Version: 0.5.0.dev4
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: inflection
 Requires-Dist: click
 Requires-Dist: uvicorn[standard]
 Requires-Dist: packaging
 Requires-Dist: watchdog
```

