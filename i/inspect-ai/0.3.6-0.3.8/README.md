# Comparing `tmp/inspect_ai-0.3.6.tar.gz` & `tmp/inspect_ai-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspect_ai-0.3.6.tar", last modified: Mon May  6 20:23:28 2024, max compression
+gzip compressed data, was "inspect_ai-0.3.8.tar", last modified: Tue May  7 22:49:42 2024, max compression
```

## Comparing `inspect_ai-0.3.6.tar` & `inspect_ai-0.3.8.tar`

### file list

```diff
@@ -1,369 +1,491 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.605315 inspect_ai-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.541315 inspect_ai-0.3.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.541315 inspect_ai-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.541315 inspect_ai-0.3.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-06 20:23:28.601315 inspect_ai-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.541315 inspect_ai-0.3.6/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/arc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.545315 inspect_ai-0.3.6/benchmarks/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/datasets/math_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/datasets/mmlu.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/gpqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/gsm8k.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/hellaswag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/mathematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/mmlu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.545315 inspect_ai-0.3.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.549315 inspect_ai-0.3.6/docs/_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/arc.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/biology_qa.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/footer.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/gsm8k.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/hellaswag.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/mathematics.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/popularity.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/security_guide.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/theory_of_mind.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/tool_use.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.549315 inspect_ai-0.3.6/docs/_format/
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_format/pre-render.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_variables.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/datasets.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/eval-logs.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/eval-suites.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/eval-tuning.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/examples.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.557315 inspect_ai-0.3.6/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/aisi-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/eval-log.png
--rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-answers.png
--rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-history.png
--rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-home.png
--rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-info.png
--rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-logging-console.png
--rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-logging.png
--rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-main.png
--rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-messages.png
--rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-metadata.png
--rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-scoring.png
--rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-sort.png
--rw-r--r--   0 runner    (1001) docker     (127)    90624 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/popularity.png
--rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/rate-limit.png
--rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/running-theory.png
--rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/log-viewer.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    18564 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/models.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/scorers.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/solvers.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/theme.scss
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/tools.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/workflow.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.557315 inspect_ai-0.3.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.533316 inspect_ai-0.3.6/examples/agents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.557315 inspect_ai-0.3.6/examples/agents/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/.env.example
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/inspect_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/wikipedia.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/biology_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/popularity.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/security_guide.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/theory_of_mind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/tool_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:23:28.605315 inspect_ai-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.533316 inspect_ai-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.561315 inspect_ai-0.3.6/src/inspect_ai/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.561315 inspect_ai-0.3.6/src/inspect_ai/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/score.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.561315 inspect_ai-0.3.6/src/inspect_ai/_display/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_display/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_display/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_display/rich.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.565315 inspect_ai-0.3.6/src/inspect_ai/_eval/
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/score.py
--rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_view/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_view/www/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/App.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/api.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.533316 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.573315 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/json5.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.573315 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/purify.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/showdown.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/log-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/log.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.573315 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/hooks.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.573315 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/htm/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/htm/htm.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/htm/preact.js
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/htm/preact.mjs
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/preact-hooks.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/preact.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.573315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/App.css
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/Constants.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/Register.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/Card.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ChatView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/CopyButton.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/Dialog.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MessageContent.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/TabSet.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ToolButton.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ansi-output.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SampleView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/title/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.581315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/Format.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/Git.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/Path.mjs
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/Type.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.581315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/tools.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.581315 inspect_ai-0.3.6/src/inspect_ai/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.581315 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/bias_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/biology_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/popularity.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/security_guide.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.581315 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.585315 inspect_ai-0.3.6/src/inspect_ai/log/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/log/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/log/_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.585315 inspect_ai-0.3.6/src/inspect_ai/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31683 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.585315 inspect_ai-0.3.6/src/inspect_ai/model/_providers/
--rw-r--r--   0 runner    (1001) docker     (127)    29724 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/azureai.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/google.py
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/together.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.589315 inspect_ai-0.3.6/src/inspect_ai/scorer/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.589315 inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/std.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.589315 inspect_ai-0.3.6/src/inspect_ai/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_critique.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_multiple_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.589315 inspect_ai-0.3.6/src/inspect_ai/solver/_tool/
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_tool/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_tool/tool_def.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_tool/use_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_tool/web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.589315 inspect_ai-0.3.6/src/inspect_ai/util/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.593315 inspect_ai-0.3.6/src/inspect_ai/util/_context/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/_context/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/_context/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/_context/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/_context/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.601315 inspect_ai-0.3.6/src/inspect_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_cloudlfare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_collapse_user_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_dataset/samples.csv
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_dataset/samples.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_dataset/samples.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_eval_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_hf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_images/
--rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_images/images.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_list_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_logprobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_num_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_stop_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_task_list/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/attribs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/multiple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/_decoy/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/_decoy/testit.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/_decoy2.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.537315 inspect_ai-0.3.6/tests/test_task_list/recurse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_task_list/recurse/.folder3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/.folder3/epsilon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_task_list/recurse/folder1/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/folder1/_decoy.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/folder1/theta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.601315 inspect_ai-0.3.6/tests/test_task_list/recurse/folder2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.601315 inspect_ai-0.3.6/tests/test_task_list/recurse/folder2/.folder3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/folder2/another.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/folder2/first.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.446029 inspect_ai-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.374029 inspect_ai-0.3.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.374029 inspect_ai-0.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/workflows/vscode.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.374029 inspect_ai-0.3.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-07 22:49:42.446029 inspect_ai-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.374029 inspect_ai-0.3.8/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/arc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.374029 inspect_ai-0.3.8/benchmarks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/datasets/math_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/datasets/mmlu.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/gpqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/gsm8k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/hellaswag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/mathematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/mmlu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.378029 inspect_ai-0.3.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.378029 inspect_ai-0.3.8/docs/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/arc.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/biology_qa.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/footer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/gsm8k.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/hellaswag.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/mathematics.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/popularity.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/security_guide.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/theory_of_mind.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/tool_use.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.378029 inspect_ai-0.3.8/docs/_format/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_format/pre-render.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_variables.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/datasets.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/eval-logs.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/eval-suites.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/eval-tuning.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/examples.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.386029 inspect_ai-0.3.8/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/aisi-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/eval-log.png
+-rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-answers.png
+-rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-home.png
+-rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-info.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-logging-console.png
+-rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-logging.png
+-rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-main.png
+-rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-messages.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-metadata.png
+-rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-scoring.png
+-rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-sort.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90624 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/popularity.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/rate-limit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/running-theory.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/log-viewer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    18564 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/models.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/scorers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/solvers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/tools.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/workflow.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.390029 inspect_ai-0.3.8/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.362029 inspect_ai-0.3.8/examples/agents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.390029 inspect_ai-0.3.8/examples/agents/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/.env.example
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/inspect_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/wikipedia.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/biology_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/popularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/security_guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/theory_of_mind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/tool_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:49:42.446029 inspect_ai-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.362029 inspect_ai-0.3.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.390029 inspect_ai-0.3.8/src/inspect_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.390029 inspect_ai-0.3.8/src/inspect_ai/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.394029 inspect_ai-0.3.8/src/inspect_ai/_display/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_display/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_display/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_display/rich.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.394029 inspect_ai-0.3.8/src/inspect_ai/_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.398029 inspect_ai-0.3.8/src/inspect_ai/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.398029 inspect_ai-0.3.8/src/inspect_ai/_view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.398029 inspect_ai-0.3.8/src/inspect_ai/_view/www/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/App.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.398029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.362029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.398029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/json5.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/purify.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/showdown.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/log-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/log.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/hooks.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/htm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/htm/htm.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/htm/preact.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/htm/preact.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/preact-hooks.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/preact.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/Constants.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/Register.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/api-browser.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/api-vscode.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/index.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/jsonrpc.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/Card.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ChatView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/CopyButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/Dialog.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MessageContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/TabSet.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ToolButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ansi-output.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SampleView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/title/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/Format.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/Git.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/Path.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/Type.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    15531 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/bias_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/biology_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/popularity.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/security_guide.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.414029 inspect_ai-0.3.8/src/inspect_ai/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/log/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.414029 inspect_ai-0.3.8/src/inspect_ai/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33705 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.414029 inspect_ai-0.3.8/src/inspect_ai/model/_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    29810 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/azureai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13793 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.414029 inspect_ai-0.3.8/src/inspect_ai/scorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.418029 inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.418029 inspect_ai-0.3.8/src/inspect_ai/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_critique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_multiple_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.418029 inspect_ai-0.3.8/src/inspect_ai/solver/_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_tool/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_tool/tool_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_tool/use_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_tool/web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.418029 inspect_ai-0.3.8/src/inspect_ai/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.418029 inspect_ai-0.3.8/src/inspect_ai/util/_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/_context/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/_context/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/_context/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/_context/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.442029 inspect_ai-0.3.8/src/inspect_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15007 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.422029 inspect_ai-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_cloudlfare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_collapse_assistant_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_collapse_user_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.422029 inspect_ai-0.3.8/tests/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_dataset/samples.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_dataset/samples.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_dataset/samples.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_eval_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.422029 inspect_ai-0.3.8/tests/test_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_images/images.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_list_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_logprobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_num_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_stop_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/attribs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/multiple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/_decoy/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/_decoy/testit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/_decoy2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.366029 inspect_ai-0.3.8/tests/test_task_list/recurse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/recurse/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/.folder3/epsilon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/recurse/folder1/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/folder1/_decoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/folder1/theta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/recurse/folder2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/recurse/folder2/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/folder2/another.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/folder2/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.366029 inspect_ai-0.3.8/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tools/vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.eslintrc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscode-test.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscodeignore
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.yarnrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.370029 inspect_ai-0.3.8/tools/vscode/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/assets/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/assets/logo/inspect.png
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/assets/logo/inspect.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/assets/templates/task.py.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.370029 inspect_ai-0.3.8/tools/vscode/assets/www/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/assets/www/codicon/
+-rw-r--r--   0 runner    (1001) docker     (127)    27023 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/assets/www/codicon/codicon.css
+-rw-r--r--   0 runner    (1001) docker     (127)    72860 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/assets/www/codicon/codicon.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/debugger.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/document.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/error.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/focus.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/notebook.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/templates.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/webview.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.434029 inspect_ai-0.3.8/tools/vscode/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/appdirs.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/command.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/dispose.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/env.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/git.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/jsonrpc.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/log.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/nonce.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/path.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/port.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/process.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.434029 inspect_ai-0.3.8/tools/vscode/src/core/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/python/code.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/python/exec.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/python/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/python/interpreter.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/random.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/string.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/text.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/wait.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/workspace.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/extension.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.434029 inspect_ai-0.3.8/tools/vscode/src/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/inspect/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/inspect/list.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/inspect/logs.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/inspect/props.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.370029 inspect_ai-0.3.8/tools/vscode/src/providers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.434029 inspect_ai-0.3.8/tools/vscode/src/providers/active-task/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/active-task/active-task-command.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/active-task/active-task-provider.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.434029 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/activity-bar-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/env-config-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-config-commands.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-config-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-outline-commands.ts
+-rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-outline-provider.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/env-config-webview.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/env-config-webview.ts
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/task-config-webview.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/task-config-webview.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/vscode-controls.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/webview-utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/codelens/
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/codelens/codelens-provider.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/inspect/inspect-constants.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/inspect/inspect-eval-commands.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/inspect/inspect-eval.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/inspect/inspect-manager.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/logview/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/commands.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-file-watcher.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-link-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-manager.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-webview.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/settings/inspect-settings.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/settings/user-settings.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-env-commands.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-env-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-init.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-state-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-task-provider.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/test/extension.test.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.370029 inspect_ai-0.3.8/tools/vscode/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.442029 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.442029 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/src/jsonrpc.ts
+-rw-r--r--   0 runner    (1001) docker     (127)   129610 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)   158647 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/yarn.lock
```

### Comparing `inspect_ai-0.3.6/.github/workflows/build.yml` & `inspect_ai-0.3.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/.github/workflows/docs.yml` & `inspect_ai-0.3.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/.github/workflows/pypi.yml` & `inspect_ai-0.3.8/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/.gitignore` & `inspect_ai-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/.pre-commit-config.yaml` & `inspect_ai-0.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/CHANGELOG.md` & `inspect_ai-0.3.8/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## v0.3.8 (07 May 2024)
+
+- Exclude null config values from listings in log viewer.
+
+## v0.3.7 (07 May 2024)
+
+- Add support for logprobs to HF provider, and create uniform API for other providers that support logprobs (Together and OpenAI).
+- Provide an option to merge asssistant messages and use it for Anthropoic models (as they don't allow consecutive assistant messages).
+- Supporting infrastructure in Inspect CLI for VS Code extension (additional list and info commands).
+
 ## v0.3.6 (06 May 2024)
 
 - Show first log file immediately (don't wait for fetching metadata for other logs)
 - Add `--version` CLI arg and `inspect info version` command for interogating version and runtime source path.
 - Fix: exclude `null` config values in output from `inspect info log-file`
 
 ## v0.3.5 (04 May 2024)
```

### Comparing `inspect_ai-0.3.6/LICENSE` & `inspect_ai-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/PKG-INFO` & `inspect_ai-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.6
+Version: 0.3.8
 Summary: Framework for large language model evaluations
 Author: UK AI Safety Institute
 License: MIT License
 Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
 Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
 Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `inspect_ai-0.3.6/README.md` & `inspect_ai-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/benchmarks/README.md` & `inspect_ai-0.3.8/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/benchmarks/arc.py` & `inspect_ai-0.3.8/benchmarks/arc.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/benchmarks/gpqa.py` & `inspect_ai-0.3.8/benchmarks/gpqa.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/benchmarks/gsm8k.py` & `inspect_ai-0.3.8/benchmarks/gsm8k.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/benchmarks/hellaswag.py` & `inspect_ai-0.3.8/benchmarks/hellaswag.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/benchmarks/mathematics.py` & `inspect_ai-0.3.8/benchmarks/mathematics.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/arc.qmd` & `inspect_ai-0.3.8/docs/_examples/arc.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/biology_qa.qmd` & `inspect_ai-0.3.8/docs/_examples/biology_qa.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/footer.qmd` & `inspect_ai-0.3.8/docs/_examples/footer.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/gsm8k.qmd` & `inspect_ai-0.3.8/docs/_examples/gsm8k.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/hellaswag.qmd` & `inspect_ai-0.3.8/docs/_examples/hellaswag.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/index.qmd` & `inspect_ai-0.3.8/docs/_examples/index.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/mathematics.qmd` & `inspect_ai-0.3.8/docs/_examples/mathematics.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/popularity.qmd` & `inspect_ai-0.3.8/docs/_examples/popularity.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/security_guide.qmd` & `inspect_ai-0.3.8/docs/_examples/security_guide.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/theory_of_mind.qmd` & `inspect_ai-0.3.8/docs/_examples/theory_of_mind.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_examples/tool_use.qmd` & `inspect_ai-0.3.8/docs/_examples/tool_use.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/_quarto.yml` & `inspect_ai-0.3.8/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/datasets.qmd` & `inspect_ai-0.3.8/docs/datasets.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/eval-logs.qmd` & `inspect_ai-0.3.8/docs/eval-logs.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/eval-suites.qmd` & `inspect_ai-0.3.8/docs/eval-suites.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/eval-tuning.qmd` & `inspect_ai-0.3.8/docs/eval-tuning.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/examples.qmd` & `inspect_ai-0.3.8/docs/examples.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/aisi-logo.png` & `inspect_ai-0.3.8/docs/images/aisi-logo.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/eval-log.png` & `inspect_ai-0.3.8/docs/images/eval-log.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-answers.png` & `inspect_ai-0.3.8/docs/images/inspect-view-answers.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-filter.png` & `inspect_ai-0.3.8/docs/images/inspect-view-filter.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-history.png` & `inspect_ai-0.3.8/docs/images/inspect-view-history.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-home.png` & `inspect_ai-0.3.8/docs/images/inspect-view-home.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-info.png` & `inspect_ai-0.3.8/docs/images/inspect-view-info.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-logging-console.png` & `inspect_ai-0.3.8/docs/images/inspect-view-logging-console.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-logging.png` & `inspect_ai-0.3.8/docs/images/inspect-view-logging.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-main.png` & `inspect_ai-0.3.8/docs/images/inspect-view-main.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-messages.png` & `inspect_ai-0.3.8/docs/images/inspect-view-messages.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-metadata.png` & `inspect_ai-0.3.8/docs/images/inspect-view-metadata.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-scoring.png` & `inspect_ai-0.3.8/docs/images/inspect-view-scoring.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-sort.png` & `inspect_ai-0.3.8/docs/images/inspect-view-sort.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/inspect-view-splash.png` & `inspect_ai-0.3.8/docs/images/inspect-view-splash.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/popularity.png` & `inspect_ai-0.3.8/docs/images/popularity.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/rate-limit.png` & `inspect_ai-0.3.8/docs/images/rate-limit.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/images/running-theory.png` & `inspect_ai-0.3.8/docs/images/running-theory.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/index.qmd` & `inspect_ai-0.3.8/docs/index.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/log-viewer.qmd` & `inspect_ai-0.3.8/docs/log-viewer.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/models.qmd` & `inspect_ai-0.3.8/docs/models.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/scorers.qmd` & `inspect_ai-0.3.8/docs/scorers.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/solvers.qmd` & `inspect_ai-0.3.8/docs/solvers.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/theme.scss` & `inspect_ai-0.3.8/docs/theme.scss`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/tools.qmd` & `inspect_ai-0.3.8/docs/tools.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/docs/workflow.qmd` & `inspect_ai-0.3.8/docs/workflow.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/examples/agents/langchain/README.md` & `inspect_ai-0.3.8/examples/agents/langchain/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/examples/agents/langchain/inspect_langchain.py` & `inspect_ai-0.3.8/examples/agents/langchain/inspect_langchain.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/examples/agents/langchain/wikipedia.jsonl` & `inspect_ai-0.3.8/examples/agents/langchain/wikipedia.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/examples/agents/langchain/wikipedia.py` & `inspect_ai-0.3.8/examples/agents/langchain/wikipedia.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/examples/biology_qa.py` & `inspect_ai-0.3.8/examples/biology_qa.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/examples/popularity.py` & `inspect_ai-0.3.8/examples/popularity.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/examples/security_guide.py` & `inspect_ai-0.3.8/examples/security_guide.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/examples/theory_of_mind.py` & `inspect_ai-0.3.8/examples/theory_of_mind.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/examples/tool_use.py` & `inspect_ai-0.3.8/examples/tool_use.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/pyproject.toml` & `inspect_ai-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/__init__.py` & `inspect_ai-0.3.8/src/inspect_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_cli/common.py` & `inspect_ai-0.3.8/src/inspect_ai/_cli/common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_cli/eval.py` & `inspect_ai-0.3.8/src/inspect_ai/_cli/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,20 +152,20 @@
     type=int,
     help="How many chat completion choices to generate for each input message.",
 )
 @click.option(
     "--logprobs",
     type=bool,
     is_flag=True,
-    help="Return log probabilities of the output tokens. OpenAI and TogetherAI only.",
+    help="Return log probabilities of the output tokens. OpenAI, TogetherAI, and Huggingface only.",
 )
 @click.option(
     "--top-logprobs",
     type=int,
-    help="Number of most likely tokens (0-20) to return at each token position, each with an associated log probability. OpenAI only.",
+    help="Number of most likely tokens (0-20) to return at each token position, each with an associated log probability. OpenAI and Huggingface only.",
 )
 @common_options
 def eval_command(
     tasks: tuple[str] | None,
     model: str,
     model_base_url: str | None,
     m: tuple[str] | None,
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_cli/info.py` & `inspect_ai-0.3.8/src/inspect_ai/_cli/info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from json import dumps
 
 import click
+from pydantic_core import to_jsonable_python
 
 from inspect_ai import __version__
 from inspect_ai._util.constants import PKG_PATH
-from inspect_ai.log import eval_log_json, read_eval_log
+from inspect_ai.log._file import eval_log_json, read_eval_log, read_eval_log_headers
 
 
 @click.group("info")
 def info_command() -> None:
     """Read configuration and log info."""
     return None
 
@@ -40,14 +41,22 @@
 )
 def log(path: str, header_only: bool) -> None:
     """Print log file contents."""
     log = read_eval_log(path, header_only=header_only)
     print(eval_log_json(log))
 
 
+@info_command.command("log-file-headers")
+@click.argument("files", nargs=-1)
+def log_file_headers(files: tuple[str]) -> None:
+    """Read and print a JSON list of log file headers."""
+    headers = read_eval_log_headers(list(files))
+    print(dumps(to_jsonable_python(headers, exclude_none=True), indent=2))
+
+
 @info_command.command("log-schema")
 def log_schema() -> None:
     """Print JSON schema for log files."""
     print(view_resource("log-schema.json"))
 
 
 @info_command.command("log-types")
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_cli/list.py` & `inspect_ai-0.3.8/src/inspect_ai/_cli/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     # list tasks
     tasks = list_tasks(
         globs=list(paths) if paths else [], absolute=absolute, filter=task_filter
     )
 
     # print as JSON or plain text
     if json:
-        print(dumps(to_jsonable_python(tasks), indent=2))
+        print(dumps(to_jsonable_python(tasks, exclude_none=True), indent=2))
     else:
         print("\n".join([f"{task.file}@{task.name}" for task in tasks]))
 
 
 @list_command.command()
 @click.option(
     "--status",
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_cli/main.py` & `inspect_ai-0.3.8/src/inspect_ai/_cli/main.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_cli/score.py` & `inspect_ai-0.3.8/src/inspect_ai/_cli/score.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_cli/util.py` & `inspect_ai-0.3.8/src/inspect_ai/_cli/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_cli/view.py` & `inspect_ai-0.3.8/src/inspect_ai/_cli/view.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_display/_display.py` & `inspect_ai-0.3.8/src/inspect_ai/_display/_display.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_display/logger.py` & `inspect_ai-0.3.8/src/inspect_ai/_display/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_display/rich.py` & `inspect_ai-0.3.8/src/inspect_ai/_display/rich.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_eval/eval.py` & `inspect_ai-0.3.8/src/inspect_ai/_eval/eval.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_eval/images.py` & `inspect_ai-0.3.8/src/inspect_ai/_eval/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_eval/list.py` & `inspect_ai-0.3.8/src/inspect_ai/_eval/list.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_eval/loader.py` & `inspect_ai-0.3.8/src/inspect_ai/_eval/loader.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_eval/log.py` & `inspect_ai-0.3.8/src/inspect_ai/_eval/log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_eval/registry.py` & `inspect_ai-0.3.8/src/inspect_ai/_eval/registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_eval/score.py` & `inspect_ai-0.3.8/src/inspect_ai/_eval/score.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_eval/task.py` & `inspect_ai-0.3.8/src/inspect_ai/_eval/task.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/dotenv.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/dotenv.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/error.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/error.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/file.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/git.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/git.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/http.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/http.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/images.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/json.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/json.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/notebook.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/notebook.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/path.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/path.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/platform.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/platform.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/registry.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/retry.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_util/url.py` & `inspect_ai-0.3.8/src/inspect_ai/_util/url.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/schema.py` & `inspect_ai-0.3.8/src/inspect_ai/_view/schema.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/view.py` & `inspect_ai-0.3.8/src/inspect_ai/_view/view.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,36 +8,43 @@
 from http.server import HTTPServer
 from io import BytesIO
 from pathlib import Path
 from typing import Any
 from urllib.parse import parse_qs, urlparse, urlunparse
 
 import psutil
+from pydantic_core import to_jsonable_python
 
 from inspect_ai._display import display
 from inspect_ai._display.logger import init_logger
 from inspect_ai._util.appdirs import inspect_runtime_dir
 from inspect_ai._util.constants import (
     DEFAULT_SERVER_HOST,
     DEFAULT_VIEW_PORT,
 )
 from inspect_ai._util.dotenv import init_dotenv
 from inspect_ai._util.error import exception_message
 from inspect_ai._util.file import FileSystem, file, filesystem
 from inspect_ai._util.http import InspectHTTPRequestHandler
-from inspect_ai.log._file import eval_log_json, list_eval_logs, read_eval_log
+from inspect_ai.log._file import (
+    eval_log_json,
+    list_eval_logs,
+    read_eval_log,
+    read_eval_log_headers,
+)
 
 logger = logging.getLogger(__name__)
 
 
 WWW_DIR = os.path.abspath((Path(__file__).parent / "www").as_posix())
 
 
 LOGS_PATH = "/api/logs"
 LOGS_DIR = f"{LOGS_PATH}/"
+LOG_HEADERS_PATH = "/api/log-headers"
 
 
 def view(
     log_dir: str | None = None,
     recursive: bool = True,
     host: str = DEFAULT_SERVER_HOST,
     port: int = DEFAULT_VIEW_PORT,
@@ -89,14 +96,16 @@
         self.recursive = recursive
         self.fs_options = fs_options
         super().__init__(*args, directory=WWW_DIR, **kwargs)
 
     def do_GET(self) -> None:
         if self.path == LOGS_PATH:
             self.handle_logs()
+        elif self.path.startswith(LOG_HEADERS_PATH):
+            self.handle_log_headers()
         elif self.path.startswith(LOGS_DIR):
             self.handle_log()
         else:
             super().do_GET()
 
     def handle_logs(self) -> None:
         """Serve log files listing from /logs/."""
@@ -117,14 +126,24 @@
                     for file in files
                 ],
                 indent=2,
             )
         )
         self.send_json(json_files)
 
+    def handle_log_headers(self) -> None:
+        # check for query params
+        parsed = urlparse(self.path)
+        query_params = parse_qs(parsed.query)
+        files = query_params.get("file", [])
+        headers = read_eval_log_headers(files)
+        self.send_json(
+            json.dumps(to_jsonable_python(headers, exclude_none=True), indent=2)
+        )
+
     def handle_log(self) -> None:
         """Serve log files from /api/logs/* url."""
         path = self.path.replace(LOGS_DIR, "", 1)  # strip /api/logs/
         path = path.replace("..", "")  # no escape
 
         # check for query params
         parsed = urlparse(path)
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/App.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/App.mjs`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import { html } from "htm/preact";
-import { useState, useEffect } from "preact/hooks";
+import { useCallback, useState, useEffect } from "preact/hooks";
 
 import { formatPrettyDecimal } from "./src/utils/Format.mjs";
 
-import { client_events, eval_logs } from "api";
 
 import "./src/Register.mjs";
 
 import { icons } from "./src/Constants.mjs";
 import { WorkSpace } from "./src/workspace/WorkSpace.mjs";
-import { eval_log } from "./api.mjs";
+import api from "./src/api/index.mjs";
 import { CopyButton } from "./src/components/CopyButton.mjs";
 
+const logFileName = (path) => {
+  return path.replace("\\", "/").split('/').pop();
+};
+
 export function App() {
   const [selected, setSelected] = useState(0);
   const [logs, setLogs] = useState({ log_dir: "", files: [] });
   const [logHeaders, setLogHeaders] = useState({});
   const [offcanvas, setOffcanvas] = useState(false);
 
   // reset selection when logs are refreshed
@@ -24,58 +27,96 @@
     let index = 0;
     setSelected(index);
   }, [logs]);
 
   useEffect(async () => {
     // Read header information for the logs
     // and then update
-    const headerResults = await Promise.all(logs.files.map((file) => {
-        return eval_log(file.name, true).then((result) => {
-          return { file: file.name, result };
-        }).catch(() => { return undefined});
-    }));
-    
-    // Update the headers
-    const updatedHeaders = logHeaders;
-    for (const headerResult of headerResults) {
-      if (headerResult) {
-        updatedHeaders[headerResult.file] = headerResult.result;
-      }
+
+    // Group into chunks
+    const chunkSize = 5;
+    const fileLists = [];
+    for (let i = 0; i < logs.files.length; i += chunkSize) {
+      let chunk = logs.files.slice(i, i + chunkSize).map((log) => { return log.name; });
+      fileLists.push(chunk);
+    }
+
+    for (const fileList of fileLists) {
+      const headers = await api.eval_log_headers(fileList);
+      const updatedHeaders = logHeaders;
+      headers.forEach((header, index) => {
+        const logFile = fileList[index];
+        updatedHeaders[logFile] = header;
+      })
+      setLogHeaders({ ...updatedHeaders });  
     }
-    setLogHeaders({ ...updatedHeaders });
   }, [logs]);
 
+  const updateLogs = useCallback(async (log) => {
+    // Set the list of logs
+    const logresult = await api.eval_logs();
+    if (logresult) {
+      setLogs(logresult);
+      if (log) {
+        const name = logFileName(log);
+        const index = logresult.files.findIndex((val) => {
+          return val.name.endsWith(name);
+        })
+        setSelected(index);
+      }
+    } else {
+      setLogs({ log_dir: "", files: [] });
+    }
+  }, [setLogs, setSelected]);
+
+  // listen for updateState messages from vscode
+  useEffect(() => {
+
+    const onMessage = (e) => {
+      switch (e.data.type || e.data.message) {
+
+        case "updateState": {
+          if (e.data.url) {
+            updateLogs(e.data.url);
+          }
+        }
+      }
+    }
+
+    window.addEventListener("message", onMessage);
+
+    return () => {
+      window.removeEventListener("message", onMessage);
+    }
+
+  }, [updateLogs]);
+
   useEffect(async () => {
     const urlParams = new URLSearchParams(window.location.search);
 
     // Note whether we should default off canvas the sidebar
     setOffcanvas(true);
 
     // If the URL provides a task file, load that
     const logPath = urlParams.get("task_file");
     const loadLogs = logPath
       ? async () => {
-          setLogs({
-            log_dir: "",
-            files: [{ name: logPath }],
-          });
-        }
-      : async () => {
-        // Set the list of logs
-          const logresult = await eval_logs();            
-          setLogs(logresult);
-
-        };
+        setLogs({
+          log_dir: "",
+          files: [{ name: logPath }],
+        });
+      }
+      : updateLogs;
 
     // initial fetch of logs
     await loadLogs();
 
     // poll every 1s for events
     setInterval(() => {
-      client_events().then((events) => {
+      api.client_events().then((events) => {
         if (events.includes("reload")) {
           window.location.reload(true);
         }
         if (events.includes("refresh-evals")) {
           loadLogs();
         }
       });
@@ -92,23 +133,23 @@
         <${Header} logs=${logs} selected=${selected} offcanvas=${offcanvas} />
         <${Sidebar}
           logs=${logs}
           logHeaders=${logHeaders}
           offcanvas=${offcanvas}
           selected=${selected}
           onSelected=${(index) => {
-            setSelected(index);
+        setSelected(index);
 
-            // hide the sidebar offcanvas
-            var myOffcanvas = document.getElementById("sidebarOffCanvas");
-            var bsOffcanvas = bootstrap.Offcanvas.getInstance(myOffcanvas);
-            if (bsOffcanvas) {
-              bsOffcanvas.hide();
-            }
-          }}
+        // hide the sidebar offcanvas
+        var myOffcanvas = document.getElementById("sidebarOffCanvas");
+        var bsOffcanvas = bootstrap.Offcanvas.getInstance(myOffcanvas);
+        if (bsOffcanvas) {
+          bsOffcanvas.hide();
+        }
+      }}
         />
       `;
   return html`
     <div>
       ${appEnvelope}
       <${WorkSpace}
         logs=${logs}
@@ -123,17 +164,15 @@
 const Header = (props) => {
   const toggleOffCanClass = props.offcanvas ? "" : " d-md-none";
   const gearOffCanClass = props.offcanvas ? "" : " d-md-inline";
 
   const logFiles = props.logs.files || [];
   const logSelected = props.selected || 0;
   const logUri = logFiles.length > logSelected ? logFiles[logSelected].name : "";
-  const logName =logUri.split('/').pop();
-  
-
+  const logName = logFileName(logUri);
 
   return html`
     <nav class="navbar sticky-top shadow-sm" style=${{ flexWrap: "nowrap" }}>
       <div class="container-fluid">
         <span
           class="navbar-brand mb-0"
           style=${{ display: "flex", alignItems: "center" }}
@@ -142,38 +181,38 @@
             id="sidebarToggle"
             class="btn${toggleOffCanClass}"
             type="button"
             data-bs-toggle="offcanvas"
             data-bs-target="#sidebarOffCanvas"
             aria-controls="sidebarOffCanvas"
             style=${{
-              padding: "0rem 0.1rem 0.1rem 0rem",
-              marginTop: ".1rem",
-              marginRight: "0.2rem",
-              lineHeight: "16px",
-            }}
+      padding: "0rem 0.1rem 0.1rem 0rem",
+      marginTop: ".1rem",
+      marginRight: "0.2rem",
+      lineHeight: "16px",
+    }}
           >
             <i class=${icons.menu}></i>
           </button>
           <i
             class="${icons.inspect} d-none ${gearOffCanClass}"
             style=${{ marginRight: "0.3rem" }}
           ></i>
           <span> Inspect View </span>
         </span>
         <div
           class="navbar-text"
           style=${{
-            paddingTop: "0.3rem",
-            paddingBottom: 0,
-            fontSize: "0.8rem",
-            whiteSpace: "nowrap",
-            textOverflow: "ellipsis",
-            overflow: "hidden",
-          }}
+      paddingTop: "0.3rem",
+      paddingBottom: 0,
+      fontSize: "0.8rem",
+      whiteSpace: "nowrap",
+      textOverflow: "ellipsis",
+      overflow: "hidden",
+    }}
         >
           ${logName}<${CopyButton} value=${logUri}/>
         </div>
       </div>
     </nav>
   `;
 };
@@ -186,26 +225,26 @@
   return html`
     <div
       class="sidebar border-end offcanvas-start${sidebarOffCanClass}"
       id="sidebarOffCanvas"
     >
       <div
         style=${{
-          display: "flex",
-          alignItems: "center",
-          justifyContent: "space-between",
-        }}
+      display: "flex",
+      alignItems: "center",
+      justifyContent: "space-between",
+    }}
       >
         <span
           style=${{
-            paddingLeft: "0.5rem",
-            fontWeight: "500",
-            fontSize: "1.1rem",
-            opacity: "0.7",
-          }}
+      paddingLeft: "0.5rem",
+      fontWeight: "500",
+      fontSize: "1.1rem",
+      opacity: "0.7",
+    }}
           >${props.offcanvas ? "Log History" : ""}</span
         >
         <button
           id="sidebarToggle"
           class="btn d-inline${btnOffCanClass}"
           type="button"
           data-bs-toggle="offcanvas"
@@ -214,100 +253,102 @@
           style=${{ padding: ".1rem", alignSelf: "end", width: "40px" }}
         >
           <i class=${icons.close}></i>
         </button>
       </div>
       <ul class="list-group">
         ${props.logs.files.map((file, index) => {
-          const active = index === props.selected ? " active" : "";
-          const time = new Date(file.mtime);
-          const logHeader = logHeaders[file.name];
-          const hyperparameters = logHeader ? {
-            ...logHeader.plan?.config,
-            ...logHeader.eval?.task_args,
-          } : undefined;
-
-          const model = logHeader?.eval?.model;
-          const dataset = logHeader?.eval?.dataset;
-          const scorer = logHeader?.results?.scorer?.name;
-          
-          return html`
+      const active = index === props.selected ? " active" : "";
+      const time = new Date(file.mtime);
+      const logHeader = logHeaders[file.name];
+      const hyperparameters = logHeader ? {
+        ...logHeader.plan?.config,
+        ...logHeader.eval?.task_args,
+      } : undefined;
+
+      const model = logHeader?.eval?.model;
+      const dataset = logHeader?.eval?.dataset;
+      const scorer = logHeader?.results?.scorer?.name;
+
+      return html`
             <li
               class="list-group-item list-group-item-action${active}"
               onclick=${() => props.onSelected(index)}
               style=${{ fontSize: "0.8rem" }}
             >
               <div
                 style=${{
-                  display: "flex",
-                  flexDirection: "row",
-                  justifyContent: "space-between",
-                }}
+          display: "flex",
+          flexDirection: "row",
+          justifyContent: "space-between",
+        }}
               >
-                <div>
+                <div style=${{overflow: "hidden"}}>
                   <div
                     style=${{
                       fontSize: "1.5em",
                       fontWeight: "600",
+                      whiteSpace: "nowrap",
+                      overflow: "hidden",
+                      textOverflow: "ellipsis"
                     }}
                   >
                     ${logHeader?.eval?.task || file.task}
                   </div>
                   <small class="mb-1 text-muted">
                     ${time.toDateString()}
                     ${time.toLocaleTimeString([], {
-                      hour: "2-digit",
-                      minute: "2-digit",
-                    })}
+          hour: "2-digit",
+          minute: "2-digit",
+        })}
                   </small>
 
-                  ${model ? html` <div><small class="mb-1 text-muted">${model}</small></div>`: ""}
+                  ${model ? html` <div><small class="mb-1 text-muted">${model}</small></div>` : ""}
                 </div>
                 ${logHeader?.results?.metrics
-                  ? html`<div style=${{display: "flex", flexDirection: "row", flexWrap: "wrap", justifyContent: "flex-end" }}>
+          ? html`<div style=${{ display: "flex", flexDirection: "row", flexWrap: "wrap", justifyContent: "flex-end" }}>
                           
                       ${Object.keys(logHeader?.results.metrics).map(
-                        (metric) => {
-                          return html`
+            (metric) => {
+              return html`
                             <div
                               style=${{
-                                display: "flex",
-                                flexDirection: "column",
-                                alignItems: "center",
-                                marginLeft: "1em"
-                              }}
+                  display: "flex",
+                  flexDirection: "column",
+                  alignItems: "center",
+                  marginLeft: "1em"
+                }}
                             >
                               <div
                                 style=${{ fontWeight: 300 }}
                               >
                                 ${logHeader?.results.metrics[metric].name}
                                 </div>
-                              <div style=${{fontWeight: 600, fontSize: "1.5em"}}>
+                              <div style=${{ fontWeight: 600, fontSize: "1.5em" }}>
                                 ${formatPrettyDecimal(
-                                  logHeader?.results.metrics[metric].value
-                                )}
+                  logHeader?.results.metrics[metric].value
+                )}
                               </div>
                             </div>
                           `;
-                        }
-                      )}
+            }
+          )}
                     </div>`
-                  : logHeader?.status === "error" ? html`<div style=${{color: "var(--bs-danger)"}}>Eval Error</div>` : ""}
+          : logHeader?.status === "error" ? html`<div style=${{ color: "var(--bs-danger)" }}>Eval Error</div>` : ""}
               </div>
               <div style=${{ marginTop: "0.4em" }}>
               <small class="mb-1 text-muted">
-              ${
-                hyperparameters ? Object.keys((hyperparameters)).map((key) => {
-                  return `${key}: ${hyperparameters[key]}`
-                }).join(", ") : ""
-              } 
+              ${hyperparameters ? Object.keys((hyperparameters)).map((key) => {
+            return `${key}: ${hyperparameters[key]}`
+          }).join(", ") : ""
+        } 
               </small>
               </div>
-              ${dataset || scorer ? html`<div style=${{display: "flex", justifyContent: "space-between", marginTop: "0.5em" }}><span>dataset: ${dataset.name || "(samples)"}</span><span>scorer: ${scorer}</span></div>` : ""}
+              ${dataset || scorer ? html`<div style=${{ display: "flex", justifyContent: "space-between", marginTop: "0.5em" }}><span>dataset: ${dataset.name || "(samples)"}</span><span>scorer: ${scorer}</span></div>` : ""}
 
             </li>
           `;
-        })}
+    })}
       </ul>
     </div>
   `;
 };
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/api.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/api-browser.mjs`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 
 
+
 const loaded_time = Date.now()
 let last_eval_time = 0
 
-export async function client_events() {
-  const params = new URLSearchParams()
-  params.append("loaded_time", loaded_time.valueOf())
-  params.append("last_eval_time", last_eval_time.valueOf())
-  return api("GET", `/api/events?${params.toString()}`)
+
+async function client_events() {
+    const params = new URLSearchParams()
+    params.append("loaded_time", loaded_time.valueOf())
+    params.append("last_eval_time", last_eval_time.valueOf())
+    return api("GET", `/api/events?${params.toString()}`)
 }
 
-export async function eval_logs() {
+async function eval_logs() {
   const logs = await api("GET", `/api/logs`)
   last_eval_time = Date.now()
   return logs
 }
 
-export async function eval_log(file, headerOnly) {
+async function eval_log(file, headerOnly) {
   if (headerOnly) {
     return api("GET", `/api/logs/${file}?header-only=true`)
   } else {
     return api("GET", `/api/logs/${file}`)
   }
 }
 
-export async function api(method, path, body) {
+async function eval_log_headers(files) {
+  const params = new URLSearchParams();
+  for (const file of files) {
+    params.append("file", file);
+  }
+  return api("GET", `/api/log-headers?${params.toString()}`)
+}
+
+async function api(method, path, body) {
   // build headers
   const headers = {
     Accept: "application/json",
     Pragma: "no-cache",
     Expires: "0",
     ['Cache-Control']: 'no-cache',
   }
@@ -46,7 +56,15 @@
     const error = new Error(`Error: ${response.status}: ${message})`)
     throw error;
   } else {
     throw new Error(`${response.status} - ${response.statusText} `);
   }
 
 }
+
+export default {
+  client_events,
+  eval_logs,
+  eval_log,
+  eval_log_headers
+}
+
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/favicon.svg` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/favicon.svg`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/index.html` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
       rel="stylesheet"
     />
 
     <link href="./src/App.css" rel="stylesheet" />
     <script type="importmap">
       {
         "imports": {
-          "api": "./api.mjs",
           "preact": "./preact/preact.mjs",
           "preact/hooks": "./preact/preact-hooks.mjs",
           "htm/preact": "./preact/htm/preact.mjs?external=preact"
         }
       }
     </script>
     <script>
@@ -32,15 +31,14 @@
       const urlParams = new URLSearchParams(window.location.search);
       const theme = urlParams.get("inspectLogviewThemeCategory");
       if (theme) {
         document.documentElement.setAttribute("data-text-highlight", theme);
         document.documentElement.setAttribute("data-bs-theme", theme);
       }
     </script>
-    <script src="./tools.js"></script>
   </head>
 
   <body>
     <div id="app"></div>
     <script type="module">
       import { render } from "preact";
       import { html } from "htm/preact";
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/clipboard.min.js` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/json5.min.js` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/json5.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism-dark.css` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism-dark.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism.min.css` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism.min.js` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/purify.min.js` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/purify.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/showdown.min.js` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/showdown.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/log-schema.json` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/log-schema.json`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/log.d.ts` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/log.d.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/hooks.js` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/hooks.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/htm/htm.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/htm/htm.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/preact.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/preact.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/Constants.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/Constants.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AnsiDisplay.css` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AnsiDisplay.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/Card.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/Card.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ChatView.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ChatView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/CopyButton.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/CopyButton.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/Dialog.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/Dialog.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/LabeledValue.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/LabeledValue.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MessageContent.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MessageContent.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MetaDataView.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MetaDataView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/RenderedContent.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/RenderedContent.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/TabSet.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/TabSet.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ansi-output.js` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ansi-output.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/plan/PlanCard.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/plan/PlanCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SampleView.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SampleView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/title/TitleBlock.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/title/TitleBlock.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/usage/UsageCard.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/usage/UsageCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/Format.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/Format.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs` & `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import { SamplesCard } from "../samples/SamplesCard.mjs";
 import { LoggingPanel } from "../logging/LoggingPanel.mjs";
 import { LoadingScreen } from "../components/LoadingScreen.mjs";
 import { ToolButton } from "../components/ToolButton.mjs";
 import { TabSet, Tab } from "../components/TabSet.mjs";
 import { SampleFilter } from "./SampleFilter.mjs";
 import { samplesDescriptor } from "./SamplesDescriptor.mjs";
-import { eval_log } from "../../api.mjs";
+import api from "../api/index.mjs";
 import { PlanCard } from "../plan/PlanCard.mjs";
 import { UsageCard } from "../usage/UsageCard.mjs";
 import { EmptyPanel } from "../components/EmptyPanel.mjs";
 import { TaskErrorCard } from "./TaskErrorPanel.mjs";
 
 const kEvalTabId = "eval-tab";
 const kJsonTabId = "json-tab";
@@ -368,18 +368,20 @@
 
   /**
    *
    * @param {import('../../log.d.ts').EvalLog} log
    */
   const showLog = (log) => {
     if (log.contents) {
-      setSelectedTab(state, kEvalTabId);
+
+      const defaultTab = log.contents?.status === "success" ? kEvalTabId : kInfoTabId;
+      setSelectedTab(state, defaultTab);
 
       divRef.current.scrollTop = 0;
-      if (log.contents.samples.length <= 200) {
+      if (log.contents.samples?.length <= 200) {
         codeRef.current.innerHTML = Prism.highlight(
           JSON.stringify(log.contents, null, 2),
           Prism.languages.javascript,
           "javacript"
         );
       } else {
         codeRef.current.innerHTML = JSON.stringify(log.contents, null, 2);
@@ -390,24 +392,26 @@
   useEffect(async () => {
     const viewState = state.viewState;
     if (props.logs.files.length > 0) {
       const log = props.logs.files[props.selected];
       if (state.log.path !== log.name) {
         setState({...state, status: "loading"});
         try {
-          const logContents = await eval_log(log?.name);
-          viewState.openSamples = [];
-          viewState.sort = kDefaultSort;
-          viewState.filter = {};
-          viewState.epoch = "all";
-
-          setState({
-            log: { contents: logContents, path: log.name },
-            viewState,
-          });
+          const logContents = await api.eval_log(log?.name, false);
+          if (logContents) {
+            viewState.openSamples = [];
+            viewState.sort = kDefaultSort;
+            viewState.filter = {};
+            viewState.epoch = "all";
+
+            setState({
+              log: { contents: logContents, path: log.name },
+              viewState,
+            });
+          }
         } catch (e) {
           // Show an error
           console.log(e);
           setState({ log: state.log, viewState, status: "error", error: e });
         }
       }
     } else {
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/__init__.py` & `inspect_ai-0.3.8/src/inspect_ai/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_dataset.py` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/bias_detection.jsonl` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/bias_detection.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/biology_qa.jsonl` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/biology_qa.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/popularity.jsonl` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/popularity.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/security_guide.jsonl` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/security_guide.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/csv.py` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/csv.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/example.py` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/example.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/file.py` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/hf.py` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/json.py` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/json.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/dataset/_util.py` & `inspect_ai-0.3.8/src/inspect_ai/dataset/_util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/log/__init__.py` & `inspect_ai-0.3.8/src/inspect_ai/log/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ._file import (
     EvalLogInfo,
-    eval_log_json,
     list_eval_logs,
     read_eval_log,
     write_eval_log,
 )
 from ._log import (
     EvalConfig,
     EvalDataset,
@@ -39,9 +38,8 @@
     "EvalStats",
     "EvalLogInfo",
     "LoggingLevel",
     "LoggingMessage",
     "list_eval_logs",
     "read_eval_log",
     "write_eval_log",
-    "eval_log_json",
 ]
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/log/_file.py` & `inspect_ai-0.3.8/src/inspect_ai/log/_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,18 @@
             raw_data = json.load(f)
             log = EvalLog(**raw_data)
             if log.version > 1:
                 raise ValueError(f"Unable to read version {log.version} of log format.")
             return log
 
 
+def read_eval_log_headers(log_files: list[str] | list[FileInfo]) -> list[EvalLog]:
+    return [read_eval_log(log_file, header_only=True) for log_file in log_files]
+
+
 class FileRecorder(Recorder):
     def __init__(
         self, log_dir: str, suffix: str, fs_options: dict[str, Any] = {}
     ) -> None:
         super().__init__()
         self.log_dir = log_dir
         self.fs = filesystem(log_dir, fs_options)
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/log/_log.py` & `inspect_ai-0.3.8/src/inspect_ai/log/_log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/__init__.py` & `inspect_ai-0.3.8/src/inspect_ai/model/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,20 +8,23 @@
     ChatMessageTool,
     ChatMessageUser,
     Content,
     ContentImage,
     ContentText,
     GenerateConfig,
     GenerateConfigArgs,
+    Logprob,
+    Logprobs,
     Model,
     ModelAPI,
     ModelName,
     ModelOutput,
     ModelUsage,
     StopReason,
+    TopLogprob,
     get_model,
 )
 from ._providers.providers import *
 from ._registry import modelapi
 from ._tool import ToolCall, ToolChoice, ToolFunction, ToolInfo, ToolParam
 
 __all__ = [
@@ -33,14 +36,17 @@
     "ChatMessage",
     "ChatMessageSystem",
     "ChatMessageUser",
     "ChatMessageAssistant",
     "ChatMessageTool",
     "ChatCompletionChoice",
     "ModelOutput",
+    "Logprobs",
+    "Logprob",
+    "TopLogprob",
     "Model",
     "ModelAPI",
     "ModelName",
     "ModelUsage",
     "StopReason",
     "ToolCall",
     "ToolChoice",
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_model.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import asyncio
 import functools
 import os
 from contextvars import ContextVar
 from copy import deepcopy
-from typing import Any, Callable, Literal, Union, cast
+from typing import Any, Callable, Literal, Type, Union, cast
 
 from pydantic import BaseModel, Field
 from tenacity import (
     retry,
     retry_if_exception,
     stop_after_attempt,
     stop_after_delay,
@@ -78,18 +78,18 @@
     top_k: int | None
     """Randomly sample the next word from the top_k most likely next words. Anthropic, Google, and HuggingFace only."""
 
     num_choices: int | None
     """How many chat completion choices to generate for each input message. Open AI, Google, and TogetherAI only."""
 
     logprobs: bool | None
-    """Return log probabilities of the output tokens. OpenAI and TogetherAI only."""
+    """Return log probabilities of the output tokens. OpenAI, TogetherAI, and Huggingface only."""
 
     top_logprobs: int | None
-    """Number of most likely tokens (0-20) to return at each token position, each with an associated log probability. OpenAI only."""
+    """Number of most likely tokens (0-20) to return at each token position, each with an associated log probability. OpenAI and Huggingface only."""
 
 
 class GenerateConfig(BaseModel):
     """Base class for model generation configs."""
 
     max_retries: int | None = Field(default=None)
     """Maximum number of times to retry request (defaults to 5)."""
@@ -136,18 +136,18 @@
     top_k: int | None = Field(default=None)
     """Randomly sample the next word from the top_k most likely next words. Anthropic, Google, and HuggingFace only."""
 
     num_choices: int | None = Field(default=None)
     """How many chat completion choices to generate for each input message. Open AI, Google, and TogetherAI only."""
 
     logprobs: bool | None = Field(default=None)
-    """Return log probabilities of the output tokens. OpenAI and TogetherAI only."""
+    """Return log probabilities of the output tokens. OpenAI, TogetherAI, and Huggingface only."""
 
     top_logprobs: int | None = Field(default=None)
-    """Number of most likely tokens (0-20) to return at each token position, each with an associated log probability. OpenAI only."""
+    """Number of most likely tokens (0-20) to return at each token position, each with an associated log probability. OpenAI and Huggingface only."""
 
     def merge(
         self, other: Union["GenerateConfig", GenerateConfigArgs]
     ) -> "GenerateConfig":
         """Merge another model configuration into this one.
 
         Args:
@@ -299,22 +299,52 @@
     """Total tokens used."""
 
 
 StopReason = Literal["stop", "length", "tool_calls", "content_filter", "unknown"]
 """Reason that the model stopped generating."""
 
 
+class TopLogprob(BaseModel):
+    token: str
+    """The top-kth token represented as a string."""
+
+    logprob: float
+    """The log probability value of the model for the top-kth token."""
+
+    bytes: list[int]
+    """The top-kth token represented as a byte array (a list of integers)."""
+
+
+class Logprob(BaseModel):
+    token: str
+    """The predicted token represented as a string."""
+
+    logprob: float
+    """The log probability value of the model for the predicted token."""
+
+    bytes: list[int]
+    """The predicted token represented as a byte array (a list of integers)."""
+
+    top_logprobs: list[TopLogprob] | None
+    """If the `top_logprobs` argument is greater than 0, this will contain an ordered list of the top K most likely tokens and their log probabilities."""
+
+
+class Logprobs(BaseModel):
+    content: list[Logprob]
+    """a (num_generated_tokens,) length list containing the individual log probabilities for each generated token."""
+
+
 class ChatCompletionChoice(BaseModel):
     message: ChatMessageAssistant
-    """Assistent message."""
+    """Assistant message."""
 
     stop_reason: StopReason = Field(default="unknown")
     """Reason that the model stopped generating."""
 
-    logprobs: dict[str, Any] | None = Field(default=None)
+    logprobs: Logprobs | None = Field(default=None)
     """Logprobs."""
 
 
 class ModelOutput(BaseModel):
     model: str = Field(default="")
     """Model used for generation."""
 
@@ -429,14 +459,18 @@
         """Check whether an exception should be considered a rate limit error."""
         return False
 
     def collapse_user_messages(self) -> bool:
         """Should consecutive user messages be collapsed into a single message."""
         return False
 
+    def collapse_assistant_messages(self) -> bool:
+        """Should consecutive assistant messages be collapsed into a single message."""
+        return False
+
 
 class Model:
     """Model interface."""
 
     def __init__(self, api: ModelAPI, config: GenerateConfig) -> None:
         """Create a model.
 
@@ -547,18 +581,21 @@
             # filter out inactive tool system messages
             input = [
                 message
                 for message in input
                 if not is_inactive_tool_system_message(message)
             ]
 
-            # optionally collapse *consecutive* user messages into one - some apis eg anthropic require this
+            # optionally collapse *consecutive* messages into one - some apis eg anthropic require this
             if self.api.collapse_user_messages():
                 input = collapse_consecutive_user_messages(input)
 
+            if self.api.collapse_assistant_messages():
+                input = collapse_consecutive_assistant_messages(input)
+
         # retry for rate limit errors
         @retry(
             wait=wait_exponential_jitter(jitter=5),
             retry=retry_if_exception(self.api.is_rate_limit),
             stop=(
                 (
                     stop_after_delay(config.timeout)
@@ -799,40 +836,64 @@
 # Functions to reduce consecutive user messages to a single user message -> required for some models
 def collapse_consecutive_user_messages(
     messages: list[ChatMessage],
 ) -> list[ChatMessage]:
     return functools.reduce(user_message_reducer, messages, [])
 
 
+# Functions to reduce consecutive assistant messages to a single user message -> required for some models
+def collapse_consecutive_assistant_messages(
+    messages: list[ChatMessage],
+) -> list[ChatMessage]:
+    return functools.reduce(assistant_message_reducer, messages, [])
+
+
 def user_message_reducer(
     messages: list[ChatMessage],
     message: ChatMessage,
 ) -> list[ChatMessage]:
+    return consecutive_message_reducer(messages, message, ChatMessageUser)
+
+
+def assistant_message_reducer(
+    messages: list[ChatMessage],
+    message: ChatMessage,
+) -> list[ChatMessage]:
+    return consecutive_message_reducer(messages, message, ChatMessageAssistant)
+
+
+def consecutive_message_reducer(
+    messages: list[ChatMessage],
+    message: ChatMessage,
+    message_type: Type[ChatMessage],
+) -> list[ChatMessage]:
     if (
-        isinstance(message, ChatMessageUser)
+        isinstance(message, message_type)
         and len(messages) > 0
-        and isinstance(messages[-1], ChatMessageUser)
+        and isinstance(messages[-1], message_type)
     ):
-        messages[-1] = combine_user_messages(messages[-1], message)
+        messages[-1] = combine_messages(messages[-1], message, message_type)
     else:
         messages.append(message)
     return messages
 
 
-def combine_user_messages(a: ChatMessageUser, b: ChatMessageUser) -> ChatMessageUser:
+def combine_messages(
+    a: ChatMessage, b: ChatMessage, message_type: Type[ChatMessage]
+) -> ChatMessageUser:
     if isinstance(a.content, str) and isinstance(b.content, str):
-        return ChatMessageUser(content=f"{a.content}\n{b.content}")
+        return message_type(content=f"{a.content}\n{b.content}")
     elif isinstance(a.content, list) and isinstance(b.content, list):
-        return ChatMessageUser(content=a.content + b.content)
+        return message_type(content=a.content + b.content)
     elif isinstance(a.content, str) and isinstance(b.content, list):
-        return ChatMessageUser(content=b.content + [ContentText(text=a.content)])
+        return message_type(content=b.content + [ContentText(text=a.content)])
     else:
         content: list[Content] = [ContentText(text=a.text)]
         content.extend(cast(list[Content], b.content))
-        return ChatMessageUser(content=content)
+        return message_type(content=content)
 
 
 def init_async_context_model(model: Model) -> None:
     active_model_context_var.set(model)
     init_model_usage()
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_providers/anthropic.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_providers/anthropic.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,18 @@
             or isinstance(ex, APIConnectionError)
         )
 
     @override
     def collapse_user_messages(self) -> bool:
         return True
 
+    @override
+    def collapse_assistant_messages(self) -> bool:
+        return True
+
 
 #######################################################################################
 # Resolve input, tools, and config into the right shape of input for the Anthropic
 # tool use beta. we also keep the legacy tools implementation around for now (see below)
 # for users on Bedrock of who want to opt out for tools beta for any reason
 #######################################################################################
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_providers/azureai.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_providers/azureai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_providers/bedrock.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_providers/bedrock.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_providers/cloudflare.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_providers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_providers/google.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_providers/google.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_providers/hf.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_providers/hf.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,28 +8,32 @@
 
 import numpy as np
 import torch
 from torch import Tensor
 from transformers import (  # type: ignore
     AutoModelForCausalLM,
     AutoTokenizer,
+    PreTrainedTokenizerBase,
     set_seed,
 )
 from typing_extensions import override
 
 from inspect_ai._util.constants import DEFAULT_MAX_TOKENS
 
 from .._model import (
     ChatCompletionChoice,
     ChatMessage,
     ChatMessageAssistant,
     GenerateConfig,
+    Logprob,
+    Logprobs,
     ModelAPI,
     ModelOutput,
     ModelUsage,
+    TopLogprob,
     simple_input_messages,
 )
 from .._tool import ToolChoice, ToolInfo
 from .._util import chat_api_input
 
 
 class HuggingFaceAPI(ModelAPI):
@@ -114,14 +118,19 @@
             kwargs["max_new_tokens"] = config.max_tokens
         if config.temperature is not None:
             kwargs["temperature"] = config.temperature
         if config.top_p is not None:
             kwargs["top_p"] = config.top_p
         if config.top_k is not None:
             kwargs["top_k"] = config.top_k
+        if config.logprobs is not None:
+            kwargs["output_logits"] = True
+        if "return_dict_in_generate" in kwargs:
+            assert kwargs["return_dict_in_generate"]
+        kwargs["return_dict_in_generate"] = True
         generator = functools.partial(self.model.generate, **kwargs)
 
         # prepare decoder
         decoder = functools.partial(
             self.tokenizer.batch_decode,
             skip_special_tokens=True,
             clean_up_tokenization_spaces=False,
@@ -135,17 +144,32 @@
                 tokenizer=tokenizer,
                 generator=generator,
                 decoder=decoder,
                 batch_size=config.max_connections or self.max_connections(),
             )
         )
 
+        # gather logprobs
+        final_logprobs = None
+        if config.logprobs is not None:
+            final_logprobs = extract_logprobs(
+                response=response,
+                top_logprobs=config.top_logprobs,
+                tokenizer=self.tokenizer,
+            )
+
         # construct choice
         choice = ChatCompletionChoice(
-            message=ChatMessageAssistant(content=response.output, source="generate")
+            message=ChatMessageAssistant(
+                content=response.output,
+                source="generate",
+            ),
+            logprobs=Logprobs(content=final_logprobs)
+            if final_logprobs is not None
+            else None,
         )
 
         # return output
         return ModelOutput(
             model=self.model_name,
             choices=[choice],
             usage=ModelUsage(
@@ -216,14 +240,15 @@
 
 @dataclass
 class GenerateOutput:
     output: str
     input_tokens: int
     output_tokens: int
     total_tokens: int
+    logprobs: torch.Tensor | None
 
 
 @dataclass
 class _QueueItem:
     input: GenerateInput
     future: asyncio.Future[GenerateOutput]
     loop: asyncio.AbstractEventLoop
@@ -286,20 +311,31 @@
             input_ids = tokenized_inputs["input_ids"]
             attention_mask = tokenized_inputs["attention_mask"]
             input_ids = input_ids.to(device)
             attention_mask = attention_mask.to(device)
 
             # generate
             with torch.inference_mode():
-                generate_ids = generator(
+                generation_outputs = generator(
                     input_ids=input_ids, attention_mask=attention_mask
                 )
+                generate_ids = generation_outputs.sequences
+                logits = generation_outputs.logits
+
+            # get logprobs from logits
+            logprobs = None
+            if logits is not None:
+                logits = torch.stack(logits).transpose(0, 1)
+                logprobs = torch.nn.functional.log_softmax(logits, dim=-1)
 
             # decode
-            outputs = decoder(sequences=generate_ids[:, input_ids.size(dim=1) :])
+            generated_tokens = generate_ids[:, input_ids.size(dim=1) :]
+            if logprobs is not None:
+                assert logprobs.shape[1] == generated_tokens.shape[1]
+            outputs = decoder(sequences=generated_tokens)
 
             # call back futures
             for i, output in enumerate(outputs):
                 future = inputs[i][1]
                 input_tokens = input_ids.size(dim=1)
                 output_tokens = generate_ids.size(dim=1) - input_ids.size(dim=1)
 
@@ -309,14 +345,48 @@
                 loop.call_soon_threadsafe(
                     future.set_result,
                     GenerateOutput(
                         output=output,
                         input_tokens=input_tokens,
                         output_tokens=output_tokens,
                         total_tokens=input_tokens + output_tokens,
+                        logprobs=logprobs[i] if logprobs is not None else None,
                     ),
                 )
 
         except Exception as ex:
             for inp in inputs:
                 future = inp[1]
                 loop.call_soon_threadsafe(future.set_exception, ex)
+
+
+def extract_logprobs(
+    response: GenerateOutput,
+    top_logprobs: int | None,
+    tokenizer: PreTrainedTokenizerBase,
+) -> list[Logprob]:
+    assert response.logprobs is not None
+    k = top_logprobs or 1
+    topk_values, topk_inds = response.logprobs.topk(k=k, dim=-1)
+    final_logprobs = []
+    for toks, vals in zip(topk_inds, topk_values):
+        top_logprobs = []
+        for tok, val in zip(toks, vals):
+            # TODO: you get byte artifacts converting single ids to tokens like this...
+            # but `tokenizer.decode` strips spaces. There must be a better way to do this.
+            token_str = tokenizer.convert_ids_to_tokens(tok.item())
+            top_logprobs.append(
+                TopLogprob(
+                    token=token_str,
+                    logprob=val,
+                    bytes=list(map(ord, token_str)),
+                )
+            )
+        final_logprobs.append(
+            Logprob(
+                token=top_logprobs[0].token,
+                logprob=top_logprobs[0].logprob,
+                bytes=top_logprobs[0].bytes,
+                top_logprobs=top_logprobs,
+            )
+        )
+    return final_logprobs
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_providers/mistral.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_providers/mistral.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_providers/openai.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_providers/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 from .._model import (
     ChatCompletionChoice,
     ChatMessage,
     ChatMessageAssistant,
     Content,
     GenerateConfig,
+    Logprobs,
     ModelAPI,
     ModelOutput,
     ModelUsage,
 )
 from .._tool import ToolCall, ToolChoice, ToolFunction, ToolInfo
 from .._util import chat_api_tool
 from .util import as_stop_reason, model_base_url
@@ -138,15 +139,15 @@
                 messages=messages,
                 tools=chat_tools(tools) if len(tools) > 0 else NOT_GIVEN,
                 tool_choice=(
                     chat_tool_choice(tool_choice) if len(tools) > 0 else NOT_GIVEN
                 ),
                 **self.completion_params(config),
             )
-            choices = chat_choices_from_response(response)
+            choices = self._chat_choices_from_response(response)
             return ModelOutput(
                 model=response.model,
                 choices=choices,
                 usage=(
                     ModelUsage(
                         input_tokens=response.usage.prompt_tokens,
                         output_tokens=response.usage.completion_tokens,
@@ -161,14 +162,20 @@
             return ModelOutput.from_content(
                 model=self.model_name,
                 content=completion,
                 stop_reason="content_filter",
                 error=str(error) if error else None,
             )
 
+    def _chat_choices_from_response(
+        self, response: ChatCompletion
+    ) -> list[ChatCompletionChoice]:
+        # adding this as a method so we can override from other classes (e.g together)
+        return chat_choices_from_response(response)
+
     @override
     def is_rate_limit(self, ex: BaseException) -> bool:
         if isinstance(ex, RateLimitError):
             # Do not retry on these rate limit errors
             if (
                 "Request too large" not in ex.message
                 and "You exceeded your current quota" not in ex.message
@@ -312,15 +319,17 @@
     choices = list(response.choices)
     choices.sort(key=lambda c: c.index)
     return [
         ChatCompletionChoice(
             message=chat_message_assistant(choice.message),
             stop_reason=as_stop_reason(choice.finish_reason),
             logprobs=(
-                choice.logprobs.model_dump() if choice.logprobs is not None else None
+                Logprobs(**choice.logprobs.model_dump())
+                if choice.logprobs is not None
+                else None
             ),
         )
         for choice in choices
     ]
 
 
 def chat_message_assistant(message: ChatCompletionMessage) -> ChatMessageAssistant:
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_providers/providers.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_providers/providers.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_providers/util.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_providers/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_registry.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_tool.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_tool.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/model/_util.py` & `inspect_ai-0.3.8/src/inspect_ai/model/_util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/__init__.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/_answer.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/_answer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/_common.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/_common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/_match.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/_match.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/_metric.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/_metric.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/accuracy.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/mean.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/mean.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/std.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/std.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/_model.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/_model.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/_pattern.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/_pattern.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/scorer/_scorer.py` & `inspect_ai-0.3.8/src/inspect_ai/scorer/_scorer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/solver/__init__.py` & `inspect_ai-0.3.8/src/inspect_ai/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/solver/_critique.py` & `inspect_ai-0.3.8/src/inspect_ai/solver/_critique.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/solver/_multiple_choice.py` & `inspect_ai-0.3.8/src/inspect_ai/solver/_multiple_choice.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/solver/_plan.py` & `inspect_ai-0.3.8/src/inspect_ai/solver/_plan.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/solver/_prompt.py` & `inspect_ai-0.3.8/src/inspect_ai/solver/_prompt.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/solver/_solver.py` & `inspect_ai-0.3.8/src/inspect_ai/solver/_solver.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/solver/_tool/tool.py` & `inspect_ai-0.3.8/src/inspect_ai/solver/_tool/tool.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/solver/_tool/tool_def.py` & `inspect_ai-0.3.8/src/inspect_ai/solver/_tool/tool_def.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/solver/_tool/use_tools.py` & `inspect_ai-0.3.8/src/inspect_ai/solver/_tool/use_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/solver/_tool/web_search.py` & `inspect_ai-0.3.8/src/inspect_ai/solver/_tool/web_search.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/util/_context/concurrency.py` & `inspect_ai-0.3.8/src/inspect_ai/util/_context/concurrency.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/util/_context/logger.py` & `inspect_ai-0.3.8/src/inspect_ai/util/_context/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/util/_context/resource.py` & `inspect_ai-0.3.8/src/inspect_ai/util/_context/resource.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai/util/_context/subprocess.py` & `inspect_ai-0.3.8/src/inspect_ai/util/_context/subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/src/inspect_ai.egg-info/PKG-INFO` & `inspect_ai-0.3.8/src/inspect_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.6
+Version: 0.3.8
 Summary: Framework for large language model evaluations
 Author: UK AI Safety Institute
 License: MIT License
 Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
 Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
 Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `inspect_ai-0.3.6/src/inspect_ai.egg-info/requires.txt` & `inspect_ai-0.3.8/src/inspect_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_anthropic.py` & `inspect_ai-0.3.8/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_collapse_user_message.py` & `inspect_ai-0.3.8/tests/test_collapse_user_message.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_dataset.py` & `inspect_ai-0.3.8/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_eval_log.py` & `inspect_ai-0.3.8/tests/test_eval_log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_hf.py` & `inspect_ai-0.3.8/tests/test_hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_images/images.jsonl` & `inspect_ai-0.3.8/tests/test_images/images.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_images.py` & `inspect_ai-0.3.8/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_list_task.py` & `inspect_ai-0.3.8/tests/test_list_task.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_logprobs.py` & `inspect_ai-0.3.8/tests/test_num_choices.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import pytest
 from utils import skip_if_no_openai, skip_if_no_together
 
-from inspect_ai.model import ChatMessageUser, GenerateConfig, ModelOutput, get_model
+from inspect_ai.model import GenerateConfig, get_model
 
 
-async def generate_with_logprobs(model_name) -> ModelOutput:
-    model = get_model(
-        model_name,
-        config=GenerateConfig(logprobs=True, top_logprobs=2),
-    )
+async def generate(model_name):
+    model = get_model(model_name)
+    return await model.generate(input="Hello.", config=GenerateConfig(num_choices=3))
+
 
-    message = ChatMessageUser(content="Hello.")
-    return await model.generate(input=[message])
+async def check_num_choices(model_name):
+    model = get_model(model_name)
+    response = await model.generate(
+        input="Hello.", config=GenerateConfig(num_choices=3)
+    )
+    assert len(response.choices) == 3
 
 
 @pytest.mark.asyncio
 @skip_if_no_openai
-async def test_openai_logprobs() -> None:
-    response = await generate_with_logprobs("openai/gpt-3.5-turbo")
-    assert response.choices[0].logprobs is not None
-    assert len(response.choices[0].logprobs["content"][0]["top_logprobs"]) == 2
+async def test_openai_num_choices() -> None:
+    await check_num_choices("openai/gpt-3.5-turbo")
 
 
 @pytest.mark.asyncio
 @skip_if_no_together
-async def test_together_logprobs() -> None:
-    response = await generate_with_logprobs("together/lmsys/vicuna-13b-v1.5")
-    assert (
-        response.choices[0].logprobs
-        and response.choices[0].logprobs["token_ids"] is not None
-    )
+async def test_together_num_choices() -> None:
+    await check_num_choices("together/google/gemma-2b-it")
+
+
+# @pytest.mark.asyncio
+# @skip_if_no_azureai
+# async def test_azureai_num_choices() -> None:
+#     await check_num_choices(None)
```

### Comparing `inspect_ai-0.3.6/tests/test_metric.py` & `inspect_ai-0.3.8/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_openai.py` & `inspect_ai-0.3.8/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_plan.py` & `inspect_ai-0.3.8/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_registry.py` & `inspect_ai-0.3.8/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_retry.py` & `inspect_ai-0.3.8/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_scorer.py` & `inspect_ai-0.3.8/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_solver.py` & `inspect_ai-0.3.8/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_stop_reason.py` & `inspect_ai-0.3.8/tests/test_stop_reason.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_subprocess.py` & `inspect_ai-0.3.8/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/test_tools.py` & `inspect_ai-0.3.8/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.6/tests/utils.py` & `inspect_ai-0.3.8/tests/utils.py`

 * *Files identical despite different names*

