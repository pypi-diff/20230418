# Comparing `tmp/pyformlang-1.0.1.tar.gz` & `tmp/pyformlang-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyformlang-1.0.1.tar", last modified: Fri Jun  3 13:13:18 2022, max compression
+gzip compressed data, was "pyformlang-1.0.2.tar", last modified: Tue Apr 18 19:14:33 2023, max compression
```

## Comparing `pyformlang-1.0.1.tar` & `pyformlang-1.0.2.tar`

### file list

```diff
@@ -1,117 +1,127 @@
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.955097 pyformlang-1.0.1/
--rw-rw-r--   0 julien    (1000) julien    (1000)     1070 2022-06-03 08:50:00.000000 pyformlang-1.0.1/LICENSE
--rw-rw-r--   0 julien    (1000) julien    (1000)     2132 2022-06-03 13:13:18.955097 pyformlang-1.0.1/PKG-INFO
--rw-rw-r--   0 julien    (1000) julien    (1000)     1673 2022-06-03 08:50:00.000000 pyformlang-1.0.1/README.md
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.951097 pyformlang-1.0.1/pyformlang/
--rw-rw-r--   0 julien    (1000) julien    (1000)      814 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/__init__.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.951097 pyformlang-1.0.1/pyformlang/cfg/
--rw-rw-r--   0 julien    (1000) julien    (1000)      728 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    40609 2022-06-03 11:51:09.000000 pyformlang-1.0.1/pyformlang/cfg/cfg.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      608 2022-06-03 11:48:11.000000 pyformlang-1.0.1/pyformlang/cfg/cfg_object.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4501 2022-06-03 11:47:34.000000 pyformlang-1.0.1/pyformlang/cfg/cyk_table.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      281 2022-06-03 09:42:15.000000 pyformlang-1.0.1/pyformlang/cfg/epsilon.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     9297 2022-06-03 12:58:26.000000 pyformlang-1.0.1/pyformlang/cfg/llone_parser.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     3257 2022-06-03 12:58:26.000000 pyformlang-1.0.1/pyformlang/cfg/parse_tree.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1439 2022-06-03 11:47:26.000000 pyformlang-1.0.1/pyformlang/cfg/pda_object_creator.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1829 2022-06-03 12:57:11.000000 pyformlang-1.0.1/pyformlang/cfg/production.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4340 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/recursive_decent_parser.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      601 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/set_queue.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      718 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/terminal.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.951097 pyformlang-1.0.1/pyformlang/cfg/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    35372 2022-06-03 12:34:46.000000 pyformlang-1.0.1/pyformlang/cfg/tests/test_cfg.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    12656 2022-06-03 12:46:13.000000 pyformlang-1.0.1/pyformlang/cfg/tests/test_llone_parser.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1267 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/tests/test_production.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2628 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/tests/test_recursive_decent_parser.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      804 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/tests/test_terminal.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      804 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/tests/test_variable.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      394 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/utils.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1468 2022-06-03 11:47:38.000000 pyformlang-1.0.1/pyformlang/cfg/utils_cfg.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1062 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/cfg/variable.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.951097 pyformlang-1.0.1/pyformlang/finite_automaton/
--rw-rw-r--   0 julien    (1000) julien    (1000)     2388 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    16748 2022-06-03 11:33:21.000000 pyformlang-1.0.1/pyformlang/finite_automaton/deterministic_finite_automaton.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1320 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/doubly_linked_list.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1046 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/doubly_linked_node.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      473 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/epsilon.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    32753 2022-06-03 11:39:19.000000 pyformlang-1.0.1/pyformlang/finite_automaton/epsilon_nfa.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    18726 2022-06-03 12:52:42.000000 pyformlang-1.0.1/pyformlang/finite_automaton/finite_automaton.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      666 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/finite_automaton_object.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1206 2022-06-03 11:24:50.000000 pyformlang-1.0.1/pyformlang/finite_automaton/hopcroft_processing_list.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4238 2022-06-03 11:10:39.000000 pyformlang-1.0.1/pyformlang/finite_automaton/nondeterministic_finite_automaton.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     6084 2022-06-03 11:37:38.000000 pyformlang-1.0.1/pyformlang/finite_automaton/nondeterministic_transition_function.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1897 2022-06-03 11:10:33.000000 pyformlang-1.0.1/pyformlang/finite_automaton/partition.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2029 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/regexable.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      883 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/state.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      756 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/symbol.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.951097 pyformlang-1.0.1/pyformlang/finite_automaton/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    12636 2022-06-03 11:34:31.000000 pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_deterministic_finite_automaton.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      456 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_epsilon.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    28438 2022-06-03 11:34:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_epsilon_nfa.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4647 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_nondeterministic_finite_automaton.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4269 2022-06-03 12:48:58.000000 pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_nondeterministic_transition_function.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1272 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_state.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1282 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_symbol.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     3817 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_transition_function.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     7065 2022-06-03 11:09:17.000000 pyformlang-1.0.1/pyformlang/finite_automaton/transition_function.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.951097 pyformlang-1.0.1/pyformlang/fst/
--rw-rw-r--   0 julien    (1000) julien    (1000)      216 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/fst/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    21016 2022-06-03 12:03:41.000000 pyformlang-1.0.1/pyformlang/fst/fst.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.951097 pyformlang-1.0.1/pyformlang/fst/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/fst/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     8317 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/fst/tests/test_fst.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.955097 pyformlang-1.0.1/pyformlang/indexed_grammar/
--rw-rw-r--   0 julien    (1000) julien    (1000)      920 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2580 2022-06-03 11:46:36.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/consumption_rule.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2723 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/duplication_rule.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2303 2022-06-03 11:47:16.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/end_rule.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    18376 2022-06-03 11:43:59.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/indexed_grammar.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2803 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/production_rule.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2422 2022-06-03 11:45:37.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/reduced_rule.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     5610 2022-06-03 11:46:58.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/rule_ordering.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     5888 2022-06-03 11:34:38.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/rules.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.955097 pyformlang-1.0.1/pyformlang/indexed_grammar/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    14169 2022-06-03 12:32:54.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/tests/test_indexed_grammar.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2026 2022-06-03 12:47:16.000000 pyformlang-1.0.1/pyformlang/indexed_grammar/tests/test_rules.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.955097 pyformlang-1.0.1/pyformlang/pda/
--rw-rw-r--   0 julien    (1000) julien    (1000)      605 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/pda/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4245 2022-06-03 12:18:27.000000 pyformlang-1.0.1/pyformlang/pda/cfg_variable_converter.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      215 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/pda/epsilon.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    27274 2022-06-03 12:51:57.000000 pyformlang-1.0.1/pyformlang/pda/pda.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      805 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/pda/stack_symbol.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      836 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/pda/state.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      714 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/pda/symbol.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.955097 pyformlang-1.0.1/pyformlang/pda/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/pda/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    15278 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/pda/tests/test_pda.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     3359 2022-06-03 12:04:14.000000 pyformlang-1.0.1/pyformlang/pda/transition_function.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1757 2022-06-03 12:18:35.000000 pyformlang-1.0.1/pyformlang/pda/utils.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.955097 pyformlang-1.0.1/pyformlang/regular_expression/
--rw-rw-r--   0 julien    (1000) julien    (1000)      771 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/regular_expression/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     8441 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/regular_expression/python_regex.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    16628 2022-06-03 11:57:40.000000 pyformlang-1.0.1/pyformlang/regular_expression/regex.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     5835 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/regular_expression/regex_objects.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     8908 2022-06-03 11:57:40.000000 pyformlang-1.0.1/pyformlang/regular_expression/regex_reader.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.955097 pyformlang-1.0.1/pyformlang/regular_expression/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/regular_expression/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     7419 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/regular_expression/tests/test_python_regex.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    11533 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/regular_expression/tests/test_regex.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.955097 pyformlang-1.0.1/pyformlang/rsa/
--rw-rw-r--   0 julien    (1000) julien    (1000)      719 2022-06-03 09:44:06.000000 pyformlang-1.0.1/pyformlang/rsa/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2529 2022-06-03 09:44:14.000000 pyformlang-1.0.1/pyformlang/rsa/box.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     6024 2022-06-03 11:58:43.000000 pyformlang-1.0.1/pyformlang/rsa/recursive_automaton.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.955097 pyformlang-1.0.1/pyformlang/rsa/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/rsa/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     3265 2022-06-03 12:01:10.000000 pyformlang-1.0.1/pyformlang/rsa/tests/test_rsa.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.955097 pyformlang-1.0.1/pyformlang/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.1/pyformlang/tests/__init__.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2022-06-03 13:13:18.951097 pyformlang-1.0.1/pyformlang.egg-info/
--rw-rw-r--   0 julien    (1000) julien    (1000)     2132 2022-06-03 13:13:18.000000 pyformlang-1.0.1/pyformlang.egg-info/PKG-INFO
--rw-rw-r--   0 julien    (1000) julien    (1000)     3782 2022-06-03 13:13:18.000000 pyformlang-1.0.1/pyformlang.egg-info/SOURCES.txt
--rw-rw-r--   0 julien    (1000) julien    (1000)        1 2022-06-03 13:13:18.000000 pyformlang-1.0.1/pyformlang.egg-info/dependency_links.txt
--rw-rw-r--   0 julien    (1000) julien    (1000)       21 2022-06-03 13:13:18.000000 pyformlang-1.0.1/pyformlang.egg-info/requires.txt
--rw-rw-r--   0 julien    (1000) julien    (1000)       11 2022-06-03 13:13:18.000000 pyformlang-1.0.1/pyformlang.egg-info/top_level.txt
--rw-rw-r--   0 julien    (1000) julien    (1000)       38 2022-06-03 13:13:18.955097 pyformlang-1.0.1/setup.cfg
--rw-rw-r--   0 julien    (1000) julien    (1000)      758 2022-06-03 13:11:25.000000 pyformlang-1.0.1/setup.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1070 2022-06-03 08:50:00.000000 pyformlang-1.0.2/LICENSE
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2294 2023-04-18 19:14:33.587721 pyformlang-1.0.2/PKG-INFO
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1872 2022-06-03 14:50:28.000000 pyformlang-1.0.2/README.md
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.583721 pyformlang-1.0.2/pyformlang/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      814 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/__init__.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.583721 pyformlang-1.0.2/pyformlang/cfg/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      728 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/cfg/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    40695 2023-04-18 16:51:27.000000 pyformlang-1.0.2/pyformlang/cfg/cfg.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      608 2022-06-03 11:48:11.000000 pyformlang-1.0.2/pyformlang/cfg/cfg_object.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4501 2022-06-03 11:47:34.000000 pyformlang-1.0.2/pyformlang/cfg/cyk_table.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      281 2022-06-03 09:42:15.000000 pyformlang-1.0.2/pyformlang/cfg/epsilon.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     9297 2022-06-03 12:58:26.000000 pyformlang-1.0.2/pyformlang/cfg/llone_parser.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     3397 2023-04-18 19:05:13.000000 pyformlang-1.0.2/pyformlang/cfg/parse_tree.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1439 2022-06-03 11:47:26.000000 pyformlang-1.0.2/pyformlang/cfg/pda_object_creator.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1828 2023-04-18 17:27:00.000000 pyformlang-1.0.2/pyformlang/cfg/production.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4340 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/cfg/recursive_decent_parser.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      601 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/cfg/set_queue.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      718 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/cfg/terminal.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.583721 pyformlang-1.0.2/pyformlang/cfg/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/cfg/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    35520 2023-04-18 13:51:56.000000 pyformlang-1.0.2/pyformlang/cfg/tests/test_cfg.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    12656 2022-06-03 12:46:13.000000 pyformlang-1.0.2/pyformlang/cfg/tests/test_llone_parser.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1267 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/cfg/tests/test_production.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2579 2023-04-18 15:32:45.000000 pyformlang-1.0.2/pyformlang/cfg/tests/test_recursive_decent_parser.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      957 2023-04-18 15:33:47.000000 pyformlang-1.0.2/pyformlang/cfg/tests/test_terminal.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      804 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/cfg/tests/test_variable.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      394 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/cfg/utils.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1468 2022-06-03 11:47:38.000000 pyformlang-1.0.2/pyformlang/cfg/utils_cfg.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1062 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/cfg/variable.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.583721 pyformlang-1.0.2/pyformlang/fcfg/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      747 2023-04-18 19:10:47.000000 pyformlang-1.0.2/pyformlang/fcfg/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     9525 2023-04-18 19:06:00.000000 pyformlang-1.0.2/pyformlang/fcfg/fcfg.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1818 2023-04-18 17:28:34.000000 pyformlang-1.0.2/pyformlang/fcfg/feature_production.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    12463 2023-04-18 18:41:19.000000 pyformlang-1.0.2/pyformlang/fcfg/feature_structure.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2093 2023-04-18 18:55:29.000000 pyformlang-1.0.2/pyformlang/fcfg/state.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.583721 pyformlang-1.0.2/pyformlang/fcfg/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2023-04-17 10:32:24.000000 pyformlang-1.0.2/pyformlang/fcfg/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     9731 2023-04-18 19:07:03.000000 pyformlang-1.0.2/pyformlang/fcfg/tests/test_fcfg.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     8739 2023-04-18 18:40:38.000000 pyformlang-1.0.2/pyformlang/fcfg/tests/test_feature_structure.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.583721 pyformlang-1.0.2/pyformlang/finite_automaton/
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2388 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    16748 2022-06-03 11:33:21.000000 pyformlang-1.0.2/pyformlang/finite_automaton/deterministic_finite_automaton.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1320 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/doubly_linked_list.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1046 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/doubly_linked_node.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      473 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/epsilon.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    32753 2022-06-03 11:39:19.000000 pyformlang-1.0.2/pyformlang/finite_automaton/epsilon_nfa.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    18726 2022-06-07 15:07:04.000000 pyformlang-1.0.2/pyformlang/finite_automaton/finite_automaton.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      666 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/finite_automaton_object.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1206 2022-06-03 11:24:50.000000 pyformlang-1.0.2/pyformlang/finite_automaton/hopcroft_processing_list.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4238 2022-06-03 11:10:39.000000 pyformlang-1.0.2/pyformlang/finite_automaton/nondeterministic_finite_automaton.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     6084 2022-06-03 11:37:38.000000 pyformlang-1.0.2/pyformlang/finite_automaton/nondeterministic_transition_function.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1897 2022-06-03 11:10:33.000000 pyformlang-1.0.2/pyformlang/finite_automaton/partition.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2029 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/regexable.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      883 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/state.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      756 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/symbol.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/finite_automaton/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    12636 2022-06-03 11:34:31.000000 pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_deterministic_finite_automaton.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      456 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_epsilon.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    28438 2022-06-03 11:34:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_epsilon_nfa.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4647 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_nondeterministic_finite_automaton.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4269 2022-06-03 12:48:58.000000 pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_nondeterministic_transition_function.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1272 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_state.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1282 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_symbol.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     3817 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_transition_function.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     7065 2022-06-03 11:09:17.000000 pyformlang-1.0.2/pyformlang/finite_automaton/transition_function.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/fst/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      216 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/fst/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    21016 2022-06-07 15:07:10.000000 pyformlang-1.0.2/pyformlang/fst/fst.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/fst/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/fst/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     8317 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/fst/tests/test_fst.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/indexed_grammar/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      920 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2580 2022-06-03 11:46:36.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/consumption_rule.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2723 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/duplication_rule.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2303 2022-06-03 11:47:16.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/end_rule.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    18369 2022-06-03 14:06:05.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/indexed_grammar.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2803 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/production_rule.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2422 2022-06-03 11:45:37.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/reduced_rule.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     5610 2022-06-03 11:46:58.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/rule_ordering.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     5889 2023-04-18 17:39:15.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/rules.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/indexed_grammar/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    14169 2022-06-03 12:32:54.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/tests/test_indexed_grammar.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2026 2022-06-03 12:47:16.000000 pyformlang-1.0.2/pyformlang/indexed_grammar/tests/test_rules.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/pda/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      605 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/pda/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4245 2022-06-03 12:18:27.000000 pyformlang-1.0.2/pyformlang/pda/cfg_variable_converter.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      215 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/pda/epsilon.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    27276 2022-06-07 15:07:16.000000 pyformlang-1.0.2/pyformlang/pda/pda.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      805 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/pda/stack_symbol.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      836 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/pda/state.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      714 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/pda/symbol.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/pda/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/pda/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    15278 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/pda/tests/test_pda.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     3359 2022-06-03 12:04:14.000000 pyformlang-1.0.2/pyformlang/pda/transition_function.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1757 2022-06-03 12:18:35.000000 pyformlang-1.0.2/pyformlang/pda/utils.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/regular_expression/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      771 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/regular_expression/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     8441 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/regular_expression/python_regex.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    16628 2022-06-03 11:57:40.000000 pyformlang-1.0.2/pyformlang/regular_expression/regex.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     5835 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/regular_expression/regex_objects.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     8908 2022-06-03 11:57:40.000000 pyformlang-1.0.2/pyformlang/regular_expression/regex_reader.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/regular_expression/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/regular_expression/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     7419 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/regular_expression/tests/test_python_regex.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    11533 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/regular_expression/tests/test_regex.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/rsa/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      719 2022-06-03 09:44:06.000000 pyformlang-1.0.2/pyformlang/rsa/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2529 2022-06-03 09:44:14.000000 pyformlang-1.0.2/pyformlang/rsa/box.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     6024 2022-06-03 11:58:43.000000 pyformlang-1.0.2/pyformlang/rsa/recursive_automaton.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/rsa/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/rsa/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     3265 2022-06-03 12:01:10.000000 pyformlang-1.0.2/pyformlang/rsa/tests/test_rsa.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.587721 pyformlang-1.0.2/pyformlang/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.2/pyformlang/tests/__init__.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 19:14:33.583721 pyformlang-1.0.2/pyformlang.egg-info/
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2294 2023-04-18 19:14:33.000000 pyformlang-1.0.2/pyformlang.egg-info/PKG-INFO
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4051 2023-04-18 19:14:33.000000 pyformlang-1.0.2/pyformlang.egg-info/SOURCES.txt
+-rw-rw-r--   0 julien    (1000) julien    (1000)        1 2023-04-18 19:14:33.000000 pyformlang-1.0.2/pyformlang.egg-info/dependency_links.txt
+-rw-rw-r--   0 julien    (1000) julien    (1000)       21 2023-04-18 19:14:33.000000 pyformlang-1.0.2/pyformlang.egg-info/requires.txt
+-rw-rw-r--   0 julien    (1000) julien    (1000)       11 2023-04-18 19:14:33.000000 pyformlang-1.0.2/pyformlang.egg-info/top_level.txt
+-rw-rw-r--   0 julien    (1000) julien    (1000)       38 2023-04-18 19:14:33.587721 pyformlang-1.0.2/setup.cfg
+-rw-rw-r--   0 julien    (1000) julien    (1000)      758 2023-04-18 19:08:42.000000 pyformlang-1.0.2/setup.py
```

### Comparing `pyformlang-1.0.1/LICENSE` & `pyformlang-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/PKG-INFO` & `pyformlang-1.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,14 @@
-Metadata-Version: 2.1
-Name: pyformlang
-Version: 1.0.1
-Summary: A python framework for formal grammars
-Home-page: https://github.com/Aunsiels/pyformlang
-Author: Julien Romero
-Author-email: romerojulien34@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyformlang
 
-[![Build Status](https://jenkins.r2.enst.fr/job/pyformlang/job/master/badge/icon)](https://jenkins.r2.enst.fr/job/pyformlang/job/master/)
+[![Python package](https://github.com/Aunsiels/pyformlang/actions/workflows/python-package.yml/badge.svg)](https://github.com/Aunsiels/pyformlang/actions/workflows/python-package.yml)
 [![pypi](https://img.shields.io/pypi/v/pyformlang.svg)](https://pypi.org/project/pyformlang/)
 [![Documentation](https://readthedocs.org/projects/pyformlang/badge/?version=latest)](https://pyformlang.readthedocs.io/en/latest/)
+![badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Aunsiels/135f01c630063c3e69d999a2edf59fdb/raw/coverage_pyformlang.json)
+
 
 A python library to manipulate formal grammar. In general, it can be used to better understand algorithms in a formal way.
 
 If you use Pyformlang in your project, please cite our paper:
 
 ```
 @InProceedings{pyformlang,
@@ -50,9 +37,7 @@
 
 [Intersection CFG/Regex](https://www.degruyter.com/downloadpdf/j/stuf.1961.14.issue-1-4/stuf.1961.14.14.143/stuf.1961.14.14.143.pdf) and [a better written version](http://www.cs.umd.edu/~gasarch/BLOGPAPERS/cfg.pdf)
 
 ## Usage
 
 Please refer to the official documentation: [pyformlang.readthedocs.io](https://pyformlang.readthedocs.io).
 
-
-
```

### Comparing `pyformlang-1.0.1/pyformlang/__init__.py` & `pyformlang-1.0.2/pyformlang/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/__init__.py` & `pyformlang-1.0.2/pyformlang/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/cfg.py` & `pyformlang-1.0.2/pyformlang/cfg/cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 class NotParsableException(Exception):
     """When the grammar cannot be parsed (parser not powerful enough)"""
 
 
 def is_special_text(text):
     """ Check if the input is given an explicit type """
     return len(text) > 5 and \
-           (text[0:5] == '"VAR:' or text[0:5] == '"TER:') and \
-           text[-1] == '"'
+        (text[0:5] == '"VAR:' or text[0:5] == '"TER:') and \
+        text[-1] == '"'
 
 
 class CFG:
     """ A class representing a context free grammar
 
     Parameters
     ----------
@@ -702,14 +702,17 @@
         Can be optimized
         """
         return self._start_symbol not in self.get_generating_symbols()
 
     def __bool__(self):
         return not self.is_empty()
 
+    def __contains__(self, word: Iterable[Terminal]) -> bool:
+        return self.contains(word)
+
     def contains(self, word: Iterable[Terminal]) -> bool:
         """ Gives the membership of a word to the grammar
 
         Parameters
         ----------
         word : iterable of :class:`~pyformlang.cfg.Terminal`
             The word to check
@@ -1055,15 +1058,15 @@
         productions = set()
         terminals = set()
         for line in text.splitlines():
             line = line.strip()
             if not line:
                 continue
             cls._read_line(line, productions, terminals, variables)
-        return CFG(variables=variables, terminals=terminals,
+        return cls(variables=variables, terminals=terminals,
                    productions=productions, start_symbol=start_symbol)
 
     @classmethod
     def _read_line(cls, line, productions, terminals, variables):
         head_s, body_s = line.split("->")
         head_text = head_s.strip()
         if is_special_text(head_text):
@@ -1079,15 +1082,15 @@
                 else:
                     type_component = ""
                 if body_component[0] in string.ascii_uppercase or \
                         type_component == "VAR":
                     body_var = Variable(body_component)
                     variables.add(body_var)
                     body.append(body_var)
-                elif body_component not in EPSILON_SYMBOLS or type_component\
+                elif body_component not in EPSILON_SYMBOLS or type_component \
                         == "TER":
                     body_ter = Terminal(body_component)
                     terminals.add(body_ter)
                     body.append(body_ter)
             productions.add(Production(head, body))
 
     def is_normal_form(self):
@@ -1095,9 +1098,9 @@
         Tells is the current grammar is in Chomsky Normal Form or not
 
         Returns
         -------
         is_normal_form : bool
             If the current grammar is in CNF
         """
-        return all(production.is_normal_form()
-                    for production in self._productions)
+        return all(
+            production.is_normal_form() for production in self._productions)
```

### Comparing `pyformlang-1.0.1/pyformlang/cfg/cfg_object.py` & `pyformlang-1.0.2/pyformlang/cfg/cfg_object.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/cyk_table.py` & `pyformlang-1.0.2/pyformlang/cfg/cyk_table.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/llone_parser.py` & `pyformlang-1.0.2/pyformlang/cfg/llone_parser.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/parse_tree.py` & `pyformlang-1.0.2/pyformlang/cfg/parse_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,18 @@
         tree = nx.DiGraph()
         tree.add_node("ROOT", label=self.value.value)
         to_process = [("ROOT", son) for son in self.sons[::-1]]
         counter = 0
         while to_process:
             previous_node, current_node = to_process.pop()
             new_node = str(counter)
-            tree.add_node(new_node, label=current_node.value.value)
+            if isinstance(current_node.value, str):
+                tree.add_node(new_node, label=current_node.value)
+            else:
+                tree.add_node(new_node, label=current_node.value.value)
             counter += 1
             tree.add_edge(previous_node, new_node)
             to_process += [(new_node, son) for son in current_node.sons[::-1]]
         return tree
 
     def write_as_dot(self, filename):
         """
```

### Comparing `pyformlang-1.0.1/pyformlang/cfg/pda_object_creator.py` & `pyformlang-1.0.2/pyformlang/cfg/pda_object_creator.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/production.py` & `pyformlang-1.0.2/pyformlang/cfg/production.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """ A production or rule of a CFG """
-
 from typing import List
 
 from .terminal import Terminal
 from .variable import Variable
 from .cfg_object import CFGObject
 from .epsilon import Epsilon
```

### Comparing `pyformlang-1.0.1/pyformlang/cfg/recursive_decent_parser.py` & `pyformlang-1.0.2/pyformlang/cfg/recursive_decent_parser.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/set_queue.py` & `pyformlang-1.0.2/pyformlang/cfg/set_queue.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/terminal.py` & `pyformlang-1.0.2/pyformlang/cfg/terminal.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/tests/test_cfg.py` & `pyformlang-1.0.2/pyformlang/cfg/tests/test_cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -705,14 +705,16 @@
         self.assertEqual(derivation,
                          [[var_s],
                           [var_c, var_b],
                           [var_a, var_a, var_b],
                           [ter_a, var_a, var_b],
                           [ter_a, ter_a, var_b],
                           [ter_a, ter_a, ter_b]])
+        with self.assertRaises(DerivationDoesNotExist):
+            cfg.get_cnf_parse_tree([])
 
     def test_get_rightmost_derivation(self):
         ter_a = Terminal("a")
         ter_b = Terminal("b")
         var_s = Variable("S")
         var_a = Variable("A")
         var_b = Variable("B")
@@ -764,18 +766,19 @@
     def test_from_text2(self):
         text = """
         S  -> A B\n\rA -> a
         B -> b\r
         """
         cfg = CFG.from_text(text)
         self.assertTrue(cfg.contains(["a", "b"]))
+        self.assertTrue(["a", "b"] in cfg)
 
     def test_from_text_union(self):
         text = """
-        S -> a | b
+        "VAR:S" -> TER:a | b
         """
         cfg = CFG.from_text(text)
         self.assertEqual(2, len(cfg.productions))
 
     def test_epsilon(self):
         text = "S -> epsilon"
         cfg = CFG.from_text(text)
```

### Comparing `pyformlang-1.0.1/pyformlang/cfg/tests/test_llone_parser.py` & `pyformlang-1.0.2/pyformlang/cfg/tests/test_llone_parser.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/tests/test_production.py` & `pyformlang-1.0.2/pyformlang/cfg/tests/test_production.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/tests/test_recursive_decent_parser.py` & `pyformlang-1.0.2/pyformlang/cfg/tests/test_recursive_decent_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,11 +59,7 @@
         cfg = CFG.from_text("""
             S -> S E
         """)
         parser = RecursiveDecentParser(cfg)
         with self.assertRaises(RecursionError):
             parser.is_parsable([")"])
         self.assertFalse(parser.is_parsable([")"], left=False))
-
-
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `pyformlang-1.0.1/pyformlang/cfg/tests/test_terminal.py` & `pyformlang-1.0.2/pyformlang/cfg/tests/test_terminal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Tests the terminal """
 
 import unittest
 
-from pyformlang.cfg import Terminal
+from pyformlang.cfg import Terminal, Epsilon
 
 
 class TestTerminal(unittest.TestCase):
     """ Tests the terminal """
     # pylint: disable=missing-function-docstring
 
     def test_creation(self):
@@ -18,7 +18,10 @@
         self.assertNotEqual(terminal0, terminal1)
         self.assertNotEqual(terminal0, terminal3)
         self.assertEqual(hash(terminal0), hash(terminal2))
         self.assertNotEqual(hash(terminal0), hash(terminal1))
         self.assertEqual(str(terminal0), str(terminal2))
         self.assertEqual(str(terminal0), str(terminal3))
         self.assertNotEqual(str(terminal0), str(terminal1))
+        epsilon = Epsilon()
+        self.assertEqual(epsilon.to_text(), "epsilon")
+        self.assertEqual(Terminal("C").to_text(), '"TER:C"')
```

### Comparing `pyformlang-1.0.1/pyformlang/cfg/tests/test_variable.py` & `pyformlang-1.0.2/pyformlang/cfg/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/utils_cfg.py` & `pyformlang-1.0.2/pyformlang/cfg/utils_cfg.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/cfg/variable.py` & `pyformlang-1.0.2/pyformlang/cfg/variable.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/__init__.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/deterministic_finite_automaton.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/deterministic_finite_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/doubly_linked_list.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/doubly_linked_list.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/doubly_linked_node.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/doubly_linked_node.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/epsilon_nfa.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/epsilon_nfa.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/finite_automaton.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/finite_automaton.py`

 * *Files 1% similar despite different names*

```diff
@@ -666,14 +666,14 @@
     if given in ("epsilon", "ɛ"):
         return Epsilon()
     return Symbol(given)
 
 
 def add_start_state_to_graph(graph, state):
     """ Adds a starting node to a given graph """
-    graph.add_node(str(state.value) + "_starting",
+    graph.add_node("starting_" + str(state.value),
                    label="",
                    shape=None,
                    height=.0,
                    width=.0)
-    graph.add_edge(str(state.value) + "_starting",
+    graph.add_edge("starting_" + str(state.value),
                    state.value)
```

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/finite_automaton_object.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/finite_automaton_object.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/hopcroft_processing_list.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/hopcroft_processing_list.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/nondeterministic_finite_automaton.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/nondeterministic_finite_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/nondeterministic_transition_function.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/nondeterministic_transition_function.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/partition.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/partition.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/regexable.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/regexable.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/state.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/state.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/symbol.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/symbol.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_deterministic_finite_automaton.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_deterministic_finite_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_epsilon_nfa.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_epsilon_nfa.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_nondeterministic_finite_automaton.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_nondeterministic_finite_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_nondeterministic_transition_function.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_nondeterministic_transition_function.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_state.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_symbol.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_symbol.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/tests/test_transition_function.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/tests/test_transition_function.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/finite_automaton/transition_function.py` & `pyformlang-1.0.2/pyformlang/finite_automaton/transition_function.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/fst/fst.py` & `pyformlang-1.0.2/pyformlang/fst/fst.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,20 +473,20 @@
         for state in self._states:
             graph.add_node(state,
                            is_start=state in self.start_states,
                            is_final=state in self.final_states,
                            peripheries=2 if state in self.final_states else 1,
                            label=state)
             if state in self.start_states:
-                graph.add_node(str(state) + "_starting",
+                graph.add_node("starting_" + str(state),
                                label="",
                                shape=None,
                                height=.0,
                                width=.0)
-                graph.add_edge(str(state) + "_starting",
+                graph.add_edge("starting_" + str(state),
                                state)
         for s_from, input_symbol in self._delta:
             for s_to, output_symbols in self._delta[(s_from, input_symbol)]:
                 graph.add_edge(
                     s_from,
                     s_to,
                     label=(json.dumps(input_symbol) + " -> " +
```

### Comparing `pyformlang-1.0.1/pyformlang/fst/tests/test_fst.py` & `pyformlang-1.0.2/pyformlang/fst/tests/test_fst.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/__init__.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/consumption_rule.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/consumption_rule.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/duplication_rule.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/duplication_rule.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/end_rule.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/end_rule.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/indexed_grammar.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/indexed_grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             self.marked[non_terminal_a] = set()
             temp = frozenset({non_terminal_a})
             self.marked[non_terminal_a].add(temp)
         # Mark all end symbols
         for non_terminal_a in self.non_terminals:
             if exists(self.rules.rules,
                       lambda x: x.is_end_rule()
-                          and x.left_term == non_terminal_a):
+                      and x.left_term == non_terminal_a):
                 self.marked[non_terminal_a].add(frozenset())
 
     @property
     def terminals(self) -> Iterable[Any]:
         """Get all the terminals in the grammar
 
         Returns
@@ -306,32 +306,32 @@
         consumption_rules = self.rules.consumption_rules
         for rule in self.rules.rules:
             if rule.is_duplication():
                 left = rule.left_term
                 right0 = rule.right_terms[0]
                 right1 = rule.right_terms[1]
                 if all(x in generating and x in reachables for x in
-                        [left, right0, right1]):
+                       [left, right0, right1]):
                     l_rules.append(rule)
             if rule.is_production():
                 left = rule.left_term
                 right = rule.right_term
                 if all(x in generating and x in reachables for x in
-                        [left, right]):
+                       [left, right]):
                     l_rules.append(rule)
             if rule.is_end_rule():
                 left = rule.left_term
                 if left in generating and left in reachables:
                     l_rules.append(rule)
         for key in consumption_rules:
             for rule in consumption_rules[key]:
                 left = rule.left_term
                 right = rule.right
                 if all(x in generating and x in reachables for x in
-                        [left, right]):
+                       [left, right]):
                     l_rules.append(rule)
         rules = Rules(l_rules, self.rules.optim)
         return IndexedGrammar(rules)
 
     def intersection(self, other: Any) -> "IndexedGrammar":
         """ Computes the intersection of the current indexed grammar with the \
         other object
```

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/production_rule.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/production_rule.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/reduced_rule.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/reduced_rule.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/rule_ordering.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/rule_ordering.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/rules.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         left : any
             The left non-terminal in the rule
         right : any
             The right non-terminal in the rule
         prod : any
             The production used in the rule
         """
-        self._rules = list(filter(lambda x: not(x.is_production() and
+        self._rules = list(filter(lambda x: not (x.is_production() and
                                                 x.left_term == left and
                                                 x.right_term == right and
                                                 x.production == prod),
                                   self._rules))
 
     def add_production(self, left: Any, right: Any, prod: Any):
         """Add the production rule:
```

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/tests/test_indexed_grammar.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/tests/test_indexed_grammar.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/indexed_grammar/tests/test_rules.py` & `pyformlang-1.0.2/pyformlang/indexed_grammar/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/pda/__init__.py` & `pyformlang-1.0.2/pyformlang/pda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/pda/cfg_variable_converter.py` & `pyformlang-1.0.2/pyformlang/pda/cfg_variable_converter.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/pda/pda.py` & `pyformlang-1.0.2/pyformlang/pda/pda.py`

 * *Files 1% similar despite different names*

```diff
@@ -621,15 +621,15 @@
 
         TODO
         -------
         * Explain the format
         """
         pda = PDA()
         for s_from in graph:
-            if isinstance(s_from, str) and s_from.endswith("_starting"):
+            if isinstance(s_from, str) and s_from.startswith("starting_"):
                 continue
             for s_to in graph[s_from]:
                 for transition in graph[s_from][s_to].values():
                     if "label" in transition:
                         in_symbol, stack_info = transition["label"].split(
                             " -> ")
                         in_symbol = json.loads(in_symbol)
```

### Comparing `pyformlang-1.0.1/pyformlang/pda/stack_symbol.py` & `pyformlang-1.0.2/pyformlang/pda/stack_symbol.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/pda/state.py` & `pyformlang-1.0.2/pyformlang/pda/state.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/pda/symbol.py` & `pyformlang-1.0.2/pyformlang/pda/symbol.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/pda/tests/test_pda.py` & `pyformlang-1.0.2/pyformlang/pda/tests/test_pda.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/pda/transition_function.py` & `pyformlang-1.0.2/pyformlang/pda/transition_function.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/pda/utils.py` & `pyformlang-1.0.2/pyformlang/pda/utils.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/regular_expression/__init__.py` & `pyformlang-1.0.2/pyformlang/regular_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/regular_expression/python_regex.py` & `pyformlang-1.0.2/pyformlang/regular_expression/python_regex.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/regular_expression/regex.py` & `pyformlang-1.0.2/pyformlang/regular_expression/regex.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/regular_expression/regex_objects.py` & `pyformlang-1.0.2/pyformlang/regular_expression/regex_objects.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/regular_expression/regex_reader.py` & `pyformlang-1.0.2/pyformlang/regular_expression/regex_reader.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/regular_expression/tests/test_python_regex.py` & `pyformlang-1.0.2/pyformlang/regular_expression/tests/test_python_regex.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/regular_expression/tests/test_regex.py` & `pyformlang-1.0.2/pyformlang/regular_expression/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/rsa/__init__.py` & `pyformlang-1.0.2/pyformlang/rsa/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/rsa/box.py` & `pyformlang-1.0.2/pyformlang/rsa/box.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/rsa/recursive_automaton.py` & `pyformlang-1.0.2/pyformlang/rsa/recursive_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang/rsa/tests/test_rsa.py` & `pyformlang-1.0.2/pyformlang/rsa/tests/test_rsa.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.1/pyformlang.egg-info/PKG-INFO` & `pyformlang-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pyformlang
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python framework for formal grammars
 Home-page: https://github.com/Aunsiels/pyformlang
 Author: Julien Romero
 Author-email: romerojulien34@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyformlang
 
-[![Build Status](https://jenkins.r2.enst.fr/job/pyformlang/job/master/badge/icon)](https://jenkins.r2.enst.fr/job/pyformlang/job/master/)
+[![Python package](https://github.com/Aunsiels/pyformlang/actions/workflows/python-package.yml/badge.svg)](https://github.com/Aunsiels/pyformlang/actions/workflows/python-package.yml)
 [![pypi](https://img.shields.io/pypi/v/pyformlang.svg)](https://pypi.org/project/pyformlang/)
 [![Documentation](https://readthedocs.org/projects/pyformlang/badge/?version=latest)](https://pyformlang.readthedocs.io/en/latest/)
+![badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Aunsiels/135f01c630063c3e69d999a2edf59fdb/raw/coverage_pyformlang.json)
+
 
 A python library to manipulate formal grammar. In general, it can be used to better understand algorithms in a formal way.
 
 If you use Pyformlang in your project, please cite our paper:
 
 ```
 @InProceedings{pyformlang,
@@ -50,9 +50,7 @@
 
 [Intersection CFG/Regex](https://www.degruyter.com/downloadpdf/j/stuf.1961.14.issue-1-4/stuf.1961.14.14.143/stuf.1961.14.14.143.pdf) and [a better written version](http://www.cs.umd.edu/~gasarch/BLOGPAPERS/cfg.pdf)
 
 ## Usage
 
 Please refer to the official documentation: [pyformlang.readthedocs.io](https://pyformlang.readthedocs.io).
 
-
-
```

### Comparing `pyformlang-1.0.1/pyformlang.egg-info/SOURCES.txt` & `pyformlang-1.0.2/pyformlang.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,22 @@
 pyformlang/cfg/tests/__init__.py
 pyformlang/cfg/tests/test_cfg.py
 pyformlang/cfg/tests/test_llone_parser.py
 pyformlang/cfg/tests/test_production.py
 pyformlang/cfg/tests/test_recursive_decent_parser.py
 pyformlang/cfg/tests/test_terminal.py
 pyformlang/cfg/tests/test_variable.py
+pyformlang/fcfg/__init__.py
+pyformlang/fcfg/fcfg.py
+pyformlang/fcfg/feature_production.py
+pyformlang/fcfg/feature_structure.py
+pyformlang/fcfg/state.py
+pyformlang/fcfg/tests/__init__.py
+pyformlang/fcfg/tests/test_fcfg.py
+pyformlang/fcfg/tests/test_feature_structure.py
 pyformlang/finite_automaton/__init__.py
 pyformlang/finite_automaton/deterministic_finite_automaton.py
 pyformlang/finite_automaton/doubly_linked_list.py
 pyformlang/finite_automaton/doubly_linked_node.py
 pyformlang/finite_automaton/epsilon.py
 pyformlang/finite_automaton/epsilon_nfa.py
 pyformlang/finite_automaton/finite_automaton.py
```

### Comparing `pyformlang-1.0.1/setup.py` & `pyformlang-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "networkx",
     "numpy",
     "pydot"
 ]
 
 setuptools.setup(
     name='pyformlang',
-    version='1.0.1',
+    version='1.0.2',
     #scripts=['pyformlang'] ,
     author="Julien Romero",
     author_email="romerojulien34@gmail.com",
     description="A python framework for formal grammars",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Aunsiels/pyformlang",
```

