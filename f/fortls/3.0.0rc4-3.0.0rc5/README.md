# Comparing `tmp/fortls-3.0.0rc4.tar.gz` & `tmp/fortls-3.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortls-3.0.0rc4.tar", last modified: Sun May  5 15:14:33 2024, max compression
+gzip compressed data, was "fortls-3.0.0rc5.tar", last modified: Wed May  8 07:54:28 2024, max compression
```

## Comparing `fortls-3.0.0rc4.tar` & `fortls-3.0.0rc5.tar`

### file list

```diff
@@ -1,257 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.601407 fortls-3.0.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.553407 fortls-3.0.0rc4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.553407 fortls-3.0.0rc4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.553407 fortls-3.0.0rc4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/workflows/docs_preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.github/workflows/update-intrinsics.yml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    41497 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-05-05 15:14:33.601407 fortls-3.0.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.557407 fortls-3.0.0rc4/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.557407 fortls-3.0.0rc4/assets/animations/
--rw-r--r--   0 runner    (1001) docker     (127)  1647490 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/animations/intro-demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/f.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/logo2-animated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    78094 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/logos.workspace.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.569407 fortls-3.0.0rc4/assets/lsp/
--rw-r--r--   0 runner    (1001) docker     (127)   791746 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/completion-ani.gif
--rw-r--r--   0 runner    (1001) docker     (127)   450880 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/completion-ani.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/completion.png
--rw-r--r--   0 runner    (1001) docker     (127)   597393 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/definition-goto.gif
--rw-r--r--   0 runner    (1001) docker     (127)   335329 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/definition-goto.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/definition-peek.png
--rw-r--r--   0 runner    (1001) docker     (127)    49007 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/diagnostics1.png
--rw-r--r--   0 runner    (1001) docker     (127)    43464 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/doc-highlight.png
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/hover.png
--rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/hover2.png
--rw-r--r--   0 runner    (1001) docker     (127)    65080 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/references-peek.png
--rw-r--r--   0 runner    (1001) docker     (127)   703611 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/rename.gif
--rw-r--r--   0 runner    (1001) docker     (127)   355841 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/rename.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   304764 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/rename2.gif
--rw-r--r--   0 runner    (1001) docker     (127)   151579 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/rename2.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   628798 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/sig-help.gif
--rw-r--r--   0 runner    (1001) docker     (127)   418094 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/sig-help.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    50499 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/symbols-crop.png
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/symbols-doc.png
--rw-r--r--   0 runner    (1001) docker     (127)    25726 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/symbols-workspace.png
--rw-r--r--   0 runner    (1001) docker     (127)    54934 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/lsp/symbols.png
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/assets/symbol-class.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.569407 fortls-3.0.0rc4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/editor_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/fortls.parsers.internal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/fortls.parsers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/fortls.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.573407 fortls-3.0.0rc4/docs/html_extra/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/html_extra/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/html_extra/google3e426562ce42e98f.html
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/html_extra/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/options.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.573407 fortls-3.0.0rc4/fortls/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-05 15:14:33.000000 fortls-3.0.0rc4/fortls/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/fortls.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/ftypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/json_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/jsonrpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    74006 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/langserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.577407 fortls-3.0.0rc4/fortls/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.581407 fortls-3.0.0rc4/fortls/parsers/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/associate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/do.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/if_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/include.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    72890 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/intrinsic.modules.json
--rw-r--r--   0 runner    (1001) docker     (127)    44156 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/intrinsic.procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)   630782 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/intrinsic.procedures.markdown.json
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/intrinsics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/keywords.json
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    86130 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/statements.json
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/subroutine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/use.py
--rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/parsers/internal/where.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/regex_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/fortls/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.597407 fortls-3.0.0rc4/fortls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-05-05 15:14:33.000000 fortls-3.0.0rc4/fortls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-05 15:14:33.000000 fortls-3.0.0rc4/fortls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 15:14:33.000000 fortls-3.0.0rc4/fortls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 15:14:33.000000 fortls-3.0.0rc4/fortls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-05 15:14:33.000000 fortls-3.0.0rc4/fortls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 15:14:33.000000 fortls-3.0.0rc4/fortls.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.581407 fortls-3.0.0rc4/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/licenses/fortran-language-server-license.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 15:14:33.601407 fortls-3.0.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.585407 fortls-3.0.0rc4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/setup_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_preproc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_regex_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26297 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server_hover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_server_signature_help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.585407 fortls-3.0.0rc4/test/test_source/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/.fortls
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.589407 fortls-3.0.0rc4/test/test_source/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/completion/test_vis_mod_completion.f90
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/completion/use_only_interface.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.589407 fortls-3.0.0rc4/test/test_source/diag/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/conf_long_lines.json
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_contains.f90
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_critical.f90
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_enum.f90
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_external.f90
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_forall.f90
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_function.f90
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_function_arg_list.f90
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_implicit_none.f90
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_lines.f90
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_scope_end_name_var.f90
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_scope_overreach.f90
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_semicolon.f90
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_use_ordering.f90
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_var_shadowing_keyword_arg.f90
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_variable.f90
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_visibility.f90
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/diag/test_where.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.589407 fortls-3.0.0rc4/test/test_source/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/docs/test_doxygen.f90
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/docs/test_ford.f90
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/docs/test_module_and_type_doc.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.549407 fortls-3.0.0rc4/test/test_source/excldir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.593407 fortls-3.0.0rc4/test/test_source/excldir/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/excldir/sub1/tmp.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.593407 fortls-3.0.0rc4/test/test_source/excldir/sub2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/excldir/sub2/fake2.f90
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/f90_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.593407 fortls-3.0.0rc4/test/test_source/hover/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/hover/associate_block.f90
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/hover/associate_block_2.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/hover/functions.f90
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/hover/intent.f90
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/hover/parameters.f90
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/hover/pointers.f90
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/hover/recursive.f90
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/hover/spaced_keywords.f90
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/hover/types.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.593407 fortls-3.0.0rc4/test/test_source/imp/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/imp/import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/imp/submodule.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.593407 fortls-3.0.0rc4/test/test_source/include/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/include/empty.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.593407 fortls-3.0.0rc4/test/test_source/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/parse/line_continuations.f90
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/parse/submodule.f90
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/parse/test_incomplete_dims.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/parse/test_kinds_and_dims.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.597407 fortls-3.0.0rc4/test/test_source/pp/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/.fortls
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/.pp_conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.597407 fortls-3.0.0rc4/test/test_source/pp/include/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/include/petscerror.h
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/include/petscpc.h
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/preproc.F90
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/preproc_elif.F90
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/preproc_elif_elif_skip.F90
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/preproc_else.F90
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/preproc_if_elif_else.F90
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/preproc_if_elif_skip.F90
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/pp/preproc_keywords.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.597407 fortls-3.0.0rc4/test/test_source/rename/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/rename/test_rename_imp_type_bound_proc.f90
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/rename/test_rename_intrinsic.f90
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/rename/test_rename_nested.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.597407 fortls-3.0.0rc4/test/test_source/signature/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/signature/help.f90
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/signature/nested_sigs.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.597407 fortls-3.0.0rc4/test/test_source/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/subdir/test_abstract.f90
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/subdir/test_fixed.f
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/subdir/test_free.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/subdir/test_generic.f90
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/subdir/test_inc2.f90
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/subdir/test_inherit.f90
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/subdir/test_rename.F90
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/subdir/test_select.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/subdir/test_submod.F90
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/subdir/test_vis.f90
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/test.f90
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/test_block.f08
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/test_diagnostic_int.f90
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/test_import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/test_inc.f90
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/test_nonintrinsic.f90
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/test_prog.f08
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/test_submodule.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:14:33.597407 fortls-3.0.0rc4/test/test_source/use/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/use/use.f90
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 15:14:27.000000 fortls-3.0.0rc4/test/test_source/wrong_syntax.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.663565 fortls-3.0.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.619565 fortls-3.0.0rc5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.619565 fortls-3.0.0rc5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.619565 fortls-3.0.0rc5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/docs_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/update-intrinsics.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    41497 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-05-08 07:54:28.663565 fortls-3.0.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.623565 fortls-3.0.0rc5/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.623565 fortls-3.0.0rc5/assets/animations/
+-rw-r--r--   0 runner    (1001) docker     (127)  1647490 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/animations/intro-demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/f.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/logo2-animated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    78094 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/logos.workspace.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.635565 fortls-3.0.0rc5/assets/lsp/
+-rw-r--r--   0 runner    (1001) docker     (127)   791746 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/completion-ani.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   450880 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/completion-ani.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/completion.png
+-rw-r--r--   0 runner    (1001) docker     (127)   597393 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/definition-goto.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   335329 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/definition-goto.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/definition-peek.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49007 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/diagnostics1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43464 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/doc-highlight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/hover2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65080 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/references-peek.png
+-rw-r--r--   0 runner    (1001) docker     (127)   703611 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/rename.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   355841 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/rename.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   304764 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/rename2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   151579 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/rename2.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   628798 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/sig-help.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   418094 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/sig-help.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    50499 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/symbols-crop.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/symbols-doc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25726 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/symbols-workspace.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54934 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/symbols.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/symbol-class.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.635565 fortls-3.0.0rc5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/editor_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/fortls.parsers.internal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/fortls.parsers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/fortls.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.635565 fortls-3.0.0rc5/docs/html_extra/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/html_extra/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/html_extra/google3e426562ce42e98f.html
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/html_extra/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/options.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.639565 fortls-3.0.0rc5/fortls/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/fortls.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/ftypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/json_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/jsonrpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74006 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/langserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.639565 fortls-3.0.0rc5/fortls/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.647565 fortls-3.0.0rc5/fortls/parsers/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/do.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/if_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72890 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.modules.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44156 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)   630782 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.procedures.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/intrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/keywords.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86115 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/statements.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/subroutine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/use.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/where.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/regex_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/fortls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.647565 fortls-3.0.0rc5/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/licenses/fortran-language-server-license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 07:54:28.663565 fortls-3.0.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.647565 fortls-3.0.0rc5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/setup_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_preproc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_regex_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26297 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_hover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_signature_help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.651565 fortls-3.0.0rc5/test/test_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/.fortls
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.651565 fortls-3.0.0rc5/test/test_source/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/completion/test_vis_mod_completion.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/completion/use_only_interface.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.651565 fortls-3.0.0rc5/test/test_source/diag/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/conf_long_lines.json
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_contains.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_critical.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_enum.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_external.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_forall.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_function.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_function_arg_list.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_implicit_none.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_lines.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_scope_end_name_var.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_scope_overreach.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_semicolon.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_use_ordering.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_var_shadowing_keyword_arg.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_variable.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_visibility.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_where.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/docs/test_doxygen.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/docs/test_ford.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/docs/test_module_and_type_doc.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.615565 fortls-3.0.0rc5/test/test_source/excldir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/excldir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/excldir/sub1/tmp.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/excldir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/excldir/sub2/fake2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/f90_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/hover/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/associate_block.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/associate_block_2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/functions.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/intent.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/parameters.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/pointers.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/recursive.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/spaced_keywords.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/types.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/imp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/imp/import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/imp/submodule.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/include/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/include/empty.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/parse/line_continuations.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/parse/submodule.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/parse/test_incomplete_dims.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/parse/test_kinds_and_dims.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/pp/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/.fortls
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/.pp_conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/pp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/include/petscerror.h
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/include/petscpc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_elif.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_elif_elif_skip.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_else.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_if_elif_else.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_if_elif_skip.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_keywords.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/rename/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/rename/test_rename_imp_type_bound_proc.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/rename/test_rename_intrinsic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/rename/test_rename_nested.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/signature/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/signature/help.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/signature/nested_sigs.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_abstract.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_fixed.f
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_free.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_generic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_inc2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_inherit.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_rename.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_select.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_submod.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_vis.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_block.f08
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_diagnostic_int.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_inc.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_nonintrinsic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_prog.f08
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_submodule.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/use/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/use/use.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/vis/private.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/wrong_syntax.json
```

### Comparing `fortls-3.0.0rc4/.github/FUNDING.yml` & `fortls-3.0.0rc5/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/.github/ISSUE_TEMPLATE/bug_report.md` & `fortls-3.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/.github/ISSUE_TEMPLATE/feature_request.md` & `fortls-3.0.0rc5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/.github/workflows/codeql-analysis.yml` & `fortls-3.0.0rc5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/.github/workflows/docs_preview.yml` & `fortls-3.0.0rc5/.github/workflows/docs_preview.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/.github/workflows/main.yml` & `fortls-3.0.0rc5/.github/workflows/main.yml`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
           python3 -m fortls.schema
           git diff --exit-code ./fortls/fortls.schema.json
 
       - name: Unittests
         run: pytest --doctest-modules -n auto
 
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v4
+        uses: codecov/codecov-action@v4.3.1
         with:
           fail_ci_if_error: true
           verbose: true
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `fortls-3.0.0rc4/.github/workflows/python-publish.yml` & `fortls-3.0.0rc5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/.github/workflows/update-intrinsics.yml` & `fortls-3.0.0rc5/.github/workflows/update-intrinsics.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/.pre-commit-config.yaml` & `fortls-3.0.0rc5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/CHANGELOG.md` & `fortls-3.0.0rc5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/CODE_OF_CONDUCT.md` & `fortls-3.0.0rc5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/CONTRIBUTING.md` & `fortls-3.0.0rc5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/LICENSE` & `fortls-3.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/PKG-INFO` & `fortls-3.0.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortls
-Version: 3.0.0rc4
+Version: 3.0.0rc5
 Summary: fortls - Fortran Language Server
 Author-email: Giannis Nikiteas <giannis.nikiteas@gmail.com>
 License: MIT
 Project-URL: homepage, https://fortls.fortran-lang.org
 Project-URL: Documentation, https://fortls.fortran-lang.org
 Project-URL: Changes, https://github.com/fortran-lang/fortls/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/fortran-lang/fortls/issues
```

### Comparing `fortls-3.0.0rc4/README.md` & `fortls-3.0.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/SECURITY.md` & `fortls-3.0.0rc5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/LICENSE` & `fortls-3.0.0rc5/assets/LICENSE`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/README.md` & `fortls-3.0.0rc5/assets/README.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/animations/intro-demo.gif` & `fortls-3.0.0rc5/assets/animations/intro-demo.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/f.svg` & `fortls-3.0.0rc5/assets/f.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/icon.svg` & `fortls-3.0.0rc5/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/logo.png` & `fortls-3.0.0rc5/assets/logo.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/logo.svg` & `fortls-3.0.0rc5/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/logo2-animated.svg` & `fortls-3.0.0rc5/assets/logo2-animated.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/logos.workspace.svg` & `fortls-3.0.0rc5/assets/logos.workspace.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/completion-ani.gif` & `fortls-3.0.0rc5/assets/lsp/completion-ani.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/completion-ani.mp4` & `fortls-3.0.0rc5/assets/lsp/completion-ani.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/completion.png` & `fortls-3.0.0rc5/assets/lsp/completion.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/definition-goto.gif` & `fortls-3.0.0rc5/assets/lsp/definition-goto.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/definition-goto.mp4` & `fortls-3.0.0rc5/assets/lsp/definition-goto.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/definition-peek.png` & `fortls-3.0.0rc5/assets/lsp/definition-peek.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/diagnostics1.png` & `fortls-3.0.0rc5/assets/lsp/diagnostics1.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/doc-highlight.png` & `fortls-3.0.0rc5/assets/lsp/doc-highlight.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/hover.png` & `fortls-3.0.0rc5/assets/lsp/hover.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/hover2.png` & `fortls-3.0.0rc5/assets/lsp/hover2.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/references-peek.png` & `fortls-3.0.0rc5/assets/lsp/references-peek.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/rename.gif` & `fortls-3.0.0rc5/assets/lsp/rename.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/rename.mp4` & `fortls-3.0.0rc5/assets/lsp/rename.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/rename2.gif` & `fortls-3.0.0rc5/assets/lsp/rename2.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/rename2.mp4` & `fortls-3.0.0rc5/assets/lsp/rename2.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/sig-help.gif` & `fortls-3.0.0rc5/assets/lsp/sig-help.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/sig-help.mp4` & `fortls-3.0.0rc5/assets/lsp/sig-help.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/symbols-crop.png` & `fortls-3.0.0rc5/assets/lsp/symbols-crop.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/symbols-doc.png` & `fortls-3.0.0rc5/assets/lsp/symbols-doc.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/symbols-workspace.png` & `fortls-3.0.0rc5/assets/lsp/symbols-workspace.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/lsp/symbols.png` & `fortls-3.0.0rc5/assets/lsp/symbols.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/assets/symbol-class.svg` & `fortls-3.0.0rc5/assets/symbol-class.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/Makefile` & `fortls-3.0.0rc5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/conf.py` & `fortls-3.0.0rc5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/contact.rst` & `fortls-3.0.0rc5/docs/contact.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/contributing.rst` & `fortls-3.0.0rc5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/editor_integration.rst` & `fortls-3.0.0rc5/docs/editor_integration.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/features.rst` & `fortls-3.0.0rc5/docs/features.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/fortls.parsers.internal.rst` & `fortls-3.0.0rc5/docs/fortls.parsers.internal.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/fortls.rst` & `fortls-3.0.0rc5/docs/fortls.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/index.rst` & `fortls-3.0.0rc5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/make.bat` & `fortls-3.0.0rc5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/options.rst` & `fortls-3.0.0rc5/docs/options.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/docs/quickstart.rst` & `fortls-3.0.0rc5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/__init__.py` & `fortls-3.0.0rc5/fortls/__init__.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/constants.py` & `fortls-3.0.0rc5/fortls/constants.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/debug.py` & `fortls-3.0.0rc5/fortls/debug.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/fortls.schema.json` & `fortls-3.0.0rc5/fortls/fortls.schema.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/ftypes.py` & `fortls-3.0.0rc5/fortls/ftypes.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/helper_functions.py` & `fortls-3.0.0rc5/fortls/helper_functions.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/interface.py` & `fortls-3.0.0rc5/fortls/interface.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/json_templates.py` & `fortls-3.0.0rc5/fortls/json_templates.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/jsonrpc.py` & `fortls-3.0.0rc5/fortls/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/langserver.py` & `fortls-3.0.0rc5/fortls/langserver.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/associate.py` & `fortls-3.0.0rc5/fortls/parsers/internal/associate.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/ast.py` & `fortls-3.0.0rc5/fortls/parsers/internal/ast.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 from .use import Use
 from .variable import Variable
 
 
 class FortranAST:
     def __init__(self, file_obj=None):
         self.file = file_obj
-        self.path: str = None
-        if file_obj is not None:
-            self.path = file_obj.path
+        self.path: str | None = file_obj.path if file_obj is not None else None
         self.global_dict: dict = {}
         self.scope_list: list = []
         self.variable_list: list = []
         self.public_list: list = []
         self.private_list: list = []
         self.scope_stack: list = []
         self.end_stack: list = []
@@ -35,18 +33,18 @@
         self.parse_errors: list = []
         self.inherit_objs: list = []
         self.linkable_objs: list = []
         self.external_objs: list = []
         self.none_scope = None
         self.inc_scope = None
         self.current_scope = None
-        self.END_SCOPE_REGEX: Pattern = None
-        self.enc_scope_name: str = None
+        self.end_scope_regex: Pattern | None = None
+        self.enc_scope_name: str | None = None
         self.last_obj = None
-        self.pending_doc: str = None
+        self.pending_doc: str | None = None
 
     def create_none_scope(self):
         """Create empty scope to hold non-module contained items"""
         if self.none_scope is not None:
             raise ValueError
         self.none_scope = Program(self, 1, "main")
         self.add_scope(
@@ -56,15 +54,15 @@
     def get_enc_scope_name(self):
         """Get current enclosing scope name"""
         return None if self.current_scope is None else self.current_scope.FQSN
 
     def add_scope(
         self,
         new_scope: Scope,
-        END_SCOPE_REGEX: Pattern[str],
+        end_scope_regex: Pattern[str],
         exportable: bool = True,
         req_container: bool = False,
     ):
         self.scope_list.append(new_scope)
         if new_scope.require_inherit():
             self.inherit_objs.append(new_scope)
         if new_scope.require_link():
@@ -76,18 +74,18 @@
                 self.current_scope.add_child(new_scope)
                 self.scope_stack.append(self.current_scope)
             elif exportable:
                 self.global_dict[new_scope.FQSN] = new_scope
         else:
             self.current_scope.add_child(new_scope)
             self.scope_stack.append(self.current_scope)
-        if self.END_SCOPE_REGEX is not None:
-            self.end_stack.append(self.END_SCOPE_REGEX)
+        if self.end_scope_regex is not None:
+            self.end_stack.append(self.end_scope_regex)
         self.current_scope = new_scope
-        self.END_SCOPE_REGEX = END_SCOPE_REGEX
+        self.end_scope_regex = end_scope_regex
         self.enc_scope_name = self.get_enc_scope_name()
         self.last_obj = new_scope
         if self.pending_doc is not None:
             self.last_obj.add_doc(self.pending_doc)
             self.pending_doc = None
 
     def end_scope(self, line_number: int, check: bool = True):
@@ -98,17 +96,17 @@
             return
         self.current_scope.end(line_number)
         if len(self.scope_stack) > 0:
             self.current_scope = self.scope_stack.pop()
         else:
             self.current_scope = None
         if len(self.end_stack) > 0:
-            self.END_SCOPE_REGEX = self.end_stack.pop()
+            self.end_scope_regex = self.end_stack.pop()
         else:
-            self.END_SCOPE_REGEX = None
+            self.end_scope_regex = None
         self.enc_scope_name = self.get_enc_scope_name()
 
     def add_variable(self, new_var: Variable):
         if self.current_scope is None:
             self.create_none_scope()
             new_var.FQSN = f"{self.none_scope.FQSN}::{new_var.name.lower()}"
         self.current_scope.add_child(new_var)
@@ -166,19 +164,19 @@
         """
         # Convert from Editor line numbers 1-base index to LSP index which is 0-based
         self.parse_errors.append(diagnostic_json(ln - 1, sch, ln - 1, ech, msg, sev))
 
     def start_ppif(self, line_number: int):
         self.pp_if.append([line_number - 1, -1])
 
-    def end_ppif(self, line_number):
+    def end_ppif(self, line_number: int):
         if len(self.pp_if) > 0:
             self.pp_if[-1][1] = line_number - 1
 
-    def get_scopes(self, line_number: int = None):
+    def get_scopes(self, line_number: int | None = None):
         """Get a list of all the scopes present in the line number provided.
 
         Parameters
         ----------
         line_number : int, optional
             Document line number, if None return all document scopes, by default None
 
@@ -187,73 +185,77 @@
         Variable,Type,Function,Subroutine,Module,Program,Interface,BlockData
             A list of scopes
         """
         if line_number is None:
             return self.scope_list
         scope_list = []
         for scope in self.scope_list:
-            if (line_number >= scope.sline) and (line_number <= scope.eline):
-                if type(scope.parent) is Interface:
-                    for use_stmnt in scope.use:
-                        if type(use_stmnt) is not Import:
-                            continue
-                        # Exclude the parent and all other scopes
-                        if use_stmnt.import_type == ImportTypes.NONE:
-                            return [scope]
-                scope_list.append(scope)
-                scope_list.extend(iter(scope.get_ancestors()))
+            if not scope.sline <= line_number <= scope.eline:
+                continue
+            if type(scope.parent) is Interface:
+                for use_stmnt in scope.use:
+                    if type(use_stmnt) is not Import:
+                        continue
+                    # Exclude the parent and all other scopes
+                    if use_stmnt.import_type == ImportTypes.NONE:
+                        return [scope]
+            scope_list.append(scope)
+            scope_list.extend(iter(scope.get_ancestors()))
         if scope_list or self.none_scope is None:
             return scope_list
-        else:
-            return [self.none_scope]
+        return [self.none_scope]
 
     def get_inner_scope(self, line_number: int):
         scope_sline = -1
         curr_scope = None
         for scope in self.scope_list:
-            if scope.sline > scope_sline and (
-                (line_number >= scope.sline) and (line_number <= scope.eline)
-            ):
+            if scope.sline > scope_sline and scope.sline <= line_number <= scope.eline:
                 curr_scope = scope
                 scope_sline = scope.sline
         if (curr_scope is None) and (self.none_scope is not None):
             return self.none_scope
         return curr_scope
 
     def get_object(self, FQSN: str):
-        FQSN_split = FQSN.split("::")
-        curr_obj = self.global_dict.get(FQSN_split[0])
-        if curr_obj is None:
-            # Look for non-exportable scopes
-            for scope in self.scope_list:
-                if FQSN_split[0] == scope.FQSN:
-                    curr_obj = scope
-                    break
-        if curr_obj is None:
+        def find_child_by_name(parent, name):
+            for child in parent.children:
+                if child.name == name:
+                    return child
+                if child.name.startswith("#GEN_INT"):
+                    found = next(
+                        (
+                            int_child
+                            for int_child in child.get_children()
+                            if int_child.name == name
+                        ),
+                        None,
+                    )
+                    if found:
+                        return found
             return None
-        if len(FQSN_split) > 1:
-            for name in FQSN_split[1:]:
-                next_obj = None
-                for child in curr_obj.children:
-                    if child.name.startswith("#GEN_INT"):
-                        for int_child in child.get_children():
-                            if int_child.name == name:
-                                next_obj = int_child
-                                break
-                        if next_obj is not None:
-                            break
-                    if child.name == name:
-                        next_obj = child
-                        break
-                if next_obj is None:
-                    return None
-                curr_obj = next_obj
-        return curr_obj
 
-    def resolve_includes(self, workspace, path: str = None):
+        parts = FQSN.split("::")
+        current = self.global_dict.get(parts[0])
+
+        # Look for non-exportable scopes
+        if current is None:
+            current = next(
+                (scope for scope in self.scope_list if scope.FQSN == parts[0]), None
+            )
+            if current is None:
+                return None
+
+        for part in parts[1:]:
+            current = find_child_by_name(current, part)
+            if current is None:
+                return None
+
+        return current
+
+    def resolve_includes(self, workspace, path: str | None = None):
         file_dir = os.path.dirname(self.path)
         for inc in self.include_statements:
             file_path = os.path.normpath(os.path.join(file_dir, inc.path))
             if path and path != file_path:
                 continue
             parent_scope = self.get_inner_scope(inc.line_number)
             added_entities = inc.scope_objs
```

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/base.py` & `fortls-3.0.0rc5/fortls/parsers/internal/base.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/block.py` & `fortls-3.0.0rc5/fortls/parsers/internal/block.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/diagnostics.py` & `fortls-3.0.0rc5/fortls/parsers/internal/diagnostics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/function.py` & `fortls-3.0.0rc5/fortls/parsers/internal/function.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/imports.py` & `fortls-3.0.0rc5/fortls/parsers/internal/imports.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/interface.py` & `fortls-3.0.0rc5/fortls/parsers/internal/interface.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/intrinsic.modules.json` & `fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.modules.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/intrinsic.procedures.json` & `fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.procedures.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/intrinsic.procedures.markdown.json` & `fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.procedures.markdown.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/intrinsics.py` & `fortls-3.0.0rc5/fortls/parsers/internal/intrinsics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/keywords.json` & `fortls-3.0.0rc5/fortls/parsers/internal/keywords.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/method.py` & `fortls-3.0.0rc5/fortls/parsers/internal/method.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/module.py` & `fortls-3.0.0rc5/fortls/parsers/internal/module.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/parser.py` & `fortls-3.0.0rc5/fortls/parsers/internal/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     from typing_extensions import Literal
 
 from re import Match, Pattern
 
 from fortls.constants import (
     DO_TYPE_ID,
     INTERFACE_TYPE_ID,
-    MODULE_TYPE_ID,
     SELECT_TYPE_ID,
     SUBMODULE_TYPE_ID,
     FRegex,
     Severity,
     log,
 )
 from fortls.ftypes import (
@@ -1348,15 +1347,15 @@
                 line_no_comment = line
             # Split lines with semicolons, place the multiple lines into a stack
             if line_stripped.find(";") >= 0:
                 multi_lines.extendleft(line_stripped.split(";"))
                 line = multi_lines.pop()
                 line_stripped = line
             # Test for scope end
-            if file_ast.END_SCOPE_REGEX is not None:
+            if file_ast.end_scope_regex is not None:
                 match = FRegex.END_WORD.match(line_no_comment)
                 # Handle end statement
                 if self.parse_end_scope_word(line_no_comment, line_no, file_ast, match):
                     continue
                 # Look for old-style end of DO loops with line labels
                 if self.parse_do_fixed_format(
                     line, line_no, file_ast, line_label, block_id_stack
@@ -1653,18 +1652,18 @@
                 log.debug("%s !!! INCLUDE - Ln:%d", line, line_no)
 
             elif obj_type == "vis":
                 if file_ast.current_scope is None:
                     msg = "Visibility statement without enclosing scope"
                     file_ast.add_error(msg, Severity.error, line_no, 0)
                 else:
-                    if (len(obj_info.obj_names) == 0) and (obj_info.type == 1):
+                    if len(obj_info.obj_names) == 0 and obj_info.type == 1:  # private
                         file_ast.current_scope.set_default_vis(-1)
                     else:
-                        if obj_info.type == MODULE_TYPE_ID:
+                        if obj_info.type == 1:  # private
                             for word in obj_info.obj_names:
                                 file_ast.add_private(word)
                         else:
                             for word in obj_info.obj_names:
                                 file_ast.add_public(word)
                 log.debug("%s !!! VISIBILITY - Ln:%d", line, line_no)
 
@@ -1762,15 +1761,15 @@
         if match.group(1) is None:
             end_scope_word = ""
             if file_ast.current_scope.req_named_end() and (
                 file_ast.current_scope is not file_ast.none_scope
             ):
                 file_ast.end_errors.append([ln, file_ast.current_scope.sline])
         else:
-            scope_match = file_ast.END_SCOPE_REGEX.match(line[match.start(1) :])
+            scope_match = file_ast.end_scope_regex.match(line[match.start(1) :])
             if scope_match is not None:
                 end_scope_word = scope_match.group(0)
         if end_scope_word is not None:
             if (file_ast.current_scope.get_type() == SELECT_TYPE_ID) and (
                 file_ast.current_scope.is_type_region()
             ):
                 file_ast.end_scope(ln)
```

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/scope.py` & `fortls-3.0.0rc5/fortls/parsers/internal/scope.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/select.py` & `fortls-3.0.0rc5/fortls/parsers/internal/select.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/statements.json` & `fortls-3.0.0rc5/fortls/parsers/internal/statements.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/submodule.py` & `fortls-3.0.0rc5/fortls/parsers/internal/submodule.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/subroutine.py` & `fortls-3.0.0rc5/fortls/parsers/internal/subroutine.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/type.py` & `fortls-3.0.0rc5/fortls/parsers/internal/type.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/use.py` & `fortls-3.0.0rc5/fortls/parsers/internal/use.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/utilities.py` & `fortls-3.0.0rc5/fortls/parsers/internal/utilities.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/parsers/internal/variable.py` & `fortls-3.0.0rc5/fortls/parsers/internal/variable.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/regex_patterns.py` & `fortls-3.0.0rc5/fortls/regex_patterns.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls/schema.py` & `fortls-3.0.0rc5/fortls/schema.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/fortls.egg-info/PKG-INFO` & `fortls-3.0.0rc5/fortls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortls
-Version: 3.0.0rc4
+Version: 3.0.0rc5
 Summary: fortls - Fortran Language Server
 Author-email: Giannis Nikiteas <giannis.nikiteas@gmail.com>
 License: MIT
 Project-URL: homepage, https://fortls.fortran-lang.org
 Project-URL: Documentation, https://fortls.fortran-lang.org
 Project-URL: Changes, https://github.com/fortran-lang/fortls/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/fortran-lang/fortls/issues
```

### Comparing `fortls-3.0.0rc4/fortls.egg-info/SOURCES.txt` & `fortls-3.0.0rc5/fortls.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -217,8 +217,9 @@
 test/test_source/subdir/test_generic.f90
 test/test_source/subdir/test_inc2.f90
 test/test_source/subdir/test_inherit.f90
 test/test_source/subdir/test_rename.F90
 test/test_source/subdir/test_select.f90
 test/test_source/subdir/test_submod.F90
 test/test_source/subdir/test_vis.f90
-test/test_source/use/use.f90
+test/test_source/use/use.f90
+test/test_source/vis/private.f90
```

### Comparing `fortls-3.0.0rc4/licenses/fortran-language-server-license.txt` & `fortls-3.0.0rc5/licenses/fortran-language-server-license.txt`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/pyproject.toml` & `fortls-3.0.0rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 Tracker = "https://github.com/fortran-lang/fortls/issues"
 "Source Code" = "https://github.com/fortran-lang/fortls"
 
 [project.scripts]
 fortls = "fortls.__init__:main"
 
 [tool.setuptools.packages.find]
-include = ["fortls"]
+include = ["fortls*"]
 
 [tool.setuptools.package-data]
 fortls = ["parsers/internal/*.json"]
 
 [tool.setuptools_scm]
 write_to = "fortls/_version.py"
```

### Comparing `fortls-3.0.0rc4/test/setup_tests.py` & `fortls-3.0.0rc5/test/setup_tests.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_interface.py` & `fortls-3.0.0rc5/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_parser.py` & `fortls-3.0.0rc5/test/test_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,7 +27,15 @@
         assert ast.scope_list[0].name == "val"
         assert ast.scope_list[0].ancestor_name == "p1"
         assert ast.scope_list[1].name == ""
         assert ast.scope_list[1].ancestor_name == "p2"
     except Exception as e:
         print(e)
         assert False
+
+
+def test_private_visibility_interfaces():
+    file_path = test_dir / "vis" / "private.f90"
+    file = FortranFile(str(file_path))
+    err_str, _ = file.load_from_disk()
+    file.parse()
+    assert err_str is None
```

### Comparing `fortls-3.0.0rc4/test/test_preproc.py` & `fortls-3.0.0rc5/test/test_preproc.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_preproc_parser.py` & `fortls-3.0.0rc5/test/test_preproc_parser.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_regex_patterns.py` & `fortls-3.0.0rc5/test/test_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server.py` & `fortls-3.0.0rc5/test/test_server.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server_completion.py` & `fortls-3.0.0rc5/test/test_server_completion.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server_definitions.py` & `fortls-3.0.0rc5/test/test_server_definitions.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server_diagnostics.py` & `fortls-3.0.0rc5/test/test_server_diagnostics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server_documentation.py` & `fortls-3.0.0rc5/test/test_server_documentation.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server_hover.py` & `fortls-3.0.0rc5/test/test_server_hover.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server_implementation.py` & `fortls-3.0.0rc5/test/test_server_implementation.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server_messages.py` & `fortls-3.0.0rc5/test/test_server_messages.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server_references.py` & `fortls-3.0.0rc5/test/test_server_references.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server_rename.py` & `fortls-3.0.0rc5/test/test_server_rename.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_server_signature_help.py` & `fortls-3.0.0rc5/test/test_server_signature_help.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/completion/use_only_interface.f90` & `fortls-3.0.0rc5/test/test_source/completion/use_only_interface.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/diag/test_function_arg_list.f90` & `fortls-3.0.0rc5/test/test_source/diag/test_function_arg_list.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/diag/test_scope_overreach.f90` & `fortls-3.0.0rc5/test/test_source/diag/test_scope_overreach.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/diag/test_semicolon.f90` & `fortls-3.0.0rc5/test/test_source/diag/test_semicolon.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/docs/test_doxygen.f90` & `fortls-3.0.0rc5/test/test_source/docs/test_doxygen.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/docs/test_ford.f90` & `fortls-3.0.0rc5/test/test_source/docs/test_ford.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/excldir/sub1/tmp.f90` & `fortls-3.0.0rc5/test/test_source/excldir/sub1/tmp.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/f90_config.json` & `fortls-3.0.0rc5/test/test_source/f90_config.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/hover/functions.f90` & `fortls-3.0.0rc5/test/test_source/hover/functions.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/hover/parameters.f90` & `fortls-3.0.0rc5/test/test_source/hover/parameters.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/hover/recursive.f90` & `fortls-3.0.0rc5/test/test_source/hover/recursive.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/imp/import.f90` & `fortls-3.0.0rc5/test/test_source/imp/import.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/imp/submodule.f90` & `fortls-3.0.0rc5/test/test_source/imp/submodule.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/parse/test_kinds_and_dims.f90` & `fortls-3.0.0rc5/test/test_source/parse/test_kinds_and_dims.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/pp/preproc_elif.F90` & `fortls-3.0.0rc5/test/test_source/pp/preproc_elif.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/pp/preproc_elif_elif_skip.F90` & `fortls-3.0.0rc5/test/test_source/pp/preproc_elif_elif_skip.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/pp/preproc_if_elif_else.F90` & `fortls-3.0.0rc5/test/test_source/pp/preproc_if_elif_else.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/pp/preproc_if_elif_skip.F90` & `fortls-3.0.0rc5/test/test_source/pp/preproc_if_elif_skip.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/rename/test_rename_intrinsic.f90` & `fortls-3.0.0rc5/test/test_source/rename/test_rename_intrinsic.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/signature/help.f90` & `fortls-3.0.0rc5/test/test_source/signature/help.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/subdir/test_fixed.f` & `fortls-3.0.0rc5/test/test_source/subdir/test_fixed.f`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/subdir/test_free.f90` & `fortls-3.0.0rc5/test/test_source/subdir/test_free.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/subdir/test_generic.f90` & `fortls-3.0.0rc5/test/test_source/subdir/test_generic.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/subdir/test_select.f90` & `fortls-3.0.0rc5/test/test_source/subdir/test_select.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/subdir/test_submod.F90` & `fortls-3.0.0rc5/test/test_source/subdir/test_submod.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/test_diagnostic_int.f90` & `fortls-3.0.0rc5/test/test_source/test_diagnostic_int.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc4/test/test_source/test_prog.f08` & `fortls-3.0.0rc5/test/test_source/test_prog.f08`

 * *Files identical despite different names*

