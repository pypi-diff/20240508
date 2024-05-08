# Comparing `tmp/ast_grep_py-0.21.4.tar.gz` & `tmp/ast_grep_py-0.22.0.tar.gz`

## Comparing `ast_grep_py-0.21.4.tar` & `ast_grep_py-0.22.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0     1001      127     2219 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/Cargo.toml
--rw-r--r--   0     1001      127     1047 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/bash.rs
--rw-r--r--   0     1001      127     1023 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/cpp.rs
--rw-r--r--   0     1001      127      860 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/csharp.rs
--rw-r--r--   0     1001      127      815 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/css.rs
--rw-r--r--   0     1001      127     2412 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/elixir.rs
--rw-r--r--   0     1001      127     1192 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/go.rs
--rw-r--r--   0     1001      127     1142 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/html.rs
--rw-r--r--   0     1001      127     1013 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/json.rs
--rw-r--r--   0     1001      127     1216 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/kotlin.rs
--rw-r--r--   0     1001      127    13416 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/lib.rs
--rw-r--r--   0     1001      127      924 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/lua.rs
--rw-r--r--   0     1001      127     3410 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/parsers.rs
--rw-r--r--   0     1001      127      372 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/php.rs
--rw-r--r--   0     1001      127     2494 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/python.rs
--rw-r--r--   0     1001      127      846 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/ruby.rs
--rw-r--r--   0     1001      127     2157 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/rust.rs
--rw-r--r--   0     1001      127     1646 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/scala.rs
--rw-r--r--   0     1001      127     1362 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/swift.rs
--rw-r--r--   0     1001      127      693 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/Cargo.toml
--rw-r--r--   0     1001      127     2331 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/language.rs
--rw-r--r--   0     1001      127     3904 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/lib.rs
--rw-r--r--   0     1001      127    15102 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/match_tree.rs
--rw-r--r--   0     1001      127     3610 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/matcher/kind.rs
--rw-r--r--   0     1001      127     3689 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/matcher/node_match.rs
--rw-r--r--   0     1001      127    15050 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/matcher/pattern.rs
--rw-r--r--   0     1001      127      982 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/matcher/text.rs
--rw-r--r--   0     1001      127     5317 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/matcher.rs
--rw-r--r--   0     1001      127    10527 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/meta_var.rs
--rw-r--r--   0     1001      127    17980 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/node.rs
--rw-r--r--   0     1001      127    15251 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/ops.rs
--rw-r--r--   0     1001      127     4789 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/pinned.rs
--rw-r--r--   0     1001      127    10854 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/replacer/indent.rs
--rw-r--r--   0     1001      127     6157 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/replacer/structural.rs
--rw-r--r--   0     1001      127    10186 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/replacer/template.rs
--rw-r--r--   0     1001      127     2855 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/replacer.rs
--rw-r--r--   0     1001      127     8489 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/source.rs
--rw-r--r--   0     1001      127    16602 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/traversal.rs
--rw-r--r--   0     1001      127      683 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/Cargo.toml
--rw-r--r--   0     1001      127     8074 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/check_var.rs
--rw-r--r--   0     1001      127     7022 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/combined.rs
--rw-r--r--   0     1001      127     8734 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/fixer.rs
--rw-r--r--   0     1001      127     5244 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/lib.rs
--rw-r--r--   0     1001      127     3677 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/maybe.rs
--rw-r--r--   0     1001      127     8987 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule/deserialize_env.rs
--rw-r--r--   0     1001      127    17978 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule/mod.rs
--rw-r--r--   0     1001      127     8432 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule/referent_rule.rs
--rw-r--r--   0     1001      127    19521 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule/relational_rule.rs
--rw-r--r--   0     1001      127     5481 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule/stop_by.rs
--rw-r--r--   0     1001      127     6342 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule_collection.rs
--rw-r--r--   0     1001      127    17934 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule_config.rs
--rw-r--r--   0     1001      127    13810 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule_core.rs
--rw-r--r--   0     1001      127     3341 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/transform/mod.rs
--rw-r--r--   0     1001      127    11131 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/transform/rewrite.rs
--rw-r--r--   0     1001      127     7418 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/transform/string_case.rs
--rw-r--r--   0     1001      127    11870 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/transform/transformation.rs
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.21.4/crates/pyo3/Cargo.toml
--rw-r--r--   0     1001      127     1459 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/README.md
--rw-r--r--   0     1001      127     1356 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1933 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1090 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/src/lib.rs
--rw-r--r--   0     1001      127     7731 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/src/py_node.rs
--rw-r--r--   0     1001      127     2358 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/src/range.rs
--rw-r--r--   0     1001      127      893 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/tests/test_range.py
--rw-r--r--   0     1001      127     3641 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/tests/test_rule.py
--rw-r--r--   0     1001      127     3463 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/tests/test_simple.py
--rw-r--r--   0     1001      127     3221 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/tests/test_traversal.py
--rw-r--r--   0     1001      127     1214 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/tests/test_wrong_usage.py
--rw-r--r--   0     1001      127    61091 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/Cargo.lock
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 ast_grep_py-0.21.4/Cargo.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.21.4/pyproject.toml
--rw-r--r--   0     1001      127     1933 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1356 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1459 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/README.md
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.21.4/PKG-INFO
+-rw-r--r--   0     1001      127      692 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/Cargo.toml
+-rw-r--r--   0     1001      127     2331 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/language.rs
+-rw-r--r--   0     1001      127     3904 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/lib.rs
+-rw-r--r--   0     1001      127    15102 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/match_tree.rs
+-rw-r--r--   0     1001      127     3610 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/matcher/kind.rs
+-rw-r--r--   0     1001      127     3689 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      127    15050 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      127      982 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/matcher/text.rs
+-rw-r--r--   0     1001      127     5317 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/matcher.rs
+-rw-r--r--   0     1001      127    10527 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/meta_var.rs
+-rw-r--r--   0     1001      127    17457 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/node.rs
+-rw-r--r--   0     1001      127    15251 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/ops.rs
+-rw-r--r--   0     1001      127     4789 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/pinned.rs
+-rw-r--r--   0     1001      127    10854 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/replacer/indent.rs
+-rw-r--r--   0     1001      127     6157 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/replacer/structural.rs
+-rw-r--r--   0     1001      127    10186 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/replacer/template.rs
+-rw-r--r--   0     1001      127     2855 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/replacer.rs
+-rw-r--r--   0     1001      127     8489 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/source.rs
+-rw-r--r--   0     1001      127    16602 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/traversal.rs
+-rw-r--r--   0     1001      127      682 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/Cargo.toml
+-rw-r--r--   0     1001      127     8074 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/check_var.rs
+-rw-r--r--   0     1001      127     7022 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/combined.rs
+-rw-r--r--   0     1001      127     8734 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/fixer.rs
+-rw-r--r--   0     1001      127     5244 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/lib.rs
+-rw-r--r--   0     1001      127     3677 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/maybe.rs
+-rw-r--r--   0     1001      127     8987 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule/deserialize_env.rs
+-rw-r--r--   0     1001      127    17978 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule/mod.rs
+-rw-r--r--   0     1001      127     8432 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule/referent_rule.rs
+-rw-r--r--   0     1001      127    19521 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule/relational_rule.rs
+-rw-r--r--   0     1001      127     5481 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule/stop_by.rs
+-rw-r--r--   0     1001      127     6342 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule_collection.rs
+-rw-r--r--   0     1001      127    17934 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule_config.rs
+-rw-r--r--   0     1001      127    13810 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule_core.rs
+-rw-r--r--   0     1001      127     3341 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/transform/mod.rs
+-rw-r--r--   0     1001      127    11131 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/transform/rewrite.rs
+-rw-r--r--   0     1001      127     7418 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/transform/string_case.rs
+-rw-r--r--   0     1001      127    11870 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/transform/transformation.rs
+-rw-r--r--   0     1001      127     2384 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/Cargo.toml
+-rw-r--r--   0     1001      127     1047 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/bash.rs
+-rw-r--r--   0     1001      127     1023 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/cpp.rs
+-rw-r--r--   0     1001      127      860 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/csharp.rs
+-rw-r--r--   0     1001      127      815 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/css.rs
+-rw-r--r--   0     1001      127     2412 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/elixir.rs
+-rw-r--r--   0     1001      127     1192 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/go.rs
+-rw-r--r--   0     1001      127     1142 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/html.rs
+-rw-r--r--   0     1001      127     1013 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/json.rs
+-rw-r--r--   0     1001      127     1216 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/kotlin.rs
+-rw-r--r--   0     1001      127    13416 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/lib.rs
+-rw-r--r--   0     1001      127      924 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/lua.rs
+-rw-r--r--   0     1001      127     3410 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/parsers.rs
+-rw-r--r--   0     1001      127      372 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/php.rs
+-rw-r--r--   0     1001      127     2494 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/python.rs
+-rw-r--r--   0     1001      127      846 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/ruby.rs
+-rw-r--r--   0     1001      127     2147 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/rust.rs
+-rw-r--r--   0     1001      127     1646 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/scala.rs
+-rw-r--r--   0     1001      127     1362 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/swift.rs
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.22.0/crates/pyo3/Cargo.toml
+-rw-r--r--   0     1001      127     1459 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/README.md
+-rw-r--r--   0     1001      127     1356 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1933 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1090 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     7731 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/src/py_node.rs
+-rw-r--r--   0     1001      127     2358 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/src/range.rs
+-rw-r--r--   0     1001      127      893 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/tests/test_range.py
+-rw-r--r--   0     1001      127     3641 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/tests/test_rule.py
+-rw-r--r--   0     1001      127     3463 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/tests/test_simple.py
+-rw-r--r--   0     1001      127     3221 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/tests/test_traversal.py
+-rw-r--r--   0     1001      127     1214 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/tests/test_wrong_usage.py
+-rw-r--r--   0     1001      127    61561 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/Cargo.lock
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 ast_grep_py-0.22.0/Cargo.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.22.0/pyproject.toml
+-rw-r--r--   0     1001      127     1933 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1356 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1459 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/README.md
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.22.0/PKG-INFO
```

### Comparing `ast_grep_py-0.21.4/crates/language/Cargo.toml` & `ast_grep_py-0.22.0/crates/language/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,35 +12,37 @@
 
 [dependencies]
 ast-grep-core.workspace = true
 
 ignore.workspace = true
 serde.workspace = true
 
-tree-sitter-bash = { version = "0.20.5", optional = true }
-tree-sitter-c = { version = "0.20.8", optional = true }
-tree-sitter-cpp = { version = "0.20.5", optional = true }
-tree-sitter-c-sharp = { version = "0.20.0", optional = true }
-tree-sitter-css = { version = "0.20.0", optional = true }
-tree-sitter-dart= { version = "0.0.3", optional = true }
-tree-sitter-elixir = { version = "0.1.1", optional = true }
-tree-sitter-go = { version = "0.20.0", optional = true }
-tree-sitter-html = { version = "0.20.0", optional = true }
-tree-sitter-java = { version = "0.20.2", optional = true }
-tree-sitter-javascript = { version = "0.20.4", optional = true }
-tree-sitter-json = { version = "0.20.2", optional = true }
-tree-sitter-kotlin = { version = "0.3.5", optional = true }
-tree-sitter-lua = { version = "0.0.19", optional = true }
-tree-sitter-php = { version = "0.22.2", optional = true }
-tree-sitter-python = { version = "0.20.4", optional = true }
-tree-sitter-ruby = { version = "0.20.1", optional = true }
-tree-sitter-rust = { version = "0.20.4", optional = true }
-tree-sitter-scala = { version = "0.20.3", optional = true }
-tree-sitter-swift = { version = "0.4.3", optional = true }
-tree-sitter-typescript= { version = "0.20.5", optional = true }
+tree-sitter-bash = { version = "0.21.0", optional = true }
+tree-sitter-c = { version = "0.21.0", optional = true }
+tree-sitter-cpp = { version = "0.22.0", optional = true }
+tree-sitter-c-sharp = { version = "0.21.1", optional = true }
+tree-sitter-css = { version = "0.21.0", optional = true }
+tree-sitter-dart= { version = "0.0.4", optional = true }
+tree-sitter-elixir = { version = "0.2.0", optional = true }
+tree-sitter-go = { version = "0.21.0", optional = true }
+tree-sitter-html = { version = "0.20.3", optional = true }
+tree-sitter-java = { version = "0.21.0", optional = true }
+# https://github.com/tree-sitter/tree-sitter-javascript/issues/316
+tree-sitter-javascript = { version = "0.21.2", optional = true, package="tree-sitter-javascript-sg" }
+tree-sitter-json = { version = "0.21.0", optional = true }
+# TODO https://github.com/fwcd/tree-sitter-kotlin/issues/118
+tree-sitter-kotlin = { version = "0.3.6", optional = true }
+tree-sitter-lua = { version = "0.1.0", optional = true }
+tree-sitter-php = { version = "0.22.4", optional = true }
+tree-sitter-python = { version = "0.21.0", optional = true }
+tree-sitter-ruby = { version = "0.21.0", optional = true }
+tree-sitter-rust = { version = "0.21.2", optional = true }
+tree-sitter-scala = { version = "0.21.0", optional = true }
+tree-sitter-swift = { version = "=0.4.2", optional = true }
+tree-sitter-typescript= { version = "0.21.1", optional = true }
 
 [features]
 builtin-parser = [
   "tree-sitter-bash",
   "tree-sitter-c",
   "tree-sitter-cpp",
   "tree-sitter-c-sharp",
```

### Comparing `ast_grep_py-0.21.4/crates/language/src/bash.rs` & `ast_grep_py-0.22.0/crates/language/src/bash.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/cpp.rs` & `ast_grep_py-0.22.0/crates/language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/csharp.rs` & `ast_grep_py-0.22.0/crates/language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/css.rs` & `ast_grep_py-0.22.0/crates/language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/elixir.rs` & `ast_grep_py-0.22.0/crates/language/src/elixir.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/go.rs` & `ast_grep_py-0.22.0/crates/language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/html.rs` & `ast_grep_py-0.22.0/crates/language/src/html.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/json.rs` & `ast_grep_py-0.22.0/crates/language/src/json.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/kotlin.rs` & `ast_grep_py-0.22.0/crates/language/src/kotlin.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/lib.rs` & `ast_grep_py-0.22.0/crates/language/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/lua.rs` & `ast_grep_py-0.22.0/crates/language/src/lua.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/parsers.rs` & `ast_grep_py-0.22.0/crates/language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/python.rs` & `ast_grep_py-0.22.0/crates/language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/ruby.rs` & `ast_grep_py-0.22.0/crates/language/src/ruby.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/rust.rs` & `ast_grep_py-0.22.0/crates/language/src/rust.rs`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 }"#,
   );
 }
 
 // it is fixed in https://github.com/tree-sitter/tree-sitter-rust/issues/218
 // but not released yet
 #[test]
-#[ignore]
 fn test_issue_1057() {
   // fix #1057
   test_match("foo(\"meaning\");", "fn t() { foo(\"meaning\");}");
   test_non_match("foo(\"meaning\");", "fn t() { foo(\"service\");}");
 }
 
 #[test]
```

### Comparing `ast_grep_py-0.21.4/crates/language/src/scala.rs` & `ast_grep_py-0.22.0/crates/language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/language/src/swift.rs` & `ast_grep_py-0.22.0/crates/language/src/swift.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/Cargo.toml` & `ast_grep_py-0.22.0/crates/core/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 thiserror.workspace = true
 tree-sitter.workspace = true
 
 [features]
 default = ["regex"]
 
 [dev-dependencies]
-tree-sitter-typescript = "0.20.5"
+tree-sitter-typescript = "0.21.1"
```

### Comparing `ast_grep_py-0.21.4/crates/core/src/language.rs` & `ast_grep_py-0.22.0/crates/core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/lib.rs` & `ast_grep_py-0.22.0/crates/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/match_tree.rs` & `ast_grep_py-0.22.0/crates/core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/matcher/kind.rs` & `ast_grep_py-0.22.0/crates/core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/matcher/node_match.rs` & `ast_grep_py-0.22.0/crates/core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/matcher/pattern.rs` & `ast_grep_py-0.22.0/crates/core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/matcher/text.rs` & `ast_grep_py-0.22.0/crates/core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/matcher.rs` & `ast_grep_py-0.22.0/crates/core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/meta_var.rs` & `ast_grep_py-0.22.0/crates/core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/node.rs` & `ast_grep_py-0.22.0/crates/core/src/node.rs`

 * *Files 8% similar despite different names*

```diff
@@ -375,64 +375,48 @@
     })
   }
 
   /// Returns all sibling nodes next to `self`.
   // NOTE: Need go to parent first, then move to current node by byte offset.
   // This is because tree_sitter cursor is scoped to the starting node.
   // See https://github.com/tree-sitter/tree-sitter/issues/567
-  // TODO: remove this target_arch dependent code branch
-  // TODO: we need to add goto_first_child_for_byte in web-tree-sitter
-  // https://github.com/tree-sitter/tree-sitter/discussions/2288
-  #[cfg(not(target_arch = "wasm32"))]
   pub fn next_all(&self) -> impl Iterator<Item = Node<'r, D>> + '_ {
     // if root is none, use self as fallback to return a type-stable Iterator
     let node = self.parent().unwrap_or_else(|| self.clone());
     let mut cursor = node.inner.walk();
     cursor.goto_first_child_for_byte(self.inner.start_byte());
     std::iter::from_fn(move || {
       if cursor.goto_next_sibling() {
         Some(self.root.adopt(cursor.node()))
       } else {
         None
       }
     })
   }
 
-  // TODO: remove this target_arch dependent code branch
-  // TODO: we need to add goto_first_child_for_byte in web-tree-sitter
-  // https://github.com/tree-sitter/tree-sitter/discussions/2288
-  #[cfg(target_arch = "wasm32")]
-  pub fn next_all(&self) -> impl Iterator<Item = Node<'r, D>> + '_ {
-    let mut node = self.clone();
-    std::iter::from_fn(move || {
-      node.next().map(|n| {
-        node = n.clone();
-        n
-      })
-    })
-  }
-
   #[must_use]
   pub fn prev(&self) -> Option<Node<'r, D>> {
     let inner = self.inner.prev_sibling()?;
     Some(Node {
       inner,
       root: self.root,
     })
   }
 
-  // TODO: use cursor to optimize clone.
-  // investigate why tree_sitter cursor cannot goto next_sibling
   pub fn prev_all(&self) -> impl Iterator<Item = Node<'r, D>> + '_ {
-    let mut node = self.clone();
+    // if root is none, use self as fallback to return a type-stable Iterator
+    let node = self.parent().unwrap_or_else(|| self.clone());
+    let mut cursor = node.inner.walk();
+    cursor.goto_first_child_for_byte(self.inner.start_byte());
     std::iter::from_fn(move || {
-      node.prev().map(|n| {
-        node = n.clone();
-        n
-      })
+      if cursor.goto_previous_sibling() {
+        Some(self.root.adopt(cursor.node()))
+      } else {
+        None
+      }
     })
   }
 
   pub fn dfs<'s>(&'s self) -> Pre<'r, D> {
     Pre::new(self)
   }
```

### Comparing `ast_grep_py-0.21.4/crates/core/src/ops.rs` & `ast_grep_py-0.22.0/crates/core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/pinned.rs` & `ast_grep_py-0.22.0/crates/core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/replacer/indent.rs` & `ast_grep_py-0.22.0/crates/core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/replacer/structural.rs` & `ast_grep_py-0.22.0/crates/core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/replacer/template.rs` & `ast_grep_py-0.22.0/crates/core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/replacer.rs` & `ast_grep_py-0.22.0/crates/core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/source.rs` & `ast_grep_py-0.22.0/crates/core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/core/src/traversal.rs` & `ast_grep_py-0.22.0/crates/core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/Cargo.toml` & `ast_grep_py-0.22.0/crates/config/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 regex = { workspace = true, optional = true }
 serde.workspace = true
 serde_yaml = "0.9.33"
 thiserror.workspace = true
 schemars.workspace = true
 
 [dev-dependencies]
-tree-sitter-typescript = "0.20.5"
+tree-sitter-typescript = "0.21.1"
```

### Comparing `ast_grep_py-0.21.4/crates/config/src/check_var.rs` & `ast_grep_py-0.22.0/crates/config/src/check_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/combined.rs` & `ast_grep_py-0.22.0/crates/config/src/combined.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/fixer.rs` & `ast_grep_py-0.22.0/crates/config/src/fixer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/lib.rs` & `ast_grep_py-0.22.0/crates/config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/maybe.rs` & `ast_grep_py-0.22.0/crates/config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/rule/deserialize_env.rs` & `ast_grep_py-0.22.0/crates/config/src/rule/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/rule/mod.rs` & `ast_grep_py-0.22.0/crates/config/src/rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/rule/referent_rule.rs` & `ast_grep_py-0.22.0/crates/config/src/rule/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/rule/relational_rule.rs` & `ast_grep_py-0.22.0/crates/config/src/rule/relational_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/rule/stop_by.rs` & `ast_grep_py-0.22.0/crates/config/src/rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/rule_collection.rs` & `ast_grep_py-0.22.0/crates/config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/rule_config.rs` & `ast_grep_py-0.22.0/crates/config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/rule_core.rs` & `ast_grep_py-0.22.0/crates/config/src/rule_core.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/transform/mod.rs` & `ast_grep_py-0.22.0/crates/config/src/transform/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/transform/rewrite.rs` & `ast_grep_py-0.22.0/crates/config/src/transform/rewrite.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/transform/string_case.rs` & `ast_grep_py-0.22.0/crates/config/src/transform/string_case.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/config/src/transform/transformation.rs` & `ast_grep_py-0.22.0/crates/config/src/transform/transformation.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/Cargo.toml` & `ast_grep_py-0.22.0/crates/pyo3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/README.md` & `ast_grep_py-0.22.0/crates/pyo3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/ast_grep_py/__init__.py` & `ast_grep_py-0.22.0/crates/pyo3/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.22.0/crates/pyo3/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/src/lib.rs` & `ast_grep_py-0.22.0/crates/pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/src/py_node.rs` & `ast_grep_py-0.22.0/crates/pyo3/src/py_node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/src/range.rs` & `ast_grep_py-0.22.0/crates/pyo3/src/range.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/tests/test_range.py` & `ast_grep_py-0.22.0/crates/pyo3/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/tests/test_rule.py` & `ast_grep_py-0.22.0/crates/pyo3/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/tests/test_simple.py` & `ast_grep_py-0.22.0/crates/pyo3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/tests/test_traversal.py` & `ast_grep_py-0.22.0/crates/pyo3/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/crates/pyo3/tests/test_wrong_usage.py` & `ast_grep_py-0.22.0/crates/pyo3/tests/test_wrong_usage.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/Cargo.lock` & `ast_grep_py-0.22.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -39,65 +39,66 @@
 checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.13"
+version = "0.6.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
+checksum = "418c75fa768af9c03be99d17643f93f79bbba589895012a80e3452a19ddda15b"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
+ "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+checksum = "c03a11a9034d92058ceb6ee011ce58af4a9bf61491aa7e1e59ecd24bd40d22d4"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+checksum = "a64c907d4e79225ac72e2a354c9ce84d50ebb4586dee56c82b3ee73004f537f5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+checksum = "61a38449feb7068f52bb06c12759005cf459ee52bb4adc1d5a7c4322d716fb19"
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.82"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
+checksum = "25bdb32cbbdce2b519a9cd7df3a678443100e265d5e25ca763b7572a5104f5f3"
 
 [[package]]
 name = "assert_cmd"
 version = "2.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed72493ac66d5804837f480ab3766c72bdfab91a65e565fc54fa9e42db0073a8"
 dependencies = [
@@ -108,15 +109,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.21.4"
+version = "0.22.0"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -139,15 +140,15 @@
  "similar",
  "tempfile",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.21.4"
+version = "0.22.0"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "schemars",
@@ -155,114 +156,114 @@
  "serde_yaml",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.21.4"
+version = "0.22.0"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.21.4"
+version = "0.22.0"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.21.4"
+version = "0.22.0"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "serde",
  "tree-sitter-bash",
  "tree-sitter-c",
  "tree-sitter-c-sharp",
  "tree-sitter-cpp",
  "tree-sitter-css",
  "tree-sitter-dart",
  "tree-sitter-elixir",
  "tree-sitter-go",
  "tree-sitter-html",
  "tree-sitter-java",
- "tree-sitter-javascript",
+ "tree-sitter-javascript-sg",
  "tree-sitter-json",
  "tree-sitter-kotlin",
  "tree-sitter-lua",
  "tree-sitter-php",
  "tree-sitter-python",
  "tree-sitter-ruby",
  "tree-sitter-rust",
  "tree-sitter-scala",
  "tree-sitter-swift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.21.4"
+version = "0.22.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "dashmap",
  "serde",
  "serde_json",
  "tokio",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.21.4"
+version = "0.22.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
  "serde_json",
  "tree-sitter-css",
  "tree-sitter-facade-sg",
  "tree-sitter-html",
- "tree-sitter-javascript",
+ "tree-sitter-javascript-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-py"
-version = "0.21.4"
+version = "0.22.0"
 dependencies = [
  "anyhow",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "pyo3",
  "pythonize",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.79"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -285,17 +286,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
 version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
@@ -306,15 +307,15 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "benches"
-version = "0.21.4"
+version = "0.22.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -378,17 +379,17 @@
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -476,17 +477,17 @@
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
 name = "colorchoice"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
 [[package]]
 name = "convert_case"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec182b0ca2f35d8fc196cf3404988fd8b8c739a4d270ff118a398feb0cbec1ca"
 dependencies = [
@@ -599,17 +600,17 @@
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "ctor"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad291aa74992b9b7a7e88c38acbbf6ad7e107f1d90ee8775b7bc1fc3394f485c"
+checksum = "edb49164822f3ee45b17acd4a208cfc1251410cf0cad9a833234c9890774dd9f"
 dependencies = [
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "dashmap"
@@ -640,17 +641,17 @@
 name = "dyn-clone"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
@@ -662,17 +663,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "float-cmp"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98de4bbd547a563b716d8dfa9aad1cb19bfab00f4fa09a6a4ed21dbcf44ce9c4"
 dependencies = [
@@ -800,27 +801,27 @@
  "log",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "half"
-version = "2.4.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -918,14 +919,20 @@
 dependencies = [
  "hermit-abi 0.3.9",
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "is_terminal_polyfill"
+version = "1.70.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8478577c03552c21db0e2724ffb8986a5ce7af88107e6be5d2ee6e158c12800"
+
+[[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
@@ -943,39 +950,39 @@
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -1030,17 +1037,17 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "napi"
-version = "2.16.4"
+version = "2.16.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da1edd9510299935e4f52a24d1e69ebd224157e3e962c6c847edec5c2e4f786f"
+checksum = "dfc300228808a0e6aea5a58115c82889240bcf8dab16fc25ad675b33e454b368"
 dependencies = [
  "anyhow",
  "bitflags 2.5.0",
  "ctor",
  "napi-derive",
  "napi-sys",
  "once_cell",
@@ -1052,31 +1059,31 @@
 name = "napi-build"
 version = "2.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1c0f5d67ee408a4685b61f5ab7e58605c8ae3f2b4189f0127d804ff13d5560a"
 
 [[package]]
 name = "napi-derive"
-version = "2.16.3"
+version = "2.16.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5a6de411b6217dbb47cd7a8c48684b162309ff48a77df9228c082400dd5b030"
+checksum = "4bb613535cde46cff231e53cd819c1694a32d48946bc2dda6b41174ace52ac08"
 dependencies = [
  "cfg-if",
  "convert_case",
  "napi-derive-backend",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "napi-derive-backend"
-version = "1.0.65"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3e35868d43b178b0eb9c17bd018960b1b5dd1732a7d47c23debe8f5c4caf498"
+checksum = "da041b19246ab4240998774e987fd9a7d92cc7406b91b5eddb6691e81feac044"
 dependencies = [
  "convert_case",
  "once_cell",
  "proc-macro2",
  "quote",
  "regex",
  "semver",
@@ -1105,17 +1112,17 @@
 name = "normalize-line-endings"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61807f77802ff30975e01f4f071c8ba10c022052f98b3294119f3e615d13e5be"
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -1145,33 +1152,33 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -1270,17 +1277,17 @@
 dependencies = [
  "predicates-core",
  "termtree",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
@@ -1353,17 +1360,17 @@
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rayon"
 version = "1.10.0"
@@ -1382,19 +1389,19 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
@@ -1420,63 +1427,63 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "schemars"
-version = "0.8.17"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f55c82c700538496bdc329bb4918a81f87cc8888811bd123cf325a0f2f8d309"
+checksum = "fc6e7ed6919cb46507fb01ff1654309219f62b4d603822501b0b80d42f6f21ef"
 dependencies = [
  "dyn-clone",
  "schemars_derive",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "schemars_derive"
-version = "0.8.17"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83263746fe5e32097f06356968a077f96089739c927a61450efa069905eec108"
+checksum = "185f2b7aa7e02d418e453790dde16890256bbd2bcd04b7dc5348811052b53f49"
 dependencies = [
  "proc-macro2",
  "quote",
  "serde_derive_internals",
  "syn",
 ]
 
@@ -1484,32 +1491,32 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "serde"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1521,29 +1528,29 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_repr"
-version = "0.1.18"
+version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b2e6b945e9d3df726b65d6ee24060aff8e3533d431f677a9695db04eff9dfdb"
+checksum = "6c64451ba24fc7a6a2d60fc75dd9c83c90903b19028d4eff35e88fc1e86564e9"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1578,17 +1585,17 @@
  "libc",
  "mio",
  "signal-hook",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "similar"
 version = "2.5.0"
@@ -1614,17 +1621,17 @@
 name = "strsim"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "syn"
-version = "2.0.57"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1658,26 +1665,26 @@
 name = "termtree"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3369f5ac52d5eb6ab48c6b4ffdc8efbcad6b89c765749064ba298f2c68a16a76"
 
 [[package]]
 name = "thiserror"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1725,24 +1732,23 @@
  "bytes",
  "num_cpus",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "toml_datetime"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
@@ -1847,240 +1853,240 @@
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "tree-sitter"
-version = "0.20.10"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e747b1f9b7b931ed39a548c1fae149101497de3c1fc8d9e18c62c1a66c683d3d"
+checksum = "705bf7c0958d0171dd7d3a6542f2f4f21d87ed5f1dc8db52919d3a6bed9a359a"
 dependencies = [
  "cc",
  "regex",
 ]
 
 [[package]]
 name = "tree-sitter-bash"
-version = "0.20.5"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57da2032c37eb2ce29fd18df7d3b94355fec8d6d854d8f80934955df542b5906"
+checksum = "b5244703ad2e08a616d859a0557d7aa290adcd5e0990188a692e628ffe9dce40"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-c"
-version = "0.20.8"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bbd5f3d8658c08581f8f2adac6c391c2e9fa00fe9246bf6c5f52213b9cc6b72"
+checksum = "d463580f35b642e3073d163c9ba84f5212bfde538e5c06c40a085b3d560190ea"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-c-sharp"
-version = "0.20.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ab3dc608f34924fa9e10533a95f62dbc14b6de0ddd7107722eba66fe19ae31"
+checksum = "ff899037068a1ffbb891891b7e94db1400ddf12c3d934b85b8c9e30be5cd18da"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-cpp"
-version = "0.20.5"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46b04a5ada71059afb9895966a6cc1094acc8d2ea1971006db26573e7dfebb74"
+checksum = "28cd45e7e51833e81da966a15b0cb42baa50d82a45467292e2e5e25999e9736b"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-css"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3306ddefa1d2681adda2613d11974ffabfbeb215e23235da6c862f3493a04fd"
+checksum = "e2f806f96136762b0121f5fdd7172a3dcd8f42d37a2f23ed7f11b35895e20eb4"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-dart"
-version = "0.0.3"
+version = "0.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fb6a2192689dd0554c558cfb81d96e446c41d101d701521fd1b452774d132ba"
+checksum = "19f1f70b80ce41343e14aafcef67b5ba2e9de89587535b4aabbabb8036f4e38a"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-elixir"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1bc0b1f3e6d9f12ca22ae5171f32fd154e3aea29dff565d05ef785c28931415b"
+checksum = "df94bf7f057768b1cab2ee1f14812ed4ae33f9e04d09254043eeaa797db4ef70"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-facade-sg"
-version = "0.9.2"
+version = "0.21.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf5a4036a699b30bb1360c9883502d8473c5fe5a7f10d4cb0fefb0fbfd97228b"
+checksum = "d56b01a682080bbfb3cc9cc52550929b936f1838b22870a82ad34aafb1010991"
 dependencies = [
  "js-sys",
  "tree-sitter",
  "wasm-bindgen",
  "web-sys",
  "web-tree-sitter-sg",
 ]
 
 [[package]]
 name = "tree-sitter-go"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ad6d11f19441b961af2fda7f12f5d0dac325f6d6de83836a1d3750018cc5114"
+checksum = "55cb318be5ccf75f44e054acf6898a5c95d59b53443eed578e16be0cd7ec037f"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-html"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "017822b6bd42843c4bd67fabb834f61ce23254e866282dd93871350fd6b7fa1d"
+checksum = "95b3492b08a786bf5cc79feb0ef2ff3b115d5174364e0ddfd7860e0b9b088b53"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-java"
-version = "0.20.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2adc5696bf5abf761081d7457d2bb82d0e3b28964f4214f63fd7e720ef462653"
+checksum = "33bc21adf831a773c075d9d00107ab43965e6a6ea7607b47fd9ec6f3db4b481b"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
-name = "tree-sitter-javascript"
-version = "0.20.4"
+name = "tree-sitter-javascript-sg"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d015c02ea98b62c806f7329ff71c383286dfc3a7a7da0cc484f6e42922f73c2c"
+checksum = "6bcc0db43c6e12fa3cc61f6341a36aba80ae95eeaf575a4292bad7a1960488f2"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-json"
-version = "0.20.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a9a38a9c679b55cc8d17350381ec08d69fa1a17a53fcf197f344516e485ed4d"
+checksum = "5b737dcb73c35d74b7d64a5f3dde158113c86a012bf3cee2bfdf2150d23b05db"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-kotlin"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8df217a0e1fec649f3e13157de932439f3d37ea4e265038dd0873971ef56e726"
+checksum = "c88dfbb22333118a5d5c5c10b19f93d115a6fa3c8a69dd0e6a260a64f9f5a79b"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-lua"
-version = "0.0.19"
+version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0968cf4962ead1d26da28921dde1fd97407e7bbcf2f959cd20cf04ba2daa9421"
+checksum = "3b9fe6fc87bd480e1943fc1fcb02453fb2da050e4e8ce0daa67d801544046856"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-php"
-version = "0.22.2"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7b46f2b021f0e1e51d4fd3b78bec588ce478b291c1affeb7e2acadda3b5fda5"
+checksum = "bcd2a1c0c0e32fe11b2cd96ef6b978ed366989c893e17f8af0f3b49beb4aaf5e"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-python"
-version = "0.20.4"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6c93b1b1fbd0d399db3445f51fd3058e43d0b4dcff62ddbdb46e66550978aa5"
+checksum = "b4066c6cf678f962f8c2c4561f205945c84834cce73d981e71392624fdc390a9"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-ruby"
-version = "0.20.1"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d50ef383469df8485f024c5fb01faced8cb90368192a7ba02605b43b2427fe"
+checksum = "c0031f687c0772f2dad7b77104c43428611099a1804c81244ada21560f41f0b1"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-rust"
-version = "0.20.4"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0832309b0b2b6d33760ce5c0e818cb47e1d72b468516bfe4134408926fa7594"
+checksum = "277690f420bf90741dea984f3da038ace46c4fe6047cba57a66822226cde1c93"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-scala"
-version = "0.20.3"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44fcf4628a88a3b5cbac3ff52658b924f3e545abddfa245ab9cf683c1adda350"
+checksum = "e4cb33e33a04b091b56541cf6663abba117cd2feefe2908e42cf9964d75a5edb"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-swift"
-version = "0.4.3"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e55ecb0372483057cb8f0f80c54d1cf76a3e301281d8db16d6c080e19395360f"
+checksum = "36b3097fc0b6a667acc2f54dd2d5a004ce85372397d8240354d3602863879089"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-typescript"
-version = "0.20.5"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8bc1d2c24276a48ef097a71b56888ac9db63717e8f8d0b324668a27fd619670"
+checksum = "f07523e51e3b88529360a89038c0cca7ee877db40a40141514eece8b4cddcbb4"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "unicode-bidi"
@@ -2107,17 +2113,17 @@
 name = "unicode-segmentation"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
@@ -2244,17 +2250,17 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "web-tree-sitter-sg"
-version = "1.3.4"
+version = "0.21.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9a450701853b465dddfd9edb45b5ab2ff191cd666d9f54382fad24fe6c5503a"
+checksum = "0034bb138c1702be373eb798c308c1ca4d7d4cfc7b60cfda9b4052cf1d41f634"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
  "wasm-bindgen-futures",
 ]
 
 [[package]]
@@ -2271,19 +2277,19 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
@@ -2299,15 +2305,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2319,116 +2325,123 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.6.5"
+version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dffa400e67ed5a4dd237983829e66475f0a4a26938c4b04c21baede6262215b8"
+checksum = "c3c52e9c97a68071b23e836c9380edae937f17b9c4667bd021973efc689f618d"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xtask"
 version = "0.0.0"
```

### Comparing `ast_grep_py-0.21.4/Cargo.toml` & `ast_grep_py-0.22.0/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 default-members = ["crates/*"]
 resolver = "2"
 
 [profile.release]
 lto = true
 
 [workspace.package]
-version = "0.21.4"
+version = "0.22.0"
 authors = ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition = "2021"
 license = "MIT"
 documentation = "https://ast-grep.github.io/guide/introduction.html"
 homepage = "https://ast-grep.github.io/"
 repository = "https://github.com/ast-grep/ast-grep"
 rust-version = "1.67"
 readme = "README.md"
 
 [workspace.dependencies]
-ast-grep-core = { path = "crates/core", version = "0.21.4" }
-ast-grep-config = { path = "crates/config", version = "0.21.4" }
-ast-grep-dynamic = { path = "crates/dynamic", version = "0.21.4" }
-ast-grep-language = { path = "crates/language", version = "0.21.4" }
-ast-grep-lsp = { path = "crates/lsp", version = "0.21.4" }
+ast-grep-core = { path = "crates/core", version = "0.22.0" }
+ast-grep-config = { path = "crates/config", version = "0.22.0" }
+ast-grep-dynamic = { path = "crates/dynamic", version = "0.22.0" }
+ast-grep-language = { path = "crates/language", version = "0.22.0" }
+ast-grep-lsp = { path = "crates/lsp", version = "0.22.0" }
 
 bit-set = { version = "0.5.3" }
 ignore = { version = "0.4.22" }
 regex = { version = "1.10.4" }
 serde = { version = "1.0.200", features = ["derive"] }
-tree-sitter = { version = "0.9.2", package = "tree-sitter-facade-sg" }
+tree-sitter = { version = "0.21.3", package = "tree-sitter-facade-sg" }
 thiserror = "1.0.59"
 schemars = "0.8.17"
 anyhow = "1.0.82"
```

### Comparing `ast_grep_py-0.21.4/pyproject.toml` & `ast_grep_py-0.22.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-py"
 requires-python = ">=3.8"
-version = "0.21.4"
+version = "0.22.0"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { text = "MIT" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_py-0.21.4/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.22.0/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/ast_grep_py/__init__.py` & `ast_grep_py-0.22.0/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/README.md` & `ast_grep_py-0.22.0/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.4/PKG-INFO` & `ast_grep_py-0.22.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ast-grep-py
-Version: 0.21.4
+Version: 0.22.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

