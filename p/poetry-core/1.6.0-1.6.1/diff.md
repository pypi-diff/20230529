# Comparing `tmp/poetry_core-1.6.0.tar.gz` & `tmp/poetry_core-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_core-1.6.0.tar", max compression
+gzip compressed data, was "poetry_core-1.6.1.tar", max compression
```

## Comparing `poetry_core-1.6.0.tar` & `poetry_core-1.6.1.tar`

### file list

```diff
@@ -1,555 +1,572 @@
--rw-r--r--   0        0        0     1062 2023-05-14 13:03:44.089980 poetry_core-1.6.0/LICENSE
--rw-r--r--   0        0        0     2392 2023-05-14 13:03:44.089980 poetry_core-1.6.0/README.md
--rw-r--r--   0        0        0     3362 2023-05-14 13:03:44.089980 poetry_core-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      394 2023-05-14 13:03:44.089980 poetry_core-1.6.0/src/poetry/core/__init__.py
--rw-r--r--   0        0        0       23 2023-05-14 13:03:44.089980 poetry_core-1.6.0/src/poetry/core/_vendor/_pyrsistent_version.py
--rw-r--r--   0        0        0     3241 2023-05-14 13:03:44.089980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/__init__.py
--rw-r--r--   0        0        0     4098 2023-05-14 13:03:44.089980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/_cmp.py
--rw-r--r--   0        0        0     5803 2023-05-14 13:03:44.089980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/_compat.py
--rw-r--r--   0        0        0      826 2023-05-14 13:03:44.089980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/_config.py
--rw-r--r--   0        0        0    16730 2023-05-14 13:03:44.089980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/_funcs.py
--rw-r--r--   0        0        0    96979 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/_make.py
--rw-r--r--   0        0        0     6271 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/_next_gen.py
--rw-r--r--   0        0        0     2121 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/_version_info.py
--rw-r--r--   0        0        0     3602 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/converters.py
--rw-r--r--   0        0        0     1890 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/exceptions.py
--rw-r--r--   0        0        0     1470 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/filters.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/py.typed
--rw-r--r--   0        0        0     1400 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/setters.py
--rw-r--r--   0        0        0    20702 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attr/validators.py
--rw-r--r--   0        0        0     1109 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attrs/LICENSE
--rw-r--r--   0        0        0     1039 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attrs/__init__.py
--rw-r--r--   0        0        0       70 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attrs/converters.py
--rw-r--r--   0        0        0       70 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attrs/exceptions.py
--rw-r--r--   0        0        0       67 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attrs/filters.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attrs/py.typed
--rw-r--r--   0        0        0       67 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attrs/setters.py
--rw-r--r--   0        0        0       70 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/attrs/validators.py
--rw-r--r--   0        0        0     1057 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/COPYING
--rw-r--r--   0        0        0     2187 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/__init__.py
--rw-r--r--   0        0        0       40 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/__main__.py
--rw-r--r--   0        0        0    14575 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/_format.py
--rw-r--r--   0        0        0    10549 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/_legacy_validators.py
--rw-r--r--   0        0        0     5425 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/_types.py
--rw-r--r--   0        0        0    10254 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/_utils.py
--rw-r--r--   0        0        0    15956 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/_validators.py
--rw-r--r--   0        0        0       70 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/benchmarks/__init__.py
--rw-r--r--   0        0        0   117105 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/benchmarks/issue232/issue.json
--rw-r--r--   0        0        0      506 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/benchmarks/issue232.py
--rw-r--r--   0        0        0      320 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/benchmarks/json_schema_test_suite.py
--rw-r--r--   0        0        0     8518 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/cli.py
--rw-r--r--   0        0        0    11336 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/exceptions.py
--rw-r--r--   0        0        0     7295 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/protocols.py
--rw-r--r--   0        0        0     1785 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft2019-09.json
--rw-r--r--   0        0        0     2452 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft2020-12.json
--rw-r--r--   0        0        0     2600 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft3.json
--rw-r--r--   0        0        0     4357 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft4.json
--rw-r--r--   0        0        0     4437 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft6.json
--rw-r--r--   0        0        0     4819 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft7.json
--rw-r--r--   0        0        0     1860 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/applicator
--rw-r--r--   0        0        0      517 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/content
--rw-r--r--   0        0        0     1531 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/core
--rw-r--r--   0        0        0      892 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/meta-data
--rw-r--r--   0        0        0     2834 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/validation
--rw-r--r--   0        0        0     1659 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/applicator
--rw-r--r--   0        0        0      519 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/content
--rw-r--r--   0        0        0     1564 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/core
--rw-r--r--   0        0        0      403 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format
--rw-r--r--   0        0        0      448 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format-annotation
--rw-r--r--   0        0        0      445 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format-assertion
--rw-r--r--   0        0        0      892 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/meta-data
--rw-r--r--   0        0        0      506 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/unevaluated
--rw-r--r--   0        0        0     2834 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/validation
--rw-r--r--   0        0        0    38171 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/validators.py
--rw-r--r--   0        0        0     1073 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/LICENSE
--rw-r--r--   0        0        0      744 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/__init__.py
--rw-r--r--   0        0        0      182 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      599 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py
--rw-r--r--   0        0        0     2092 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/ast_utils.py
--rw-r--r--   0        0        0     2814 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/common.py
--rw-r--r--   0        0        0    10940 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/exceptions.py
--rw-r--r--   0        0        0     3427 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/grammar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/grammars/__init__.py
--rw-r--r--   0        0        0      944 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/grammars/common.lark
--rw-r--r--   0        0        0     1467 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/grammars/lark.lark
--rw-r--r--   0        0        0    10995 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/grammars/python.lark
--rw-r--r--   0        0        0      103 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/grammars/unicode.lark
--rw-r--r--   0        0        0     3076 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/indenter.py
--rw-r--r--   0        0        0    27483 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/lark.py
--rw-r--r--   0        0        0    20633 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/lexer.py
--rw-r--r--   0        0        0    53453 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/load_grammar.py
--rw-r--r--   0        0        0    14112 2023-05-14 13:03:44.093980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parse_tree_builder.py
--rw-r--r--   0        0        0     9338 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parser_frontends.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/__init__.py
--rw-r--r--   0        0        0    12251 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/cyk.py
--rw-r--r--   0        0        0    13990 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/earley.py
--rw-r--r--   0        0        0     1581 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/earley_common.py
--rw-r--r--   0        0        0    31391 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/earley_forest.py
--rw-r--r--   0        0        0     6421 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/grammar_analysis.py
--rw-r--r--   0        0        0    10614 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/lalr_analysis.py
--rw-r--r--   0        0        0     5296 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/lalr_interactive_parser.py
--rw-r--r--   0        0        0     7216 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/lalr_parser.py
--rw-r--r--   0        0        0     2497 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/resolve_ambig.py
--rw-r--r--   0        0        0     7505 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/xearley.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/py.typed
--rw-r--r--   0        0        0     3728 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/reconstruct.py
--rw-r--r--   0        0        0     2319 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/tools/__init__.py
--rw-r--r--   0        0        0     6265 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/tools/nearley.py
--rw-r--r--   0        0        0     1014 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/tools/serialize.py
--rw-r--r--   0        0        0     5550 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/tools/standalone.py
--rw-r--r--   0        0        0     8178 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/tree.py
--rw-r--r--   0        0        0     6004 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/tree_matcher.py
--rw-r--r--   0        0        0     5958 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/tree_templates.py
--rw-r--r--   0        0        0    11089 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/utils.py
--rw-r--r--   0        0        0    21096 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/lark/visitors.py
--rw-r--r--   0        0        0      197 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      501 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8926 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0    10194 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/markers.py
--rw-r--r--   0        0        0    16397 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/metadata.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3287 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18106 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16326 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1060 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/LICENSE.mit
--rw-r--r--   0        0        0     1479 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/__init__.py
--rw-r--r--   0        0        0    18372 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_checked_types.py
--rw-r--r--   0        0        0    11963 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_field_common.py
--rw-r--r--   0        0        0     3232 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_helpers.py
--rw-r--r--   0        0        0     3287 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_immutable.py
--rw-r--r--   0        0        0     6730 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pbag.py
--rw-r--r--   0        0        0     9702 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pclass.py
--rw-r--r--   0        0        0    12203 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pdeque.py
--rw-r--r--   0        0        0     8293 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_plist.py
--rw-r--r--   0        0        0    18781 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pmap.py
--rw-r--r--   0        0        0     7032 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_precord.py
--rw-r--r--   0        0        0     5693 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pset.py
--rw-r--r--   0        0        0    22694 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pvector.py
--rw-r--r--   0        0        0     3425 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_toolz.py
--rw-r--r--   0        0        0     3800 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_transformations.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/py.typed
--rw-r--r--   0        0        0     1767 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/typing.py
--rw-r--r--   0        0        0     1072 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/tomli/LICENSE
--rw-r--r--   0        0        0      396 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-05-14 13:03:44.097980 poetry_core-1.6.0/src/poetry/core/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/_vendor/tomli/py.typed
--rw-r--r--   0        0        0    12787 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/_vendor/typing_extensions.LICENSE
--rw-r--r--   0        0        0    84065 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      489 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/_vendor/vendor.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/__init__.py
--rw-r--r--   0        0        0      719 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/generic/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/generic/any_constraint.py
--rw-r--r--   0        0        0     1109 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/generic/base_constraint.py
--rw-r--r--   0        0        0     4642 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/generic/constraint.py
--rw-r--r--   0        0        0     1151 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/generic/empty_constraint.py
--rw-r--r--   0        0        0     3948 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/generic/multi_constraint.py
--rw-r--r--   0        0        0     2036 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/generic/parser.py
--rw-r--r--   0        0        0     6672 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/generic/union_constraint.py
--rw-r--r--   0        0        0      954 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/__init__.py
--rw-r--r--   0        0        0     1416 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/empty_constraint.py
--rw-r--r--   0        0        0       86 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/exceptions.py
--rw-r--r--   0        0        0     7238 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/parser.py
--rw-r--r--   0        0        0      938 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/patterns.py
--rw-r--r--   0        0        0     1543 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/util.py
--rw-r--r--   0        0        0     5081 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/version.py
--rw-r--r--   0        0        0     3401 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/version_constraint.py
--rw-r--r--   0        0        0    15669 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/version_range.py
--rw-r--r--   0        0        0     3693 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/version_range_constraint.py
--rw-r--r--   0        0        0    10813 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/constraints/version/version_union.py
--rw-r--r--   0        0        0      133 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/exceptions/__init__.py
--rw-r--r--   0        0        0       84 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/exceptions/base.py
--rw-r--r--   0        0        0    17302 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/factory.py
--rw-r--r--   0        0        0      974 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/json/__init__.py
--rw-r--r--   0        0        0    18504 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/json/schemas/poetry-schema.json
--rw-r--r--   0        0        0      255 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/__init__.py
--rw-r--r--   0        0        0     2686 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/api.py
--rw-r--r--   0        0        0      994 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/builder.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/builders/__init__.py
--rw-r--r--   0        0        0    12900 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/builders/builder.py
--rw-r--r--   0        0        0    14996 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/builders/sdist.py
--rw-r--r--   0        0        0    14398 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/builders/wheel.py
--rw-r--r--   0        0        0     3012 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/metadata.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/utils/__init__.py
--rw-r--r--   0        0        0     3098 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/utils/helpers.py
--rw-r--r--   0        0        0     1100 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/utils/include.py
--rw-r--r--   0        0        0     3697 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/utils/module.py
--rw-r--r--   0        0        0     2662 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/masonry/utils/package_include.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/__init__.py
--rw-r--r--   0        0        0      930 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/constraints/__init__.py
--rw-r--r--   0        0        0    18354 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/dependency.py
--rw-r--r--   0        0        0     1479 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/dependency_group.py
--rw-r--r--   0        0        0     1814 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/directory_dependency.py
--rw-r--r--   0        0        0     1937 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/file_dependency.py
--rw-r--r--   0        0        0    21747 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/package.py
--rw-r--r--   0        0        0     2645 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/path_dependency.py
--rw-r--r--   0        0        0     2912 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/project_package.py
--rw-r--r--   0        0        0     6366 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/specification.py
--rw-r--r--   0        0        0     1597 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/url_dependency.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/utils/__init__.py
--rw-r--r--   0        0        0     6890 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/utils/link.py
--rw-r--r--   0        0        0    13656 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/utils/utils.py
--rw-r--r--   0        0        0     3119 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/packages/vcs_dependency.py
--rw-r--r--   0        0        0     1106 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/poetry.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/py.typed
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/pyproject/__init__.py
--rw-r--r--   0        0        0      149 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/pyproject/exceptions.py
--rw-r--r--   0        0        0     2127 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/pyproject/tables.py
--rw-r--r--   0        0        0     2304 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/pyproject/toml.py
--rw-r--r--   0        0        0      199 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/__init__.py
--rw-r--r--   0        0        0      129 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/empty_constraint.py
--rw-r--r--   0        0        0      150 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/exceptions.py
--rw-r--r--   0        0        0      239 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/helpers.py
--rw-r--r--   0        0        0      622 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/patterns.py
--rw-r--r--   0        0        0      135 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/util.py
--rw-r--r--   0        0        0      113 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/version.py
--rw-r--r--   0        0        0      133 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/version_constraint.py
--rw-r--r--   0        0        0      123 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/version_range.py
--rw-r--r--   0        0        0      143 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/version_range_constraint.py
--rw-r--r--   0        0        0      123 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/semver/version_union.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.101980 poetry_core-1.6.0/src/poetry/core/spdx/__init__.py
--rw-r--r--   0        0        0    30125 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/spdx/data/licenses.json
--rw-r--r--   0        0        0     1343 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/spdx/helpers.py
--rw-r--r--   0        0        0     5639 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/spdx/license.py
--rw-r--r--   0        0        0     1106 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/spdx/updater.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/utils/__init__.py
--rw-r--r--   0        0        0      417 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/utils/_compat.py
--rw-r--r--   0        0        0     3577 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/utils/helpers.py
--rw-r--r--   0        0        0      252 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/utils/patterns.py
--rw-r--r--   0        0        0      722 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/vcs/__init__.py
--rw-r--r--   0        0        0    11250 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/vcs/git.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/__init__.py
--rw-r--r--   0        0        0       80 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/exceptions.py
--rw-r--r--   0        0        0      214 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/grammars/__init__.py
--rw-r--r--   0        0        0      972 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/grammars/markers.lark
--rw-r--r--   0        0        0     1398 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/grammars/pep508.lark
--rw-r--r--   0        0        0     1601 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/helpers.py
--rw-r--r--   0        0        0    34345 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/markers.py
--rw-r--r--   0        0        0      752 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/parser.py
--rw-r--r--   0        0        0      352 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/pep440/__init__.py
--rw-r--r--   0        0        0     2864 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/pep440/parser.py
--rw-r--r--   0        0        0     5549 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/pep440/segments.py
--rw-r--r--   0        0        0    11383 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/pep440/version.py
--rw-r--r--   0        0        0     3381 2023-05-14 13:03:44.105980 poetry_core-1.6.0/src/poetry/core/version/requirements.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/__init__.py
--rw-r--r--   0        0        0     2687 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/generic/__init__.py
--rw-r--r--   0        0        0    13498 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/generic/test_constraint.py
--rw-r--r--   0        0        0     1800 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/generic/test_main.py
--rw-r--r--   0        0        0     1187 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/generic/test_multi_constraint.py
--rw-r--r--   0        0        0     1169 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/generic/test_union_constraint.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/version/__init__.py
--rw-r--r--   0        0        0    13388 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/version/test_helpers.py
--rw-r--r--   0        0        0     8288 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/version/test_parse_constraint.py
--rw-r--r--   0        0        0     2925 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/version/test_utils.py
--rw-r--r--   0        0        0    17763 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/version/test_version.py
--rw-r--r--   0        0        0      943 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/version/test_version_constraint.py
--rw-r--r--   0        0        0    23674 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/version/test_version_range.py
--rw-r--r--   0        0        0     4901 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/constraints/version/test_version_union.py
--rw-r--r--   0        0        0     1329 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/complete.toml
--rw-r--r--   0        0        0     1717 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/distributions/demo-0.1.0-in-subdir.zip
--rw-r--r--   0        0        0     1116 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0      961 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/distributions/demo-0.1.0.tar.gz
--rw-r--r--   0        0        0      209 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/invalid_pyproject/pyproject.toml
--rw-r--r--   0        0        0      110 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/pep_517_backend/README.md
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/pep_517_backend/foo/__init__.py
--rw-r--r--   0        0        0     1190 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/pep_517_backend/pyproject.toml
--rw-r--r--   0        0        0      634 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_failing_strict_validation/pyproject.toml
--rw-r--r--   0        0        0      407 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_build_system_requires/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_dependencies_with_subdirectory/README.rst
--rw-r--r--   0        0        0     1231 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_dependencies_with_subdirectory/pyproject.toml
--rw-r--r--   0        0        0      611 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_duplicated_classifiers/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_groups_and_explicit_main/README.rst
--rw-r--r--   0        0        0      326 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_groups_and_explicit_main/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_groups_and_explicit_main/simple_project/__init__.py
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_groups_and_legacy_dev/README.rst
--rw-r--r--   0        0        0      376 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_groups_and_legacy_dev/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_groups_and_legacy_dev/simple_project/__init__.py
--rw-r--r--   0        0        0      278 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_invalid_dev_deps/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_markers_and_extras/project/__init__.py
--rw-r--r--   0        0        0      602 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_markers_and_extras/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_multi_constraints_dependency/project/__init__.py
--rw-r--r--   0        0        0      394 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_multi_constraints_dependency/pyproject.toml
--rw-r--r--   0        0        0      255 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_pep517_non_poetry/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_setup/my_package/__init__.py
--rw-r--r--   0        0        0      346 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_setup/setup.py
--rw-r--r--   0        0        0      444 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/project_with_setup_cfg_only/setup.cfg
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/sample_project/README.rst
--rw-r--r--   0        0        0     2261 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/sample_project/pyproject.toml
--rw-r--r--   0        0        0       83 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/script-files/sample_script.py
--rw-r--r--   0        0        0       41 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/script-files/sample_script.sh
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/simple_project/README.rst
--rw-r--r--   0        0        0     1320 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1106 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz
--rw-r--r--   0        0        0      590 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/simple_project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/simple_project/simple_project/__init__.py
--rw-r--r--   0        0        0       28 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/with_readme_files/README-1.rst
--rw-r--r--   0        0        0       20 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/with_readme_files/README-2.rst
--rw-r--r--   0        0        0       79 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/with_readme_files/my_package/__init__.py
--rw-r--r--   0        0        0      300 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/fixtures/with_readme_files/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     2721 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/integration/test_pep517.py
--rw-r--r--   0        0        0     1503 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/integration/test_pep517_backend.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/json/__init__.py
--rw-r--r--   0        0        0     2277 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/json/test_poetry_schema.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/__init__.py
--rw-r--r--   0        0        0      294 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/build_script_in_subdir/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/build_script_in_subdir/scripts/build.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/build_script_in_subdir/src/foo.py
--rw-r--r--   0        0        0     1062 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/LICENSE
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/README.rst
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/Bar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/IncludedBar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/SecondBar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/lowercasebar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/FooBar/Bar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/FooBar/lowercasebar.py
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.105980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/bar/CapitalFoo.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/bar/foo.py
--rw-r--r--   0        0        0     1160 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/comma_file/comma_file/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/comma_file/comma_file/a,b.py
--rw-r--r--   0        0        0      224 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/comma_file/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/LICENSE
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/README.rst
--rw-r--r--   0        0        0       40 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/bin/script.sh
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/my_package/__init__.py
--rw-r--r--   0        0        0        3 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/my_package/data1/test.json
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/my_package/sub_pkg1/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/my_package/sub_pkg1/extra_file.xml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/my_package/sub_pkg2/__init__.py
--rw-r--r--   0        0        0        3 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/my_package/sub_pkg2/data2/data.json
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/my_package/sub_pkg3/foo.py
--rw-r--r--   0        0        0     1348 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_src_with_excluded_data/LICENSE
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_src_with_excluded_data/README.rst
--rw-r--r--   0        0        0      874 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_src_with_excluded_data/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/data1.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/sub_data/data2.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/sub_data/data3.txt
--rw-r--r--   0        0        0     1062 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data/LICENSE
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data/README.rst
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/data1.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/sub_data/data2.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/sub_data/data3.txt
--rw-r--r--   0        0        0      874 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data_toml/LICENSE
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data_toml/README.rst
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/data1.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/sub_data/data2.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/sub_data/data3.txt
--rw-r--r--   0        0        0      915 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data_toml/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/disable_setup_py/README.rst
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/disable_setup_py/my_package/__init__.py
--rw-r--r--   0        0        0      740 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/disable_setup_py/pyproject.toml
--rw-r--r--   0        0        0       12 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/epoch/README.rst
--rw-r--r--   0        0        0       44 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/epoch/epoch.py
--rw-r--r--   0        0        0      223 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/epoch/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/compiled/source.c
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/compiled/source.h
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/cython_code.pyx
--rw-r--r--   0        0        0      474 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude-whl-include-sdist/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/LICENSE
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/README.rst
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/data1.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/data2.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/sub_data/data2.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/sub_data/data3.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item1/itemdata1.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item1/subitem/subitemdata.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item2/itemdata2.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/publicdata.txt
--rw-r--r--   0        0        0      952 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/pyproject.toml
--rw-r--r--   0        0        0       21 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/excluded_subpackage/README.rst
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/excluded_subpackage/example/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/excluded_subpackage/example/test/__init__.py
--rw-r--r--   0        0        0      148 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/excluded_subpackage/example/test/excluded.py
--rw-r--r--   0        0        0      329 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/excluded_subpackage/pyproject.toml
--rw-r--r--   0        0        0       18 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended/README.rst
--rw-r--r--   0        0        0      186 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended/build.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended/extended/__init__.py
--rw-r--r--   0        0        0      888 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended/extended/extended.c
--rw-r--r--   0        0        0      292 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended/pyproject.toml
--rw-r--r--   0        0        0      539 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended/setup.py
--rw-r--r--   0        0        0       18 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended_with_no_setup/README.rst
--rw-r--r--   0        0        0      753 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended_with_no_setup/build.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended_with_no_setup/extended/__init__.py
--rw-r--r--   0        0        0      888 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended_with_no_setup/extended/extended.c
--rw-r--r--   0        0        0      293 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/extended_with_no_setup/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/include_excluded_code/lib/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/include_excluded_code/lib/my_package/generated.py
--rw-r--r--   0        0        0      485 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/include_excluded_code/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/LICENSE
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/README.rst
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Bar/foo/bar/Foo.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/Bar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/IncludedBar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/SecondBar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/lowercasebar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/FooBar/Bar.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/FooBar/lowercasebar.py
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/__init__.py
--rw-r--r--   0        0        0     1011 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/COPYING
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/COPYING.txt
--rw-r--r--   0        0        0     1062 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE.md
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/BSD-3.md
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/CUSTOM-LICENSE
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/MIT.txt
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/README.rst
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/my_package/__init__.py
--rw-r--r--   0        0        0     1231 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/pyproject.toml
--rw-r--r--   0        0        0       74 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/localversionlabel/localversionlabel.py
--rw-r--r--   0        0        0      133 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/localversionlabel/pyproject.toml
--rw-r--r--   0        0        0       18 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/module1/README.rst
--rw-r--r--   0        0        0       42 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/module1/module1.py
--rw-r--r--   0        0        0      265 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/module1/pyproject.toml
--rw-r--r--   0        0        0      261 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/pep_561_stub_only/pyproject.toml
--rw-r--r--   0        0        0        8 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/py.typed
--rw-r--r--   0        0        0      291 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pyproject.toml
--rw-r--r--   0        0        0        8 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/pep_561_stub_only_partial_namespace/pkg-stubs/subpkg/py.typed
--rw-r--r--   0        0        0      306 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/pep_561_stub_only_partial_namespace/pyproject.toml
--rw-r--r--   0        0        0      294 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/pep_561_stub_only_src/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/prerelease/README.rst
--rw-r--r--   0        0        0       42 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/prerelease/prerelease.py
--rw-r--r--   0        0        0      233 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/prerelease/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.109980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_callable_legacy_string/README.rst
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_callable_legacy_string/my_package/__init__.py
--rw-r--r--   0        0        0      346 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_callable_legacy_string/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_callable_legacy_table/README.rst
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_callable_legacy_table/my_package/__init__.py
--rw-r--r--   0        0        0      471 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_callable_legacy_table/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_console/README.rst
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_console/my_package/__init__.py
--rw-r--r--   0        0        0      481 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_console/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file/README.rst
--rw-r--r--   0        0        0       40 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file/bin/script.sh
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file/my_package/__init__.py
--rw-r--r--   0        0        0      371 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/README.rst
--rw-r--r--   0        0        0       40 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/bin/script.sh
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/my_package/__init__.py
--rw-r--r--   0        0        0      384 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file_missing/README.rst
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file_missing/my_package/__init__.py
--rw-r--r--   0        0        0      371 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/script_reference_file_missing/pyproject.toml
--rw-r--r--   0        0        0       18 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/simple_version/README.rst
--rw-r--r--   0        0        0      217 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/simple_version/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/simple_version/simple_version.py
--rw-r--r--   0        0        0       28 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/single_python/README.rst
--rw-r--r--   0        0        0      276 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/single_python/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/single_python/single_python.py
--rw-r--r--   0        0        0       18 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/source_file/README.rst
--rw-r--r--   0        0        0      268 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/source_file/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/source_file/src/module_src.py
--rw-r--r--   0        0        0       18 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/source_package/README.rst
--rw-r--r--   0        0        0      268 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/source_package/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/source_package/src/package_src/__init__.py
--rw-r--r--   0        0        0       42 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/source_package/src/package_src/module.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/split_source/lib_a/module_a/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/split_source/lib_b/module_b/__init__.py
--rw-r--r--   0        0        0      331 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/split_source/pyproject.toml
--rw-r--r--   0        0        0       18 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/src_extended/README.rst
--rw-r--r--   0        0        0      190 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/src_extended/build.py
--rw-r--r--   0        0        0      292 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/src_extended/pyproject.toml
--rw-r--r--   0        0        0      598 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/src_extended/setup.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/src_extended/src/extended/__init__.py
--rw-r--r--   0        0        0      888 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/src_extended/src/extended/extended.c
--rw-r--r--   0        0        0     1062 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/LICENSE
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/README.rst
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/extra_dir/README.md
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/extra_dir/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/extra_dir/sub_pkg/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/extra_dir/sub_pkg/vcs_excluded.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/extra_dir/vcs_excluded.txt
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/for_wheel_only/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/my_module.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/notes.txt
--rw-r--r--   0        0        0       22 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/package_with_include/__init__.py
--rw-r--r--   0        0        0     1259 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/src/src_package/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/tests/__init__.py
--rw-r--r--   0        0        0      238 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_bad_path_dep/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_bad_path_dep/with_bad_path_dep/__init__.py
--rw-r--r--   0        0        0      274 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_bad_path_dev_dep/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_bad_path_dev_dep/with_bad_path_dev_dep/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_include_inline_table/both.txt
--rw-r--r--   0        0        0     1050 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_include_inline_table/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_include_inline_table/src/src_package/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_include_inline_table/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_include_inline_table/tests/test_foo/test.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_include_inline_table/wheel_only.txt
--rw-r--r--   0        0        0      656 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_url_dependency/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_url_dependency/with_url_dependency/__init__.py
--rw-r--r--   0        0        0      641 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_vcs_dependency/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_vcs_dependency/with_vcs_dependency/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_wildcard_dependency_constraint/my_package/__init__.py
--rw-r--r--   0        0        0      236 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/fixtures/with_wildcard_dependency_constraint/pyproject.toml
--rw-r--r--   0        0        0     8986 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/test_builder.py
--rw-r--r--   0        0        0    12699 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/test_complete.py
--rw-r--r--   0        0        0    20450 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/test_sdist.py
--rw-r--r--   0        0        0    11300 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/builders/test_wheel.py
--rw-r--r--   0        0        0    10211 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/test_api.py
--rw-r--r--   0        0        0     2202 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/test_builder.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/utils/__init__.py
--rw-r--r--   0        0        0        8 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/utils/fixtures/pep_561_stub_only_partial_namespace/good-stubs/subpkg/py.typed
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/utils/fixtures/with_includes/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/utils/fixtures/with_includes/bar/baz.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/utils/fixtures/with_includes/extra_package/some_dir/foo.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/utils/fixtures/with_includes/extra_package/some_dir/quux.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/utils/fixtures/with_includes/not_a_python_pkg/baz.txt
--rw-r--r--   0        0        0      530 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/utils/test_helpers.py
--rw-r--r--   0        0        0     3047 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/masonry/utils/test_package_include.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/__init__.py
--rw-r--r--   0        0        0    13625 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/test_dependency.py
--rw-r--r--   0        0        0      948 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/test_dependency_group.py
--rw-r--r--   0        0        0     6439 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/test_directory_dependency.py
--rw-r--r--   0        0        0     8783 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/test_file_dependency.py
--rw-r--r--   0        0        0    10840 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/test_main.py
--rw-r--r--   0        0        0    20553 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/test_package.py
--rw-r--r--   0        0        0     3814 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/test_specification.py
--rw-r--r--   0        0        0     2588 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/test_url_dependency.py
--rw-r--r--   0        0        0     5052 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/test_vcs_dependency.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/utils/__init__.py
--rw-r--r--   0        0        0     9279 2023-05-14 13:03:44.113980 poetry_core-1.6.0/tests/packages/utils/test_utils.py
--rw-r--r--   0        0        0     3929 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/packages/utils/test_utils_link.py
--rw-r--r--   0        0        0     2248 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/packages/utils/test_utils_urls.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/pyproject/__init__.py
--rw-r--r--   0        0        0      813 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/pyproject/conftest.py
--rw-r--r--   0        0        0     2373 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/pyproject/test_pyproject_toml.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/spdx/__init__.py
--rw-r--r--   0        0        0     1413 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/spdx/test_helpers.py
--rw-r--r--   0        0        0     1497 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/spdx/test_license.py
--rw-r--r--   0        0        0      343 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/test_core_version.py
--rw-r--r--   0        0        0    17197 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/test_factory.py
--rw-r--r--   0        0        0     2721 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/testutils.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     5913 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/utils/test_helpers.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/vcs/__init__.py
--rw-r--r--   0        0        0    15077 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/vcs/test_vcs.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/version/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/version/pep440/__init__.py
--rw-r--r--   0        0        0     5298 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/version/pep440/test_segments.py
--rw-r--r--   0        0        0    14354 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/version/pep440/test_version.py
--rw-r--r--   0        0        0    66656 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/version/test_markers.py
--rw-r--r--   0        0        0     4452 2023-05-14 13:03:44.117980 poetry_core-1.6.0/tests/version/test_requirements.py
--rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 poetry_core-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-29 08:06:23.979418 poetry_core-1.6.1/LICENSE
+-rw-r--r--   0        0        0     2392 2023-05-29 08:06:23.979418 poetry_core-1.6.1/README.md
+-rw-r--r--   0        0        0     3287 2023-05-29 08:06:23.979418 poetry_core-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      394 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/_pyrsistent_version.py
+-rw-r--r--   0        0        0     3241 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/__init__.py
+-rw-r--r--   0        0        0     4098 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/_cmp.py
+-rw-r--r--   0        0        0     5803 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/_compat.py
+-rw-r--r--   0        0        0      826 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/_config.py
+-rw-r--r--   0        0        0    16730 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/_funcs.py
+-rw-r--r--   0        0        0    96979 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/_make.py
+-rw-r--r--   0        0        0     6271 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/_next_gen.py
+-rw-r--r--   0        0        0     2121 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/_version_info.py
+-rw-r--r--   0        0        0     3602 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/converters.py
+-rw-r--r--   0        0        0     1890 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/exceptions.py
+-rw-r--r--   0        0        0     1470 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/filters.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/py.typed
+-rw-r--r--   0        0        0     1400 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/setters.py
+-rw-r--r--   0        0        0    20702 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attr/validators.py
+-rw-r--r--   0        0        0     1109 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attrs/LICENSE
+-rw-r--r--   0        0        0     1039 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attrs/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attrs/converters.py
+-rw-r--r--   0        0        0       70 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attrs/exceptions.py
+-rw-r--r--   0        0        0       67 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attrs/filters.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attrs/py.typed
+-rw-r--r--   0        0        0       67 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attrs/setters.py
+-rw-r--r--   0        0        0       70 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/attrs/validators.py
+-rw-r--r--   0        0        0     1057 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/COPYING
+-rw-r--r--   0        0        0     2187 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/__main__.py
+-rw-r--r--   0        0        0    14575 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/_format.py
+-rw-r--r--   0        0        0    10549 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/_legacy_validators.py
+-rw-r--r--   0        0        0     5425 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/_types.py
+-rw-r--r--   0        0        0    10254 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/_utils.py
+-rw-r--r--   0        0        0    15956 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/_validators.py
+-rw-r--r--   0        0        0       70 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/benchmarks/__init__.py
+-rw-r--r--   0        0        0   117105 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/benchmarks/issue232/issue.json
+-rw-r--r--   0        0        0      506 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/benchmarks/issue232.py
+-rw-r--r--   0        0        0      320 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/benchmarks/json_schema_test_suite.py
+-rw-r--r--   0        0        0     8518 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/cli.py
+-rw-r--r--   0        0        0    11336 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/exceptions.py
+-rw-r--r--   0        0        0     7295 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/protocols.py
+-rw-r--r--   0        0        0     1785 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft2019-09.json
+-rw-r--r--   0        0        0     2452 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft2020-12.json
+-rw-r--r--   0        0        0     2600 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft3.json
+-rw-r--r--   0        0        0     4357 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft4.json
+-rw-r--r--   0        0        0     4437 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft6.json
+-rw-r--r--   0        0        0     4819 2023-05-29 08:06:23.979418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft7.json
+-rw-r--r--   0        0        0     1860 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/applicator
+-rw-r--r--   0        0        0      517 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/content
+-rw-r--r--   0        0        0     1531 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/core
+-rw-r--r--   0        0        0      892 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/meta-data
+-rw-r--r--   0        0        0     2834 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/validation
+-rw-r--r--   0        0        0     1659 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/applicator
+-rw-r--r--   0        0        0      519 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/content
+-rw-r--r--   0        0        0     1564 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/core
+-rw-r--r--   0        0        0      403 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format
+-rw-r--r--   0        0        0      448 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format-annotation
+-rw-r--r--   0        0        0      445 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format-assertion
+-rw-r--r--   0        0        0      892 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/meta-data
+-rw-r--r--   0        0        0      506 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/unevaluated
+-rw-r--r--   0        0        0     2834 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/validation
+-rw-r--r--   0        0        0    38171 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/validators.py
+-rw-r--r--   0        0        0     1073 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/LICENSE
+-rw-r--r--   0        0        0      744 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py
+-rw-r--r--   0        0        0     2092 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/ast_utils.py
+-rw-r--r--   0        0        0     2814 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/common.py
+-rw-r--r--   0        0        0    10940 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/exceptions.py
+-rw-r--r--   0        0        0     3427 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/grammar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/grammars/__init__.py
+-rw-r--r--   0        0        0      944 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/grammars/common.lark
+-rw-r--r--   0        0        0     1467 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/grammars/lark.lark
+-rw-r--r--   0        0        0    10995 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/grammars/python.lark
+-rw-r--r--   0        0        0      103 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/grammars/unicode.lark
+-rw-r--r--   0        0        0     3076 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/indenter.py
+-rw-r--r--   0        0        0    27483 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/lark.py
+-rw-r--r--   0        0        0    20633 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/lexer.py
+-rw-r--r--   0        0        0    53453 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/load_grammar.py
+-rw-r--r--   0        0        0    14112 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parse_tree_builder.py
+-rw-r--r--   0        0        0     9338 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parser_frontends.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/__init__.py
+-rw-r--r--   0        0        0    12251 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/cyk.py
+-rw-r--r--   0        0        0    13990 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/earley.py
+-rw-r--r--   0        0        0     1581 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/earley_common.py
+-rw-r--r--   0        0        0    31391 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/earley_forest.py
+-rw-r--r--   0        0        0     6421 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/grammar_analysis.py
+-rw-r--r--   0        0        0    10614 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/lalr_analysis.py
+-rw-r--r--   0        0        0     5296 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/lalr_interactive_parser.py
+-rw-r--r--   0        0        0     7216 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/lalr_parser.py
+-rw-r--r--   0        0        0     2497 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/resolve_ambig.py
+-rw-r--r--   0        0        0     7505 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/xearley.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/py.typed
+-rw-r--r--   0        0        0     3728 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/reconstruct.py
+-rw-r--r--   0        0        0     2319 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/tools/__init__.py
+-rw-r--r--   0        0        0     6265 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/tools/nearley.py
+-rw-r--r--   0        0        0     1014 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/tools/serialize.py
+-rw-r--r--   0        0        0     5550 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/tools/standalone.py
+-rw-r--r--   0        0        0     8178 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/tree.py
+-rw-r--r--   0        0        0     6004 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/tree_matcher.py
+-rw-r--r--   0        0        0     5958 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/tree_templates.py
+-rw-r--r--   0        0        0    11089 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/utils.py
+-rw-r--r--   0        0        0    21096 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/lark/visitors.py
+-rw-r--r--   0        0        0      197 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      501 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2023-05-29 08:06:23.983418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3287 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1060 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/LICENSE.mit
+-rw-r--r--   0        0        0     1479 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/__init__.py
+-rw-r--r--   0        0        0    18372 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_checked_types.py
+-rw-r--r--   0        0        0    11963 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_field_common.py
+-rw-r--r--   0        0        0     3232 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_helpers.py
+-rw-r--r--   0        0        0     3287 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_immutable.py
+-rw-r--r--   0        0        0     6730 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pbag.py
+-rw-r--r--   0        0        0     9702 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pclass.py
+-rw-r--r--   0        0        0    12203 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pdeque.py
+-rw-r--r--   0        0        0     8293 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_plist.py
+-rw-r--r--   0        0        0    18781 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pmap.py
+-rw-r--r--   0        0        0     7032 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_precord.py
+-rw-r--r--   0        0        0     5693 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pset.py
+-rw-r--r--   0        0        0    22694 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pvector.py
+-rw-r--r--   0        0        0     3425 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_toolz.py
+-rw-r--r--   0        0        0     3800 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_transformations.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/py.typed
+-rw-r--r--   0        0        0     1767 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/typing.py
+-rw-r--r--   0        0        0     1072 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/tomli/LICENSE
+-rw-r--r--   0        0        0      396 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0    12787 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/typing_extensions.LICENSE
+-rw-r--r--   0        0        0    84065 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      489 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/_vendor/vendor.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/generic/__init__.py
+-rw-r--r--   0        0        0     1236 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/generic/any_constraint.py
+-rw-r--r--   0        0        0     1109 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/generic/base_constraint.py
+-rw-r--r--   0        0        0     4642 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/generic/constraint.py
+-rw-r--r--   0        0        0     1151 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/generic/empty_constraint.py
+-rw-r--r--   0        0        0     4405 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/generic/multi_constraint.py
+-rw-r--r--   0        0        0     2036 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/generic/parser.py
+-rw-r--r--   0        0        0     6672 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/generic/union_constraint.py
+-rw-r--r--   0        0        0      954 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/__init__.py
+-rw-r--r--   0        0        0     1416 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/empty_constraint.py
+-rw-r--r--   0        0        0       86 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/exceptions.py
+-rw-r--r--   0        0        0     7238 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/parser.py
+-rw-r--r--   0        0        0      938 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/patterns.py
+-rw-r--r--   0        0        0     1543 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/util.py
+-rw-r--r--   0        0        0     5081 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/version.py
+-rw-r--r--   0        0        0     3401 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/version_constraint.py
+-rw-r--r--   0        0        0    15669 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/version_range.py
+-rw-r--r--   0        0        0     3693 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/version_range_constraint.py
+-rw-r--r--   0        0        0    10813 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/constraints/version/version_union.py
+-rw-r--r--   0        0        0      133 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/exceptions/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/exceptions/base.py
+-rw-r--r--   0        0        0    17302 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/factory.py
+-rw-r--r--   0        0        0      974 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/json/__init__.py
+-rw-r--r--   0        0        0    18504 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/json/schemas/poetry-schema.json
+-rw-r--r--   0        0        0      255 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/masonry/__init__.py
+-rw-r--r--   0        0        0     2686 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/masonry/api.py
+-rw-r--r--   0        0        0      994 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/masonry/builder.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.987418 poetry_core-1.6.1/src/poetry/core/masonry/builders/__init__.py
+-rw-r--r--   0        0        0    12900 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/masonry/builders/builder.py
+-rw-r--r--   0        0        0    14996 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/masonry/builders/sdist.py
+-rw-r--r--   0        0        0    15941 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/masonry/builders/wheel.py
+-rw-r--r--   0        0        0     3012 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/masonry/metadata.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/masonry/utils/__init__.py
+-rw-r--r--   0        0        0     3098 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/masonry/utils/helpers.py
+-rw-r--r--   0        0        0     1100 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/masonry/utils/include.py
+-rw-r--r--   0        0        0     3697 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/masonry/utils/module.py
+-rw-r--r--   0        0        0     2662 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/masonry/utils/package_include.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/constraints/__init__.py
+-rw-r--r--   0        0        0    18354 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/dependency.py
+-rw-r--r--   0        0        0     1479 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/dependency_group.py
+-rw-r--r--   0        0        0     1814 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/directory_dependency.py
+-rw-r--r--   0        0        0     1937 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/file_dependency.py
+-rw-r--r--   0        0        0    21747 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/package.py
+-rw-r--r--   0        0        0     2645 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/path_dependency.py
+-rw-r--r--   0        0        0     2912 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/project_package.py
+-rw-r--r--   0        0        0     6366 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/specification.py
+-rw-r--r--   0        0        0     1597 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/url_dependency.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/utils/__init__.py
+-rw-r--r--   0        0        0     6890 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/utils/link.py
+-rw-r--r--   0        0        0    13656 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/utils/utils.py
+-rw-r--r--   0        0        0     3119 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/packages/vcs_dependency.py
+-rw-r--r--   0        0        0     1106 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/poetry.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/py.typed
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/pyproject/__init__.py
+-rw-r--r--   0        0        0      149 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/pyproject/exceptions.py
+-rw-r--r--   0        0        0     2127 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/pyproject/tables.py
+-rw-r--r--   0        0        0     2304 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/pyproject/toml.py
+-rw-r--r--   0        0        0      199 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/empty_constraint.py
+-rw-r--r--   0        0        0      150 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/exceptions.py
+-rw-r--r--   0        0        0      239 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/helpers.py
+-rw-r--r--   0        0        0      622 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/patterns.py
+-rw-r--r--   0        0        0      135 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/util.py
+-rw-r--r--   0        0        0      113 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/version.py
+-rw-r--r--   0        0        0      133 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/version_constraint.py
+-rw-r--r--   0        0        0      123 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/version_range.py
+-rw-r--r--   0        0        0      143 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/version_range_constraint.py
+-rw-r--r--   0        0        0      123 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/semver/version_union.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/spdx/__init__.py
+-rw-r--r--   0        0        0    30125 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/spdx/data/licenses.json
+-rw-r--r--   0        0        0     1343 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/spdx/helpers.py
+-rw-r--r--   0        0        0     5639 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/spdx/license.py
+-rw-r--r--   0        0        0     1106 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/spdx/updater.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/utils/__init__.py
+-rw-r--r--   0        0        0      417 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/utils/_compat.py
+-rw-r--r--   0        0        0     4001 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/utils/helpers.py
+-rw-r--r--   0        0        0      252 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/utils/patterns.py
+-rw-r--r--   0        0        0      722 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/vcs/__init__.py
+-rw-r--r--   0        0        0    11250 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/vcs/git.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/__init__.py
+-rw-r--r--   0        0        0       80 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/exceptions.py
+-rw-r--r--   0        0        0      214 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/grammars/__init__.py
+-rw-r--r--   0        0        0      972 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/grammars/markers.lark
+-rw-r--r--   0        0        0     1398 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/grammars/pep508.lark
+-rw-r--r--   0        0        0     1601 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/helpers.py
+-rw-r--r--   0        0        0    34345 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/markers.py
+-rw-r--r--   0        0        0      752 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/parser.py
+-rw-r--r--   0        0        0      352 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/pep440/__init__.py
+-rw-r--r--   0        0        0     2864 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/pep440/parser.py
+-rw-r--r--   0        0        0     5549 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/pep440/segments.py
+-rw-r--r--   0        0        0    11383 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/pep440/version.py
+-rw-r--r--   0        0        0     3381 2023-05-29 08:06:23.991418 poetry_core-1.6.1/src/poetry/core/version/requirements.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     2687 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/generic/__init__.py
+-rw-r--r--   0        0        0    14104 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/generic/test_constraint.py
+-rw-r--r--   0        0        0     1800 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/generic/test_main.py
+-rw-r--r--   0        0        0     1187 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/generic/test_multi_constraint.py
+-rw-r--r--   0        0        0     1169 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/generic/test_union_constraint.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/version/__init__.py
+-rw-r--r--   0        0        0    13388 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/version/test_helpers.py
+-rw-r--r--   0        0        0     8288 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/version/test_parse_constraint.py
+-rw-r--r--   0        0        0     2925 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/version/test_utils.py
+-rw-r--r--   0        0        0    17763 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/version/test_version.py
+-rw-r--r--   0        0        0      943 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/version/test_version_constraint.py
+-rw-r--r--   0        0        0    23674 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/version/test_version_range.py
+-rw-r--r--   0        0        0     4901 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/constraints/version/test_version_union.py
+-rw-r--r--   0        0        0     1329 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/fixtures/complete.toml
+-rw-r--r--   0        0        0     1717 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/fixtures/distributions/demo-0.1.0-in-subdir.zip
+-rw-r--r--   0        0        0     1116 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      961 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/fixtures/distributions/demo-0.1.0.tar.gz
+-rw-r--r--   0        0        0      209 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/fixtures/invalid_pyproject/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/fixtures/pep_517_backend/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/fixtures/pep_517_backend/foo/__init__.py
+-rw-r--r--   0        0        0     1190 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/fixtures/pep_517_backend/pyproject.toml
+-rw-r--r--   0        0        0      634 2023-05-29 08:06:23.991418 poetry_core-1.6.1/tests/fixtures/project_failing_strict_validation/pyproject.toml
+-rw-r--r--   0        0        0      407 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_build_system_requires/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_dependencies_with_subdirectory/README.rst
+-rw-r--r--   0        0        0     1231 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_dependencies_with_subdirectory/pyproject.toml
+-rw-r--r--   0        0        0      611 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_duplicated_classifiers/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_groups_and_explicit_main/README.rst
+-rw-r--r--   0        0        0      326 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_groups_and_explicit_main/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_groups_and_explicit_main/simple_project/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_groups_and_legacy_dev/README.rst
+-rw-r--r--   0        0        0      376 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_groups_and_legacy_dev/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_groups_and_legacy_dev/simple_project/__init__.py
+-rw-r--r--   0        0        0      278 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_invalid_dev_deps/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_markers_and_extras/project/__init__.py
+-rw-r--r--   0        0        0      602 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_markers_and_extras/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_multi_constraints_dependency/project/__init__.py
+-rw-r--r--   0        0        0      394 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_multi_constraints_dependency/pyproject.toml
+-rw-r--r--   0        0        0      255 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_pep517_non_poetry/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_setup/my_package/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_setup/setup.py
+-rw-r--r--   0        0        0      444 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/project_with_setup_cfg_only/setup.cfg
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/sample_project/README.rst
+-rw-r--r--   0        0        0     2261 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/sample_project/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/script-files/sample_script.py
+-rw-r--r--   0        0        0       41 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/script-files/sample_script.sh
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/simple_project/README.rst
+-rw-r--r--   0        0        0     1320 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1106 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz
+-rw-r--r--   0        0        0      590 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/simple_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/simple_project/simple_project/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/with_readme_files/README-1.rst
+-rw-r--r--   0        0        0       20 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/with_readme_files/README-2.rst
+-rw-r--r--   0        0        0       79 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/with_readme_files/my_package/__init__.py
+-rw-r--r--   0        0        0      300 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/fixtures/with_readme_files/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2721 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/integration/test_pep517.py
+-rw-r--r--   0        0        0     1503 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/integration/test_pep517_backend.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/json/__init__.py
+-rw-r--r--   0        0        0     2277 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/json/test_poetry_schema.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/__init__.py
+-rw-r--r--   0        0        0      294 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/build_script_in_subdir/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/build_script_in_subdir/scripts/build.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/build_script_in_subdir/src/foo.py
+-rw-r--r--   0        0        0     1062 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/README.rst
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/Bar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/IncludedBar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/SecondBar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/lowercasebar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/FooBar/Bar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/FooBar/lowercasebar.py
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/bar/CapitalFoo.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/bar/foo.py
+-rw-r--r--   0        0        0     1160 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/comma_file/comma_file/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/comma_file/comma_file/a,b.py
+-rw-r--r--   0        0        0      224 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/comma_file/pyproject.toml
+-rw-r--r--   0        0        0     1062 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/README.rst
+-rw-r--r--   0        0        0       40 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/bin/script.sh
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/my_package/__init__.py
+-rw-r--r--   0        0        0        3 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/my_package/data1/test.json
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/my_package/sub_pkg1/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/my_package/sub_pkg1/extra_file.xml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/my_package/sub_pkg2/__init__.py
+-rw-r--r--   0        0        0        3 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/my_package/sub_pkg2/data2/data.json
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/my_package/sub_pkg3/foo.py
+-rw-r--r--   0        0        0     1348 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/pyproject.toml
+-rw-r--r--   0        0        0     1062 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/README.rst
+-rw-r--r--   0        0        0      874 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/data1.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/sub_data/data2.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/sub_data/data3.txt
+-rw-r--r--   0        0        0     1062 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data/README.rst
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/data1.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/sub_data/data2.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/sub_data/data3.txt
+-rw-r--r--   0        0        0      874 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data/pyproject.toml
+-rw-r--r--   0        0        0     1062 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/README.rst
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/data1.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/sub_data/data2.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/sub_data/data3.txt
+-rw-r--r--   0        0        0      915 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/disable_setup_py/README.rst
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/disable_setup_py/my_package/__init__.py
+-rw-r--r--   0        0        0      740 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/disable_setup_py/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/epoch/README.rst
+-rw-r--r--   0        0        0       44 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/epoch/epoch.py
+-rw-r--r--   0        0        0      223 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/epoch/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/compiled/source.c
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/compiled/source.h
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/cython_code.pyx
+-rw-r--r--   0        0        0      474 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude-whl-include-sdist/pyproject.toml
+-rw-r--r--   0        0        0     1062 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/README.rst
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/data1.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/data2.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/sub_data/data2.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/sub_data/data3.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item1/itemdata1.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item1/subitem/subitemdata.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item2/itemdata2.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/publicdata.txt
+-rw-r--r--   0        0        0      952 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/excluded_subpackage/README.rst
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/excluded_subpackage/example/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/excluded_subpackage/example/test/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/excluded_subpackage/example/test/excluded.py
+-rw-r--r--   0        0        0      329 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/excluded_subpackage/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended/README.rst
+-rw-r--r--   0        0        0      186 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended/build.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended/extended/__init__.py
+-rw-r--r--   0        0        0      888 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended/extended/extended.c
+-rw-r--r--   0        0        0      292 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended/pyproject.toml
+-rw-r--r--   0        0        0      539 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended/setup.py
+-rw-r--r--   0        0        0       18 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended_with_no_setup/README.rst
+-rw-r--r--   0        0        0      753 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended_with_no_setup/build.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended_with_no_setup/extended/__init__.py
+-rw-r--r--   0        0        0      888 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended_with_no_setup/extended/extended.c
+-rw-r--r--   0        0        0      293 2023-05-29 08:06:23.995418 poetry_core-1.6.1/tests/masonry/builders/fixtures/extended_with_no_setup/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/include_excluded_code/lib/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/include_excluded_code/lib/my_package/generated.py
+-rw-r--r--   0        0        0      485 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/include_excluded_code/pyproject.toml
+-rw-r--r--   0        0        0     1062 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/README.rst
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Bar/foo/bar/Foo.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/Bar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/IncludedBar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/SecondBar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/lowercasebar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/FooBar/Bar.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/FooBar/lowercasebar.py
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/__init__.py
+-rw-r--r--   0        0        0     1011 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/COPYING
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/COPYING.txt
+-rw-r--r--   0        0        0     1062 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/BSD-3.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/CUSTOM-LICENSE
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/MIT.txt
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/README.rst
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/my_package/__init__.py
+-rw-r--r--   0        0        0     1231 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/localversionlabel/localversionlabel.py
+-rw-r--r--   0        0        0      133 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/localversionlabel/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/module1/README.rst
+-rw-r--r--   0        0        0       42 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/module1/module1.py
+-rw-r--r--   0        0        0      265 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/module1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0      261 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        8 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/py.typed
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0      291 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial_namespace/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial_namespace/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0        8 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial_namespace/pkg-stubs/subpkg/py.typed
+-rw-r--r--   0        0        0      306 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial_namespace/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/prerelease/README.rst
+-rw-r--r--   0        0        0       42 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/prerelease/prerelease.py
+-rw-r--r--   0        0        0      233 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/prerelease/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_callable_legacy_string/README.rst
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_callable_legacy_string/my_package/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_callable_legacy_string/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_callable_legacy_table/README.rst
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_callable_legacy_table/my_package/__init__.py
+-rw-r--r--   0        0        0      471 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_callable_legacy_table/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_console/README.rst
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_console/my_package/__init__.py
+-rw-r--r--   0        0        0      481 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_console/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file/README.rst
+-rw-r--r--   0        0        0       40 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file/bin/script.sh
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file/my_package/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/README.rst
+-rw-r--r--   0        0        0       40 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/bin/script.sh
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/my_package/__init__.py
+-rw-r--r--   0        0        0      384 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file_missing/README.rst
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file_missing/my_package/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/script_reference_file_missing/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/simple_version/README.rst
+-rw-r--r--   0        0        0      217 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/simple_version/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/simple_version/simple_version.py
+-rw-r--r--   0        0        0       28 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/single_python/README.rst
+-rw-r--r--   0        0        0      276 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/single_python/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/single_python/single_python.py
+-rw-r--r--   0        0        0       18 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/source_file/README.rst
+-rw-r--r--   0        0        0      268 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/source_file/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/source_file/src/module_src.py
+-rw-r--r--   0        0        0       18 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/source_package/README.rst
+-rw-r--r--   0        0        0      268 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/source_package/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/source_package/src/package_src/__init__.py
+-rw-r--r--   0        0        0       42 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/source_package/src/package_src/module.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/split_source/lib_a/module_a/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/split_source/lib_b/module_b/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/split_source/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/src_extended/README.rst
+-rw-r--r--   0        0        0      190 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/src_extended/build.py
+-rw-r--r--   0        0        0      292 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/src_extended/pyproject.toml
+-rw-r--r--   0        0        0      598 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/src_extended/setup.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/src_extended/src/extended/__init__.py
+-rw-r--r--   0        0        0      888 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/src_extended/src/extended/extended.c
+-rw-r--r--   0        0        0     1062 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/README.rst
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/extra_dir/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/extra_dir/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/extra_dir/sub_pkg/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/extra_dir/sub_pkg/vcs_excluded.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/extra_dir/vcs_excluded.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/for_wheel_only/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/my_module.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/notes.txt
+-rw-r--r--   0        0        0       22 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/package_with_include/__init__.py
+-rw-r--r--   0        0        0     1259 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/src/src_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/tests/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_bad_path_dep/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_bad_path_dep/with_bad_path_dep/__init__.py
+-rw-r--r--   0        0        0      274 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_bad_path_dev_dep/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_bad_path_dev_dep/with_bad_path_dev_dep/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_include_inline_table/both.txt
+-rw-r--r--   0        0        0     1050 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_include_inline_table/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_include_inline_table/src/src_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_include_inline_table/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_include_inline_table/tests/test_foo/test.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_include_inline_table/wheel_only.txt
+-rw-r--r--   0        0        0      656 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_url_dependency/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_url_dependency/with_url_dependency/__init__.py
+-rw-r--r--   0        0        0      641 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_vcs_dependency/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_vcs_dependency/with_vcs_dependency/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_wildcard_dependency_constraint/my_package/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/fixtures/with_wildcard_dependency_constraint/pyproject.toml
+-rw-r--r--   0        0        0     8986 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/test_builder.py
+-rw-r--r--   0        0        0    12699 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/test_complete.py
+-rw-r--r--   0        0        0    20450 2023-05-29 08:06:23.999418 poetry_core-1.6.1/tests/masonry/builders/test_sdist.py
+-rw-r--r--   0        0        0    12011 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/builders/test_wheel.py
+-rw-r--r--   0        0        0    10211 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/test_api.py
+-rw-r--r--   0        0        0     2202 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/test_builder.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/pep_561_stub_only/bad/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/pep_561_stub_only/bad/module.pyi
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/pep_561_stub_only/good-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/pep_561_stub_only/good-stubs/module.pyi
+-rw-r--r--   0        0        0       83 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/pep_561_stub_only_partial_namespace/good-stubs/module.pyi
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/pep_561_stub_only_partial_namespace/good-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0        8 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/pep_561_stub_only_partial_namespace/good-stubs/subpkg/py.typed
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/with_includes/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/with_includes/bar/baz.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/with_includes/extra_package/some_dir/foo.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/with_includes/extra_package/some_dir/quux.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/fixtures/with_includes/not_a_python_pkg/baz.txt
+-rw-r--r--   0        0        0      530 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/test_helpers.py
+-rw-r--r--   0        0        0     3047 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/masonry/utils/test_package_include.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/__init__.py
+-rw-r--r--   0        0        0    13625 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/test_dependency.py
+-rw-r--r--   0        0        0      948 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/test_dependency_group.py
+-rw-r--r--   0        0        0     6439 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/test_directory_dependency.py
+-rw-r--r--   0        0        0     8783 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/test_file_dependency.py
+-rw-r--r--   0        0        0    10840 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/test_main.py
+-rw-r--r--   0        0        0    20553 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/test_package.py
+-rw-r--r--   0        0        0     3814 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/test_specification.py
+-rw-r--r--   0        0        0     2588 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/test_url_dependency.py
+-rw-r--r--   0        0        0     5052 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/test_vcs_dependency.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/utils/__init__.py
+-rw-r--r--   0        0        0     9279 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/utils/test_utils.py
+-rw-r--r--   0        0        0     3929 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/utils/test_utils_link.py
+-rw-r--r--   0        0        0     2248 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/packages/utils/test_utils_urls.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/pyproject/__init__.py
+-rw-r--r--   0        0        0      813 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/pyproject/conftest.py
+-rw-r--r--   0        0        0     2373 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/pyproject/test_pyproject_toml.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/spdx/__init__.py
+-rw-r--r--   0        0        0     1413 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/spdx/test_helpers.py
+-rw-r--r--   0        0        0     1497 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/spdx/test_license.py
+-rw-r--r--   0        0        0      343 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/test_core_version.py
+-rw-r--r--   0        0        0    17197 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/test_factory.py
+-rw-r--r--   0        0        0     2721 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/testutils.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5913 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/utils/test_helpers.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/vcs/__init__.py
+-rw-r--r--   0        0        0    15077 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/vcs/test_vcs.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/version/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/version/pep440/__init__.py
+-rw-r--r--   0        0        0     5298 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/version/pep440/test_segments.py
+-rw-r--r--   0        0        0    14354 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/version/pep440/test_version.py
+-rw-r--r--   0        0        0    66656 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/version/test_markers.py
+-rw-r--r--   0        0        0     4452 2023-05-29 08:06:24.003418 poetry_core-1.6.1/tests/version/test_requirements.py
+-rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 poetry_core-1.6.1/PKG-INFO
```

### Comparing `poetry_core-1.6.0/LICENSE` & `poetry_core-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/README.md` & `poetry_core-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/pyproject.toml` & `poetry_core-1.6.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,52 @@
 [tool.poetry]
 name = "poetry-core"
-version = "1.6.0"
+version = "1.6.1"
 description = "Poetry PEP 517 Build Backend"
 authors = ["Sébastien Eustace <sebastien@eustace.io>"]
-
 license = "MIT"
-
 readme = "README.md"
-
 homepage = "https://github.com/python-poetry/poetry-core"
 repository = "https://github.com/python-poetry/poetry-core"
-
 keywords = ["packaging", "dependency", "poetry"]
-
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
-
 packages = [
     { include = "poetry", from = "src" },
 ]
 include = [
     { path = "tests", format = "sdist" },
 ]
-exclude = [
-    "**/*.pyc",
-    "**/*.pyi",
-]
-
-[tool.poetry.build]
-generate-setup-file = false
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/python-poetry/poetry/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 # required for compatibility
 importlib-metadata = {version = ">=1.7.0", python = "<3.8"}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.15.0"
-pyrsistent = ">=0.18.0"
-pytest = ">=7.1.2"
-pytest-cov = ">=3.0.0"
-pytest-mock = ">=3.5"
 tox = ">=3.0"
 vendoring = {version = ">=1.0", python = "^3.8"}
+
+[tool.poetry.group.test.dependencies]
+pytest = ">=7.1.2"
+pytest-cov = ">=3.0.0"
+pytest-mock = ">=3.10"
 build = ">=0.10.0"
-mypy = ">=1.0"
 setuptools = ">=60"
 tomli-w = "^1.0.0"
+
+[tool.poetry.group.typing.dependencies]
+mypy = ">=1.0"
 types-jsonschema = ">=4.4.4"
 types-setuptools = ">=57.4.14"
 
 
 [tool.ruff]
 fix = true
 unfixable = [
@@ -98,17 +88,15 @@
 lines-after-imports = 2
 known-first-party = ["poetry.core"]
 known-third-party = ["poetry.core._vendor"]
 required-imports = ["from __future__ import annotations"]
 
 
 [tool.black]
-line-length = 88
 preview = true
-include = '\.pyi?$'
 extend-exclude = "src/poetry/core/_vendor/*"
 
 
 [tool.mypy]
 strict = true
 explicit_package_bases = true
 namespace_packages = true
```

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/__init__.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/_cmp.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/_cmp.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/_compat.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/_compat.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/_config.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/_config.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/_funcs.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/_funcs.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/_make.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/_make.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/_next_gen.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/_next_gen.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/_version_info.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/_version_info.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/converters.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/converters.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/exceptions.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/filters.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/filters.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/setters.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/setters.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attr/validators.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attr/validators.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attrs/LICENSE` & `poetry_core-1.6.1/src/poetry/core/_vendor/attrs/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/attrs/__init__.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/attrs/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/COPYING` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/COPYING`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/__init__.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/_format.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/_format.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/_legacy_validators.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/_legacy_validators.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/_types.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/_types.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/_utils.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/_utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/_validators.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/_validators.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/benchmarks/issue232/issue.json` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/benchmarks/issue232/issue.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/cli.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/cli.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/exceptions.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/protocols.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/protocols.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft2019-09.json` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft2019-09.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft2020-12.json` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft2020-12.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft3.json` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft3.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft4.json` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft4.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft6.json` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft6.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/draft7.json` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/draft7.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/applicator` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/applicator`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/content` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/content`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/core` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/core`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/meta-data` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/meta-data`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/validation` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/validation`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/applicator` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/applicator`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/content` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/content`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/core` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/core`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/meta-data` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/meta-data`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/validation` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/validation`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/jsonschema/validators.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/jsonschema/validators.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/LICENSE` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/__init__.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/ast_utils.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/ast_utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/common.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/common.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/exceptions.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/grammar.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/grammar.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/grammars/common.lark` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/grammars/common.lark`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/grammars/lark.lark` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/grammars/lark.lark`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/grammars/python.lark` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/grammars/python.lark`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/indenter.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/indenter.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/lark.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/lark.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/lexer.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/lexer.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/load_grammar.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/load_grammar.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parse_tree_builder.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parse_tree_builder.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parser_frontends.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parser_frontends.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/cyk.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/cyk.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/earley.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/earley.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/earley_common.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/earley_common.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/earley_forest.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/earley_forest.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/grammar_analysis.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/grammar_analysis.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/lalr_analysis.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/lalr_analysis.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/lalr_interactive_parser.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/lalr_interactive_parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/lalr_parser.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/lalr_parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/resolve_ambig.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/resolve_ambig.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/parsers/xearley.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/parsers/xearley.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/reconstruct.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/reconstruct.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/tools/__init__.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/tools/nearley.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/tools/nearley.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/tools/serialize.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/tools/serialize.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/tools/standalone.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/tools/standalone.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/tree.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/tree.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/tree_matcher.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/tree_matcher.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/tree_templates.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/tree_templates.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/utils.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/lark/visitors.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/lark/visitors.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/LICENSE.APACHE` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/LICENSE.BSD` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_elffile.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_manylinux.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_musllinux.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_parser.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_structures.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/_tokenizer.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/markers.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/metadata.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/requirements.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/specifiers.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/tags.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/utils.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/packaging/version.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/LICENSE.mit` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/__init__.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_checked_types.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_checked_types.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_field_common.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_field_common.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_helpers.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_immutable.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_immutable.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pbag.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pbag.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pclass.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pclass.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pdeque.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pdeque.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_plist.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_plist.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pmap.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pmap.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_precord.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_precord.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pset.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pset.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_pvector.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_pvector.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_toolz.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_toolz.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/_transformations.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/_transformations.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/pyrsistent/typing.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/pyrsistent/typing.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/tomli/LICENSE` & `poetry_core-1.6.1/src/poetry/core/_vendor/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/tomli/_parser.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/tomli/_re.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/typing_extensions.LICENSE` & `poetry_core-1.6.1/src/poetry/core/_vendor/typing_extensions.LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/_vendor/typing_extensions.py` & `poetry_core-1.6.1/src/poetry/core/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/generic/__init__.py` & `poetry_core-1.6.1/src/poetry/core/constraints/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/generic/any_constraint.py` & `poetry_core-1.6.1/src/poetry/core/constraints/generic/any_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/generic/base_constraint.py` & `poetry_core-1.6.1/src/poetry/core/constraints/generic/base_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/generic/constraint.py` & `poetry_core-1.6.1/src/poetry/core/constraints/generic/constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/generic/empty_constraint.py` & `poetry_core-1.6.1/src/poetry/core/constraints/generic/empty_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/generic/multi_constraint.py` & `poetry_core-1.6.1/src/poetry/core/constraints/generic/multi_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,21 @@
 
     def invert(self) -> UnionConstraint:
         from poetry.core.constraints.generic import UnionConstraint
 
         return UnionConstraint(*(c.invert() for c in self._constraints))
 
     def intersect(self, other: BaseConstraint) -> BaseConstraint:
+        if isinstance(other, MultiConstraint):
+            ours = set(self.constraints)
+            union = list(self.constraints) + [
+                c for c in other.constraints if c not in ours
+            ]
+            return MultiConstraint(*union)
+
         if not isinstance(other, Constraint):
             return other.intersect(self)
 
         if other in self._constraints:
             return self
 
         if other.value in (c.value for c in self._constraints):
@@ -86,14 +93,19 @@
 
         if other.operator == "==":
             return other
 
         return MultiConstraint(*self._constraints, other)
 
     def union(self, other: BaseConstraint) -> BaseConstraint:
+        if isinstance(other, MultiConstraint):
+            theirs = set(other.constraints)
+            common = [c for c in self.constraints if c in theirs]
+            return MultiConstraint(*common)
+
         if not isinstance(other, Constraint):
             return other.union(self)
 
         if other in self._constraints:
             return other
 
         if other.value not in (c.value for c in self._constraints):
```

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/generic/parser.py` & `poetry_core-1.6.1/src/poetry/core/constraints/generic/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/generic/union_constraint.py` & `poetry_core-1.6.1/src/poetry/core/constraints/generic/union_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/version/__init__.py` & `poetry_core-1.6.1/src/poetry/core/constraints/version/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/version/empty_constraint.py` & `poetry_core-1.6.1/src/poetry/core/constraints/version/empty_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/version/parser.py` & `poetry_core-1.6.1/src/poetry/core/constraints/version/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/version/patterns.py` & `poetry_core-1.6.1/src/poetry/core/constraints/version/patterns.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/version/util.py` & `poetry_core-1.6.1/src/poetry/core/constraints/version/util.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/version/version.py` & `poetry_core-1.6.1/src/poetry/core/constraints/version/version.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/version/version_constraint.py` & `poetry_core-1.6.1/src/poetry/core/constraints/version/version_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/version/version_range.py` & `poetry_core-1.6.1/src/poetry/core/constraints/version/version_range.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/version/version_range_constraint.py` & `poetry_core-1.6.1/src/poetry/core/constraints/version/version_range_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/constraints/version/version_union.py` & `poetry_core-1.6.1/src/poetry/core/constraints/version/version_union.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/factory.py` & `poetry_core-1.6.1/src/poetry/core/factory.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/json/__init__.py` & `poetry_core-1.6.1/src/poetry/core/json/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/json/schemas/poetry-schema.json` & `poetry_core-1.6.1/src/poetry/core/json/schemas/poetry-schema.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/masonry/api.py` & `poetry_core-1.6.1/src/poetry/core/masonry/api.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/masonry/builder.py` & `poetry_core-1.6.1/src/poetry/core/masonry/builder.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/masonry/builders/builder.py` & `poetry_core-1.6.1/src/poetry/core/masonry/builders/builder.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/masonry/builders/sdist.py` & `poetry_core-1.6.1/src/poetry/core/masonry/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/masonry/builders/wheel.py` & `poetry_core-1.6.1/src/poetry/core/masonry/builders/wheel.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 import csv
 import hashlib
 import logging
 import os
 import shutil
 import stat
 import subprocess
+import sys
 import tempfile
 import zipfile
 
 from base64 import urlsafe_b64encode
 from io import StringIO
 from pathlib import Path
 from typing import TYPE_CHECKING
 from typing import TextIO
 
-from packaging.tags import sys_tags
+import packaging.tags
 
 from poetry.core import __version__
 from poetry.core.constraints.version import parse_constraint
 from poetry.core.masonry.builders.builder import Builder
 from poetry.core.masonry.builders.sdist import SdistBuilder
 from poetry.core.masonry.utils.helpers import distribution_name
 from poetry.core.masonry.utils.helpers import normalize_file_permissions
 from poetry.core.masonry.utils.package_include import PackageInclude
+from poetry.core.utils.helpers import decode
 from poetry.core.utils.helpers import temporary_directory
 
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
     from packaging.utils import NormalizedName
@@ -323,24 +325,67 @@
             parse_constraint(">=2.0.0 <3.0.0")
         )
 
     def dist_info_name(self, name: NormalizedName, version: str) -> str:
         escaped_name = distribution_name(name)
         return f"{escaped_name}-{version}.dist-info"
 
+    def _get_sys_tags(self) -> list[str]:
+        """Get sys_tags via subprocess.
+        Required if poetry-core is not run inside the build environment.
+        """
+        try:
+            output = subprocess.check_output(
+                [
+                    self.executable.as_posix(),
+                    "-c",
+                    f"""
+import importlib.util
+import sys
+
+from pathlib import Path
+
+spec = importlib.util.spec_from_file_location(
+    "packaging", Path(r"{packaging.__file__}")
+)
+
+packaging = importlib.util.module_from_spec(spec)
+sys.modules[spec.name] = packaging
+
+spec = importlib.util.spec_from_file_location(
+    "packaging.tags", Path(r"{packaging.tags.__file__}")
+)
+packaging_tags = importlib.util.module_from_spec(spec)
+spec.loader.exec_module(packaging_tags)
+for t in packaging_tags.sys_tags():
+    print(t.interpreter, t.abi, t.platform, sep="-")
+""",
+                ],
+                stderr=subprocess.STDOUT,
+            )
+        except subprocess.CalledProcessError as e:
+            raise RuntimeError(
+                "Failed to get sys_tags for python interpreter"
+                f" '{self.executable.as_posix()}':\n{decode(e.output)}"
+            )
+        return decode(output).strip().splitlines()
+
     @property
     def tag(self) -> str:
         if self._package.build_script:
-            sys_tag = next(sys_tags())
+            if self.executable != Path(sys.executable):
+                # poetry-core is not run in the build environment
+                # -> this is probably not a PEP 517 build but a poetry build
+                return self._get_sys_tags()[0]
+            sys_tag = next(packaging.tags.sys_tags())
             tag = (sys_tag.interpreter, sys_tag.abi, sys_tag.platform)
         else:
             platform = "any"
             impl = "py2.py3" if self.supports_python2() else "py3"
             tag = (impl, "none", platform)
-
         return "-".join(tag)
 
     def _add_file(
         self,
         wheel: zipfile.ZipFile,
         full_path: Path,
         rel_path: Path,
```

### Comparing `poetry_core-1.6.0/src/poetry/core/masonry/metadata.py` & `poetry_core-1.6.1/src/poetry/core/masonry/metadata.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/masonry/utils/helpers.py` & `poetry_core-1.6.1/src/poetry/core/masonry/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/masonry/utils/include.py` & `poetry_core-1.6.1/src/poetry/core/masonry/utils/include.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/masonry/utils/module.py` & `poetry_core-1.6.1/src/poetry/core/masonry/utils/module.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/masonry/utils/package_include.py` & `poetry_core-1.6.1/src/poetry/core/masonry/utils/package_include.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/constraints/__init__.py` & `poetry_core-1.6.1/src/poetry/core/packages/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/dependency.py` & `poetry_core-1.6.1/src/poetry/core/packages/dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/dependency_group.py` & `poetry_core-1.6.1/src/poetry/core/packages/dependency_group.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/directory_dependency.py` & `poetry_core-1.6.1/src/poetry/core/packages/directory_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/file_dependency.py` & `poetry_core-1.6.1/src/poetry/core/packages/file_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/package.py` & `poetry_core-1.6.1/src/poetry/core/packages/package.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/path_dependency.py` & `poetry_core-1.6.1/src/poetry/core/packages/path_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/project_package.py` & `poetry_core-1.6.1/src/poetry/core/packages/project_package.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/specification.py` & `poetry_core-1.6.1/src/poetry/core/packages/specification.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/url_dependency.py` & `poetry_core-1.6.1/src/poetry/core/packages/url_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/utils/link.py` & `poetry_core-1.6.1/src/poetry/core/packages/utils/link.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/utils/utils.py` & `poetry_core-1.6.1/src/poetry/core/packages/utils/utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/packages/vcs_dependency.py` & `poetry_core-1.6.1/src/poetry/core/packages/vcs_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/poetry.py` & `poetry_core-1.6.1/src/poetry/core/poetry.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/pyproject/tables.py` & `poetry_core-1.6.1/src/poetry/core/pyproject/tables.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/pyproject/toml.py` & `poetry_core-1.6.1/src/poetry/core/pyproject/toml.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/semver/patterns.py` & `poetry_core-1.6.1/src/poetry/core/semver/patterns.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/spdx/data/licenses.json` & `poetry_core-1.6.1/src/poetry/core/spdx/data/licenses.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/spdx/helpers.py` & `poetry_core-1.6.1/src/poetry/core/spdx/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/spdx/license.py` & `poetry_core-1.6.1/src/poetry/core/spdx/license.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/spdx/updater.py` & `poetry_core-1.6.1/src/poetry/core/spdx/updater.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/utils/helpers.py` & `poetry_core-1.6.1/src/poetry/core/utils/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sys
 import tempfile
 import time
 import unicodedata
 import warnings
 
 from contextlib import contextmanager
+from contextlib import suppress
 from pathlib import Path
 from typing import TYPE_CHECKING
 from typing import Any
 
 from packaging.utils import canonicalize_name
 
 from poetry.core.version.pep440 import PEP440Version
@@ -23,14 +24,27 @@
     from collections.abc import Iterator
 
 
 def combine_unicode(string: str) -> str:
     return unicodedata.normalize("NFC", string)
 
 
+def decode(string: bytes | str, encodings: list[str] | None = None) -> str:
+    if not isinstance(string, bytes):
+        return string
+
+    encodings = encodings or ["utf-8", "latin1", "ascii"]
+
+    for encoding in encodings:
+        with suppress(UnicodeEncodeError, UnicodeDecodeError):
+            return string.decode(encoding)
+
+    return string.decode(encodings[0], errors="ignore")
+
+
 def module_name(name: str) -> str:
     return canonicalize_name(name).replace("-", "_")
 
 
 def normalize_version(version: str) -> str:
     warnings.warn(
         "normalize_version() is deprecated. Use Version.parse().to_string() instead.",
```

### Comparing `poetry_core-1.6.0/src/poetry/core/vcs/__init__.py` & `poetry_core-1.6.1/src/poetry/core/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/vcs/git.py` & `poetry_core-1.6.1/src/poetry/core/vcs/git.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/version/grammars/markers.lark` & `poetry_core-1.6.1/src/poetry/core/version/grammars/markers.lark`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/version/grammars/pep508.lark` & `poetry_core-1.6.1/src/poetry/core/version/grammars/pep508.lark`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/version/helpers.py` & `poetry_core-1.6.1/src/poetry/core/version/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/version/markers.py` & `poetry_core-1.6.1/src/poetry/core/version/markers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/version/parser.py` & `poetry_core-1.6.1/src/poetry/core/version/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/version/pep440/parser.py` & `poetry_core-1.6.1/src/poetry/core/version/pep440/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/version/pep440/segments.py` & `poetry_core-1.6.1/src/poetry/core/version/pep440/segments.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/version/pep440/version.py` & `poetry_core-1.6.1/src/poetry/core/version/pep440/version.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/src/poetry/core/version/requirements.py` & `poetry_core-1.6.1/src/poetry/core/version/requirements.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/conftest.py` & `poetry_core-1.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/constraints/generic/test_constraint.py` & `poetry_core-1.6.1/tests/constraints/generic/test_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,23 @@
             Constraint("linux"),
         ),
         (
             UnionConstraint(Constraint("win32"), Constraint("linux")),
             MultiConstraint(Constraint("win32", "!="), Constraint("linux", "!=")),
             EmptyConstraint(),
         ),
+        (
+            MultiConstraint(Constraint("win32", "!="), Constraint("linux", "!=")),
+            MultiConstraint(Constraint("win32", "!="), Constraint("darwin", "!=")),
+            MultiConstraint(
+                Constraint("win32", "!="),
+                Constraint("linux", "!="),
+                Constraint("darwin", "!="),
+            ),
+        ),
     ],
 )
 def test_intersect(
     constraint1: BaseConstraint,
     constraint2: BaseConstraint,
     expected: BaseConstraint,
 ) -> None:
@@ -389,14 +398,19 @@
             MultiConstraint(Constraint("win32", "!="), Constraint("linux", "!=")),
             UnionConstraint(
                 Constraint("win32"),
                 Constraint("linux"),
                 MultiConstraint(Constraint("win32", "!="), Constraint("linux", "!=")),
             ),
         ),
+        (
+            MultiConstraint(Constraint("win32", "!="), Constraint("linux", "!=")),
+            MultiConstraint(Constraint("win32", "!="), Constraint("darwin", "!=")),
+            MultiConstraint(Constraint("win32", "!=")),
+        ),
     ],
 )
 def test_union(
     constraint1: BaseConstraint,
     constraint2: BaseConstraint,
     expected: BaseConstraint,
 ) -> None:
```

### Comparing `poetry_core-1.6.0/tests/constraints/generic/test_main.py` & `poetry_core-1.6.1/tests/constraints/generic/test_main.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/constraints/generic/test_multi_constraint.py` & `poetry_core-1.6.1/tests/constraints/generic/test_multi_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/constraints/generic/test_union_constraint.py` & `poetry_core-1.6.1/tests/constraints/generic/test_union_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/constraints/version/test_helpers.py` & `poetry_core-1.6.1/tests/constraints/version/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/constraints/version/test_parse_constraint.py` & `poetry_core-1.6.1/tests/constraints/version/test_parse_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/constraints/version/test_utils.py` & `poetry_core-1.6.1/tests/constraints/version/test_utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/constraints/version/test_version.py` & `poetry_core-1.6.1/tests/constraints/version/test_version.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/constraints/version/test_version_constraint.py` & `poetry_core-1.6.1/tests/constraints/version/test_version_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/constraints/version/test_version_range.py` & `poetry_core-1.6.1/tests/constraints/version/test_version_range.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/constraints/version/test_version_union.py` & `poetry_core-1.6.1/tests/constraints/version/test_version_union.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/complete.toml` & `poetry_core-1.6.1/tests/fixtures/complete.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/distributions/demo-0.1.0-in-subdir.zip` & `poetry_core-1.6.1/tests/fixtures/distributions/demo-0.1.0-in-subdir.zip`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl` & `poetry_core-1.6.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/distributions/demo-0.1.0.tar.gz` & `poetry_core-1.6.1/tests/fixtures/distributions/demo-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/pep_517_backend/pyproject.toml` & `poetry_core-1.6.1/tests/fixtures/pep_517_backend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/project_failing_strict_validation/pyproject.toml` & `poetry_core-1.6.1/tests/fixtures/project_failing_strict_validation/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/project_with_dependencies_with_subdirectory/pyproject.toml` & `poetry_core-1.6.1/tests/fixtures/project_with_dependencies_with_subdirectory/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/project_with_duplicated_classifiers/pyproject.toml` & `poetry_core-1.6.1/tests/fixtures/project_with_duplicated_classifiers/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/project_with_markers_and_extras/pyproject.toml` & `poetry_core-1.6.1/tests/fixtures/project_with_markers_and_extras/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/sample_project/pyproject.toml` & `poetry_core-1.6.1/tests/fixtures/sample_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl` & `poetry_core-1.6.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz` & `poetry_core-1.6.1/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/fixtures/simple_project/pyproject.toml` & `poetry_core-1.6.1/tests/fixtures/simple_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/integration/test_pep517.py` & `poetry_core-1.6.1/tests/integration/test_pep517.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/integration/test_pep517_backend.py` & `poetry_core-1.6.1/tests/integration/test_pep517_backend.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/json/test_poetry_schema.py` & `poetry_core-1.6.1/tests/json/test_poetry_schema.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/LICENSE` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/case_sensitive_exclusions/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/LICENSE` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/complete/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/complete/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/default_src_with_excluded_data/LICENSE` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/default_src_with_excluded_data/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data/LICENSE` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data_toml/LICENSE` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/default_with_excluded_data_toml/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/disable_setup_py/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/disable_setup_py/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/LICENSE` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/exclude_nested_data_toml/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/extended/extended/extended.c` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/extended/extended/extended.c`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/extended/setup.py` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/extended/setup.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/extended_with_no_setup/build.py` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/extended_with_no_setup/build.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/extended_with_no_setup/extended/extended.c` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/extended_with_no_setup/extended/extended.c`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/LICENSE` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/licenses_and_copying/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/licenses_and_copying/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/src_extended/setup.py` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/src_extended/setup.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/src_extended/src/extended/extended.c` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/src_extended/src/extended/extended.c`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/LICENSE` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/with-include/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/with-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/with_include_inline_table/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/with_include_inline_table/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/with_url_dependency/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/with_url_dependency/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/fixtures/with_vcs_dependency/pyproject.toml` & `poetry_core-1.6.1/tests/masonry/builders/fixtures/with_vcs_dependency/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/test_builder.py` & `poetry_core-1.6.1/tests/masonry/builders/test_builder.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/test_complete.py` & `poetry_core-1.6.1/tests/masonry/builders/test_complete.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/test_sdist.py` & `poetry_core-1.6.1/tests/masonry/builders/test_sdist.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/builders/test_wheel.py` & `poetry_core-1.6.1/tests/masonry/builders/test_wheel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import os
+import re
 import shutil
 import zipfile
 
 from pathlib import Path
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Iterator
@@ -346,7 +347,26 @@
     monkeypatch.setattr(os, "fdopen", capturing_fdopen)
 
     module_path = fixtures_dir / "module1"
     WheelBuilder.make(Factory().create_poetry(module_path))
 
     assert fd_file[0] is not None
     assert fd_file[0].closed
+
+
+@pytest.mark.parametrize("in_venv_build", [True, False])
+def test_tag(in_venv_build: bool, mocker: MockerFixture) -> None:
+    """Tests that tag returns a valid tag if a build script is used,
+    no matter if poetry-core lives inside the build environment or not.
+    """
+    root = fixtures_dir / "extended"
+    builder = WheelBuilder(Factory().create_poetry(root))
+
+    get_sys_tags_spy = mocker.spy(builder, "_get_sys_tags")
+    if not in_venv_build:
+        mocker.patch("sys.executable", "other/python")
+
+    assert re.match("^cp[23]_?\\d+-cp[23]_?\\d+m?u?-.+$", builder.tag)
+    if in_venv_build:
+        get_sys_tags_spy.assert_not_called()
+    else:
+        get_sys_tags_spy.assert_called()
```

### Comparing `poetry_core-1.6.0/tests/masonry/test_api.py` & `poetry_core-1.6.1/tests/masonry/test_api.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/test_builder.py` & `poetry_core-1.6.1/tests/masonry/test_builder.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/utils/test_helpers.py` & `poetry_core-1.6.1/tests/masonry/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/masonry/utils/test_package_include.py` & `poetry_core-1.6.1/tests/masonry/utils/test_package_include.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/test_dependency.py` & `poetry_core-1.6.1/tests/packages/test_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/test_dependency_group.py` & `poetry_core-1.6.1/tests/packages/test_dependency_group.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/test_directory_dependency.py` & `poetry_core-1.6.1/tests/packages/test_directory_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/test_file_dependency.py` & `poetry_core-1.6.1/tests/packages/test_file_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/test_main.py` & `poetry_core-1.6.1/tests/packages/test_main.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/test_package.py` & `poetry_core-1.6.1/tests/packages/test_package.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/test_specification.py` & `poetry_core-1.6.1/tests/packages/test_specification.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/test_url_dependency.py` & `poetry_core-1.6.1/tests/packages/test_url_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/test_vcs_dependency.py` & `poetry_core-1.6.1/tests/packages/test_vcs_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/utils/test_utils.py` & `poetry_core-1.6.1/tests/packages/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/utils/test_utils_link.py` & `poetry_core-1.6.1/tests/packages/utils/test_utils_link.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/packages/utils/test_utils_urls.py` & `poetry_core-1.6.1/tests/packages/utils/test_utils_urls.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/pyproject/conftest.py` & `poetry_core-1.6.1/tests/pyproject/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/pyproject/test_pyproject_toml.py` & `poetry_core-1.6.1/tests/pyproject/test_pyproject_toml.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/spdx/test_helpers.py` & `poetry_core-1.6.1/tests/spdx/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/spdx/test_license.py` & `poetry_core-1.6.1/tests/spdx/test_license.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/test_factory.py` & `poetry_core-1.6.1/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/testutils.py` & `poetry_core-1.6.1/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/utils/test_helpers.py` & `poetry_core-1.6.1/tests/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/vcs/test_vcs.py` & `poetry_core-1.6.1/tests/vcs/test_vcs.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/version/pep440/test_segments.py` & `poetry_core-1.6.1/tests/version/pep440/test_segments.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/version/pep440/test_version.py` & `poetry_core-1.6.1/tests/version/pep440/test_version.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/version/test_markers.py` & `poetry_core-1.6.1/tests/version/test_markers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/tests/version/test_requirements.py` & `poetry_core-1.6.1/tests/version/test_requirements.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.6.0/PKG-INFO` & `poetry_core-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-core
-Version: 1.6.0
+Version: 1.6.1
 Summary: Poetry PEP 517 Build Backend
 Home-page: https://github.com/python-poetry/poetry-core
 License: MIT
 Keywords: packaging,dependency,poetry
 Author: Sébastien Eustace
 Author-email: sebastien@eustace.io
 Requires-Python: >=3.7,<4.0
```

