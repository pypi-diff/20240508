# Comparing `tmp/OZI-1.4.2.tar.gz` & `tmp/OZI-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.4.2.tar", last modified: Sun May  5 04:35:02 2024, max compression
+gzip compressed data, was "OZI-1.4.3.tar", last modified: Wed May  8 03:06:38 2024, max compression
```

## Comparing `OZI-1.4.2.tar` & `OZI-1.4.3.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.441914 OZI-1.4.2/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.413914 OZI-1.4.2/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.413914 OZI-1.4.2/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.413914 OZI-1.4.2/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-05-05 04:30:50.000000 OZI-1.4.2/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-05 04:30:50.000000 OZI-1.4.2/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   299924 2024-05-05 04:30:50.000000 OZI-1.4.2/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-05 04:30:50.000000 OZI-1.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-05 04:35:02.213912 OZI-1.4.2/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-05 04:30:50.000000 OZI-1.4.2/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    16724 2024-05-05 04:30:50.000000 OZI-1.4.2/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-05-05 04:30:50.000000 OZI-1.4.2/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.437914 OZI-1.4.2/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.421914 OZI-1.4.2/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.421914 OZI-1.4.2/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.421914 OZI-1.4.2/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/dist/sigstore/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.429914 OZI-1.4.2/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.425914 OZI-1.4.2/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.429914 OZI-1.4.2/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.429914 OZI-1.4.2/ozi/lint/restructuredtext-lint/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/restructuredtext-lint/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/lint/restructuredtext-lint/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.429914 OZI-1.4.2/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     4854 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.433914 OZI-1.4.2/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.433914 OZI-1.4.2/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6066 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6345 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.437914 OZI-1.4.2/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.433914 OZI-1.4.2/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.437914 OZI-1.4.2/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.437914 OZI-1.4.2/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.437914 OZI-1.4.2/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-05 04:30:50.000000 OZI-1.4.2/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10899 2024-05-05 04:30:50.000000 OZI-1.4.2/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      190 2024-05-05 04:30:50.000000 OZI-1.4.2/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.441914 OZI-1.4.2/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-05 04:30:50.000000 OZI-1.4.2/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:35:02.441914 OZI-1.4.2/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-05 04:30:50.000000 OZI-1.4.2/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11072 2024-05-05 04:30:50.000000 OZI-1.4.2/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14164 2024-05-05 04:30:50.000000 OZI-1.4.2/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-05 04:30:50.000000 OZI-1.4.2/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.368252 OZI-1.4.3/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.340252 OZI-1.4.3/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.340252 OZI-1.4.3/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.340252 OZI-1.4.3/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-08 03:02:20.000000 OZI-1.4.3/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   301620 2024-05-08 03:02:20.000000 OZI-1.4.3/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-08 03:02:20.000000 OZI-1.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-08 03:06:38.136252 OZI-1.4.3/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-08 03:02:20.000000 OZI-1.4.3/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    16724 2024-05-08 03:02:20.000000 OZI-1.4.3/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-05-08 03:02:20.000000 OZI-1.4.3/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.364252 OZI-1.4.3/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.348252 OZI-1.4.3/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.348252 OZI-1.4.3/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.348252 OZI-1.4.3/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/dist/sigstore/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.356252 OZI-1.4.3/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.356252 OZI-1.4.3/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.356252 OZI-1.4.3/ozi/lint/restructuredtext-lint/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/restructuredtext-lint/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/restructuredtext-lint/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.356252 OZI-1.4.3/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     4801 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.360252 OZI-1.4.3/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.360252 OZI-1.4.3/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6066 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.364252 OZI-1.4.3/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.360252 OZI-1.4.3/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.364252 OZI-1.4.3/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.364252 OZI-1.4.3/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.364252 OZI-1.4.3/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10899 2024-05-08 03:02:20.000000 OZI-1.4.3/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      190 2024-05-08 03:02:20.000000 OZI-1.4.3/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.368252 OZI-1.4.3/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-08 03:02:20.000000 OZI-1.4.3/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.368252 OZI-1.4.3/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-08 03:02:20.000000 OZI-1.4.3/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11072 2024-05-08 03:02:20.000000 OZI-1.4.3/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14164 2024-05-08 03:02:20.000000 OZI-1.4.3/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-08 03:02:20.000000 OZI-1.4.3/tests/test_tap.py
```

### Comparing `OZI-1.4.2/.github/CODEOWNERS` & `OZI-1.4.3/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/.github/CODE_OF_CONDUCT.md` & `OZI-1.4.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/.github/CONTRIBUTING.md` & `OZI-1.4.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.4.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.4.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/.github/SECURITY.md` & `OZI-1.4.3/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/.github/workflows/codeql.yml` & `OZI-1.4.3/.github/workflows/codeql.yml`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,15 @@
           allowed-endpoints: >
             api.github.com:443
             github.com:443
             objects.githubusercontent.com:443
             uploads.github.com:443
 
       - name: Checkout repository
-        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
+        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
         uses: github/codeql-action/init@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
         with:
           languages: ${{ matrix.language }}
           # If you wish to specify custom queries, you can do so here or in a config file.
```

### Comparing `OZI-1.4.2/.github/workflows/dependency-review.yml` & `OZI-1.4.3/.github/workflows/dependency-review.yml`

 * *Files 4% similar despite different names*

```diff
@@ -23,12 +23,12 @@
     steps:
       - name: Harden Runner
         uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           egress-policy: audit
 
       - name: 'Checkout Repository'
-        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
+        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
       - name: 'Dependency Review'
         uses: actions/dependency-review-action@0c155c5e8556a497adf53f2c18edabf945ed8e70 # v4.3.2
         with:
           head-ref: main
```

### Comparing `OZI-1.4.2/.github/workflows/dist-workflow.yml` & `OZI-1.4.3/.github/workflows/dist-workflow.yml`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@a6290f1edcd89a03dca8d123327e25f0c3bfc91c
+      - uses: OZI-Project/checkpoint@1ad9ec15d60558ee3da890634bb8b0406838e17a
         with:
           python-version: "3.10"
 
   checkpoint-cp311-ubuntu-latest:
     name: checkpoint (Python 3.11 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -62,15 +62,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@a6290f1edcd89a03dca8d123327e25f0c3bfc91c
+      - uses: OZI-Project/checkpoint@1ad9ec15d60558ee3da890634bb8b0406838e17a
         with:
           python-version: "3.11"
 
   checkpoint-cp312-ubuntu-latest:
     name: checkpoint (Python 3.12 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -90,15 +90,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@a6290f1edcd89a03dca8d123327e25f0c3bfc91c
+      - uses: OZI-Project/checkpoint@1ad9ec15d60558ee3da890634bb8b0406838e17a
         with:
           python-version: "3.12"
 
   checkpoint:
     runs-on: ubuntu-latest
     needs: [checkpoint-cp310-ubuntu-latest, checkpoint-cp311-ubuntu-latest, checkpoint-cp312-ubuntu-latest]
     steps:
@@ -138,15 +138,15 @@
             files.pythonhosted.org:443
             fulcio.sigstore.dev:443
             github.com:443
             pypi.org:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/release@3067778a8ac4622c1075321b46b7a7333bea64a0
+      - uses: OZI-Project/release@41916dbfb9a8fd0e73da21453fb999796cda9b52
         id: release
         with:
           python-dist: ${{ matrix.py }}
           github-token: ${{ secrets.GITHUB_TOKEN }}
 
   generate-provenance:
     needs: [release, checkpoint]
@@ -179,10 +179,10 @@
         disable-sudo: true
         egress-policy: block
         allowed-endpoints: >
           api.github.com:443
           upload.pypi.org:443
           uploads.github.com:443
 
-    - uses: OZI-Project/publish@d9173e726b4cbb2ecd631fff0259656737e0dc23
+    - uses: OZI-Project/publish@87aae4bed7ea3ab8b864689945200ecd71ecc29f
       with:
         github-token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `OZI-1.4.2/.github/workflows/scorecard.yml` & `OZI-1.4.3/.github/workflows/scorecard.yml`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             github.com:443
             oss-fuzz-build-logs.storage.googleapis.com:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
             www.bestpractices.dev:443
 
       - name: "Checkout code"
-        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
+        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
         with:
           persist-credentials: false
 
       - name: "Run analysis"
         uses: ossf/scorecard-action@0864cf19026789058feabb7e87baa5f140aac736 # v2.3.1
         with:
           results_file: results.sarif
```

### Comparing `OZI-1.4.2/.gitignore` & `OZI-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/CHANGELOG.md` & `OZI-1.4.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,52 @@
 # CHANGELOG
+## 1.4.3 (2024-05-08)
+
+### :arrow_up:
+
+* :arrow_up: Bump OZI-Project workflow actions
+
+* OZI-Project/checkpoint 0.1.6
+* OZI-Project/release 0.3.2
+* OZI-Project/release 0.1.1
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`fb19e5a`](https://github.com/OZI-Project/OZI/commit/fb19e5a1140d3a8fc617d7d3cdca0b8880e1e465))
+
+* :arrow_up: Bump actions/checkout from 4.1.4 to 4.1.5
+
+Bumps [actions/checkout](https://github.com/actions/checkout) from 4.1.4 to 4.1.5.
+- [Release notes](https://github.com/actions/checkout/releases)
+- [Changelog](https://github.com/actions/checkout/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/actions/checkout/compare/0ad4b8fadaa221de15dcec353f45205ec38ea70b...44c2b7a8a4ea60a981eaca3cf939b5f4305c123b)
+
+---
+updated-dependencies:
+- dependency-name: actions/checkout
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`971c548`](https://github.com/OZI-Project/OZI/commit/971c5483215457df5c70d99bcf34bb7513622882))
+
+### :hammer:
+
+* :hammer: clean up jinja2 import.
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`b6e6f50`](https://github.com/OZI-Project/OZI/commit/b6e6f505c8221bcab9e2f80ea44de65505cdc6ae))
+
+### :pencil2:
+
+* :pencil2: missing ``from __future__ import annotations``
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`508291a`](https://github.com/OZI-Project/OZI/commit/508291ade1880fdd0e96aeefb78d43265126f600))
+
+* :pencil2: fix RuntimeWarning that should be FutureWarning
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`0f23f31`](https://github.com/OZI-Project/OZI/commit/0f23f3121e2434cbe509b1230735c8a6dba56cd9))
+
 ## 1.4.2 (2024-05-05)
 
 ### :bug:
 
 * :bug: correct deprecated Python warnings.
 
 User-facing deprecation warnings should always use FutureWarning.
```

### Comparing `OZI-1.4.2/LICENSE.txt` & `OZI-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/PKG-INFO` & `OZI-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.4.2
+Version: 1.4.3
 Summary: Packager for Python projects using Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.4.2.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.4.3.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Rose Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
```

### Comparing `OZI-1.4.2/README.rst` & `OZI-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/meson.build` & `OZI-1.4.3/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/meson.options` & `OZI-1.4.3/meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/__main__.py` & `OZI-1.4.3/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/actions.py` & `OZI-1.4.3/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/comment.py` & `OZI-1.4.3/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/fix/__main__.py` & `OZI-1.4.3/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/fix/build_definition.py` & `OZI-1.4.3/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/fix/meson.build` & `OZI-1.4.3/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/fix/missing.py` & `OZI-1.4.3/ozi/fix/missing.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/fix/parser.py` & `OZI-1.4.3/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/fix/rewrite_command.py` & `OZI-1.4.3/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/lint/meson.build` & `OZI-1.4.3/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/lint/pyright/meson.build` & `OZI-1.4.3/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/meson.build` & `OZI-1.4.3/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/meson.py` & `OZI-1.4.3/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/new/__main__.py` & `OZI-1.4.3/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/new/meson.build` & `OZI-1.4.3/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/new/parser.py` & `OZI-1.4.3/ozi/new/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/new/validate.py` & `OZI-1.4.3/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/pkg_extra.py` & `OZI-1.4.3/ozi/pkg_extra.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/render.py` & `OZI-1.4.3/ozi/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # ozi/render.py
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 """Rendering utilities for the OZI project templates.
-
-.. versionremoved:: 1.2
-   The function ``load_environment`` was moved to ``blastpipe.ozi_templates``
-
 """
+from __future__ import annotations
+
 from pathlib import Path
+from typing import TYPE_CHECKING
 from warnings import warn
 
 from blastpipe.ozi_templates.filter import underscorify  # pyright: ignore
 from git import InvalidGitRepositoryError
 from git import Repo
-from jinja2 import Environment
-from jinja2 import TemplateNotFound
+
+if TYPE_CHECKING:
+    from jinja2 import Environment
 
 from ozi.spec import METADATA
 from ozi.tap import TAP
 
 
 def find_user_template(target: str, file: str, fix: str) -> str | None:
     """Find a user-defined project template file e.g. :file:`{target}/templates/{fix}/{file}`.
@@ -108,15 +108,15 @@
     Path(target, 'subprojects').mkdir()
     Path(target, 'tests').mkdir()
     templates = METADATA.spec.python.src.template
     for filename in templates.root:
         template = env.get_template(f'{filename}.j2')
         try:
             content = template.render(filename=filename)
-        except TemplateNotFound:  # pragma: defer to good-first-issue
+        except LookupError:  # pragma: defer to good-first-issue
             content = f'template "{filename}" failed to render.'
             warn(content, RuntimeWarning, stacklevel=0)
         with open(target / filename, 'w') as f:
             f.write(content)
 
     for filename in templates.source:
         template = env.get_template(f'{filename}.j2')
```

### Comparing `OZI-1.4.2/ozi/scripts/core_metadata_template.py` & `OZI-1.4.3/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/scripts/meson.build` & `OZI-1.4.3/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.4.3/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.4.3/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/scripts/render_requirements.py` & `OZI-1.4.3/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.4.3/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/scripts/scm_version_snip.py` & `OZI-1.4.3/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/scripts/to_distribution_template.py` & `OZI-1.4.3/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/scripts/version_metadata_template.py` & `OZI-1.4.3/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/spdx.py` & `OZI-1.4.3/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/spec/_license.py` & `OZI-1.4.3/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/spec/_spec.py` & `OZI-1.4.3/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/spec/base.py` & `OZI-1.4.3/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/spec/ci.py` & `OZI-1.4.3/ozi/spec/ci.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Publish(Default):
     """Publishing patterns for packaged project."""
 
     include: tuple[str, ...] = ('*.tar.gz', '*.whl', 'sig/*')
-    version: str = '0.1.0'
+    version: str = '0.1.1'
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Release(Default):
     """Release patterns for packaged project."""
 
-    version: str = '0.3.0'
+    version: str = '0.3.2'
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Checkpoint(Default):
     """Checkpoint suites to run."""
 
     suites: tuple[str, ...] = ('dist', 'lint', 'test')
-    version: str = '0.1.5'
+    version: str = '0.1.6'
 
 
 @dataclass(kw_only=True, frozen=True, eq=True)
 class CheckpointSuite(Default):
     """OZI checkpoint base class."""
 
     exclude: tuple[str, ...] = field(default_factory=tuple)
```

### Comparing `OZI-1.4.2/ozi/spec/meson.build` & `OZI-1.4.3/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/spec/pkg.py` & `OZI-1.4.3/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/spec/project.py` & `OZI-1.4.3/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/spec/python.py` & `OZI-1.4.3/ozi/spec/python.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,18 @@
     current_date: str = field(
         init=False,
         compare=False,
         default_factory=lambda: datetime.now(tz=timezone.utc).date().strftime(DATE_FORMAT),
     )
 
     def __post_init__(self: Self) -> None:
+        """Warn the user if the python version is deprecated or pending deprecation.
+
+        :raises: FutureWarning
+        """
         python3_eol = (
             datetime.strptime(
                 self.deprecation_schedule.get(
                     pyminor,
                     date(2008, 12, 3).strftime(DATE_FORMAT),
                 ),
                 DATE_FORMAT,
@@ -74,21 +78,21 @@
             .replace(tzinfo=timezone.utc)
             .date()
         )
         ozi_support_eol = python3_eol - timedelta(weeks=DEPRECATION_DELTA_WEEKS)
         if datetime.now(tz=timezone.utc).date() > python3_eol:  # pragma: no cover
             warn(
                 f'Python {pymajor}.{pyminor}.{pypatch} is not supported as of {python3_eol}.',
-                RuntimeWarning,
+                FutureWarning,
             )
         elif datetime.now(tz=timezone.utc).date() > ozi_support_eol:  # pragma: no cover
             warn(
                 f'Python {pymajor}.{pyminor}.{pypatch} support is pending deprecation '
                 f'as of {ozi_support_eol}.',
-                RuntimeWarning,
+                FutureWarning,
             )
 
     @cached_property
     def _minor_versions(self: Self) -> list[int]:
         return sorted(
             [
                 k
```

### Comparing `OZI-1.4.2/ozi/spec/src.py` & `OZI-1.4.3/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/tap.py` & `OZI-1.4.3/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/trove.py` & `OZI-1.4.3/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/vendor/email_validator/__init__.py` & `OZI-1.4.3/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/vendor/email_validator/__main__.py` & `OZI-1.4.3/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/vendor/email_validator/deliverability.py` & `OZI-1.4.3/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.4.3/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/vendor/email_validator/meson.build` & `OZI-1.4.3/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.4.3/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/vendor/email_validator/syntax.py` & `OZI-1.4.3/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/vendor/email_validator/validate_email.py` & `OZI-1.4.3/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/ozi/vendor/meson.build` & `OZI-1.4.3/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/pyproject.toml` & `OZI-1.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/templates/CHANGELOG.md.j2` & `OZI-1.4.3/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/tests/meson.build` & `OZI-1.4.3/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/tests/test_ozi_fix.py` & `OZI-1.4.3/tests/test_ozi_fix.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/tests/test_ozi_new.py` & `OZI-1.4.3/tests/test_ozi_new.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.2/tests/test_tap.py` & `OZI-1.4.3/tests/test_tap.py`

 * *Files identical despite different names*

