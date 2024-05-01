# Comparing `tmp/mountaineer-0.4.2.dev3.tar.gz` & `tmp/mountaineer-0.5.0.dev1.tar.gz`

## Comparing `mountaineer-0.4.2.dev3.tar` & `mountaineer-0.5.0.dev1.tar`

### file list

```diff
@@ -1,260 +1,264 @@
--rw-r--r--   0     1001      127      269 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/Cargo.toml
--rw-r--r--   0     1001      127     1995 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/build.rs
--rw-r--r--   0     1001      127     4195 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/go/js_build.go
--rw-r--r--   0     1001      127      168 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/go.mod
--rw-r--r--   0     1001      127      376 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/go.sum
--rw-r--r--   0     1001      127     6499 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/src/lib.rs
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.4.2.dev3/Cargo.toml
--rw-r--r--   0     1001      127      133 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.git-blame-ignore-revs
--rw-r--r--   0     1001      127      138 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.gitattributes
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/README_SCRIPTS.md
--rw-r--r--   0     1001      127    14036 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/poetry.lock
--rw-r--r--   0     1001      127      767 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/scripts/__init__.py
--rw-r--r--   0     1001      127     3032 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/scripts/__tests__/test_update_version.py
--rw-r--r--   0     1001      127     2181 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/scripts/check_dependencies.py
--rw-r--r--   0     1001      127     3382 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/scripts/update_version.py
--rw-r--r--   0     1001      127     1321 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/workflows/publish_docs.yml
--rw-r--r--   0     1001      127    20289 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/workflows/test.yml
--rw-r--r--   0     1001      127      504 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/workflows/validate.yml
--rw-r--r--   0     1001      127     3404 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.gitignore
--rw-r--r--   0     1001      127     1750 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/Dockerfile
--rw-r--r--   0     1001      127     1079 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/LICENSE
--rw-r--r--   0     1001      127     4976 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/Makefile
--rw-r--r--   0     1001      127    14891 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/README.md
--rw-r--r--   0     1001      127      105 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/benchmarking/README.md
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/benchmarking/benchmarking/__init__.py
--rw-r--r--   0     1001      127      425 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/benchmarking/benchmarking/simple_render.py
--rw-r--r--   0     1001      127   127093 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/benchmarking/poetry.lock
--rw-r--r--   0     1001      127      291 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/benchmarking/pyproject.toml
--rw-r--r--   0     1001      127      850 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/README.md
--rw-r--r--   0     1001      127        1 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/__init__.py
--rw-r--r--   0     1001      127      775 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/app.py
--rw-r--r--   0     1001      127      489 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/cli.py
--rw-r--r--   0     1001      127      111 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/config.py
--rw-r--r--   0     1001      127        1 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/__init__.py
--rw-r--r--   0     1001      127     1433 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/complex.py
--rw-r--r--   0     1001      127      581 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/detail.py
--rw-r--r--   0     1001      127     1658 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/home.py
--rw-r--r--   0     1001      127      559 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/stream.py
--rw-r--r--   0     1001      127       77 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/main.py
--rw-r--r--   0     1001      127      208 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/__init__.py
--rw-r--r--   0     1001      127     2261 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/complex/page.tsx
--rw-r--r--   0     1001      127      453 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/detail/page.tsx
--rw-r--r--   0     1001      127     2822 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/home/page.tsx
--rw-r--r--   0     1001      127       59 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/main.css
--rw-r--r--   0     1001      127      708 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/stream/page.tsx
--rw-r--r--   0     1001      127   125408 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/package-lock.json
--rw-r--r--   0     1001      127      453 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/postcss.config.js
--rw-r--r--   0     1001      127      161 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/tailwind.config.js
--rw-r--r--   0     1001      127   109872 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/poetry.lock
--rw-r--r--   0     1001      127      724 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/pyproject.toml
--rw-r--r--   0     1001      127     1593 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/README.md
--rw-r--r--   0     1001      127        1 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0     1001      127     1055 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0     1001      127     7904 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0     1001      127      292 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0     1001      127      816 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0     1001      127     4277 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/builder.py
--rw-r--r--   0     1001      127     4656 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/cli.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0     1001      127     1383 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/base.py
--rw-r--r--   0     1001      127     4591 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0     1001      127     1832 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/venv.py
--rw-r--r--   0     1001      127     1336 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/external.py
--rw-r--r--   0     1001      127     1925 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/generation.py
--rw-r--r--   0     1001      127      327 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/io.py
--rw-r--r--   0     1001      127       30 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
--rw-r--r--   0     1001      127      212 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0     1001      127      190 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0     1001      127      137 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0     1001      127      109 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0     1001      127      170 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.env
--rw-r--r--   0     1001      127     3373 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0     1001      127      645 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0     1001      127       17 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0     1001      127      767 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0     1001      127      947 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0     1001      127      282 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0     1001      127      227 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0     1001      127     1702 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0     1001      127     1124 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0     1001      127       84 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0     1001      127      157 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0     1001      127     1219 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0     1001      127      995 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0     1001      127       95 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0     1001      127      524 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0     1001      127      117 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0     1001      127      195 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0     1001      127      332 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0     1001      127     1493 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0     1001      127    61104 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/poetry.lock
--rw-r--r--   0     1001      127     1214 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/pyproject.toml
--rw-r--r--   0     1001      127       30 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/.zed/settings.json
--rw-r--r--   0     1001      127      107 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/README.md
--rw-r--r--   0     1001      127       15 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/CNAME
--rw-r--r--   0     1001      127      310 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/actions.md
--rw-r--r--   0     1001      127      454 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/api_exception.md
--rw-r--r--   0     1001      127       99 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/app-controller.md
--rw-r--r--   0     1001      127      281 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/build_plugins/base.md
--rw-r--r--   0     1001      127       57 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/build_plugins/javascript.md
--rw-r--r--   0     1001      127       62 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/build_plugins/postcss.md
--rw-r--r--   0     1001      127      411 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/cli.md
--rw-r--r--   0     1001      127      376 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/config.md
--rw-r--r--   0     1001      127       61 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/controller.md
--rw-r--r--   0     1001      127       67 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/core_dependencies.md
--rw-r--r--   0     1001      127       66 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/database/config.md
--rw-r--r--   0     1001      127       71 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/database/dependencies.md
--rw-r--r--   0     1001      127       80 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/logging.md
--rw-r--r--   0     1001      127      479 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/render.md
--rw-r--r--   0     1001      127      365 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/ssr.md
--rw-r--r--   0     1001      127      299 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/watch_server.md
--rw-r--r--   0     1001      127     9375 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/client_actions.md
--rw-r--r--   0     1001      127      753 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/cma.md
--rw-r--r--   0     1001      127     3021 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/database.md
--rw-r--r--   0     1001      127     4677 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/deploy.md
--rw-r--r--   0     1001      127     7698 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/error_handling.md
--rw-r--r--   0     1001      127     1081 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/index.md
--rw-r--r--   0     1001      127     1541 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/internal/core_library.md
--rw-r--r--   0     1001      127     2156 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/links.md
--rw-r--r--   0     1001      127   365251 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/media/final_todo_list.png
--rw-r--r--   0     1001      127   148261 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/media/ide_typehints.png
--rw-r--r--   0     1001      127   545494 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/media/network_debug.png
--rw-r--r--   0     1001      127   346903 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/media/server_side_rendering.png
--rw-r--r--   0     1001      127     2263 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/metadata.md
--rw-r--r--   0     1001      127     2347 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/postcss.md
--rw-r--r--   0     1001      127    12265 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/quickstart.md
--rw-r--r--   0     1001      127     4875 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/static_analysis.md
--rw-r--r--   0     1001      127     2490 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/structure.md
--rw-r--r--   0     1001      127     1219 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127     4080 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/views.md
--rw-r--r--   0     1001      127     1823 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/mkdocs.yml
--rw-r--r--   0     1001      127      109 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/overrides/partials/footer.html
--rw-r--r--   0     1001      127   156250 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/poetry.lock
--rw-r--r--   0     1001      127      479 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/pyproject.toml
--rw-r--r--   0     1001      127   675789 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/media/header.png
--rw-r--r--   0     1001      127      954 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/__init__.py
--rw-r--r--   0     1001      127     7884 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_fields.py
--rw-r--r--   0     1001      127     9707 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_passthrough.py
--rw-r--r--   0     1001      127     9074 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_sideeffect.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/__init__.py
--rw-r--r--   0     1001      127    14334 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_actions.py
--rw-r--r--   0     1001      127     4816 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_links.py
--rw-r--r--   0     1001      127    10097 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_schemas.py
--rw-r--r--   0     1001      127     5001 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_builder.py
--rw-r--r--   0     1001      127     4153 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_typescript.py
--rw-r--r--   0     1001      127      319 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/common.py
--rw-r--r--   0     1001      127      497 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/conftest.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/dependencies/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/dependencies/conftest.py
--rw-r--r--   0     1001      127      801 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/dependencies/test_core.py
--rw-r--r--   0     1001      127      627 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/test_config.py
--rw-r--r--   0     1001      127      616 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/test_sqlmodel.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/dependencies/__init__.py
--rw-r--r--   0     1001      127     2567 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/dependencies/test_base.py
--rw-r--r--   0     1001      127      211 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/__init__.py
--rw-r--r--   0     1001      127   571338 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
--rw-r--r--   0     1001      127  1638568 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
--rw-r--r--   0     1001      127   575422 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/__init__.py
--rw-r--r--   0     1001      127     9973 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_javascript.py
--rw-r--r--   0     1001      127      808 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_postcss.py
--rw-r--r--   0     1001      127     2823 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_source_maps.py
--rw-r--r--   0     1001      127     1236 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_annotation_helpers.py
--rw-r--r--   0     1001      127     8602 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_app.py
--rw-r--r--   0     1001      127      734 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cache.py
--rw-r--r--   0     1001      127     5281 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cli.py
--rw-r--r--   0     1001      127      494 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_config.py
--rw-r--r--   0     1001      127     6571 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_controller.py
--rw-r--r--   0     1001      127     3239 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cropper.py
--rw-r--r--   0     1001      127     1227 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_exceptions.py
--rw-r--r--   0     1001      127     1924 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_logging.py
--rw-r--r--   0     1001      127     8419 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_paths.py
--rw-r--r--   0     1001      127     2565 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_ssr.py
--rw-r--r--   0     1001      127     3177 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_watch.py
--rw-r--r--   0     1001      127      397 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/actions/__init__.py
--rw-r--r--   0     1001      127    12321 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/actions/fields.py
--rw-r--r--   0     1001      127     6835 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/actions/passthrough.py
--rw-r--r--   0     1001      127    11635 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/actions/sideeffect.py
--rw-r--r--   0     1001      127     4352 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/annotation_helpers.py
--rw-r--r--   0     1001      127    18916 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/app.py
--rw-r--r--   0     1001      127     3216 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/cache.py
--rw-r--r--   0     1001      127    19226 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/cli.py
--rw-r--r--   0     1001      127    11390 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/build_actions.py
--rw-r--r--   0     1001      127     4002 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/build_links.py
--rw-r--r--   0     1001      127    10172 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/build_schemas.py
--rw-r--r--   0     1001      127    29298 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/builder.py
--rw-r--r--   0     1001      127    11199 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/openapi.py
--rw-r--r--   0     1001      127     5070 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/typescript.py
--rw-r--r--   0     1001      127     2424 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/config.py
--rw-r--r--   0     1001      127      197 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/console.py
--rw-r--r--   0     1001      127       40 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/constants.py
--rw-r--r--   0     1001      127    14854 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/controller.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/controllers/__init__.py
--rw-r--r--   0     1001      127     1216 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/controllers/exception_controller.py
--rw-r--r--   0     1001      127    10359 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/cropper.py
--rw-r--r--   0     1001      127      327 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/__init__.py
--rw-r--r--   0     1001      127     1866 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/cli.py
--rw-r--r--   0     1001      127     1822 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/config.py
--rw-r--r--   0     1001      127      133 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/dependencies/__init__.py
--rw-r--r--   0     1001      127     3188 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/dependencies/core.py
--rw-r--r--   0     1001      127     7969 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/sqlmodel.py
--rw-r--r--   0     1001      127     8737 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/validator.py
--rw-r--r--   0     1001      127      251 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/dependencies/__init__.py
--rw-r--r--   0     1001      127     5122 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/dependencies/base.py
--rw-r--r--   0     1001      127      116 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/dependencies/core/__init__.py
--rw-r--r--   0     1001      127     1069 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/dependencies/core/core.py
--rw-r--r--   0     1001      127     3317 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/exceptions.py
--rw-r--r--   0     1001      127     1188 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/io.py
--rw-r--r--   0     1001      127        1 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/__init__.py
--rw-r--r--   0     1001      127     1731 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/base.py
--rw-r--r--   0     1001      127      199 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/exceptions.py
--rw-r--r--   0     1001      127    16439 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/javascript.py
--rw-r--r--   0     1001      127     4163 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/postcss.py
--rw-r--r--   0     1001      127     5614 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/source_maps.py
--rw-r--r--   0     1001      127     2313 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/logging.py
--rw-r--r--   0     1001      127    12826 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/paths.py
--rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/py.typed
--rw-r--r--   0     1001      127     5816 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/render.py
--rw-r--r--   0     1001      127     3228 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/ssr.py
--rw-r--r--   0     1001      127      210 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/static/__init__.py
--rw-r--r--   0     1001      127     6299 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/static/api.ts
--rw-r--r--   0     1001      127     3976 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/static/live_reload.ts
--rw-r--r--   0     1001      127      323 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/static/ssr_polyfills.js
--rw-r--r--   0     1001      127     7261 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/test_utilities.py
--rw-r--r--   0     1001      127      213 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/__init__.py
--rw-r--r--   0     1001      127      432 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/core/exception/page.tsx
--rw-r--r--   0     1001      127      178 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/core/layout.tsx
--rw-r--r--   0     1001      127       59 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/core/main.css
--rw-r--r--   0     1001      127     1478 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/package-lock.json
--rw-r--r--   0     1001      127      257 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/postcss.config.js
--rw-r--r--   0     1001      127      162 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/tailwind.config.js
--rw-r--r--   0     1001      127     8414 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/watch.py
--rw-r--r--   0     1001      127     3087 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/watch_server.py
--rw-r--r--   0     1001      127     1213 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/webservice.py
--rw-r--r--   0     1001      127   127639 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/poetry.lock
--rw-r--r--   0     1001      127   453080 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/fixtures/complex_sourcemap_mapping.txt
--rw-r--r--   0     1001      127   575422 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127      322 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/fixtures/ssr_polyfill_archive.js
--rw-r--r--   0     1001      127      899 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/lexers_benchmark.rs
--rw-r--r--   0     1001      127     1089 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/source_map_benchmark.rs
--rw-r--r--   0     1001      127     1595 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/ssr_benchmark.rs
--rw-r--r--   0     1001      127      499 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/errors.rs
--rw-r--r--   0     1001      127     4648 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/lexers.rs
--rw-r--r--   0     1001      127     9118 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/lib.rs
--rw-r--r--   0     1001      127      680 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/logging.rs
--rw-r--r--   0     1001      127    17549 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/source_map.rs
--rw-r--r--   0     1001      127    15113 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/ssr.rs
--rw-r--r--   0     1001      127     3998 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/timeout.rs
--rw-r--r--   0     1001      127    32093 2024-04-29 06:28:33.000000 mountaineer-0.4.2.dev3/Cargo.lock
--rw-r--r--   0     1001      127     1624 2024-04-29 06:28:24.000000 mountaineer-0.4.2.dev3/pyproject.toml
--rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.4.2.dev3/PKG-INFO
+-rw-r--r--   0     1001      127      269 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src_go/Cargo.toml
+-rw-r--r--   0     1001      127     1995 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src_go/build.rs
+-rw-r--r--   0     1001      127     4195 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src_go/go/js_build.go
+-rw-r--r--   0     1001      127      168 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src_go/go.mod
+-rw-r--r--   0     1001      127      376 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src_go/go.sum
+-rw-r--r--   0     1001      127     6499 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src_go/src/lib.rs
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.5.0.dev1/Cargo.toml
+-rw-r--r--   0     1001      127      133 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.git-blame-ignore-revs
+-rw-r--r--   0     1001      127      138 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.gitattributes
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.github/README_SCRIPTS.md
+-rw-r--r--   0     1001      127    14036 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.github/poetry.lock
+-rw-r--r--   0     1001      127      767 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.github/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.github/scripts/__init__.py
+-rw-r--r--   0     1001      127     3032 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.github/scripts/__tests__/test_update_version.py
+-rw-r--r--   0     1001      127     2181 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.github/scripts/check_dependencies.py
+-rw-r--r--   0     1001      127     3382 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.github/scripts/update_version.py
+-rw-r--r--   0     1001      127     1321 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.github/workflows/publish_docs.yml
+-rw-r--r--   0     1001      127    20289 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      504 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.github/workflows/validate.yml
+-rw-r--r--   0     1001      127     3414 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/.gitignore
+-rw-r--r--   0     1001      127     1750 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/Dockerfile
+-rw-r--r--   0     1001      127     1079 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/LICENSE
+-rw-r--r--   0     1001      127     4976 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/Makefile
+-rw-r--r--   0     1001      127    14891 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/README.md
+-rw-r--r--   0     1001      127      105 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/benchmarking/README.md
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/benchmarking/benchmarking/__init__.py
+-rw-r--r--   0     1001      127      425 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/benchmarking/benchmarking/simple_render.py
+-rw-r--r--   0     1001      127   127093 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/benchmarking/poetry.lock
+-rw-r--r--   0     1001      127      291 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/benchmarking/pyproject.toml
+-rw-r--r--   0     1001      127      850 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/README.md
+-rw-r--r--   0     1001      127        1 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/__init__.py
+-rw-r--r--   0     1001      127      886 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/app.py
+-rw-r--r--   0     1001      127      489 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/cli.py
+-rw-r--r--   0     1001      127      111 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/config.py
+-rw-r--r--   0     1001      127        1 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/controllers/__init__.py
+-rw-r--r--   0     1001      127     1433 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/controllers/complex.py
+-rw-r--r--   0     1001      127      581 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/controllers/detail.py
+-rw-r--r--   0     1001      127     1658 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/controllers/home.py
+-rw-r--r--   0     1001      127      558 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/controllers/root_layout.py
+-rw-r--r--   0     1001      127      559 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/controllers/stream.py
+-rw-r--r--   0     1001      127       77 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/main.py
+-rw-r--r--   0     1001      127      208 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/__init__.py
+-rw-r--r--   0     1001      127     2261 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/app/complex/page.tsx
+-rw-r--r--   0     1001      127      453 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127     2822 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/app/home/page.tsx
+-rw-r--r--   0     1001      127      602 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/app/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/app/main.css
+-rw-r--r--   0     1001      127      708 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/app/stream/page.tsx
+-rw-r--r--   0     1001      127   125408 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/package-lock.json
+-rw-r--r--   0     1001      127      453 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/package.json
+-rw-r--r--   0     1001      127       83 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/postcss.config.js
+-rw-r--r--   0     1001      127      161 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/tailwind.config.js
+-rw-r--r--   0     1001      127   109872 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/poetry.lock
+-rw-r--r--   0     1001      127      724 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/ci_webapp/pyproject.toml
+-rw-r--r--   0     1001      127     1593 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/README.md
+-rw-r--r--   0     1001      127        1 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0     1001      127     1055 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0     1001      127     7904 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0     1001      127      292 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      816 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0     1001      127     4277 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/builder.py
+-rw-r--r--   0     1001      127     4656 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/cli.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0     1001      127     1383 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/environments/base.py
+-rw-r--r--   0     1001      127     4591 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0     1001      127     1832 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0     1001      127     1336 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/external.py
+-rw-r--r--   0     1001      127     1925 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/generation.py
+-rw-r--r--   0     1001      127      327 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/io.py
+-rw-r--r--   0     1001      127       30 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0     1001      127      212 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0     1001      127      246 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0     1001      127      162 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0     1001      127      109 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0     1001      127      170 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0     1001      127     3383 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0     1001      127      645 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0     1001      127       17 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0     1001      127      767 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0     1001      127      947 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0     1001      127      282 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0     1001      127      227 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0     1001      127     1702 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0     1001      127     1124 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0     1001      127       84 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0     1001      127      157 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0     1001      127      208 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0     1001      127     1219 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127      995 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       95 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0     1001      127      524 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0     1001      127      117 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0     1001      127      195 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0     1001      127      332 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0     1001      127     1493 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0     1001      127    61104 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/poetry.lock
+-rw-r--r--   0     1001      127     1214 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/create_mountaineer_app/pyproject.toml
+-rw-r--r--   0     1001      127       30 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/.zed/settings.json
+-rw-r--r--   0     1001      127      107 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/README.md
+-rw-r--r--   0     1001      127       15 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/CNAME
+-rw-r--r--   0     1001      127      310 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/actions.md
+-rw-r--r--   0     1001      127      454 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/api_exception.md
+-rw-r--r--   0     1001      127       99 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/app-controller.md
+-rw-r--r--   0     1001      127      281 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/build_plugins/base.md
+-rw-r--r--   0     1001      127       57 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/build_plugins/javascript.md
+-rw-r--r--   0     1001      127       62 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/build_plugins/postcss.md
+-rw-r--r--   0     1001      127      411 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/cli.md
+-rw-r--r--   0     1001      127      376 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/config.md
+-rw-r--r--   0     1001      127      138 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/controller.md
+-rw-r--r--   0     1001      127       67 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/core_dependencies.md
+-rw-r--r--   0     1001      127       66 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/database/config.md
+-rw-r--r--   0     1001      127       71 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/database/dependencies.md
+-rw-r--r--   0     1001      127       80 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/logging.md
+-rw-r--r--   0     1001      127      479 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/render.md
+-rw-r--r--   0     1001      127      365 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/ssr.md
+-rw-r--r--   0     1001      127      299 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/api/watch_server.md
+-rw-r--r--   0     1001      127     9375 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/client_actions.md
+-rw-r--r--   0     1001      127      753 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/cma.md
+-rw-r--r--   0     1001      127     3021 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/database.md
+-rw-r--r--   0     1001      127     4690 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/deploy.md
+-rw-r--r--   0     1001      127     7698 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/error_handling.md
+-rw-r--r--   0     1001      127     1081 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/index.md
+-rw-r--r--   0     1001      127     1541 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/internal/core_library.md
+-rw-r--r--   0     1001      127     2156 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/links.md
+-rw-r--r--   0     1001      127   365251 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/media/final_todo_list.png
+-rw-r--r--   0     1001      127   148261 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/media/ide_typehints.png
+-rw-r--r--   0     1001      127   545494 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/media/network_debug.png
+-rw-r--r--   0     1001      127   346903 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/media/server_side_rendering.png
+-rw-r--r--   0     1001      127     2263 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/metadata.md
+-rw-r--r--   0     1001      127     2347 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/postcss.md
+-rw-r--r--   0     1001      127    12263 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/quickstart.md
+-rw-r--r--   0     1001      127     4875 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/static_analysis.md
+-rw-r--r--   0     1001      127     2490 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/structure.md
+-rw-r--r--   0     1001      127     1219 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127     6802 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/docs/views.md
+-rw-r--r--   0     1001      127     1823 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/mkdocs.yml
+-rw-r--r--   0     1001      127      109 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/overrides/partials/footer.html
+-rw-r--r--   0     1001      127   156250 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/poetry.lock
+-rw-r--r--   0     1001      127      500 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/docs_website/pyproject.toml
+-rw-r--r--   0     1001      127   675789 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/media/header.png
+-rw-r--r--   0     1001      127     1041 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/actions/__init__.py
+-rw-r--r--   0     1001      127     8306 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/actions/test_fields.py
+-rw-r--r--   0     1001      127     9757 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/actions/test_passthrough.py
+-rw-r--r--   0     1001      127     9206 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/actions/test_sideeffect.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/__init__.py
+-rw-r--r--   0     1001      127    14334 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/test_build_actions.py
+-rw-r--r--   0     1001      127     4816 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/test_build_links.py
+-rw-r--r--   0     1001      127    10097 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/test_build_schemas.py
+-rw-r--r--   0     1001      127     6322 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/test_builder.py
+-rw-r--r--   0     1001      127     4153 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/test_typescript.py
+-rw-r--r--   0     1001      127      319 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/common.py
+-rw-r--r--   0     1001      127      497 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/conftest.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/database/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127      208 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/database/dependencies/conftest.py
+-rw-r--r--   0     1001      127      801 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/database/dependencies/test_core.py
+-rw-r--r--   0     1001      127      627 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/database/test_config.py
+-rw-r--r--   0     1001      127      616 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/database/test_sqlmodel.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/dependencies/__init__.py
+-rw-r--r--   0     1001      127     2567 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/dependencies/test_base.py
+-rw-r--r--   0     1001      127      211 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/fixtures/__init__.py
+-rw-r--r--   0     1001      127   571338 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127  1638568 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
+-rw-r--r--   0     1001      127   575422 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     9973 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/js_compiler/test_javascript.py
+-rw-r--r--   0     1001      127      808 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/js_compiler/test_postcss.py
+-rw-r--r--   0     1001      127     2823 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/js_compiler/test_source_maps.py
+-rw-r--r--   0     1001      127     1236 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_annotation_helpers.py
+-rw-r--r--   0     1001      127     9460 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_app.py
+-rw-r--r--   0     1001      127      734 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_cache.py
+-rw-r--r--   0     1001      127     5304 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      494 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_config.py
+-rw-r--r--   0     1001      127     6824 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_controller.py
+-rw-r--r--   0     1001      127     1126 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_controller_layout.py
+-rw-r--r--   0     1001      127     3239 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_cropper.py
+-rw-r--r--   0     1001      127     1227 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_exceptions.py
+-rw-r--r--   0     1001      127     1924 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_logging.py
+-rw-r--r--   0     1001      127     8494 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_paths.py
+-rw-r--r--   0     1001      127     2667 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_ssr.py
+-rw-r--r--   0     1001      127     3177 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/__tests__/test_watch.py
+-rw-r--r--   0     1001      127      397 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/actions/__init__.py
+-rw-r--r--   0     1001      127    13033 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/actions/fields.py
+-rw-r--r--   0     1001      127     6847 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/actions/passthrough.py
+-rw-r--r--   0     1001      127    12023 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/actions/sideeffect.py
+-rw-r--r--   0     1001      127     4352 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/annotation_helpers.py
+-rw-r--r--   0     1001      127    22160 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/app.py
+-rw-r--r--   0     1001      127     3216 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/cache.py
+-rw-r--r--   0     1001      127    19195 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/cli.py
+-rw-r--r--   0     1001      127    11390 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/client_builder/build_actions.py
+-rw-r--r--   0     1001      127     4002 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/client_builder/build_links.py
+-rw-r--r--   0     1001      127    10172 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/client_builder/build_schemas.py
+-rw-r--r--   0     1001      127    30715 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/client_builder/builder.py
+-rw-r--r--   0     1001      127    11199 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/client_builder/openapi.py
+-rw-r--r--   0     1001      127     5070 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/client_builder/typescript.py
+-rw-r--r--   0     1001      127     2424 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/config.py
+-rw-r--r--   0     1001      127      197 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/console.py
+-rw-r--r--   0     1001      127       40 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/constants.py
+-rw-r--r--   0     1001      127    16758 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/controller.py
+-rw-r--r--   0     1001      127      881 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/controller_layout.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/controllers/__init__.py
+-rw-r--r--   0     1001      127     1216 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/controllers/exception_controller.py
+-rw-r--r--   0     1001      127    10359 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/cropper.py
+-rw-r--r--   0     1001      127      327 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/database/__init__.py
+-rw-r--r--   0     1001      127     1866 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/database/cli.py
+-rw-r--r--   0     1001      127     1822 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/database/config.py
+-rw-r--r--   0     1001      127      133 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127     3188 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/database/dependencies/core.py
+-rw-r--r--   0     1001      127     7969 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/database/sqlmodel.py
+-rw-r--r--   0     1001      127     8737 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/database/validator.py
+-rw-r--r--   0     1001      127      251 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/dependencies/__init__.py
+-rw-r--r--   0     1001      127     5122 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/dependencies/base.py
+-rw-r--r--   0     1001      127      116 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/dependencies/core/__init__.py
+-rw-r--r--   0     1001      127     1069 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/dependencies/core/core.py
+-rw-r--r--   0     1001      127     3317 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/exceptions.py
+-rw-r--r--   0     1001      127     1188 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/io.py
+-rw-r--r--   0     1001      127        1 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     1731 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/js_compiler/base.py
+-rw-r--r--   0     1001      127      199 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/js_compiler/exceptions.py
+-rw-r--r--   0     1001      127    17413 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/js_compiler/javascript.py
+-rw-r--r--   0     1001      127     4163 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/js_compiler/postcss.py
+-rw-r--r--   0     1001      127     5614 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/js_compiler/source_maps.py
+-rw-r--r--   0     1001      127     2313 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/logging.py
+-rw-r--r--   0     1001      127    13337 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/paths.py
+-rw-r--r--   0     1001      127        0 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/py.typed
+-rw-r--r--   0     1001      127     5816 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/render.py
+-rw-r--r--   0     1001      127     3237 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/ssr.py
+-rw-r--r--   0     1001      127      210 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/static/__init__.py
+-rw-r--r--   0     1001      127     6454 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/static/api.ts
+-rw-r--r--   0     1001      127     3976 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/static/live_reload.ts
+-rw-r--r--   0     1001      127      323 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/static/ssr_polyfills.js
+-rw-r--r--   0     1001      127     7261 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/test_utilities.py
+-rw-r--r--   0     1001      127      213 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/views/__init__.py
+-rw-r--r--   0     1001      127      432 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/views/core/exception/page.tsx
+-rw-r--r--   0     1001      127      178 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/views/core/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/views/core/main.css
+-rw-r--r--   0     1001      127     1478 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/views/package-lock.json
+-rw-r--r--   0     1001      127      257 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/views/package.json
+-rw-r--r--   0     1001      127       83 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/views/postcss.config.js
+-rw-r--r--   0     1001      127      162 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/views/tailwind.config.js
+-rw-r--r--   0     1001      127     8427 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/watch.py
+-rw-r--r--   0     1001      127     4062 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/watch_server.py
+-rw-r--r--   0     1001      127     1213 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/mountaineer/webservice.py
+-rw-r--r--   0     1001      127   127639 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/poetry.lock
+-rw-r--r--   0     1001      127   453080 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/benches/fixtures/complex_sourcemap_mapping.txt
+-rw-r--r--   0     1001      127   575422 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/benches/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127      322 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/benches/fixtures/ssr_polyfill_archive.js
+-rw-r--r--   0     1001      127      899 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/benches/lexers_benchmark.rs
+-rw-r--r--   0     1001      127     1089 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/benches/source_map_benchmark.rs
+-rw-r--r--   0     1001      127     1595 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/benches/ssr_benchmark.rs
+-rw-r--r--   0     1001      127      499 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/errors.rs
+-rw-r--r--   0     1001      127     4648 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/lexers.rs
+-rw-r--r--   0     1001      127     9118 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/lib.rs
+-rw-r--r--   0     1001      127      680 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/logging.rs
+-rw-r--r--   0     1001      127    17549 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/source_map.rs
+-rw-r--r--   0     1001      127    15113 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/ssr.rs
+-rw-r--r--   0     1001      127     3998 2024-05-01 23:34:00.000000 mountaineer-0.5.0.dev1/src/timeout.rs
+-rw-r--r--   0     1001      127    32093 2024-05-01 23:34:16.000000 mountaineer-0.5.0.dev1/Cargo.lock
+-rw-r--r--   0     1001      127     1624 2024-05-01 23:34:13.000000 mountaineer-0.5.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.5.0.dev1/PKG-INFO
```

### Comparing `mountaineer-0.4.2.dev3/src_go/build.rs` & `mountaineer-0.5.0.dev1/src_go/build.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src_go/go/js_build.go` & `mountaineer-0.5.0.dev1/src_go/go/js_build.go`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src_go/src/lib.rs` & `mountaineer-0.5.0.dev1/src_go/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/Cargo.toml` & `mountaineer-0.5.0.dev1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [[bench]]
 path = "src/benches/lexers_benchmark.rs"
 name = "lexers_benchmark"
 harness = false
 
 [package]
 name = "mountaineer"
-version = "0.4.2-dev3"
+version = "0.5.0-dev1"
 edition = "2021"
 
 [dependencies]
 v8 = "0.89.0"
 deno_core_icudata = "0.73.0"
 lazy_static = "1.4.0"
 serde_json = "1.0"
```

### Comparing `mountaineer-0.4.2.dev3/.github/poetry.lock` & `mountaineer-0.5.0.dev1/.github/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/.github/pyproject.toml` & `mountaineer-0.5.0.dev1/.github/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/.github/scripts/__tests__/test_update_version.py` & `mountaineer-0.5.0.dev1/.github/scripts/__tests__/test_update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/.github/scripts/check_dependencies.py` & `mountaineer-0.5.0.dev1/.github/scripts/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/.github/scripts/update_version.py` & `mountaineer-0.5.0.dev1/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/.github/workflows/publish_docs.yml` & `mountaineer-0.5.0.dev1/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/.github/workflows/test.yml` & `mountaineer-0.5.0.dev1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/.gitignore` & `mountaineer-0.5.0.dev1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,15 @@
 !*/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
 
 # We don't commit our automatically managed files - you can in your project, but these
 # change so much we'd like to avoid them in code reviews.
 _server
 _ssr
 _static
+_metadata
 
 # Ignore template files that might be used locally for testing
 # but shouldn't be added to the downstream templates
 **/create_mountaineer_app/templates/poetry.lock
 
 .DS_Store
```

### Comparing `mountaineer-0.4.2.dev3/Dockerfile` & `mountaineer-0.5.0.dev1/Dockerfile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/LICENSE` & `mountaineer-0.5.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/Makefile` & `mountaineer-0.5.0.dev1/Makefile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/README.md` & `mountaineer-0.5.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/benchmarking/poetry.lock` & `mountaineer-0.5.0.dev1/benchmarking/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/README.md` & `mountaineer-0.5.0.dev1/ci_webapp/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/app.py` & `mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from mountaineer import AppController, LinkAttribute, Metadata
 from mountaineer.js_compiler.postcss import PostCSSBundler
 
 from ci_webapp.config import AppConfig
 from ci_webapp.controllers.complex import ComplexController
 from ci_webapp.controllers.detail import DetailController
 from ci_webapp.controllers.home import HomeController
+from ci_webapp.controllers.root_layout import RootLayoutController
 from ci_webapp.controllers.stream import StreamController
 
 controller = AppController(
     global_metadata=Metadata(
         links=[LinkAttribute(rel="stylesheet", href="/static/app_main.css")]
     ),
     custom_builders=[
@@ -16,7 +17,8 @@
     ],
     config=AppConfig(),
 )
 controller.register(HomeController())
 controller.register(DetailController())
 controller.register(ComplexController())
 controller.register(StreamController())
+controller.register(RootLayoutController())
```

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/complex.py` & `mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/controllers/complex.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/detail.py` & `mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/home.py` & `mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/stream.py` & `mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/controllers/stream.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/complex/page.tsx` & `mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/app/complex/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/home/page.tsx` & `mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/stream/page.tsx` & `mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/app/stream/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/package-lock.json` & `mountaineer-0.5.0.dev1/ci_webapp/ci_webapp/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/poetry.lock` & `mountaineer-0.5.0.dev1/ci_webapp/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/ci_webapp/pyproject.toml` & `mountaineer-0.5.0.dev1/ci_webapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/README.md` & `mountaineer-0.5.0.dev1/create_mountaineer_app/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/common.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/builder.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/cli.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/base.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/poetry.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/venv.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/external.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/generation.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # General Javascript excludes
 node_modules
 
 # Exclude files generated by mountaineer
 _server
 _ssr
 _static
+_metadata
 .watchdog.lock
 
 # General Python excludes
 # see: https://github.com/github/gitignore/blob/main/Python.gitignore
 #
 # Byte-compiled / optimized / DLL files
 __pycache__/
```

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/README.md` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml` & `mountaineer-0.5.0.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/poetry.lock` & `mountaineer-0.5.0.dev1/create_mountaineer_app/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/create_mountaineer_app/pyproject.toml` & `mountaineer-0.5.0.dev1/create_mountaineer_app/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/client_actions.md` & `mountaineer-0.5.0.dev1/docs_website/docs/client_actions.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/cma.md` & `mountaineer-0.5.0.dev1/docs_website/docs/cma.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/database.md` & `mountaineer-0.5.0.dev1/docs_website/docs/database.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/deploy.md` & `mountaineer-0.5.0.dev1/docs_website/docs/deploy.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 First, add the following to your `.dockerignore` file. This will prevent Docker from trying to copy over heavy artifacts that aren't needed for the build.
 
 ```title=".dockerignore"
 **/node_modules
 **/_server
 **/_ssr
 **/_static
+**/_metadata
 ```
 
 ### Image 1: Frontend Dependencies
 
 Our first stage uses `npm` to fetch your frontend dependencies. This is an isolated context since it's the only place we need node / npm in the build pipeline.
 
 ```docker
```

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/error_handling.md` & `mountaineer-0.5.0.dev1/docs_website/docs/error_handling.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/index.md` & `mountaineer-0.5.0.dev1/docs_website/docs/index.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/internal/core_library.md` & `mountaineer-0.5.0.dev1/docs_website/docs/internal/core_library.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/links.md` & `mountaineer-0.5.0.dev1/docs_website/docs/links.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/media/final_todo_list.png` & `mountaineer-0.5.0.dev1/docs_website/docs/media/final_todo_list.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/media/ide_typehints.png` & `mountaineer-0.5.0.dev1/docs_website/docs/media/ide_typehints.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/media/network_debug.png` & `mountaineer-0.5.0.dev1/docs_website/docs/media/network_debug.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/media/server_side_rendering.png` & `mountaineer-0.5.0.dev1/docs_website/docs/media/server_side_rendering.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/metadata.md` & `mountaineer-0.5.0.dev1/docs_website/docs/metadata.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/postcss.md` & `mountaineer-0.5.0.dev1/docs_website/docs/postcss.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/quickstart.md` & `mountaineer-0.5.0.dev1/docs_website/docs/quickstart.md`

 * *Files 1% similar despite different names*

```diff
@@ -290,14 +290,14 @@
 export default Home;
 ```
 
 `useServer()` exposes our `add_todo` function so we can call our backend directly from our frontend. Also notice that we don't have to read or parse the output value of this function to render the new todo item to the list. Since the function is marked as a sideeffect, the frontend will automatically refresh its data after the function is called.
 
 Go ahead and load it in your browser. If you open up your web tools, you can create a new Todo and see POST requests sending data to the backend and receiving the current server state. The actual data updates and merging happens internally by Mountaineer.
 
-![Getting Started Final TODO App](/media/final_todo_list.png){ height="400" }
+![Getting Started Final TODO App](media/final_todo_list.png){ height="400" }
 
-![Getting Started Final TODO App](/media/network_debug.png){ height="400" }
+![Getting Started Final TODO App](media/network_debug.png){ height="400" }
 
 You can use these serverState variables anywhere you'd use dynamic React state variables (useEffect, useCallback, etc). But unlike React state, these variables are automatically updated when a relevant sideeffect is triggered.
 
 And that's it. We've just built a fully interactive web application without having to worry about an explicit API. You specify the data model and actions on the server and the appropriate frontend hooks are generated and updated automatically. It gives you the power of server rendered html and the interactivity of a virtual DOM, without having to compromise on complicated data mutations to keep everything in sync.
```

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/static_analysis.md` & `mountaineer-0.5.0.dev1/docs_website/docs/static_analysis.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/structure.md` & `mountaineer-0.5.0.dev1/docs_website/docs/structure.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/docs/stylesheets/extra.css` & `mountaineer-0.5.0.dev1/docs_website/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/mkdocs.yml` & `mountaineer-0.5.0.dev1/docs_website/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/docs_website/poetry.lock` & `mountaineer-0.5.0.dev1/docs_website/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/media/header.png` & `mountaineer-0.5.0.dev1/media/header.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__init__.py` & `mountaineer-0.5.0.dev1/mountaineer/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # be used across projects
 from fastapi import Depends as Depends
 
 from mountaineer.actions import passthrough as passthrough, sideeffect as sideeffect
 from mountaineer.app import AppController as AppController
 from mountaineer.config import ConfigBase as ConfigBase
 from mountaineer.controller import ControllerBase as ControllerBase
+from mountaineer.controller_layout import LayoutControllerBase as LayoutControllerBase
 from mountaineer.dependencies import CoreDependencies as CoreDependencies
 from mountaineer.exceptions import APIException as APIException
 from mountaineer.js_compiler.postcss import PostCSSBundler as PostCSSBundler
 from mountaineer.paths import ManagedViewPath as ManagedViewPath
 from mountaineer.render import (
     LinkAttribute as LinkAttribute,
     MetaAttribute as MetaAttribute,
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_fields.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/actions/test_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import AsyncIterator, Iterator, Optional, Type
+from typing import AsyncIterator, Iterator, Optional, Type, cast
 
 import pytest
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel
 from pydantic.fields import FieldInfo
 
 from mountaineer.actions.fields import (
@@ -11,26 +11,32 @@
     ResponseModelType,
     annotation_is_metadata,
     extract_response_model_from_signature,
     fuse_metadata_to_response_typehint,
     get_function_metadata,
 )
 from mountaineer.actions.sideeffect import sideeffect
+from mountaineer.controller import ControllerBase
 from mountaineer.render import Metadata, RenderBase
 
 
 class ExampleRenderModel(RenderBase):
     render_value_a: str
     render_value_b: int
 
 
 class ExamplePassthroughModel(BaseModel):
     passthrough_value_a: str
 
 
+class ExampleController(ControllerBase):
+    async def render(self) -> None:
+        pass
+
+
 def basic_compare_model_fields(
     actual: dict[str, FieldInfo],
     expected: dict[str, FieldInfo],
 ):
     """
     FieldInfo objects can't be compared with native Python comparitors.
 
@@ -109,16 +115,24 @@
 def test_fuse_metadata_to_response_typehint(
     metadata: FunctionMetadata,
     render_model: Type[RenderBase],
     expected_model_name: str,
     expected_sideeffect_fields: dict[str, FieldInfo],
     expected_passthrough_fields: dict[str, FieldInfo],
 ):
-    fused_model = fuse_metadata_to_response_typehint(metadata, render_model)
+    sample_controller = ExampleController()
+    raw_model = fuse_metadata_to_response_typehint(
+        metadata, sample_controller, render_model
+    )
 
+    assert "ExampleController" in raw_model.model_fields.keys()
+
+    fused_model = cast(
+        BaseModel, raw_model.model_fields["ExampleController"].annotation
+    )
     if expected_sideeffect_fields:
         assert "sideeffect" in fused_model.model_fields.keys()
         assert fused_model.model_fields["sideeffect"].annotation
         basic_compare_model_fields(
             fused_model.model_fields["sideeffect"].annotation.model_fields,
             expected_sideeffect_fields,
         )
@@ -127,40 +141,41 @@
         assert "passthrough" in fused_model.model_fields.keys()
         assert fused_model.model_fields["passthrough"].annotation
         basic_compare_model_fields(
             fused_model.model_fields["passthrough"].annotation.model_fields,
             expected_passthrough_fields,
         )
 
-    assert fused_model.__name__ == expected_model_name
+    assert raw_model.__name__ == expected_model_name
 
 
 class ParentRender(RenderBase):
     render_value_a: str
 
 
 class ChildRender(ParentRender):
     render_value_b: int
 
 
 def test_fuse_metadata_to_response_typehint_inherit_render():
-    class ParentController(BaseModel):
+    class ParentController(ControllerBase):
         def render(self) -> ParentRender:
             return ParentRender(render_value_a="example")
 
         @sideeffect(reload=(ParentRender.render_value_a,))
         def sideeffect(self) -> None:
             pass
 
     class ChildController(ParentController):
         def render(self) -> ChildRender:
             return ChildRender(render_value_a="example", render_value_b=1)
 
     model_fused = fuse_metadata_to_response_typehint(
         get_function_metadata(ChildController.sideeffect),
+        ChildController(),
         ChildRender,
     )
     assert set(
         model_fused.model_json_schema()["$defs"]["SideeffectResponseSideEffect"][
             "properties"
         ].keys()
     ) == {"render_value_a"}
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_passthrough.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/actions/test_passthrough.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,17 +96,19 @@
 
     return_value_async = await controller.call_passthrough_async(
         {},
     )
 
     # The response payload should be the same both both sync and async endpoints
     expected_response = {
-        "passthrough": ExamplePassthroughModel(
-            status="success",
-        )
+        "TestController": {
+            "passthrough": ExamplePassthroughModel(
+                status="success",
+            )
+        }
     }
 
     assert return_value_sync == expected_response
     assert return_value_async == expected_response
 
     assert controller.counter == 2
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_sideeffect.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/actions/test_sideeffect.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,19 +97,21 @@
         return_value_async = await controller.call_sideeffect_async(
             {},
             request=Request({"type": "http"}),  # type: ignore
         )
 
         # The response payload should be the same both both sync and async endpoints
         expected_response = {
-            "sideeffect": ExampleRenderModel(
-                value_a="Hello",
-                value_b="World",
-            ),
-            "passthrough": None,
+            controller.__class__.__name__: {
+                "sideeffect": ExampleRenderModel(
+                    value_a="Hello",
+                    value_b="World",
+                ),
+                "passthrough": None,
+            }
         }
 
         assert return_value_sync == expected_response
         assert return_value_async == expected_response
 
         assert controller.counter == 2
         assert controller.render_counts == 2
@@ -273,16 +275,18 @@
             # From the original view page that is calling this sub-function
             "referer": "http://example.com/test/5/",
         },
     )
     elapsed = (monotonic_ns() - start) / 1e9
     assert response.status_code == 200
     assert response.json() == {
-        "sideeffect": {
-            "value_a": "Hello 1229",
+        "ExampleController": {
+            "sideeffect": {
+                "value_a": "Hello 1229",
+            }
         }
     }
 
     LOGGER.info(f"Use Experimental: {use_experimental}\nElapsed: {elapsed}")
 
     if min_time is not None:
         assert elapsed >= min_time
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_actions.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/test_build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_links.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/test_build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_schemas.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/test_build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_builder.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/test_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from tempfile import TemporaryDirectory
 
 import pytest
 
 from mountaineer.app import AppController
 from mountaineer.client_builder.builder import ClientBuilder
 from mountaineer.controller import ControllerBase
+from mountaineer.controller_layout import LayoutControllerBase
 
 
 class ExampleHomeController(ControllerBase):
     url = "/"
     view_path = "/page.tsx"
 
     def render(self) -> None:
@@ -165,7 +166,55 @@
                 },
             },
             sort_keys=True,
         )
     )
 
     assert builder.cache_is_outdated() is True
+
+
+def test_validate_unique_paths_exact_definition(
+    builder: ClientBuilder,
+):
+    """
+    Two controllers can't manage the same view path.
+
+    """
+
+    class ConflictingDetailController(ControllerBase):
+        url = "/detail/other_url/"
+        view_path = "/detail/page.tsx"
+
+        def render(self) -> None:
+            return None
+
+    builder.app.register(ConflictingDetailController())
+
+    # Raises for the same exact view path
+    with pytest.raises(
+        ValueError, match="duplicate view paths under controller management"
+    ):
+        builder.validate_unique_paths()
+
+
+def test_validate_unique_paths_conflicting_layout(
+    builder: ClientBuilder,
+):
+    """
+    Layouts need to be placed in their own directory. Even if the literal paths
+    under management are different we still need to throw a validation error.
+
+    """
+
+    class ConflictingLayoutController(LayoutControllerBase):
+        view_path = "/detail/layout.tsx"
+
+        def render(self) -> None:
+            return None
+
+    builder.app.register(ConflictingLayoutController())
+
+    # Raises for the same exact view path
+    with pytest.raises(
+        ValueError, match="duplicate view paths under controller management"
+    ):
+        builder.validate_unique_paths()
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_typescript.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/client_builder/test_typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/database/dependencies/test_core.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/database/dependencies/test_core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/database/test_config.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/database/test_config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/database/test_sqlmodel.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/database/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/dependencies/test_base.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/dependencies/test_base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/home_controller_source_map.js.map` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/fixtures/home_controller_source_map.js.map`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_javascript.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/js_compiler/test_javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_postcss.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/js_compiler/test_postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_source_maps.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/js_compiler/test_source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_annotation_helpers.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_app.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_app.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pydantic import BaseModel
 
 from mountaineer.actions import passthrough
 from mountaineer.app import AppController
 from mountaineer.client_builder.openapi import OpenAPIDefinition
 from mountaineer.config import ConfigBase
 from mountaineer.controller import ControllerBase
+from mountaineer.controller_layout import LayoutControllerBase
 from mountaineer.exceptions import APIException
 
 
 def test_requires_render_return_value():
     """
     The AppController is in charge of validating our render return value. Since renders are not
     decorated, the best place to validate is during a mount.
@@ -39,14 +40,34 @@
     app = AppController(view_root=Path(""))
     with pytest.raises(ValueError, match="must have a return type annotation"):
         app.register(TestControllerWithoutRenderMarkup())
 
     app.register(TestControllerWithRenderMarkup())
 
 
+def test_validates_layouts_exclude_urls():
+    """
+    The app controller should reject the registration of layouts that specify
+    a url.
+
+    """
+
+    class TestLayoutController(LayoutControllerBase):
+        # Not allowed, but might typehint correctly because the ControllerBase
+        # superclass supports it.
+        url = "/layout_url"
+
+        async def render(self) -> None:
+            pass
+
+    app_controller = AppController(view_root=Path(""))
+    with pytest.raises(ValueError, match="are not directly mountable to the router"):
+        app_controller.register(TestLayoutController())
+
+
 def test_generate_openapi():
     class ExampleSubModel(BaseModel):
         sub_value: str
 
     class ExampleException(APIException):
         status_code = 401
         invalid_reason: str
@@ -68,14 +89,15 @@
     openapi_spec = app.generate_openapi()
     openapi_definition = OpenAPIDefinition(**openapi_spec)
 
     assert openapi_definition.components.schemas.keys() == {
         "TestExceptionActionResponse",
         "ExampleException",
         "ExampleSubModel",
+        "TestExceptionActionResponseRaw",
     }
 
 
 def test_format_exception_model():
     class ExampleException(APIException):
         status_code = 401
         value: str
@@ -129,14 +151,15 @@
     app.register(ExampleController())
 
     openapi_spec = app.generate_openapi()
     openapi_definition = OpenAPIDefinition(**openapi_spec)
 
     assert openapi_definition.components.schemas.keys() == {
         "TestExceptionActionResponse",
+        "TestExceptionActionResponseRaw",
         "mountaineer.__tests__.test_1.ExampleException",
         "mountaineer.__tests__.test_2.ExampleException",
     }
 
 
 def test_inherit_parent_spec():
     """
@@ -195,14 +218,17 @@
         .responses
     )
 
     # Test that the controller definitions remain separate
     assert parent_controller.definition
     assert child_controller.definition
 
+    assert parent_controller.definition.render_router
+    assert child_controller.definition.render_router
+
     parent_routes = parent_controller.definition.render_router.routes
     child_routes = child_controller.definition.render_router.routes
 
     assert len(parent_routes) == 1
     assert parent_routes[0].path == "/parent"  # type: ignore
     assert len(child_routes) == 1
     assert child_routes[0].path == "/child"  # type: ignore
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cache.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cli.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     def post(content: EchoModel):
         return content
 
     with TestClient(app=app, raise_server_exceptions=False) as test_client:
         response = test_client.get("/")
         assert response.status_code == 500
         assert (
-            '<div id="root">Passthrough: {"exception":"This is a test",'
+            '<div id="root">Passthrough: {"ExceptionController":{"exception":"This is a test",'
             in response.text
         )
 
         response = test_client.post("/api", json={"value": 123})
         assert response.status_code == 422
         assert response.json() == {
             "detail": [
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_controller.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 import pytest
 
-from mountaineer.controller import ControllerBase
+from mountaineer.controller import BuildMetadata, ControllerBase
 from mountaineer.render import (
     LinkAttribute,
     MetaAttribute,
     Metadata,
     RenderBase,
     ScriptAttribute,
     ThemeColorMeta,
@@ -192,14 +192,15 @@
     assert controller._merge_metadatas(metadatas) == expected_metadata
 
 
 def test_resolve_paths(tmp_path: Path):
     view_base = tmp_path / "views"
     ssr_base = view_base / "_ssr"
     static_base = view_base / "_static"
+    metadata_base = view_base / "_metadata"
 
     controller = StubController()
     assert not controller.resolve_paths(view_base)
 
     # Now create an actual view path that we can sniff
     # This will get further in the pipeline but still won't be valid
     # because we don't have any of the global script files
@@ -208,19 +209,25 @@
 
     # Now we create the SSR script file
     ssr_base.mkdir()
     (ssr_base / "stub_controller.js").touch()
     (ssr_base / "stub_controller.js.map").touch()
     assert not controller.resolve_paths(view_base)
 
-    # Finally, create the static script file
     # Our hash has to be exactly 32 digits to match the regex
     static_base.mkdir()
     random_hash = "b5ecd0c4405374100d6ef93088b86898"
     (static_base / f"stub_controller-{random_hash}.js").touch()
     (static_base / f"stub_controller-{random_hash}.js.map").touch()
+    assert not controller.resolve_paths(view_base)
+
+    # Finally, create the metadata file
+    metadata_base.mkdir()
+    (metadata_base / "stub_controller.json").write_text(
+        BuildMetadata(view_path=Path()).model_dump_json()
+    )
     assert controller.resolve_paths(view_base)
 
     # Now ensure that the paths are correctly set
     assert controller.view_base_path == view_base
     assert controller.ssr_path == ssr_base / "stub_controller.js"
     assert controller.bundled_scripts == [f"stub_controller-{random_hash}.js"]
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cropper.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_exceptions.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_logging.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_paths.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     Ensure that the paths can correctly derive the managed folders.
 
     """
     root_path = ManagedViewPath.from_view_root(tmpdir)
     assert root_path.get_managed_code_dir() == root_path / "_server"
     assert root_path.get_managed_static_dir() == root_path / "_static"
     assert root_path.get_managed_ssr_dir() == root_path / "_ssr"
+    assert root_path.get_managed_metadata_dir() == root_path / "_metadata"
 
     # Non-root paths should only yield the server directory
     non_root_path = root_path / "subdir"
     non_root_path.mkdir()
 
     assert non_root_path.get_managed_code_dir() == root_path / "subdir" / "_server"
     with pytest.raises(ValueError):
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_ssr.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_ssr.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             "frozen": True,
         }
 
     for _ in range(50):
         start = monotonic_ns()
         render_ssr(
             js_contents,
-            FakeModel(random_id=uuid4()),
+            FakeModel(random_id=uuid4()).model_dump(mode="json"),
             hard_timeout=1,
         )
         all_measurements.append((monotonic_ns() - start) / 1e9)
 
     assert max(all_measurements) < 0.5
 
 
@@ -50,15 +50,17 @@
             "frozen": True,
         }
 
     start = monotonic_ns()
     with pytest.raises(TimeoutError):
         render_ssr(
             script=js_contents,
-            render_data=FakeWaitDurationModel(delay_loops=5, random_id=uuid4()),
+            render_data=FakeWaitDurationModel(
+                delay_loops=5, random_id=uuid4()
+            ).model_dump(mode="json"),
             hard_timeout=0.5,
         )
     assert ((monotonic_ns() - start) / 1e9) < 1.0
 
 
 def test_ssr_exception_context():
     """
@@ -80,15 +82,15 @@
     };
     """
 
     # with pytest.raises(V8RuntimeError, match="custom_error_text"):
     try:
         render_ssr(
             script=js_contents,
-            render_data=FakeModel(random_id=uuid4()),
+            render_data=FakeModel(random_id=uuid4()).model_dump(mode="json"),
             hard_timeout=0,
         )
     except V8RuntimeError as e:
         assert re_sub(r"\s+", "", str(e)) == (
             re_sub(
                 r"\s+",
                 "",
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_watch.py` & `mountaineer-0.5.0.dev1/mountaineer/__tests__/test_watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/actions/fields.py` & `mountaineer-0.5.0.dev1/mountaineer/actions/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from enum import Enum
 from inspect import (
     isclass,
     ismethod,
 )
 from json import loads as json_loads
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Optional,
     Type,
     get_args,
     get_origin,
 )
@@ -23,14 +24,17 @@
 from pydantic import BaseModel, create_model
 from pydantic.fields import FieldInfo
 
 from mountaineer.annotation_helpers import MountaineerUnsetValue
 from mountaineer.exceptions import APIException
 from mountaineer.render import FieldClassDefinition, Metadata, RenderBase, RenderNull
 
+if TYPE_CHECKING:
+    from mountaineer.controller import ControllerBase
+
 
 class FunctionActionType(Enum):
     RENDER = "render"
     SIDEEFFECT = "sideeffect"
     PASSTHROUGH = "passthrough"
 
 
@@ -147,14 +151,15 @@
         return
 
     return annotation == Metadata or annotation == Optional[Metadata]
 
 
 def fuse_metadata_to_response_typehint(
     metadata: FunctionMetadata,
+    controller: "ControllerBase",
     render_model: Type[RenderBase] | None,
 ) -> Type[BaseModel]:
     """
     Functions can either be marked up with side effects, explicit responses, or both.
     This function merges them into the expected output payload so we can typehint the responses.
     """
     passthrough_fields = {}
@@ -224,21 +229,30 @@
                     for field_name, field_definition in sideeffect_fields.items()
                 },
             ),
             FieldInfo(alias="sideeffect"),
         )
 
     model: Type[BaseModel] = create_model(
-        base_response_name,
+        base_response_name + "Raw",
         **base_response_params,  # type: ignore
     )
-    return model
 
+    # Each action also includes the controller type in the response
+    # signature so the frontend can differentiate between different controllers
+    wrapper_model: Type[BaseModel] = create_model(
+        base_response_name,
+        **{controller.__class__.__name__: (model, FieldInfo())},  # type: ignore
+    )
 
-def handle_explicit_responses(
+    return wrapper_model
+
+
+def format_final_action_response(
+    controller: "ControllerBase",
     dict_payload: dict[str, Any],
 ):
     """
     Wrapper to allow actions to respond with an explicit JSONResponse, or a dictionary. This lets
     both sideeffects and passthrough payloads to inject header metadata that otherwise can't be captured
     in a regular BaseModel.
 
@@ -251,23 +265,27 @@
         for key, response in dict_payload.items()
         if isinstance(response, JSONResponse)
     ]
 
     if len(responses) > 1:
         raise ValueError(f"Multiple conflicting responses returned: {responses}")
 
+    # The final transformation should include our controller name
+    # This signals to the frontend which state subset we want to update
+    action_root = controller.__class__.__name__
+
     if len(responses) == 0:
-        return dict_payload
+        return {action_root: dict_payload}
 
     response_key, response = responses[0]
     dict_payload[response_key] = json_loads(response.body)
 
     # Now inject the newly formatted response into the response object
     return JSONResponse(
-        content=dict_payload,
+        content={action_root: dict_payload},
         status_code=response.status_code,
         headers={
             key: value
             for key, value in response.headers.items()
             if key not in {"content-length", "content-type"}
         },
     )
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/actions/passthrough.py` & `mountaineer-0.5.0.dev1/mountaineer/actions/passthrough.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from fastapi.responses import JSONResponse, Response, StreamingResponse
 from pydantic import BaseModel
 
 from mountaineer.actions.fields import (
     FunctionActionType,
     ResponseModelType,
     extract_response_model_from_signature,
-    handle_explicit_responses,
+    format_final_action_response,
     init_function_metadata,
 )
 from mountaineer.constants import STREAM_EVENT_TYPE
 from mountaineer.exceptions import APIException
 
 if TYPE_CHECKING:
     from mountaineer.controller import ControllerBase
@@ -153,15 +153,15 @@
 
                 if raw_response:
                     return response
 
                 if isasyncgen(response):
                     return wrap_passthrough_generator(response)
 
-                return handle_explicit_responses(dict(passthrough=response))
+                return format_final_action_response(self, dict(passthrough=response))
 
             metadata = init_function_metadata(inner, FunctionActionType.PASSTHROUGH)
             metadata.passthrough_model = passthrough_model
             metadata.exception_models = exception_models
             metadata.is_raw_response = raw_response or False
             metadata.media_type = (
                 STREAM_EVENT_TYPE
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/actions/sideeffect.py` & `mountaineer-0.5.0.dev1/mountaineer/actions/sideeffect.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 from pydantic import BaseModel
 from starlette.routing import Match
 
 from mountaineer.actions.fields import (
     FunctionActionType,
     ResponseModelType,
     extract_response_model_from_signature,
-    handle_explicit_responses,
+    format_final_action_response,
     init_function_metadata,
 )
+from mountaineer.controller_layout import LayoutControllerBase
 from mountaineer.cropper import crop_function_for_return_keys
 from mountaineer.dependencies import get_function_dependencies
 from mountaineer.exceptions import APIException
 from mountaineer.render import FieldClassDefinition
 
 if TYPE_CHECKING:
     from mountaineer.controller import ControllerBase
@@ -165,19 +166,20 @@
                     # For this we rely on the Referrer header that is sent on the fetch(). Note that this
                     # referrer can be spoofed, so it assumes that the endpoint also internally validates
                     # the caller has correct permissions to access the data.
                     server_data = render_fn(**values)
                     if isawaitable(server_data):
                         server_data = await server_data
 
-                    return handle_explicit_responses(
+                    return format_final_action_response(
+                        self,
                         dict(
                             sideeffect=server_data,
                             passthrough=passthrough_values,
-                        )
+                        ),
                     )
 
             # Update the signature of 'inner' to include 'request: Request'
             # We need to modify this to conform to the request parameters that are sniffed
             # when the component is mounted
             # https://github.com/tiangolo/fastapi/blob/a235d93002b925b0d2d7aa650b7ab6d7bb4b24dd/fastapi/dependencies/utils.py#L250
             sig = signature(inner)
@@ -249,29 +251,39 @@
         )
 
     # Follow starlette's original logic to resolve routes, since this provides us the necessary
     # metadata about URL paths. Unlike in the general-purpose URL resolution case, however,
     # we already know which route should be resolved so we can shortcut having to
     # match non-relevant paths.
     # https://github.com/encode/starlette/blob/5c43dde0ec0917673bb280bcd7ab0c37b78061b7/starlette/routing.py#L544
-    for route in controller.definition.render_router.routes:
+    for route in (
+        controller.definition.render_router.routes
+        if controller.definition.render_router is not None
+        else []
+    ):
         match, child_scope = route.matches(view_request.scope)
         if match != Match.FULL:
             raise RuntimeError(
                 f"Route {route} did not match ({match}) {view_request.scope}"
             )
         view_request.scope = {
             **view_request.scope,
             "path_params": {},
             "query_string": "",
             **child_scope,
         }
 
     try:
         async with get_function_dependencies(
-            callable=controller.render, url=controller.url, request=view_request
+            callable=controller.render,
+            url=controller.url
+            if not isinstance(controller, LayoutControllerBase)
+            else None,
+            request=view_request
+            if not isinstance(controller, LayoutControllerBase)
+            else None,
         ) as values:
             yield values
     except RuntimeError as e:
         raise RuntimeError(
             f"Error occurred while resolving dependencies for render(): {controller}: {e}"
         ) from e
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/annotation_helpers.py` & `mountaineer-0.5.0.dev1/mountaineer/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/app.py` & `mountaineer-0.5.0.dev1/mountaineer/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import defaultdict
 from functools import wraps
-from inspect import isclass, signature
+from inspect import isawaitable, isclass, signature
 from pathlib import Path
 from typing import Any, Callable, Type
 
 from fastapi import APIRouter, FastAPI, HTTPException, Request
 from fastapi.openapi.utils import get_openapi
 from fastapi.responses import JSONResponse
 from fastapi.staticfiles import StaticFiles
@@ -17,31 +17,35 @@
     fuse_metadata_to_response_typehint,
     init_function_metadata,
 )
 from mountaineer.actions.fields import FunctionMetadata
 from mountaineer.annotation_helpers import MountaineerUnsetValue
 from mountaineer.config import ConfigBase
 from mountaineer.controller import ControllerBase
+from mountaineer.controller_layout import LayoutControllerBase
+from mountaineer.dependencies.base import get_function_dependencies
 from mountaineer.exceptions import APIException, APIExceptionInternalModelBase
 from mountaineer.js_compiler.base import ClientBuilderBase
 from mountaineer.js_compiler.javascript import JavascriptBundler
 from mountaineer.logging import LOGGER
 from mountaineer.paths import ManagedViewPath, resolve_package_path
-from mountaineer.render import Metadata, RenderBase
+from mountaineer.render import Metadata, RenderBase, RenderNull
 
 
 class ControllerDefinition(BaseModel):
     controller: ControllerBase
     router: APIRouter
     # URL prefix to the root of the server
     url_prefix: str
     # Dynamically generated function that actually renders the html content
     # This is a hybrid between render() and _generate_html()
     view_route: Callable
-    render_router: APIRouter
+    # Render router is provided for all pages, only None for layouts that can't
+    # be independently rendered as a webpage
+    render_router: APIRouter | None
 
     model_config = {
         "arbitrary_types_allowed": True,
     }
 
     def get_url_for_metadata(self, metadata: FunctionMetadata):
         return f"{self.url_prefix}/{metadata.function_name.strip('/')}"
@@ -173,17 +177,61 @@
         # We need to passthrough the API of the render function to the FastAPI router so it's called properly
         # with the dependency injection kwargs
         @wraps(controller.render)
         async def generate_controller_html(*args, **kwargs):
             if self.build_exception:
                 raise self.build_exception
 
+            # Assemble all the layout controllers that will have to be rendered alongside
+            # the main controller
+            # We need access to the controller metadata to determine which layouts to render
+            if not controller.build_metadata:
+                raise ValueError("Controller metadata not built before rendering")
+
+            layout_controllers = [
+                candidate_layout_controller
+                for candidate_layout_controller in self.controllers
+                if (
+                    candidate_layout_controller.controller.build_metadata
+                    and candidate_layout_controller.controller.build_metadata.view_path
+                    in controller.build_metadata.layout_view_paths
+                )
+            ]
+
+            # Perform their initial rendering, we only need their data to hydrate
+            # the controller view
+            layout_metadata: dict[str, Any] = {}
+            for definition in layout_controllers:
+                # We won't be able to rely on fastapi to get the required params, because the function
+                # signature of the render function just applies to the page itself. We could create
+                # a synthetic signature here where they're all aggregated, but this would require us
+                # to wait until we have registered all of the layout controllers to then register the
+                # page render function - and this would come at the expense of allowing dynamic
+                # registration of page controllers. We would need to "lock" the app controller to know when
+                # we expect to have complete coverage of pages.
+                #
+                # For now we assume that the render method of layouts will specify no URL parameters
+                # and can be leveraged in an isoltaed context.
+                async with get_function_dependencies(
+                    callable=definition.controller.render, url=controller.url
+                ) as values:
+                    server_data = definition.controller.render(**values)
+                    if isawaitable(server_data):
+                        server_data = await server_data
+                    if server_data is None:
+                        server_data = RenderNull()
+
+                layout_metadata[definition.controller.__class__.__name__] = server_data
+
             try:
                 return await controller._generate_html(
-                    *args, global_metadata=self.global_metadata, **kwargs
+                    *args,
+                    global_metadata=self.global_metadata,
+                    other_render_contexts=layout_metadata,
+                    **kwargs,
                 )
             except Exception as e:
                 # If a user explicitly is raising an APIException, we don't want to log it
                 if not isinstance(e, (APIExceptionInternalModelBase, HTTPException)):
                     # Forward along the exception, just modify it to include
                     # the controller name for additional context
                     LOGGER.error(
@@ -227,17 +275,27 @@
             controller.render, FunctionActionType.RENDER
         )
         render_metadata.render_model = return_model
 
         # Register the rendering view to an isolated APIRoute, so we can keep track of its
         # the resulting router independently of the rest of the application
         # This is useful in cases where we need to do a render()->FastAPI lookup
-        view_router = APIRouter()
-        view_router.get(controller.url)(generate_controller_html)
-        self.app.include_router(view_router)
+        #
+        # We only mount standard controllers, we don't expect LayoutControllers to have
+        # a directly accessible URL
+        if isinstance(controller, LayoutControllerBase):
+            if hasattr(controller, "url"):
+                raise ValueError(
+                    f"LayoutControllers are not directly mountable to the router. {controller} should not have a url specified."
+                )
+            view_router = None
+        else:
+            view_router = APIRouter()
+            view_router.get(controller.url)(generate_controller_html)
+            self.app.include_router(view_router)
 
         # Create a wrapper router for each controller to hold the side-effects
         controller_api = APIRouter()
         controller_url_prefix = (
             f"{self.internal_api_prefix}/{underscore(controller.__class__.__name__)}"
         )
         for _, fn, metadata in controller._get_client_functions():
@@ -247,15 +305,15 @@
 
             if not metadata.get_is_raw_response():
                 # We need to delay adding the typehint for each function until we are here, adding the view. Since
                 # decorators run before the class is actually mounted, they're isolated from the larger class/controller
                 # context that the action function is being defined within. Here since we have a global view
                 # of the controller (render function + actions) this becomes trivial
                 metadata.return_model = fuse_metadata_to_response_typehint(
-                    metadata, render_metadata.get_render_model()
+                    metadata, controller, render_metadata.get_render_model()
                 )
 
                 # Update the signature of the internal function, which fastapi will sniff for the return declaration
                 # https://github.com/tiangolo/fastapi/blob/a235d93002b925b0d2d7aa650b7ab6d7bb4b24dd/fastapi/dependencies/utils.py#L207
                 method_function: Callable = fn.__func__  # type: ignore
                 method_function.__signature__ = signature(method_function).replace(  # type: ignore
                     return_annotation=metadata.return_model
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/cache.py` & `mountaineer-0.5.0.dev1/mountaineer/cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/cli.py` & `mountaineer-0.5.0.dev1/mountaineer/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from signal import SIGINT, signal
 from tempfile import mkdtemp
 from threading import Thread
 from time import monotonic_ns, sleep, time
 from traceback import format_exception
 from typing import Any, Callable, MutableMapping
 
-from click import secho
 from fastapi import Request
 from rich.traceback import install as rich_traceback_install
 
 from mountaineer.app import AppController
 from mountaineer.client_builder.builder import ClientBuilder
 from mountaineer.console import CONSOLE, ERROR_CONSOLE
 from mountaineer.controllers.exception_controller import ExceptionController
@@ -236,15 +235,15 @@
             )
 
             # Completed successfully
             app_controller.build_exception = None
 
             self.alert_notification_channel()
         except BuildProcessException as e:
-            CONSOLE.print(f"[bold red]⚠️ Build failed: {e}")
+            CONSOLE.print(f"[bold red]🪲 Build failed: {e}")
             app_controller.build_exception = e
 
     def stop(self, hard_timeout: float = 5.0):
         """
         Client-side stop method to shut down the running process.
         """
         # If we've already stopped, don't try to stop again
@@ -259,17 +258,16 @@
 
         # Try to give the process time to shut down gracefully
         while self.is_alive() and hard_timeout > 0:
             self.join(1)
             hard_timeout -= 1
 
         if hard_timeout == 0:
-            secho(
-                f"Server shutdown reached hard timeout deadline: {self.is_alive()}",
-                fg="red",
+            CONSOLE.print(
+                f"[bold red]Server shutdown reached hard timeout deadline: {self.is_alive()}",
             )
 
         # As a last resort we send a hard termination signal
         if self.is_alive():
             self.terminate()
 
     async def handle_dev_exception(self, request: Request, exc: Exception):
@@ -409,15 +407,15 @@
     # Install a signal handler to catch SIGINT and try to
     # shut down gracefully
     def graceful_shutdown(signum, frame):
         if current_process is not None:
             current_process.stop()
         if watcher_webservice is not None:
             watcher_webservice.stop()
-        secho("Services shutdown, now exiting...", fg="yellow")
+        CONSOLE.print("[yellow]Services shutdown, now exiting...")
         exit(0)
 
     signal(SIGINT, graceful_shutdown)
 
     with init_global_state(webcontroller) as global_state:
         watchdog = build_common_watchdog(
             package,
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/client_builder/build_actions.py` & `mountaineer-0.5.0.dev1/mountaineer/client_builder/build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/client_builder/build_links.py` & `mountaineer-0.5.0.dev1/mountaineer/client_builder/build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/client_builder/build_schemas.py` & `mountaineer-0.5.0.dev1/mountaineer/client_builder/build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/client_builder/builder.py` & `mountaineer-0.5.0.dev1/mountaineer/client_builder/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 from mountaineer.client_builder.openapi import OpenAPIDefinition, OpenAPISchema
 from mountaineer.client_builder.typescript import (
     TSLiteral,
     python_payload_to_typescript,
 )
 from mountaineer.console import CONSOLE
 from mountaineer.controller import ControllerBase
+from mountaineer.controller_layout import LayoutControllerBase
 from mountaineer.io import gather_with_concurrency
 from mountaineer.js_compiler.base import ClientBundleMetadata
 from mountaineer.js_compiler.exceptions import BuildProcessException
 from mountaineer.logging import LOGGER
 from mountaineer.paths import ManagedViewPath, generate_relative_import
 from mountaineer.static import get_static_path
 
 
 @dataclass
 class RenderSpec:
-    url: str
+    url: str | None
     view_path: str
     spec: dict[Any, Any] | None
 
 
 class ClientBuilder:
     """
     Main entrypoint for building the auto-generated typescript code.
@@ -229,14 +230,23 @@
             controller_links_path = controller_code_dir / "links.ts"
 
             root_common_handler = root_code_dir / "api.ts"
             root_api_import_path = generate_relative_import(
                 controller_links_path, root_common_handler
             )
             render_route = controller_definition.render_router
+
+            # This controller isn't accessible via a URL so shouldn't have a
+            # link associated with it
+            # This file still needs to exist for downstream exports so we write
+            # a blank file
+            if render_route is None:
+                controller_links_path.write_text("")
+                continue
+
             render_openapi = self.app.generate_openapi(
                 routes=render_route.routes,
             )
 
             content = ""
             content += f"import {{ __getLink }} from '{root_api_import_path}';\n"
             content += self.openapi_link_converter.convert(render_openapi)
@@ -291,14 +301,15 @@
         Generate the useServer() hooks within each local view. These will reference the main
         server provider and allow each view to access the particular server state that
         is linked to that controller.
 
         """
         for controller_definition in self.app.controllers:
             controller = controller_definition.controller
+            controller_key = controller.__class__.__name__
 
             chunks: list[str] = []
 
             # Step 1: Interface to optionally override the current controller state
             # We want to have an inline reference to a model which is compatible with the base render model alongside
             # all sideeffect sub-models. Since we're re-declaring this in the server file, we also
             # have to bring with us all of the other sub-model imports.
@@ -359,15 +370,15 @@
                 + "}\n"
             )
 
             # Step 6: Final implementation of the useServer() hook, which returns a subview of the overall
             # server state that's only relevant to this controller
             chunks.append(
                 "export const useServer = () : ServerState => {\n"
-                + f"const [ serverState, setServerState ] = useState(SERVER_DATA as {render_model_name});\n"
+                + f"const [ serverState, setServerState ] = useState(SERVER_DATA['{controller_key}'] as {render_model_name});\n"
                 # Local function to just override the current controller
                 # We make sure to wait for the previous state to be set, in case of a
                 # differential update
                 + f"const setControllerState = (payload: {optional_model_name}) => {{\n"
                 + "setServerState((state) => ({\n"
                 + "...state,\n"
                 + "...payload,\n"
@@ -375,15 +386,15 @@
                 + "};\n"
                 + "return {\n"
                 + "...serverState,\n"
                 + "linkGenerator: LinkGenerator,\n"
                 + ",\n".join(
                     [
                         (
-                            f"{metadata.function_name}: applySideEffect({metadata.function_name}, setControllerState)"
+                            f"{metadata.function_name}: applySideEffect({metadata.function_name}, setControllerState, '{controller_key}')"
                             if metadata.action_type == FunctionActionType.SIDEEFFECT
                             else f"{metadata.function_name}: {metadata.function_name}"
                         )
                         for metadata in controller_action_metadata
                     ]
                 )
                 + "}\n"
@@ -490,42 +501,52 @@
         outdated md5 content hashes from being served
 
         """
         with TemporaryDirectory() as tmp_dir:
             tmp_path = Path(tmp_dir)
             tmp_static_dir = tmp_path / "static"
             tmp_ssr_dir = tmp_path / "ssr"
+            tmp_metadata_dir = tmp_path / "metadata"
 
             # Since the tmp builds are within their parent folder, we need to move
             # them out of the way before we clear
             # Unlike the standard rename operation, shutil will treat this move as a rename if the files
             # exist within the same OS and will do a copy/replace if they live across volumes
             # This is necessary for some docker build pipelines where /tmp is auto-mounted
             # as a shared volume between stages and therefore the act of building temporary files
             # would cause a "Invalid cross-device link" when we try to copy
             shutil_move(
                 self.view_root.get_managed_static_dir(tmp_build=True), tmp_static_dir
             )
             shutil_move(self.view_root.get_managed_ssr_dir(tmp_build=True), tmp_ssr_dir)
+            shutil_move(
+                self.view_root.get_managed_metadata_dir(tmp_build=True),
+                tmp_metadata_dir,
+            )
 
             static_dir = self.view_root.get_managed_static_dir()
             ssr_dir = self.view_root.get_managed_ssr_dir()
-            for clear_dir in [static_dir, ssr_dir]:
+            metadata_dir = self.view_root.get_managed_metadata_dir()
+            for clear_dir in [static_dir, ssr_dir, metadata_dir]:
                 if clear_dir.exists():
                     shutil_rmtree(clear_dir)
 
             # Final move - shutil requires the destination directory to not exist, otherwise
             # it will place the folder within the given folder. Since we just want a regular
             # rename, we make sure to not create the destination directory
             shutil_move(
                 tmp_static_dir, self.view_root.get_managed_static_dir(create_dir=False)
             )
             shutil_move(
                 tmp_ssr_dir, self.view_root.get_managed_ssr_dir(create_dir=False)
             )
+            shutil_move(
+                tmp_metadata_dir,
+                self.view_root.get_managed_metadata_dir(create_dir=False),
+            )
 
     def cache_is_outdated(self):
         """
         Determines if our last build is outdated and we need to rebuild the client. Running
         this function will also update the cache to the current state.
 
         """
@@ -553,15 +574,15 @@
         if cached_metadata.read_text() != cached_str:
             cached_metadata.write_text(cached_str)
             return True
 
         return False
 
     def get_static_files(self):
-        ignore_directories = ["_ssr", "_static", "_server", "node_modules"]
+        ignore_directories = ["_ssr", "_static", "_server", "_metadata", "node_modules"]
 
         for view_root in self.get_all_root_views():
             for dir_path, _, filenames in view_root.walk():
                 for filename in filenames:
                     if any(
                         [
                             directory in dir_path.parts
@@ -574,14 +595,19 @@
     def validate_unique_paths(self):
         """
         Validate that all controller paths are unique. Otherwise we risk stomping
         on other server metadata that has already been written.
 
         """
         # Validation 1: Ensure that all view paths are unique
+        # This applies to both exact equivalence (two controllers pointing to the
+        # same page.tsx) as well as conflicting folder structures (one controller pointing
+        # to a page and another pointing to a layout in the same directory).
+        # Both of these causes would cause conflicting _server files to be generated
+        # which we need to avoid
         view_counts = defaultdict(list)
         for controller_definition in self.app.controllers:
             controller = controller_definition.controller
             view_counts[
                 self.view_root.get_controller_view_path(controller).parent
             ].append(controller)
         duplicate_views = [
@@ -700,13 +726,15 @@
 
                 spec = (
                     self.openapi_schema_converter.get_model_json_schema(render_model)
                     if render_model
                     else None
                 )
                 self._openapi_render_specs[controller] = RenderSpec(
-                    url=controller.url,
+                    url=None
+                    if isinstance(controller, LayoutControllerBase)
+                    else controller.url,
                     view_path=str(controller.view_path),
                     spec=spec,
                 )
 
         return self._openapi_render_specs
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/client_builder/openapi.py` & `mountaineer-0.5.0.dev1/mountaineer/client_builder/openapi.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/client_builder/typescript.py` & `mountaineer-0.5.0.dev1/mountaineer/client_builder/typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/config.py` & `mountaineer-0.5.0.dev1/mountaineer/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/controller.py` & `mountaineer-0.5.0.dev1/mountaineer/controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC, abstractmethod
 from importlib.metadata import PackageNotFoundError
 from inspect import getmembers, isawaitable, ismethod
+from json import dumps as json_dumps
 from pathlib import Path
 from re import compile as re_compile
 from time import monotonic_ns
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -15,14 +16,15 @@
     Optional,
     ParamSpec,
     cast,
 )
 
 from fastapi.responses import HTMLResponse
 from inflection import underscore
+from pydantic import BaseModel
 
 from mountaineer.actions import (
     FunctionActionType,
     FunctionMetadata,
     get_function_metadata,
 )
 from mountaineer.config import get_config
@@ -41,14 +43,31 @@
 
 if TYPE_CHECKING:
     from mountaineer.app import ControllerDefinition
 
 RenderInput = ParamSpec("RenderInput")
 
 
+class BuildMetadata(BaseModel):
+    """
+    Controller metadata that is established during build-time and might be stripped
+    during the final output. For instance, layout.tsx files might not be included
+    in production payloads but this metadata object still stores their hierarchy
+    relative to the controllers.
+
+    """
+
+    # All paths in the metadata should be absolute paths, since they are consistent
+    # with regard to the builder filesystem but might be different when deployed
+    view_path: Path
+
+    # Organized by hierarchy, first index is the outermost layout
+    layout_view_paths: list[Path] = []
+
+
 class ControllerBase(ABC, Generic[RenderInput]):
     url: str
     # Typically, view paths should be a relative path to the local
     # Paths are only used if you need to specify an absolute path to another
     # file on disk
     view_path: str | ManagedViewPath
 
@@ -77,16 +96,18 @@
         # Injected by the build framework
         self.bundled_scripts: list[str] = []
         self.initialized = True
         self.slow_ssr_threshold = slow_ssr_threshold
         self.hard_ssr_timeout = hard_ssr_timeout
         self.source_map: SourceMapParser | None = None
 
+        # Set by the path resolution layer
         self.view_base_path: Path | None = None
         self.ssr_path: Path | None = None
+        self.build_metadata: BuildMetadata | None = None
 
         self.resolve_paths()
 
     @abstractmethod
     def render(
         self, *args: RenderInput.args, **kwargs: RenderInput.kwargs
     ) -> RenderBase | None | Coroutine[Any, Any, RenderBase | None]:
@@ -132,15 +153,30 @@
                 ...
         ```
 
         :return: A RenderBase instance or None
         """
         pass
 
-    async def _generate_html(self, *args, global_metadata: Metadata | None, **kwargs):
+    async def _generate_html(
+        self,
+        *args,
+        global_metadata: Metadata | None,
+        other_render_contexts: dict[str, RenderBase | RenderNull] | None = None,
+        **kwargs,
+    ):
+        """
+        Generate the HTML that will populate the loaded page of the controller.
+
+        :param other_render_contexts: The dictionary should be constructed in the order of
+        precedence, with the first element being the most hierarchical related element to
+        this controller. This is used by our metadata resolution layer to figure out what
+        is the best metadata attribute to fall back to.
+
+        """
         # Because JSON is a subset of JavaScript, we can just dump the model as JSON and
         # insert it into the page.
         server_data = self.render(*args, **kwargs)
         if isawaitable(server_data):
             server_data = await server_data
         if server_data is None:
             server_data = RenderNull()
@@ -155,26 +191,40 @@
         # render process and return a redirect response
         if server_data.metadata and server_data.metadata.explicit_response:
             return server_data.metadata.explicit_response
 
         metadatas: list[Metadata] = []
         if server_data.metadata:
             metadatas.append(server_data.metadata)
+        if other_render_contexts and (
+            server_data.metadata is None
+            or not server_data.metadata.ignore_global_metadata
+        ):
+            for other_render_context in other_render_contexts.values():
+                if other_render_context.metadata:
+                    metadatas.append(other_render_context.metadata)
         if global_metadata and (
             server_data.metadata is None
             or not server_data.metadata.ignore_global_metadata
         ):
             metadatas.append(global_metadata)
 
         header_str = "\n".join(self._build_header(self._merge_metadatas(metadatas)))
 
-        ssr_html = self._generate_ssr_html(server_data)
-
         # Client-side react scripts that will hydrate the server side contents on load
-        server_data_json = server_data.model_dump_json()
+        server_data_json = {
+            render_key: context.model_dump(mode="json")
+            for render_key, context in [
+                (self.__class__.__name__, server_data),
+                *list(other_render_contexts.items() if other_render_contexts else []),
+            ]
+        }
+
+        ssr_html = self._generate_ssr_html(server_data_json)
+
         optional_scripts = "\n".join(
             [
                 f"<script src='/static/{script_name}'></script>"
                 for script_name in self.bundled_scripts
             ]
         )
 
@@ -182,36 +232,30 @@
         <html>
         <head>
         {header_str}
         </head>
         <body>
         <div id="root">{ssr_html}</div>
         <script type="text/javascript">
-        const SERVER_DATA = {server_data_json};
+        const SERVER_DATA = {json_dumps(server_data_json)};
         </script>
         {optional_scripts}
         </body>
         </html>
         """
 
         return HTMLResponse(page_contents)
 
-    def _generate_ssr_html(self, server_data: RenderBase) -> str:
+    def _generate_ssr_html(self, server_data: dict[str, Any]) -> str:
         self.resolve_paths()
 
         if not self.ssr_path:
             # Try to resolve the path dynamically now
             raise ValueError("No SSR path set for this controller")
 
-        # Now that we've built the header, we can remove it from the server data
-        # This makes our cache more efficient, since metadata changes don't affect
-        # the actual page contents.
-        server_data = server_data.model_copy(update={"metadata": None})
-
-        # TODO: Provide a function to automatically sniff for the client view folder
         start = monotonic_ns()
         try:
             ssr_html = render_ssr(
                 self.ssr_path.read_text(),
                 server_data,
                 hard_timeout=self.hard_ssr_timeout,
             )
@@ -359,14 +403,22 @@
                 found_dependencies = False
             LOGGER.debug(
                 f"[{self.__class__.__name__}] Resolved paths... {self.bundled_scripts}"
             )
         else:
             found_dependencies = False
 
+        # Find the metadata
+        metadata_path = view_base / "_metadata" / f"{script_name}.json"
+        if metadata_path.exists():
+            metadata = BuildMetadata.model_validate_json(metadata_path.read_text())
+            self.build_metadata = metadata
+        else:
+            found_dependencies = False
+
         return found_dependencies
 
     def _merge_metadatas(self, metadatas: list[Metadata]):
         """
         Merges a list of metadata objects, sorted by priority. Some fields will
         take the union (like scripts) - others will prioritize earlier entries (title).
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/controllers/exception_controller.py` & `mountaineer-0.5.0.dev1/mountaineer/controllers/exception_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/cropper.py` & `mountaineer-0.5.0.dev1/mountaineer/cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/database/cli.py` & `mountaineer-0.5.0.dev1/mountaineer/database/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/database/config.py` & `mountaineer-0.5.0.dev1/mountaineer/database/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/database/dependencies/core.py` & `mountaineer-0.5.0.dev1/mountaineer/database/dependencies/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/database/sqlmodel.py` & `mountaineer-0.5.0.dev1/mountaineer/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/database/validator.py` & `mountaineer-0.5.0.dev1/mountaineer/database/validator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/dependencies/base.py` & `mountaineer-0.5.0.dev1/mountaineer/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/dependencies/core/core.py` & `mountaineer-0.5.0.dev1/mountaineer/dependencies/core/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/exceptions.py` & `mountaineer-0.5.0.dev1/mountaineer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/io.py` & `mountaineer-0.5.0.dev1/mountaineer/io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/js_compiler/base.py` & `mountaineer-0.5.0.dev1/mountaineer/js_compiler/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/js_compiler/javascript.py` & `mountaineer-0.5.0.dev1/mountaineer/js_compiler/javascript.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any
 
 from inflection import underscore
 from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
 
 from mountaineer import mountaineer as mountaineer_rs  # type: ignore
 from mountaineer.console import CONSOLE
-from mountaineer.controller import ControllerBase
+from mountaineer.controller import BuildMetadata, ControllerBase
 from mountaineer.js_compiler.base import ClientBuilderBase, ClientBundleMetadata
 from mountaineer.js_compiler.exceptions import BuildProcessException
 from mountaineer.logging import LOGGER
 from mountaineer.paths import ManagedViewPath, generate_relative_import
 
 
 @dataclass
@@ -168,14 +168,24 @@
         if controller is None:
             # Require a controller for our bundling
             return None
         if file_path.suffix not in [".tsx", ".jsx"]:
             # We only know how to parse tsx and jsx files
             return None
 
+        # Build the metadata archive for this controller now that
+        # we have the file location context
+        controller_base = underscore(controller.__class__.__name__)
+        root_path = file_path.get_package_root_link()
+        metadata_dir = root_path.get_managed_metadata_dir(tmp_build=True)
+        metadata_payload = self.build_metadata_archive(
+            page_path=file_path, controller=controller
+        )
+        (metadata_dir / f"{controller_base}.json").write_text(metadata_payload)
+
         # Now we can process the files in bulk
         payload = self.generate_js_bundle(
             file_path=file_path, controller=controller, metadata=metadata
         )
         self.pending_files.append(payload)
 
     async def finish_build(self):
@@ -320,14 +330,26 @@
 
         lines.append(
             f"export const Index = () => renderToString(<{synthetic_endpoint_name} />);"
         )
 
         return "\n".join(lines)
 
+    def build_metadata_archive(
+        self, *, page_path: ManagedViewPath, controller: ControllerBase
+    ):
+        layout_paths = self.sniff_for_layouts(
+            page_path=page_path, view_root_path=page_path.get_root_link()
+        )
+        metadata = BuildMetadata(
+            view_path=page_path,
+            layout_view_paths=layout_paths,
+        )
+        return metadata.model_dump_json()
+
     def build_synthetic_endpoint(
         self, *, page_path: ManagedViewPath, layout_paths: list[Path], output_path: Path
     ):
         """
         Following the Next.js syntax, layouts wrap individual pages in a top-down order. Here we
         create a synthetic page that wraps the actual page in the correct order.
         The output is a valid React file that acts as the page entrypoint
@@ -429,17 +451,17 @@
             current_path = current_path.parent
 
         # Return the layouts in the order they should be rendered
         return list(reversed(layouts))
 
     def validate_page(self, *, page_path: Path, view_root_path: Path):
         # Validate that we're actually calling on a path file
-        if page_path.name not in {"page.tsx", "page.jsx"}:
+        if page_path.name not in {"page.tsx", "page.jsx", "layout.tsx", "layout.jsx"}:
             raise ValueError(
-                f"Invalid page path; view need to be specified in a `page.tsx` file: {page_path}"
+                f"Invalid page path. View needs to be specified in a `page.tsx` or `layout.tsx` file: {page_path}"
             )
 
         # Validate that the page_path is within the view root. The following
         # logic assumes a hierarchical relationship between the two.
         if not page_path.is_relative_to(view_root_path):
             raise ValueError(
                 f"Invalid page path, not relative to view root: {page_path} (root: {view_root_path})"
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/js_compiler/postcss.py` & `mountaineer-0.5.0.dev1/mountaineer/js_compiler/postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/js_compiler/source_maps.py` & `mountaineer-0.5.0.dev1/mountaineer/js_compiler/source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/logging.py` & `mountaineer-0.5.0.dev1/mountaineer/logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/paths.py` & `mountaineer-0.5.0.dev1/mountaineer/paths.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,14 +110,28 @@
             )
         path = self.get_managed_dir_common("_ssr", create_dir=create_dir)
         if tmp_build:
             path = path / "tmp"
             path.mkdir(exist_ok=True)
         return path
 
+    def get_managed_metadata_dir(
+        self, tmp_build: bool = False, create_dir: bool = True
+    ):
+        # Only root paths can have metadata directories
+        if not self.is_root_link:
+            raise ValueError(
+                "Cannot get metadata directory from a non-root linked view path"
+            )
+        path = self.get_managed_dir_common("_metadata", create_dir=create_dir)
+        if tmp_build:
+            path = path / "tmp"
+            path.mkdir(exist_ok=True)
+        return path
+
     def get_managed_dir_common(
         self,
         managed_dir: str,
         create_dir: bool = True,
     ):
         # If the path is to a file, we want to get the parent directory
         # so that we can create the managed code directory
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/render.py` & `mountaineer-0.5.0.dev1/mountaineer/render.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/ssr.py` & `mountaineer-0.5.0.dev1/mountaineer/ssr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+from json import dumps as json_dumps
 from re import finditer as re_finditer
-from typing import cast
-
-from pydantic import BaseModel
+from typing import Any, cast
 
 from mountaineer import mountaineer as mountaineer_rs  # type: ignore
 from mountaineer.cache import extended_lru_cache
 from mountaineer.static import get_static_path
 
 
 class V8RuntimeError(Exception):
@@ -41,15 +40,15 @@
         exception = exception[:start] + replacement + exception[end:]
 
     return exception
 
 
 @extended_lru_cache(maxsize=128, max_size_mb=5)
 def render_ssr(
-    script: str, render_data: BaseModel, hard_timeout: int | float | None = None
+    script: str, render_data: dict[str, Any], hard_timeout: int | float | None = None
 ) -> str:
     """
     Render the React component in the provided SSR javascript bundle. This file will
     be directly executed within the V8 runtime.
 
     To speed up requests for the same exact content (ie. same react and same data)
     we cache the result of the render_ssr_rust call by default for a limited amount of
@@ -62,15 +61,15 @@
         longer than this time, our thread supervisor will kick in and terminate the rust worker.
 
     :raises TimeoutError: If the render takes longer than the hard_timeout
     :raises V8RuntimeError: If the V8 runtime throws an exception during the render
 
     """
     polyfill_script = get_static_path("ssr_polyfills.js").read_text()
-    data_json = render_data.model_dump_json()
+    data_json = json_dumps(render_data)
 
     injected_script = f"const SERVER_DATA = {data_json};\n{polyfill_script}\n"
     full_script = f"{injected_script}{script}"
 
     try:
         # Convert to milliseconds for the rust worker
         render_result = mountaineer_rs.render_ssr(
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/static/api.ts` & `mountaineer-0.5.0.dev1/mountaineer/static/api.ts`

 * *Files 4% similar despite different names*

```diff
@@ -147,35 +147,40 @@
         // Yield the line in the requested format.
         yield format === "text" ? line : JSON.parse(line);
       }
     }
   })();
 };
 
-type ApiFunctionReturnType<S, P> = {
-  sideeffect: S;
-  passthrough?: P;
+type ApiFunctionReturnType<S, P, K extends PropertyKey> = {
+  // Generic typehint for any key parameter
+  [key in K]: {
+    sideeffect: S;
+    passthrough?: P;
+  };
 };
 
 export function applySideEffect<
   ARG extends any[],
   S,
   P,
-  RE extends ApiFunctionReturnType<S, P>,
+  K extends PropertyKey,
+  RE extends ApiFunctionReturnType<S, P, K>,
 >(
   apiFunction: (...args: ARG) => Promise<RE>,
   setControllerState: (payload: S) => void,
+  controllerKey: K,
 ): (...args: ARG) => Promise<RE> {
   /*
    * Executes an API server function, triggering any appropriate exceptions.
    * If the fetch succeeds, the sideeffect is applied to the controller state.
    */
   return async (...args: ARG) => {
     const result = await apiFunction(...args);
-    setControllerState(result.sideeffect);
+    setControllerState(result[controllerKey].sideeffect);
     return result;
   };
 }
 
 interface GetLinkParams {
   rawUrl: string;
   queryParameters: Record<string, string>;
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/static/live_reload.ts` & `mountaineer-0.5.0.dev1/mountaineer/static/live_reload.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/test_utilities.py` & `mountaineer-0.5.0.dev1/mountaineer/test_utilities.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/views/package-lock.json` & `mountaineer-0.5.0.dev1/mountaineer/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/mountaineer/watch.py` & `mountaineer-0.5.0.dev1/mountaineer/watch.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     callback: Callable[[CallbackMetadata], None]
 
 
 class ChangeEventHandler(FileSystemEventHandler):
     def __init__(
         self,
         callbacks: list[CallbackDefinition],
-        ignore_list=["__pycache__", "_ssr", "_static", "_server"],
+        ignore_list=["__pycache__", "_ssr", "_static", "_server", "_metadata"],
         ignore_hidden=True,
         debounce_interval=0.1,
     ):
         """
         :param debounce_interval: Seconds to wait for more events. Will only send one event per batched
         interval to avoid saturating clients with one action that results in many files.
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/watch_server.py` & `mountaineer-0.5.0.dev1/mountaineer/watch_server.py`

 * *Files 22% similar despite different names*

```diff
@@ -67,29 +67,49 @@
                 break
             asyncio.run(self.broadcast_listeners())
 
     def start(self):
         if self.has_started:
             raise Exception("WatcherWebservice has already started")
 
+        # UvicornThreads are daemon threads by default
         self.webservice_thread = UvicornThread(
             app=self.app,
             port=self.port,
             log_level="warning",
         )
 
         LOGGER.debug("Starting WatcherWebservice on port %d", self.port)
         self.webservice_thread.start()
 
-        self.monitor_build_thread = Thread(target=self.monitor_builds)
+        self.monitor_build_thread = Thread(target=self.monitor_builds, daemon=True)
         self.monitor_build_thread.start()
 
         self.has_started = True
 
-    def stop(self):
+    def stop(self, wait_for_completion: int = 1) -> bool:
+        """
+        Attempts to stop the separate WatcherWebservice threads. We will send a termination
+        signal to the threads and wait the desired interval for full completion. If the threads
+        haven't exited after the interval, we will return False. Clients can then decide whether
+        to send a harder termination signal to terminate the threads on the OS level.
+
+        """
+        success: bool = True
         if self.webservice_thread is not None:
             self.webservice_thread.stop()
-            self.webservice_thread.join()
+            self.webservice_thread.join(wait_for_completion)
         if self.monitor_build_thread is not None:
             self.notification_queue.put(None)
-            self.monitor_build_thread.join()
-        LOGGER.info("WatcherWebservice has stopped")
+            self.monitor_build_thread.join(wait_for_completion)
+
+        if (self.webservice_thread and self.webservice_thread.is_alive()) or (
+            self.monitor_build_thread and self.monitor_build_thread.is_alive()
+        ):
+            success = False
+            LOGGER.info(
+                f"WatcherWebservice still has outstanding threads: {self.webservice_thread} {self.monitor_build_thread}"
+            )
+        else:
+            LOGGER.info("WatcherWebservice has fully stopped")
+
+        return success
```

### Comparing `mountaineer-0.4.2.dev3/mountaineer/webservice.py` & `mountaineer-0.5.0.dev1/mountaineer/webservice.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/poetry.lock` & `mountaineer-0.5.0.dev1/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/benches/fixtures/complex_sourcemap_mapping.txt` & `mountaineer-0.5.0.dev1/src/benches/fixtures/complex_sourcemap_mapping.txt`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/benches/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.5.0.dev1/src/benches/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/benches/lexers_benchmark.rs` & `mountaineer-0.5.0.dev1/src/benches/lexers_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/benches/source_map_benchmark.rs` & `mountaineer-0.5.0.dev1/src/benches/source_map_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/benches/ssr_benchmark.rs` & `mountaineer-0.5.0.dev1/src/benches/ssr_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/lexers.rs` & `mountaineer-0.5.0.dev1/src/lexers.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/lib.rs` & `mountaineer-0.5.0.dev1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/logging.rs` & `mountaineer-0.5.0.dev1/src/logging.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/source_map.rs` & `mountaineer-0.5.0.dev1/src/source_map.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/ssr.rs` & `mountaineer-0.5.0.dev1/src/ssr.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/src/timeout.rs` & `mountaineer-0.5.0.dev1/src/timeout.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev3/Cargo.lock` & `mountaineer-0.5.0.dev1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mountaineer"
-version = "0.4.2-dev3"
+version = "0.5.0-dev1"
 dependencies = [
  "criterion",
  "deno_core_icudata",
  "env_logger",
  "lazy_static",
  "libc",
  "log",
```

### Comparing `mountaineer-0.4.2.dev3/pyproject.toml` & `mountaineer-0.5.0.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "mountaineer"
 dependencies = [ "pydantic", "fastapi", "inflection", "click", "uvicorn[standard]", "packaging", "watchdog", "pydantic-settings", "sqlmodel", "asyncpg", "sqlalchemy[asyncio]", "rich",]
 exclude = [ "fixtures", "ci_webapp", "create_mountaineer_app", "media", "docs_website", "benchmarking",]
 
 [tool.poetry]
 name = "mountaineer"
-version = "0.4.2.dev3"
+version = "0.5.0.dev1"
 description = ""
 authors = [ "Pierce Freeman <pierce@freeman.vc>",]
 readme = "README.md"
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
```

### Comparing `mountaineer-0.4.2.dev3/PKG-INFO` & `mountaineer-0.5.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mountaineer
-Version: 0.4.2.dev3
+Version: 0.5.0.dev1
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: inflection
 Requires-Dist: click
 Requires-Dist: uvicorn[standard]
 Requires-Dist: packaging
 Requires-Dist: watchdog
```

