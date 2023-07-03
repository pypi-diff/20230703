# Comparing `tmp/pydantic_core-2.0.1.tar.gz` & `tmp/pydantic_core-2.0.2.tar.gz`

## Comparing `pydantic_core-2.0.1.tar` & `pydantic_core-2.0.2.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 pydantic_core-2.0.1/Cargo.toml
--rw-r--r--   0     1001      123      312 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/.cargo/config.toml
--rw-r--r--   0     1001      123     1080 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/LICENSE
--rw-r--r--   0     1001      123     3745 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/Makefile
--rw-r--r--   0     1001      123     3708 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/README.md
--rw-r--r--   0     1001      123     1366 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/build.rs
--rw-r--r--   0     1001      123     8313 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/generate_self_schema.py
--rw-r--r--   0     1001      123     3150 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/pyproject.toml
--rw-r--r--   0     1001      123     3065 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/argument_markers.rs
--rw-r--r--   0     1001      123     5811 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/build_tools.rs
--rw-r--r--   0     1001      123     4486 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/definitions.rs
--rw-r--r--   0     1001      123     5441 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/errors/line_error.rs
--rw-r--r--   0     1001      123     7101 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/errors/location.rs
--rw-r--r--   0     1001      123     1065 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/errors/mod.rs
--rw-r--r--   0     1001      123    32685 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/errors/types.rs
--rw-r--r--   0     1001      123    16290 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/errors/validation_exception.rs
--rw-r--r--   0     1001      123     5046 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/errors/value_exception.rs
--rw-r--r--   0     1001      123    13991 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/input/datetime.rs
--rw-r--r--   0     1001      123     8292 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/input/input_abstract.rs
--rw-r--r--   0     1001      123    17728 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/input/input_json.rs
--rw-r--r--   0     1001      123    26556 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/input/input_python.rs
--rw-r--r--   0     1001      123      956 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/input/mod.rs
--rw-r--r--   0     1001      123     5342 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/input/parse_json.rs
--rw-r--r--   0     1001      123    31974 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/input/return_enums.rs
--rw-r--r--   0     1001      123     3426 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/input/shared.rs
--rw-r--r--   0     1001      123     1756 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/lazy_index_map.rs
--rw-r--r--   0     1001      123     2569 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/lib.rs
--rw-r--r--   0     1001      123    17853 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/lookup_key.rs
--rw-r--r--   0     1001      123     2138 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/recursion_guard.rs
--rw-r--r--   0     1001      123     5605 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/computed_fields.rs
--rw-r--r--   0     1001      123     5486 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/config.rs
--rw-r--r--   0     1001      123     2779 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/errors.rs
--rw-r--r--   0     1001      123    12020 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/extra.rs
--rw-r--r--   0     1001      123    12054 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/fields.rs
--rw-r--r--   0     1001      123    14578 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/filter.rs
--rw-r--r--   0     1001      123    25370 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/infer.rs
--rw-r--r--   0     1001      123     7814 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/mod.rs
--rw-r--r--   0     1001      123    11222 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/ob_type.rs
--rw-r--r--   0     1001      123    14829 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/shared.rs
--rw-r--r--   0     1001      123     1419 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/any.rs
--rw-r--r--   0     1001      123     2507 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/bytes.rs
--rw-r--r--   0     1001      123     6558 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/dataclass.rs
--rw-r--r--   0     1001      123     3921 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/datetime_etc.rs
--rw-r--r--   0     1001      123     3226 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/definitions.rs
--rw-r--r--   0     1001      123     5250 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/dict.rs
--rw-r--r--   0     1001      123     6534 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/format.rs
--rw-r--r--   0     1001      123    22198 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/function.rs
--rw-r--r--   0     1001      123     7344 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/generator.rs
--rw-r--r--   0     1001      123     2961 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/json.rs
--rw-r--r--   0     1001      123     2196 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/json_or_python.rs
--rw-r--r--   0     1001      123     4053 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/list.rs
--rw-r--r--   0     1001      123     5517 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/literal.rs
--rw-r--r--   0     1001      123     1077 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/mod.rs
--rw-r--r--   0     1001      123     8181 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/model.rs
--rw-r--r--   0     1001      123     2388 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/nullable.rs
--rw-r--r--   0     1001      123     3513 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/other.rs
--rw-r--r--   0     1001      123     4489 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/set_frozenset.rs
--rw-r--r--   0     1001      123     5912 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/simple.rs
--rw-r--r--   0     1001      123     2576 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/string.rs
--rw-r--r--   0     1001      123     2464 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/timedelta.rs
--rw-r--r--   0     1001      123    12727 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/tuple.rs
--rw-r--r--   0     1001      123     2482 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/typed_dict.rs
--rw-r--r--   0     1001      123     6947 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/union.rs
--rw-r--r--   0     1001      123     3114 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/url.rs
--rw-r--r--   0     1001      123     2054 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/serializers/type_serializers/with_default.rs
--rw-r--r--   0     1001      123     2736 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/tools.rs
--rw-r--r--   0     1001      123    11321 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/url.rs
--rw-r--r--   0     1001      123     1468 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/any.rs
--rw-r--r--   0     1001      123    15665 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/arguments.rs
--rw-r--r--   0     1001      123     1662 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/bool.rs
--rw-r--r--   0     1001      123     3769 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/bytes.rs
--rw-r--r--   0     1001      123     4399 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/call.rs
--rw-r--r--   0     1001      123     1504 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/callable.rs
--rw-r--r--   0     1001      123     3391 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/chain.rs
--rw-r--r--   0     1001      123     3928 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/custom_error.rs
--rw-r--r--   0     1001      123    25171 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/dataclass.rs
--rw-r--r--   0     1001      123     7033 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/date.rs
--rw-r--r--   0     1001      123     9231 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/datetime.rs
--rw-r--r--   0     1001      123     7156 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/definitions.rs
--rw-r--r--   0     1001      123     6528 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/dict.rs
--rw-r--r--   0     1001      123     6276 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/float.rs
--rw-r--r--   0     1001      123     2035 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/frozenset.rs
--rw-r--r--   0     1001      123    18983 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/function.rs
--rw-r--r--   0     1001      123    11243 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/generator.rs
--rw-r--r--   0     1001      123     4929 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/int.rs
--rw-r--r--   0     1001      123     3256 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/is_instance.rs
--rw-r--r--   0     1001      123     2201 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/is_subclass.rs
--rw-r--r--   0     1001      123     2600 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/json.rs
--rw-r--r--   0     1001      123     2568 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/json_or_python.rs
--rw-r--r--   0     1001      123     2752 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/lax_or_strict.rs
--rw-r--r--   0     1001      123     5826 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/list.rs
--rw-r--r--   0     1001      123     6500 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/literal.rs
--rw-r--r--   0     1001      123    23627 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/mod.rs
--rw-r--r--   0     1001      123    15066 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/model.rs
--rw-r--r--   0     1001      123    17037 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/model_fields.rs
--rw-r--r--   0     1001      123     1477 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/none.rs
--rw-r--r--   0     1001      123     1953 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/nullable.rs
--rw-r--r--   0     1001      123     3158 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/set.rs
--rw-r--r--   0     1001      123     6190 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/string.rs
--rw-r--r--   0     1001      123     3888 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/time.rs
--rw-r--r--   0     1001      123     3875 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/timedelta.rs
--rw-r--r--   0     1001      123     9993 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/tuple.rs
--rw-r--r--   0     1001      123    12754 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/typed_dict.rs
--rw-r--r--   0     1001      123    16840 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/union.rs
--rw-r--r--   0     1001      123    17932 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/url.rs
--rw-r--r--   0     1001      123     6970 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/src/validators/with_default.rs
--rw-r--r--   0     1001      123        0 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/__init__.py
--rw-r--r--   0     1001      123    23377 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/benchmarks/README.md
--rw-r--r--   0     1001      123        0 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/benchmarks/__init__.py
--rw-r--r--   0     1001      123    18351 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/benchmarks/complete_schema.py
--rw-r--r--   0     1001      123     6636 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/benchmarks/test_complete_benchmark.py
--rw-r--r--   0     1001      123    45917 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/benchmarks/test_micro_benchmarks.py
--rw-r--r--   0     1001      123    16670 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/benchmarks/test_serialization_micro.py
--rw-r--r--   0     1001      123     3950 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/conftest.py
--rw-r--r--   0     1001      123     3272 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/emscripten_runner.js
--rw-r--r--   0     1001      123       72 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/requirements-linting.txt
--rw-r--r--   0     1001      123      229 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/requirements.txt
--rw-r--r--   0     1001      123        0 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/__init__.py
--rw-r--r--   0     1001      123    23407 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_any.py
--rw-r--r--   0     1001      123     4342 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_bytes.py
--rw-r--r--   0     1001      123     5571 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_dataclasses.py
--rw-r--r--   0     1001      123     4798 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_datetime.py
--rw-r--r--   0     1001      123     3901 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_definitions.py
--rw-r--r--   0     1001      123     4164 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_definitions_recursive.py
--rw-r--r--   0     1001      123     7509 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_dict.py
--rw-r--r--   0     1001      123     4659 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_format.py
--rw-r--r--   0     1001      123    22938 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_functions.py
--rw-r--r--   0     1001      123     5424 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_generator.py
--rw-r--r--   0     1001      123     1853 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_json.py
--rw-r--r--   0     1001      123      540 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_json_or_python.py
--rw-r--r--   0     1001      123    18385 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_list_tuple.py
--rw-r--r--   0     1001      123     2172 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_literal.py
--rw-r--r--   0     1001      123      517 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_misc.py
--rw-r--r--   0     1001      123    32725 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_model.py
--rw-r--r--   0     1001      123     5749 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_model_root.py
--rw-r--r--   0     1001      123      953 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_none.py
--rw-r--r--   0     1001      123      566 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_nullable.py
--rw-r--r--   0     1001      123     2174 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_other.py
--rw-r--r--   0     1001      123     2052 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_set_frozenset.py
--rw-r--r--   0     1001      123     2172 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_simple.py
--rw-r--r--   0     1001      123     2503 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_string.py
--rw-r--r--   0     1001      123     1665 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_timedelta.py
--rw-r--r--   0     1001      123    12753 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_typed_dict.py
--rw-r--r--   0     1001      123    13375 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_union.py
--rw-r--r--   0     1001      123     4287 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/serializers/test_url.py
--rw-r--r--   0     1001      123     2065 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test.rs
--rw-r--r--   0     1001      123     4756 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_build.py
--rw-r--r--   0     1001      123     4675 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_config.py
--rw-r--r--   0     1001      123     1246 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_docstrings.py
--rw-r--r--   0     1001      123    27365 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_errors.py
--rw-r--r--   0     1001      123     2187 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_garbage_collection.py
--rw-r--r--   0     1001      123     6159 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_hypothesis.py
--rw-r--r--   0     1001      123     2184 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_isinstance.py
--rw-r--r--   0     1001      123    11414 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_json.py
--rw-r--r--   0     1001      123     6242 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_misc.py
--rw-r--r--   0     1001      123    12707 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_schema_functions.py
--rw-r--r--   0     1001      123     1795 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_strict.py
--rw-r--r--   0     1001      123     9150 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_typing.py
--rw-r--r--   0     1001      123     5013 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/test_validation_context.py
--rw-r--r--   0     1001      123        0 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/__init__.py
--rw-r--r--   0     1001      123    35668 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_arguments.py
--rw-r--r--   0     1001      123     4100 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_bool.py
--rw-r--r--   0     1001      123     4396 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_bytes.py
--rw-r--r--   0     1001      123     7161 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_call.py
--rw-r--r--   0     1001      123     1492 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_callable.py
--rw-r--r--   0     1001      123     4083 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_chain.py
--rw-r--r--   0     1001      123     1699 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_custom_error.py
--rw-r--r--   0     1001      123    50500 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_dataclasses.py
--rw-r--r--   0     1001      123    12120 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_date.py
--rw-r--r--   0     1001      123    20089 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_datetime.py
--rw-r--r--   0     1001      123     4913 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_definitions.py
--rw-r--r--   0     1001      123    31709 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_definitions_recursive.py
--rw-r--r--   0     1001      123     9074 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_dict.py
--rw-r--r--   0     1001      123    11686 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_float.py
--rw-r--r--   0     1001      123    11389 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_frozenset.py
--rw-r--r--   0     1001      123    29984 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_function.py
--rw-r--r--   0     1001      123     6819 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_generator.py
--rw-r--r--   0     1001      123    14047 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_int.py
--rw-r--r--   0     1001      123     5119 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_is_instance.py
--rw-r--r--   0     1001      123     2065 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_is_subclass.py
--rw-r--r--   0     1001      123     5260 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_json.py
--rw-r--r--   0     1001      123     1027 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_json_or_python.py
--rw-r--r--   0     1001      123     1640 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_lax_or_strict.py
--rw-r--r--   0     1001      123    16717 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_list.py
--rw-r--r--   0     1001      123    12324 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_literal.py
--rw-r--r--   0     1001      123    38914 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_model.py
--rw-r--r--   0     1001      123    62068 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_model_fields.py
--rw-r--r--   0     1001      123    13996 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_model_init.py
--rw-r--r--   0     1001      123     7100 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_model_root.py
--rw-r--r--   0     1001      123      760 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_none.py
--rw-r--r--   0     1001      123     1056 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_nullable.py
--rw-r--r--   0     1001      123    10405 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_set.py
--rw-r--r--   0     1001      123     8318 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_string.py
--rw-r--r--   0     1001      123    22574 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_tagged_union.py
--rw-r--r--   0     1001      123    12215 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_time.py
--rw-r--r--   0     1001      123    12328 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_timedelta.py
--rw-r--r--   0     1001      123    18166 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_tuple.py
--rw-r--r--   0     1001      123    41928 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_typed_dict.py
--rw-r--r--   0     1001      123    15395 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_union.py
--rw-r--r--   0     1001      123    53089 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_url.py
--rw-r--r--   0     1001      123    21767 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/tests/validators/test_with_default.py
--rw-r--r--   0     1001      123    16495 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/Cargo.lock
--rw-r--r--   0     1001      123   127915 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/python/pydantic_core/core_schema.py
--rw-r--r--   0     1001      123     8728 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/python/pydantic_core/_pydantic_core.pyi
--rw-r--r--   0     1001      123     2190 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/python/pydantic_core/__init__.py
--rw-r--r--   0     1001      123        1 2023-06-30 14:01:23.000000 pydantic_core-2.0.1/python/pydantic_core/py.typed
--rw-r--r--   0        0        0     5195 1970-01-01 00:00:00.000000 pydantic_core-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 pydantic_core-2.0.2/Cargo.toml
+-rw-r--r--   0     1001      123      312 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/.cargo/config.toml
+-rw-r--r--   0     1001      123     1080 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/LICENSE
+-rw-r--r--   0     1001      123     3745 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/Makefile
+-rw-r--r--   0     1001      123     3708 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/README.md
+-rw-r--r--   0     1001      123     1366 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/build.rs
+-rw-r--r--   0     1001      123     8313 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/generate_self_schema.py
+-rw-r--r--   0     1001      123     2918 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/pyproject.toml
+-rw-r--r--   0     1001      123     3065 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/argument_markers.rs
+-rw-r--r--   0     1001      123     5811 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/build_tools.rs
+-rw-r--r--   0     1001      123     4486 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/definitions.rs
+-rw-r--r--   0     1001      123     5441 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/errors/line_error.rs
+-rw-r--r--   0     1001      123     7101 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/errors/location.rs
+-rw-r--r--   0     1001      123     1065 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/errors/mod.rs
+-rw-r--r--   0     1001      123    32685 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/errors/types.rs
+-rw-r--r--   0     1001      123    16290 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/errors/validation_exception.rs
+-rw-r--r--   0     1001      123     5046 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/errors/value_exception.rs
+-rw-r--r--   0     1001      123    13991 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/input/datetime.rs
+-rw-r--r--   0     1001      123     8292 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/input/input_abstract.rs
+-rw-r--r--   0     1001      123    17728 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/input/input_json.rs
+-rw-r--r--   0     1001      123    26556 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/input/input_python.rs
+-rw-r--r--   0     1001      123      956 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/input/mod.rs
+-rw-r--r--   0     1001      123     5342 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/input/parse_json.rs
+-rw-r--r--   0     1001      123    31974 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/input/return_enums.rs
+-rw-r--r--   0     1001      123     3426 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/input/shared.rs
+-rw-r--r--   0     1001      123     1756 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/lazy_index_map.rs
+-rw-r--r--   0     1001      123     2569 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/lib.rs
+-rw-r--r--   0     1001      123    17853 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/lookup_key.rs
+-rw-r--r--   0     1001      123     2138 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/recursion_guard.rs
+-rw-r--r--   0     1001      123     5605 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/computed_fields.rs
+-rw-r--r--   0     1001      123     5486 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/config.rs
+-rw-r--r--   0     1001      123     2779 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/errors.rs
+-rw-r--r--   0     1001      123    12020 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/extra.rs
+-rw-r--r--   0     1001      123    12054 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/fields.rs
+-rw-r--r--   0     1001      123    14578 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/filter.rs
+-rw-r--r--   0     1001      123    25370 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/infer.rs
+-rw-r--r--   0     1001      123     7814 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/mod.rs
+-rw-r--r--   0     1001      123    11222 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/ob_type.rs
+-rw-r--r--   0     1001      123    14829 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/shared.rs
+-rw-r--r--   0     1001      123     1419 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/any.rs
+-rw-r--r--   0     1001      123     2507 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/bytes.rs
+-rw-r--r--   0     1001      123     6558 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/dataclass.rs
+-rw-r--r--   0     1001      123     3921 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/datetime_etc.rs
+-rw-r--r--   0     1001      123     3226 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/definitions.rs
+-rw-r--r--   0     1001      123     5250 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/dict.rs
+-rw-r--r--   0     1001      123     6534 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/format.rs
+-rw-r--r--   0     1001      123    22198 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/function.rs
+-rw-r--r--   0     1001      123     7344 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/generator.rs
+-rw-r--r--   0     1001      123     2961 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/json.rs
+-rw-r--r--   0     1001      123     2196 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/json_or_python.rs
+-rw-r--r--   0     1001      123     4053 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/list.rs
+-rw-r--r--   0     1001      123     5517 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/literal.rs
+-rw-r--r--   0     1001      123     1077 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/mod.rs
+-rw-r--r--   0     1001      123     8181 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/model.rs
+-rw-r--r--   0     1001      123     2388 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/nullable.rs
+-rw-r--r--   0     1001      123     3513 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/other.rs
+-rw-r--r--   0     1001      123     4489 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/set_frozenset.rs
+-rw-r--r--   0     1001      123     5912 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/simple.rs
+-rw-r--r--   0     1001      123     2576 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/string.rs
+-rw-r--r--   0     1001      123     2464 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/timedelta.rs
+-rw-r--r--   0     1001      123    12727 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/tuple.rs
+-rw-r--r--   0     1001      123     2482 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/typed_dict.rs
+-rw-r--r--   0     1001      123     6947 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/union.rs
+-rw-r--r--   0     1001      123     3114 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/url.rs
+-rw-r--r--   0     1001      123     2054 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/serializers/type_serializers/with_default.rs
+-rw-r--r--   0     1001      123     2736 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/tools.rs
+-rw-r--r--   0     1001      123    11321 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/url.rs
+-rw-r--r--   0     1001      123     1468 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/any.rs
+-rw-r--r--   0     1001      123    15665 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/arguments.rs
+-rw-r--r--   0     1001      123     1662 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/bool.rs
+-rw-r--r--   0     1001      123     3769 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/bytes.rs
+-rw-r--r--   0     1001      123     4399 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/call.rs
+-rw-r--r--   0     1001      123     1504 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/callable.rs
+-rw-r--r--   0     1001      123     3391 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/chain.rs
+-rw-r--r--   0     1001      123     3928 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/custom_error.rs
+-rw-r--r--   0     1001      123    25171 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/dataclass.rs
+-rw-r--r--   0     1001      123     7033 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/date.rs
+-rw-r--r--   0     1001      123     9231 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/datetime.rs
+-rw-r--r--   0     1001      123     7156 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/definitions.rs
+-rw-r--r--   0     1001      123     6528 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/dict.rs
+-rw-r--r--   0     1001      123     6276 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/float.rs
+-rw-r--r--   0     1001      123     2035 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/frozenset.rs
+-rw-r--r--   0     1001      123    18983 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/function.rs
+-rw-r--r--   0     1001      123    11243 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/generator.rs
+-rw-r--r--   0     1001      123     4929 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/int.rs
+-rw-r--r--   0     1001      123     3256 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/is_instance.rs
+-rw-r--r--   0     1001      123     2201 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/is_subclass.rs
+-rw-r--r--   0     1001      123     2600 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/json.rs
+-rw-r--r--   0     1001      123     2568 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/json_or_python.rs
+-rw-r--r--   0     1001      123     2752 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/lax_or_strict.rs
+-rw-r--r--   0     1001      123     5826 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/list.rs
+-rw-r--r--   0     1001      123     6500 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/literal.rs
+-rw-r--r--   0     1001      123    23627 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/mod.rs
+-rw-r--r--   0     1001      123    15066 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/model.rs
+-rw-r--r--   0     1001      123    17147 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/model_fields.rs
+-rw-r--r--   0     1001      123     1477 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/none.rs
+-rw-r--r--   0     1001      123     1953 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/nullable.rs
+-rw-r--r--   0     1001      123     3158 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/set.rs
+-rw-r--r--   0     1001      123     6190 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/string.rs
+-rw-r--r--   0     1001      123     3888 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/time.rs
+-rw-r--r--   0     1001      123     3875 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/timedelta.rs
+-rw-r--r--   0     1001      123     9993 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/tuple.rs
+-rw-r--r--   0     1001      123    12754 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/typed_dict.rs
+-rw-r--r--   0     1001      123    16840 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/union.rs
+-rw-r--r--   0     1001      123    17932 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/url.rs
+-rw-r--r--   0     1001      123     6970 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/src/validators/with_default.rs
+-rw-r--r--   0     1001      123        0 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/__init__.py
+-rw-r--r--   0     1001      123    23377 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/benchmarks/README.md
+-rw-r--r--   0     1001      123        0 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/benchmarks/__init__.py
+-rw-r--r--   0     1001      123    18351 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/benchmarks/complete_schema.py
+-rw-r--r--   0     1001      123     6636 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/benchmarks/test_complete_benchmark.py
+-rw-r--r--   0     1001      123    45917 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/benchmarks/test_micro_benchmarks.py
+-rw-r--r--   0     1001      123    16670 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/benchmarks/test_serialization_micro.py
+-rw-r--r--   0     1001      123     3950 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/conftest.py
+-rw-r--r--   0     1001      123     3272 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/emscripten_runner.js
+-rw-r--r--   0     1001      123       72 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/requirements-linting.txt
+-rw-r--r--   0     1001      123      229 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/requirements.txt
+-rw-r--r--   0     1001      123        0 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/__init__.py
+-rw-r--r--   0     1001      123    23407 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_any.py
+-rw-r--r--   0     1001      123     4342 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_bytes.py
+-rw-r--r--   0     1001      123     5571 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_dataclasses.py
+-rw-r--r--   0     1001      123     4798 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_datetime.py
+-rw-r--r--   0     1001      123     3901 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_definitions.py
+-rw-r--r--   0     1001      123     4164 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_definitions_recursive.py
+-rw-r--r--   0     1001      123     7509 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_dict.py
+-rw-r--r--   0     1001      123     4659 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_format.py
+-rw-r--r--   0     1001      123    22938 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_functions.py
+-rw-r--r--   0     1001      123     5424 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_generator.py
+-rw-r--r--   0     1001      123     1853 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_json.py
+-rw-r--r--   0     1001      123      540 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_json_or_python.py
+-rw-r--r--   0     1001      123    18385 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_list_tuple.py
+-rw-r--r--   0     1001      123     2172 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_literal.py
+-rw-r--r--   0     1001      123      517 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_misc.py
+-rw-r--r--   0     1001      123    32725 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_model.py
+-rw-r--r--   0     1001      123     5749 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_model_root.py
+-rw-r--r--   0     1001      123      953 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_none.py
+-rw-r--r--   0     1001      123      566 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_nullable.py
+-rw-r--r--   0     1001      123     2174 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_other.py
+-rw-r--r--   0     1001      123     2052 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_set_frozenset.py
+-rw-r--r--   0     1001      123     2172 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_simple.py
+-rw-r--r--   0     1001      123     2503 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_string.py
+-rw-r--r--   0     1001      123     1665 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_timedelta.py
+-rw-r--r--   0     1001      123    12753 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_typed_dict.py
+-rw-r--r--   0     1001      123    13375 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_union.py
+-rw-r--r--   0     1001      123     4287 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/serializers/test_url.py
+-rw-r--r--   0     1001      123     2065 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test.rs
+-rw-r--r--   0     1001      123     4756 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_build.py
+-rw-r--r--   0     1001      123     4675 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_config.py
+-rw-r--r--   0     1001      123     1246 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_docstrings.py
+-rw-r--r--   0     1001      123    27365 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_errors.py
+-rw-r--r--   0     1001      123     2187 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_garbage_collection.py
+-rw-r--r--   0     1001      123     6159 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_hypothesis.py
+-rw-r--r--   0     1001      123     2184 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_isinstance.py
+-rw-r--r--   0     1001      123    11414 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_json.py
+-rw-r--r--   0     1001      123     6242 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_misc.py
+-rw-r--r--   0     1001      123    12707 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_schema_functions.py
+-rw-r--r--   0     1001      123     1795 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_strict.py
+-rw-r--r--   0     1001      123     9150 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_typing.py
+-rw-r--r--   0     1001      123     5013 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/test_validation_context.py
+-rw-r--r--   0     1001      123        0 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/__init__.py
+-rw-r--r--   0     1001      123    35668 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_arguments.py
+-rw-r--r--   0     1001      123     4100 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_bool.py
+-rw-r--r--   0     1001      123     4396 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_bytes.py
+-rw-r--r--   0     1001      123     7161 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_call.py
+-rw-r--r--   0     1001      123     1492 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_callable.py
+-rw-r--r--   0     1001      123     4083 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_chain.py
+-rw-r--r--   0     1001      123     1699 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_custom_error.py
+-rw-r--r--   0     1001      123    50500 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_dataclasses.py
+-rw-r--r--   0     1001      123    12120 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_date.py
+-rw-r--r--   0     1001      123    20089 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_datetime.py
+-rw-r--r--   0     1001      123     4913 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_definitions.py
+-rw-r--r--   0     1001      123    31709 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_definitions_recursive.py
+-rw-r--r--   0     1001      123     9074 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_dict.py
+-rw-r--r--   0     1001      123    11686 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_float.py
+-rw-r--r--   0     1001      123    11389 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_frozenset.py
+-rw-r--r--   0     1001      123    29984 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_function.py
+-rw-r--r--   0     1001      123     6819 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_generator.py
+-rw-r--r--   0     1001      123    14047 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_int.py
+-rw-r--r--   0     1001      123     5119 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_is_instance.py
+-rw-r--r--   0     1001      123     2065 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_is_subclass.py
+-rw-r--r--   0     1001      123     5260 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_json.py
+-rw-r--r--   0     1001      123     1027 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_json_or_python.py
+-rw-r--r--   0     1001      123     1640 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_lax_or_strict.py
+-rw-r--r--   0     1001      123    16717 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_list.py
+-rw-r--r--   0     1001      123    12324 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_literal.py
+-rw-r--r--   0     1001      123    38914 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_model.py
+-rw-r--r--   0     1001      123    62070 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_model_fields.py
+-rw-r--r--   0     1001      123    13996 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_model_init.py
+-rw-r--r--   0     1001      123     7100 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_model_root.py
+-rw-r--r--   0     1001      123      760 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_none.py
+-rw-r--r--   0     1001      123     1056 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_nullable.py
+-rw-r--r--   0     1001      123    10405 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_set.py
+-rw-r--r--   0     1001      123     8318 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_string.py
+-rw-r--r--   0     1001      123    22574 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_tagged_union.py
+-rw-r--r--   0     1001      123    12215 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_time.py
+-rw-r--r--   0     1001      123    12328 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_timedelta.py
+-rw-r--r--   0     1001      123    18166 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_tuple.py
+-rw-r--r--   0     1001      123    41928 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_typed_dict.py
+-rw-r--r--   0     1001      123    15395 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_union.py
+-rw-r--r--   0     1001      123    53089 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_url.py
+-rw-r--r--   0     1001      123    21767 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/tests/validators/test_with_default.py
+-rw-r--r--   0     1001      123    16495 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/Cargo.lock
+-rw-r--r--   0     1001      123   127915 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/python/pydantic_core/core_schema.py
+-rw-r--r--   0     1001      123     8728 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/python/pydantic_core/_pydantic_core.pyi
+-rw-r--r--   0     1001      123     2190 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/python/pydantic_core/__init__.py
+-rw-r--r--   0     1001      123        1 2023-07-03 01:49:45.000000 pydantic_core-2.0.2/python/pydantic_core/py.typed
+-rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 pydantic_core-2.0.2/PKG-INFO
```

### Comparing `pydantic_core-2.0.1/Cargo.toml` & `pydantic_core-2.0.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pydantic-core"
-version = "2.0.1"
+version = "2.0.2"
 edition = "2021"
 license = "MIT"
 homepage = "https://github.com/pydantic/pydantic-core"
 repository = "https://github.com/pydantic/pydantic-core.git"
 readme = "README.md"
 include = [
     "/pyproject.toml",
```

### Comparing `pydantic_core-2.0.1/LICENSE` & `pydantic_core-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/Makefile` & `pydantic_core-2.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/README.md` & `pydantic_core-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/build.rs` & `pydantic_core-2.0.2/build.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/generate_self_schema.py` & `pydantic_core-2.0.2/generate_self_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/pyproject.toml` & `pydantic_core-2.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [build-system]
 requires = [
     'maturin>=1,<2',
-    'typing-extensions >=4.6.0; platform_python_implementation != "PyPy"',
-    'typing-extensions >=4.6.0,<4.7.0; platform_python_implementation == "PyPy"'
+    'typing-extensions >=4.6.0,!=4.7.0'
 ]
 build-backend = 'maturin'
 
 [project]
 name = 'pydantic_core'
 requires-python = '>=3.7'
 authors = [
@@ -29,16 +28,15 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: POSIX :: Linux',
     'Operating System :: Microsoft :: Windows',
     'Operating System :: MacOS',
     'Typing :: Typed',
 ]
 dependencies = [
-    'typing-extensions >=4.6.0; platform_python_implementation != "PyPy"',
-    'typing-extensions >=4.6.0,<4.7.0; platform_python_implementation == "PyPy"'
+    'typing-extensions >=4.6.0,!=4.7.0'
 ]
 dynamic = [
     'description',
     'license',
     'readme',
     'version'
 ]
```

### Comparing `pydantic_core-2.0.1/src/argument_markers.rs` & `pydantic_core-2.0.2/src/argument_markers.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/build_tools.rs` & `pydantic_core-2.0.2/src/build_tools.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/definitions.rs` & `pydantic_core-2.0.2/src/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/errors/line_error.rs` & `pydantic_core-2.0.2/src/errors/line_error.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/errors/location.rs` & `pydantic_core-2.0.2/src/errors/location.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/errors/mod.rs` & `pydantic_core-2.0.2/src/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/errors/types.rs` & `pydantic_core-2.0.2/src/errors/types.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/errors/validation_exception.rs` & `pydantic_core-2.0.2/src/errors/validation_exception.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/errors/value_exception.rs` & `pydantic_core-2.0.2/src/errors/value_exception.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/input/datetime.rs` & `pydantic_core-2.0.2/src/input/datetime.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/input/input_abstract.rs` & `pydantic_core-2.0.2/src/input/input_abstract.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/input/input_json.rs` & `pydantic_core-2.0.2/src/input/input_json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/input/input_python.rs` & `pydantic_core-2.0.2/src/input/input_python.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/input/mod.rs` & `pydantic_core-2.0.2/src/input/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/input/parse_json.rs` & `pydantic_core-2.0.2/src/input/parse_json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/input/return_enums.rs` & `pydantic_core-2.0.2/src/input/return_enums.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/input/shared.rs` & `pydantic_core-2.0.2/src/input/shared.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/lazy_index_map.rs` & `pydantic_core-2.0.2/src/lazy_index_map.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/lib.rs` & `pydantic_core-2.0.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/lookup_key.rs` & `pydantic_core-2.0.2/src/lookup_key.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/recursion_guard.rs` & `pydantic_core-2.0.2/src/recursion_guard.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/computed_fields.rs` & `pydantic_core-2.0.2/src/serializers/computed_fields.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/config.rs` & `pydantic_core-2.0.2/src/serializers/config.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/errors.rs` & `pydantic_core-2.0.2/src/serializers/errors.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/extra.rs` & `pydantic_core-2.0.2/src/serializers/extra.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/fields.rs` & `pydantic_core-2.0.2/src/serializers/fields.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/filter.rs` & `pydantic_core-2.0.2/src/serializers/filter.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/infer.rs` & `pydantic_core-2.0.2/src/serializers/infer.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/mod.rs` & `pydantic_core-2.0.2/src/serializers/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/ob_type.rs` & `pydantic_core-2.0.2/src/serializers/ob_type.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/shared.rs` & `pydantic_core-2.0.2/src/serializers/shared.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/any.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/any.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/bytes.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/bytes.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/dataclass.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/dataclass.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/datetime_etc.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/datetime_etc.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/definitions.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/dict.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/format.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/format.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/function.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/function.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/generator.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/generator.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/json.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/json_or_python.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/json_or_python.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/list.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/list.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/literal.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/literal.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/mod.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/model.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/model.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/nullable.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/nullable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/other.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/other.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/set_frozenset.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/set_frozenset.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/simple.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/simple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/string.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/string.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/timedelta.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/timedelta.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/tuple.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/tuple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/typed_dict.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/typed_dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/union.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/union.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/url.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/url.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/serializers/type_serializers/with_default.rs` & `pydantic_core-2.0.2/src/serializers/type_serializers/with_default.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/tools.rs` & `pydantic_core-2.0.2/src/tools.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/url.rs` & `pydantic_core-2.0.2/src/url.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/any.rs` & `pydantic_core-2.0.2/src/validators/any.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/arguments.rs` & `pydantic_core-2.0.2/src/validators/arguments.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/bool.rs` & `pydantic_core-2.0.2/src/validators/bool.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/bytes.rs` & `pydantic_core-2.0.2/src/validators/bytes.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/call.rs` & `pydantic_core-2.0.2/src/validators/call.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/callable.rs` & `pydantic_core-2.0.2/src/validators/callable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/chain.rs` & `pydantic_core-2.0.2/src/validators/chain.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/custom_error.rs` & `pydantic_core-2.0.2/src/validators/custom_error.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/dataclass.rs` & `pydantic_core-2.0.2/src/validators/dataclass.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/date.rs` & `pydantic_core-2.0.2/src/validators/date.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/datetime.rs` & `pydantic_core-2.0.2/src/validators/datetime.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/definitions.rs` & `pydantic_core-2.0.2/src/validators/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/dict.rs` & `pydantic_core-2.0.2/src/validators/dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/float.rs` & `pydantic_core-2.0.2/src/validators/float.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/frozenset.rs` & `pydantic_core-2.0.2/src/validators/frozenset.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/function.rs` & `pydantic_core-2.0.2/src/validators/function.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/generator.rs` & `pydantic_core-2.0.2/src/validators/generator.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/int.rs` & `pydantic_core-2.0.2/src/validators/int.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/is_instance.rs` & `pydantic_core-2.0.2/src/validators/is_instance.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/is_subclass.rs` & `pydantic_core-2.0.2/src/validators/is_subclass.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/json.rs` & `pydantic_core-2.0.2/src/validators/json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/json_or_python.rs` & `pydantic_core-2.0.2/src/validators/json_or_python.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/lax_or_strict.rs` & `pydantic_core-2.0.2/src/validators/lax_or_strict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/list.rs` & `pydantic_core-2.0.2/src/validators/list.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/literal.rs` & `pydantic_core-2.0.2/src/validators/literal.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/mod.rs` & `pydantic_core-2.0.2/src/validators/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/model.rs` & `pydantic_core-2.0.2/src/validators/model.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/model_fields.rs` & `pydantic_core-2.0.2/src/validators/model_fields.rs`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,17 @@
                                 } else {
                                     model_extra_dict.set_item(py_key, value.to_object(py))?;
                                     fields_set_vec.push(py_key.into_py(py));
                                 };
                             }
                         }
                     }
-                    model_extra_dict_op = Some(model_extra_dict);
+                    if matches!(self.extra_behavior, ExtraBehavior::Allow) {
+                        model_extra_dict_op = Some(model_extra_dict);
+                    }
                 }
             }};
         }
         match dict {
             GenericMapping::PyDict(d) => process!(d, py_get_dict_item, DictGenericIterator),
             GenericMapping::PyGetAttr(d, kwargs) => process!(d, py_get_attr, AttributesGenericIterator, kwargs),
             GenericMapping::PyMapping(d) => process!(d, py_get_mapping_item, MappingGenericIterator),
@@ -275,17 +277,17 @@
         }
 
         if !errors.is_empty() {
             Err(ValError::LineErrors(errors))
         } else {
             let fields_set = PySet::new(py, &fields_set_vec)?;
 
-            // if we have extra=allow, but we didn't create a dict because we were validate attributes, set it now
-            // so __pydantic_extra__ is always a dict if extra=allow
-            if model_extra_dict_op.is_none() && matches!(self.extra_behavior, ExtraBehavior::Allow) {
+            // if we have extra=allow, but we didn't create a dict because we were validating
+            // from attributes, set it now so __pydantic_extra__ is always a dict if extra=allow
+            if matches!(self.extra_behavior, ExtraBehavior::Allow) && model_extra_dict_op.is_none() {
                 model_extra_dict_op = Some(PyDict::new(py));
             };
 
             Ok((model_dict, model_extra_dict_op, fields_set).to_object(py))
         }
     }
```

### Comparing `pydantic_core-2.0.1/src/validators/none.rs` & `pydantic_core-2.0.2/src/validators/none.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/nullable.rs` & `pydantic_core-2.0.2/src/validators/nullable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/set.rs` & `pydantic_core-2.0.2/src/validators/set.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/string.rs` & `pydantic_core-2.0.2/src/validators/string.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/time.rs` & `pydantic_core-2.0.2/src/validators/time.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/timedelta.rs` & `pydantic_core-2.0.2/src/validators/timedelta.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/tuple.rs` & `pydantic_core-2.0.2/src/validators/tuple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/typed_dict.rs` & `pydantic_core-2.0.2/src/validators/typed_dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/union.rs` & `pydantic_core-2.0.2/src/validators/union.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/url.rs` & `pydantic_core-2.0.2/src/validators/url.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/src/validators/with_default.rs` & `pydantic_core-2.0.2/src/validators/with_default.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/benchmarks/README.md` & `pydantic_core-2.0.2/tests/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/benchmarks/complete_schema.py` & `pydantic_core-2.0.2/tests/benchmarks/complete_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/benchmarks/test_complete_benchmark.py` & `pydantic_core-2.0.2/tests/benchmarks/test_complete_benchmark.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/benchmarks/test_micro_benchmarks.py` & `pydantic_core-2.0.2/tests/benchmarks/test_micro_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/benchmarks/test_serialization_micro.py` & `pydantic_core-2.0.2/tests/benchmarks/test_serialization_micro.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/conftest.py` & `pydantic_core-2.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/emscripten_runner.js` & `pydantic_core-2.0.2/tests/emscripten_runner.js`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_any.py` & `pydantic_core-2.0.2/tests/serializers/test_any.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_bytes.py` & `pydantic_core-2.0.2/tests/serializers/test_bytes.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_dataclasses.py` & `pydantic_core-2.0.2/tests/serializers/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_datetime.py` & `pydantic_core-2.0.2/tests/serializers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_definitions.py` & `pydantic_core-2.0.2/tests/serializers/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_definitions_recursive.py` & `pydantic_core-2.0.2/tests/serializers/test_definitions_recursive.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_dict.py` & `pydantic_core-2.0.2/tests/serializers/test_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_format.py` & `pydantic_core-2.0.2/tests/serializers/test_format.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_functions.py` & `pydantic_core-2.0.2/tests/serializers/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_generator.py` & `pydantic_core-2.0.2/tests/serializers/test_generator.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_json.py` & `pydantic_core-2.0.2/tests/serializers/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_json_or_python.py` & `pydantic_core-2.0.2/tests/serializers/test_json_or_python.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_list_tuple.py` & `pydantic_core-2.0.2/tests/serializers/test_list_tuple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_literal.py` & `pydantic_core-2.0.2/tests/serializers/test_literal.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_misc.py` & `pydantic_core-2.0.2/tests/serializers/test_misc.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_model.py` & `pydantic_core-2.0.2/tests/serializers/test_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_model_root.py` & `pydantic_core-2.0.2/tests/serializers/test_model_root.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_none.py` & `pydantic_core-2.0.2/tests/serializers/test_none.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_nullable.py` & `pydantic_core-2.0.2/tests/serializers/test_nullable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_other.py` & `pydantic_core-2.0.2/tests/serializers/test_other.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_set_frozenset.py` & `pydantic_core-2.0.2/tests/serializers/test_set_frozenset.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_simple.py` & `pydantic_core-2.0.2/tests/serializers/test_simple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_string.py` & `pydantic_core-2.0.2/tests/serializers/test_string.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_timedelta.py` & `pydantic_core-2.0.2/tests/serializers/test_timedelta.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_typed_dict.py` & `pydantic_core-2.0.2/tests/serializers/test_typed_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_union.py` & `pydantic_core-2.0.2/tests/serializers/test_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/serializers/test_url.py` & `pydantic_core-2.0.2/tests/serializers/test_url.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test.rs` & `pydantic_core-2.0.2/tests/test.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_build.py` & `pydantic_core-2.0.2/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_config.py` & `pydantic_core-2.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_docstrings.py` & `pydantic_core-2.0.2/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_errors.py` & `pydantic_core-2.0.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_garbage_collection.py` & `pydantic_core-2.0.2/tests/test_garbage_collection.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_hypothesis.py` & `pydantic_core-2.0.2/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_isinstance.py` & `pydantic_core-2.0.2/tests/test_isinstance.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_json.py` & `pydantic_core-2.0.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_misc.py` & `pydantic_core-2.0.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_schema_functions.py` & `pydantic_core-2.0.2/tests/test_schema_functions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_strict.py` & `pydantic_core-2.0.2/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_typing.py` & `pydantic_core-2.0.2/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/test_validation_context.py` & `pydantic_core-2.0.2/tests/test_validation_context.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_arguments.py` & `pydantic_core-2.0.2/tests/validators/test_arguments.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_bool.py` & `pydantic_core-2.0.2/tests/validators/test_bool.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_bytes.py` & `pydantic_core-2.0.2/tests/validators/test_bytes.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_call.py` & `pydantic_core-2.0.2/tests/validators/test_call.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_callable.py` & `pydantic_core-2.0.2/tests/validators/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_chain.py` & `pydantic_core-2.0.2/tests/validators/test_chain.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_custom_error.py` & `pydantic_core-2.0.2/tests/validators/test_custom_error.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_dataclasses.py` & `pydantic_core-2.0.2/tests/validators/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_date.py` & `pydantic_core-2.0.2/tests/validators/test_date.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_datetime.py` & `pydantic_core-2.0.2/tests/validators/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_definitions.py` & `pydantic_core-2.0.2/tests/validators/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_definitions_recursive.py` & `pydantic_core-2.0.2/tests/validators/test_definitions_recursive.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_dict.py` & `pydantic_core-2.0.2/tests/validators/test_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_float.py` & `pydantic_core-2.0.2/tests/validators/test_float.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_frozenset.py` & `pydantic_core-2.0.2/tests/validators/test_frozenset.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_function.py` & `pydantic_core-2.0.2/tests/validators/test_function.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_generator.py` & `pydantic_core-2.0.2/tests/validators/test_generator.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_int.py` & `pydantic_core-2.0.2/tests/validators/test_int.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_is_instance.py` & `pydantic_core-2.0.2/tests/validators/test_is_instance.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_is_subclass.py` & `pydantic_core-2.0.2/tests/validators/test_is_subclass.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_json.py` & `pydantic_core-2.0.2/tests/validators/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_json_or_python.py` & `pydantic_core-2.0.2/tests/validators/test_json_or_python.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_lax_or_strict.py` & `pydantic_core-2.0.2/tests/validators/test_lax_or_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_list.py` & `pydantic_core-2.0.2/tests/validators/test_list.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_literal.py` & `pydantic_core-2.0.2/tests/validators/test_literal.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_model.py` & `pydantic_core-2.0.2/tests/validators/test_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_model_fields.py` & `pydantic_core-2.0.2/tests/validators/test_model_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1441,15 +1441,15 @@
     v = py_and_json(
         {
             'type': 'model-fields',
             'extra_behavior': 'forbid',
             'fields': {'field_a': {'type': 'model-field', 'validation_alias': 'FieldA', 'schema': {'type': 'int'}}},
         }
     )
-    assert v.validate_test({'FieldA': 1}) == ({'field_a': 1}, {}, {'field_a'})
+    assert v.validate_test({'FieldA': 1}) == ({'field_a': 1}, None, {'field_a'})
 
 
 def test_with_default_factory():
     v = SchemaValidator(
         {
             'type': 'model-fields',
             'fields': {
```

### Comparing `pydantic_core-2.0.1/tests/validators/test_model_init.py` & `pydantic_core-2.0.2/tests/validators/test_model_init.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_model_root.py` & `pydantic_core-2.0.2/tests/validators/test_model_root.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_none.py` & `pydantic_core-2.0.2/tests/validators/test_none.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_nullable.py` & `pydantic_core-2.0.2/tests/validators/test_nullable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_set.py` & `pydantic_core-2.0.2/tests/validators/test_set.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_string.py` & `pydantic_core-2.0.2/tests/validators/test_string.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_tagged_union.py` & `pydantic_core-2.0.2/tests/validators/test_tagged_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_time.py` & `pydantic_core-2.0.2/tests/validators/test_time.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_timedelta.py` & `pydantic_core-2.0.2/tests/validators/test_timedelta.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_tuple.py` & `pydantic_core-2.0.2/tests/validators/test_tuple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_typed_dict.py` & `pydantic_core-2.0.2/tests/validators/test_typed_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_union.py` & `pydantic_core-2.0.2/tests/validators/test_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_url.py` & `pydantic_core-2.0.2/tests/validators/test_url.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/tests/validators/test_with_default.py` & `pydantic_core-2.0.2/tests/validators/test_with_default.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/Cargo.lock` & `pydantic_core-2.0.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pydantic-core"
-version = "2.0.1"
+version = "2.0.2"
 dependencies = [
  "ahash",
  "base64",
  "enum_dispatch",
  "idna",
  "mimalloc",
  "num-bigint",
```

### Comparing `pydantic_core-2.0.1/python/pydantic_core/core_schema.py` & `pydantic_core-2.0.2/python/pydantic_core/core_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/python/pydantic_core/_pydantic_core.pyi` & `pydantic_core-2.0.2/python/pydantic_core/_pydantic_core.pyi`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/python/pydantic_core/__init__.py` & `pydantic_core-2.0.2/python/pydantic_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.0.1/PKG-INFO` & `pydantic_core-2.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_core
-Version: 2.0.1
+Version: 2.0.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,16 +15,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Typing :: Typed
-Requires-Dist: typing-extensions >=4.6.0 ; platform_python_implementation != 'PyPy'
-Requires-Dist: typing-extensions >=4.6.0, <4.7.0 ; platform_python_implementation == 'PyPy'
+Requires-Dist: typing-extensions >=4.6.0, !=4.7.0
 License-File: LICENSE
 Home-Page: https://github.com/pydantic/pydantic-core
 Author-email: Samuel Colvin <s@muelcolvin.com>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/pydantic/pydantic-core
```

