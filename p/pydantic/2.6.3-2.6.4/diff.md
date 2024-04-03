# Comparing `tmp/pydantic-2.6.3.tar.gz` & `tmp/pydantic-2.6.4.tar.gz`

## Comparing `pydantic-2.6.3.tar` & `pydantic-2.6.4.tar`

### file list

```diff
@@ -1,292 +1,292 @@
--rw-r--r--   0        0        0   180882 2020-02-02 00:00:00.000000 pydantic-2.6.3/HISTORY.md
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 pydantic-2.6.3/Makefile
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 pydantic-2.6.3/README.md
--rw-r--r--   0        0        0    12780 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/__init__.py
--rw-r--r--   0        0        0    11913 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_migration.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/alias_generators.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/aliases.py
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/annotated_handlers.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/class_validators.py
--rw-r--r--   0        0        0    21493 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/color.py
--rw-r--r--   0        0        0    29141 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/config.py
--rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/dataclasses.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/datetime_parse.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/decorator.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/env_settings.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/error_wrappers.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/errors.py
--rw-r--r--   0        0        0    45930 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/fields.py
--rw-r--r--   0        0        0    14621 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/functional_serializers.py
--rw-r--r--   0        0        0    24313 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/functional_validators.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/generics.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/json.py
--rw-r--r--   0        0        0   102807 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/json_schema.py
--rw-r--r--   0        0        0    65892 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/main.py
--rw-r--r--   0        0        0    54695 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/mypy.py
--rw-r--r--   0        0        0    21225 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/networks.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/py.typed
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/root_model.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/schema.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/tools.py
--rw-r--r--   0        0        0    18034 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/type_adapter.py
--rw-r--r--   0        0        0    89607 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/types.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/typing.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/utils.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/validate_call_decorator.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/validators.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/version.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_config.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    24673 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    30627 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_decorators_v1.py
--rw-r--r--   0        0        0    27134 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0    97945 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    22227 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_git.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_internal_dataclass.py
--rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_known_annotated_metadata.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_mock_val_ser.py
--rw-r--r--   0        0        0    28114 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_schema_generation_shared.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_signature.py
--rw-r--r--   0        0        0    29085 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_validate_call.py
--rw-r--r--   0        0        0    10054 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/deprecated/__init__.py
--rw-r--r--   0        0        0     9871 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/deprecated/class_validators.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/deprecated/config.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/deprecated/decorator.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/deprecated/tools.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/plugin/__init__.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/plugin/_loader.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/plugin/_schema_validator.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/__init__.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/_hypothesis_plugin.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/annotated_types.py
--rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/class_validators.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/color.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/config.py
--rw-r--r--   0        0        0    18073 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/dataclasses.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/datetime_parse.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/decorator.py
--rw-r--r--   0        0        0    14039 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/env_settings.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/error_wrappers.py
--rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/errors.py
--rw-r--r--   0        0        0    50485 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/fields.py
--rw-r--r--   0        0        0    17805 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/generics.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/json.py
--rw-r--r--   0        0        0    44376 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/main.py
--rw-r--r--   0        0        0    38745 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/mypy.py
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/networks.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/py.typed
--rw-r--r--   0        0        0    47614 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/schema.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/tools.py
--rw-r--r--   0        0        0    35379 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/types.py
--rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/typing.py
--rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/utils.py
--rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/validators.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydantic-2.6.3/pydantic/v1/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/__init__.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/check_usage_docs.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/conftest.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_abc.py
--rw-r--r--   0        0        0    22099 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_aliases.py
--rw-r--r--   0        0        0    15073 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_annotated.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_assert_in_validators.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_callable.py
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_color.py
--rw-r--r--   0        0        0    22038 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_computed_fields.py
--rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_config.py
--rw-r--r--   0        0        0    14127 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_construction.py
--rw-r--r--   0        0        0    18535 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_create_model.py
--rw-r--r--   0        0        0    78195 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_dataclasses.py
--rw-r--r--   0        0        0    22681 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_datetime.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_decorators.py
--rw-r--r--   0        0        0    24974 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_deprecated.py
--rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_deprecated_validate_arguments.py
--rw-r--r--   0        0        0    71553 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_discriminated_union.py
--rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_docs.py
--rw-r--r--   0        0        0    83621 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_edge_cases.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_errors.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_exports.py
--rwxr-xr-x   0        0        0      748 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_fastapi.sh
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_fastapi_json_schema.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_fields.py
--rw-r--r--   0        0        0    30168 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_forward_ref.py
--rw-r--r--   0        0        0    84716 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_generics.py
--rw-r--r--   0        0        0     8025 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_internal.py
--rw-r--r--   0        0        0    16902 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_json.py
--rw-r--r--   0        0        0   187127 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_json_schema.py
--rw-r--r--   0        0        0    92469 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_main.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_migration.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_model_signature.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_model_validator.py
--rw-r--r--   0        0        0    31026 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_networks.py
--rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_networks_ipaddress.py
--rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_parse.py
--rw-r--r--   0        0        0     8608 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_pickle.py
--rw-r--r--   0        0        0    16672 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_plugins.py
--rw-r--r--   0        0        0    11378 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_private_attributes.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_pydantic_extra_types.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_pydantic_settings.sh
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_rich_repr.py
--rw-r--r--   0        0        0    17984 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_root_model.py
--rw-r--r--   0        0        0    35524 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_serialize.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_strict.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_structural_pattern_matching.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_tools.py
--rw-r--r--   0        0        0    13292 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_type_adapter.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_type_alias_type.py
--rw-r--r--   0        0        0   198927 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_types.py
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_types_namedtuple.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_types_payment_card_number.py
--rw-r--r--   0        0        0    27453 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_types_typeddict.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_typing.py
--rw-r--r--   0        0        0    21237 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_v1.py
--rw-r--r--   0        0        0    24074 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_validate_call.py
--rw-r--r--   0        0        0    82071 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_validators.py
--rwxr-xr-x   0        0        0     4737 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_validators_dataclass.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_version.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/test_warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0    22802 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/benchmarks/basemodel_eq_performance.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/benchmarks/generate_north_star_data.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/benchmarks/test_fastapi_startup_generics.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/benchmarks/test_fastapi_startup_simple.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/benchmarks/test_north_star.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/__init__.py
--rw-r--r--   0        0        0    11084 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/test_mypy.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/configs/mypy-plugin-strict-no-any.ini
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/configs/mypy-plugin-strict.ini
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/configs/mypy-plugin-very-strict.ini
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/configs/mypy-plugin.ini
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/configs/pyproject-default.toml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/configs/pyproject-plugin-bad-param.toml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/configs/pyproject-plugin-no-strict-optional.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/configs/pyproject-plugin-strict.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/configs/pyproject-plugin.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/computed_fields.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/custom_constructor.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/dataclass_no_any.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/fail1.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/fail2.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/fail3.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/fail4.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/fail_defaults.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/generics.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/metaclass_args.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/no_strict_optional.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/plugin_default_factory.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/plugin_fail.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/plugin_success.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/pydantic_settings.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/root_models.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/modules/success.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/fail2.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py
--rw-r--r--   0        0        0     8716 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict-no-any_ini/dataclass_no_any.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py
--rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/custom_constructor.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/root_models.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail2.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py
--rw-r--r--   0        0        0     8716 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-no-strict-optional_toml/no_strict_optional.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py
--rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/root_models.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-plugin_ini/root_models.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.1.1/pyproject-default_toml/root_models.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-default_ini/root_models.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py
--rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py
--rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-default_toml/root_models.py
--rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py
--rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/plugin/example_plugin.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/plugin/pyproject.toml
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/pyright/pyproject.toml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.6.3/tests/pyright/pyright_example.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pydantic-2.6.3/.gitignore
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.6.3/LICENSE
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 pydantic-2.6.3/pyproject.toml
--rw-r--r--   0        0        0    84448 2020-02-02 00:00:00.000000 pydantic-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0   181418 2020-02-02 00:00:00.000000 pydantic-2.6.4/HISTORY.md
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 pydantic-2.6.4/Makefile
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 pydantic-2.6.4/README.md
+-rw-r--r--   0        0        0    12780 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/__init__.py
+-rw-r--r--   0        0        0    11913 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_migration.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/alias_generators.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/aliases.py
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/annotated_handlers.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/class_validators.py
+-rw-r--r--   0        0        0    21493 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/color.py
+-rw-r--r--   0        0        0    29141 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/config.py
+-rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/dataclasses.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/datetime_parse.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/decorator.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/env_settings.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/error_wrappers.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/errors.py
+-rw-r--r--   0        0        0    45930 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/fields.py
+-rw-r--r--   0        0        0    14621 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/functional_serializers.py
+-rw-r--r--   0        0        0    24313 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/functional_validators.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/generics.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/json.py
+-rw-r--r--   0        0        0   102807 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/json_schema.py
+-rw-r--r--   0        0        0    65892 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/main.py
+-rw-r--r--   0        0        0    55131 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/mypy.py
+-rw-r--r--   0        0        0    21225 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/networks.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/py.typed
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/root_model.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/schema.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/tools.py
+-rw-r--r--   0        0        0    18104 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/type_adapter.py
+-rw-r--r--   0        0        0    89607 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/typing.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/utils.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/validate_call_decorator.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/validators.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/version.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    24332 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    30627 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_decorators_v1.py
+-rw-r--r--   0        0        0    26369 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0    98557 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    22227 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_git.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_known_annotated_metadata.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_mock_val_ser.py
+-rw-r--r--   0        0        0    28114 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_schema_generation_shared.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_signature.py
+-rw-r--r--   0        0        0    29085 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_validate_call.py
+-rw-r--r--   0        0        0    10054 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/deprecated/__init__.py
+-rw-r--r--   0        0        0     9871 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/deprecated/class_validators.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/deprecated/decorator.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/deprecated/tools.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/plugin/__init__.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/plugin/_loader.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/plugin/_schema_validator.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/__init__.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/annotated_types.py
+-rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/class_validators.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/color.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/config.py
+-rw-r--r--   0        0        0    18073 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/dataclasses.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/datetime_parse.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/decorator.py
+-rw-r--r--   0        0        0    14039 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/env_settings.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/error_wrappers.py
+-rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/errors.py
+-rw-r--r--   0        0        0    50485 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/fields.py
+-rw-r--r--   0        0        0    17805 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/generics.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/json.py
+-rw-r--r--   0        0        0    44376 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/main.py
+-rw-r--r--   0        0        0    38745 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/mypy.py
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/networks.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/py.typed
+-rw-r--r--   0        0        0    47614 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/schema.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/tools.py
+-rw-r--r--   0        0        0    35379 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/types.py
+-rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/typing.py
+-rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/utils.py
+-rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/validators.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydantic-2.6.4/pydantic/v1/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/__init__.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/check_usage_docs.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/conftest.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_abc.py
+-rw-r--r--   0        0        0    22974 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_aliases.py
+-rw-r--r--   0        0        0    15073 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_annotated.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_assert_in_validators.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_callable.py
+-rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_color.py
+-rw-r--r--   0        0        0    22038 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_computed_fields.py
+-rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_config.py
+-rw-r--r--   0        0        0    14127 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_construction.py
+-rw-r--r--   0        0        0    18535 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_create_model.py
+-rw-r--r--   0        0        0    78195 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_dataclasses.py
+-rw-r--r--   0        0        0    22681 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_datetime.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_decorators.py
+-rw-r--r--   0        0        0    24974 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_deprecated.py
+-rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_deprecated_validate_arguments.py
+-rw-r--r--   0        0        0    74454 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_discriminated_union.py
+-rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_docs.py
+-rw-r--r--   0        0        0    83621 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_edge_cases.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_errors.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_exports.py
+-rwxr-xr-x   0        0        0      748 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_fastapi.sh
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_fastapi_json_schema.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_fields.py
+-rw-r--r--   0        0        0    30168 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_forward_ref.py
+-rw-r--r--   0        0        0    84716 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_generics.py
+-rw-r--r--   0        0        0     8025 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_internal.py
+-rw-r--r--   0        0        0    16902 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_json.py
+-rw-r--r--   0        0        0   187127 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_json_schema.py
+-rw-r--r--   0        0        0    92469 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_main.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_migration.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_model_signature.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_model_validator.py
+-rw-r--r--   0        0        0    31026 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_networks.py
+-rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_networks_ipaddress.py
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_parse.py
+-rw-r--r--   0        0        0     8608 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_pickle.py
+-rw-r--r--   0        0        0    16672 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_plugins.py
+-rw-r--r--   0        0        0    11378 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_private_attributes.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_pydantic_extra_types.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_pydantic_settings.sh
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_rich_repr.py
+-rw-r--r--   0        0        0    17984 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_root_model.py
+-rw-r--r--   0        0        0    35524 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_serialize.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_strict.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_structural_pattern_matching.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_tools.py
+-rw-r--r--   0        0        0    13292 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_type_adapter.py
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_type_alias_type.py
+-rw-r--r--   0        0        0   198927 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_types.py
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_types_namedtuple.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_types_payment_card_number.py
+-rw-r--r--   0        0        0    27453 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_types_typeddict.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_typing.py
+-rw-r--r--   0        0        0    21237 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_v1.py
+-rw-r--r--   0        0        0    24074 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_validate_call.py
+-rw-r--r--   0        0        0    82071 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_validators.py
+-rwxr-xr-x   0        0        0     4737 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_validators_dataclass.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_version.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/test_warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0    22802 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/benchmarks/basemodel_eq_performance.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/benchmarks/generate_north_star_data.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/benchmarks/test_fastapi_startup_generics.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/benchmarks/test_fastapi_startup_simple.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/benchmarks/test_north_star.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/__init__.py
+-rw-r--r--   0        0        0    11084 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/test_mypy.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/configs/mypy-plugin-strict-no-any.ini
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/configs/mypy-plugin-strict.ini
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/configs/mypy-plugin-very-strict.ini
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/configs/mypy-plugin.ini
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/configs/pyproject-default.toml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/configs/pyproject-plugin-bad-param.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/configs/pyproject-plugin-no-strict-optional.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/configs/pyproject-plugin-strict.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/configs/pyproject-plugin.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/computed_fields.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/custom_constructor.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/dataclass_no_any.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/fail1.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/fail2.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/fail3.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/fail4.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/fail_defaults.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/generics.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/metaclass_args.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/no_strict_optional.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/plugin_default_factory.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/plugin_fail.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/plugin_success.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/pydantic_settings.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/root_models.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/modules/success.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/fail2.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py
+-rw-r--r--   0        0        0     8716 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict-no-any_ini/dataclass_no_any.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py
+-rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/custom_constructor.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/root_models.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail2.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py
+-rw-r--r--   0        0        0     8716 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-no-strict-optional_toml/no_strict_optional.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py
+-rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/root_models.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-plugin_ini/root_models.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.1.1/pyproject-default_toml/root_models.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-default_ini/root_models.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py
+-rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py
+-rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-default_toml/root_models.py
+-rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py
+-rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/plugin/example_plugin.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/plugin/pyproject.toml
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/pyright/pyproject.toml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.6.4/tests/pyright/pyright_example.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pydantic-2.6.4/.gitignore
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.6.4/LICENSE
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 pydantic-2.6.4/pyproject.toml
+-rw-r--r--   0        0        0    85087 2020-02-02 00:00:00.000000 pydantic-2.6.4/PKG-INFO
```

### Comparing `pydantic-2.6.3/HISTORY.md` & `pydantic-2.6.4/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+## v2.6.4 (2024-03-08)
+
+[GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.6.4)
+
+### What's Changed
+
+#### Fixes
+
+* Fix usage of `AliasGenerator` with `computed_field` decorator by @sydney-runkle in [#8806](https://github.com/pydantic/pydantic/pull/8806)
+* Fix nested discriminated union schema gen, pt 2 by @sydney-runkle in [#8932](https://github.com/pydantic/pydantic/pull/8932)
+* Fix bug with no_strict_optional=True caused by API deferral by @dmontagu in [#8826](https://github.com/pydantic/pydantic/pull/8826)
+
+
 ## v2.6.3 (2024-02-27)
 
 [GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.6.3)
 
 ### What's Changed
 
 #### Packaging
```

### Comparing `pydantic-2.6.3/Makefile` & `pydantic-2.6.4/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/README.md` & `pydantic-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/__init__.py` & `pydantic-2.6.4/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_migration.py` & `pydantic-2.6.4/pydantic/_migration.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/alias_generators.py` & `pydantic-2.6.4/pydantic/alias_generators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/aliases.py` & `pydantic-2.6.4/pydantic/aliases.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/annotated_handlers.py` & `pydantic-2.6.4/pydantic/annotated_handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/color.py` & `pydantic-2.6.4/pydantic/color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/config.py` & `pydantic-2.6.4/pydantic/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/dataclasses.py` & `pydantic-2.6.4/pydantic/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/errors.py` & `pydantic-2.6.4/pydantic/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/fields.py` & `pydantic-2.6.4/pydantic/fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/functional_serializers.py` & `pydantic-2.6.4/pydantic/functional_serializers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/functional_validators.py` & `pydantic-2.6.4/pydantic/functional_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/json_schema.py` & `pydantic-2.6.4/pydantic/json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/main.py` & `pydantic-2.6.4/pydantic/main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/mypy.py` & `pydantic-2.6.4/pydantic/mypy.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,45 +336,55 @@
         self.has_dynamic_alias = has_dynamic_alias
         self.has_default = has_default
         self.line = line
         self.column = column
         self.type = type
         self.info = info
 
-    def to_argument(self, current_info: TypeInfo, typed: bool, force_optional: bool, use_alias: bool) -> Argument:
+    def to_argument(
+        self,
+        current_info: TypeInfo,
+        typed: bool,
+        force_optional: bool,
+        use_alias: bool,
+        api: SemanticAnalyzerPluginInterface,
+    ) -> Argument:
         """Based on mypy.plugins.dataclasses.DataclassAttribute.to_argument."""
+        variable = self.to_var(current_info, api, use_alias)
+        type_annotation = self.expand_type(current_info, api) if typed else AnyType(TypeOfAny.explicit)
         return Argument(
-            variable=self.to_var(current_info, use_alias),
-            type_annotation=self.expand_type(current_info) if typed else AnyType(TypeOfAny.explicit),
+            variable=variable,
+            type_annotation=type_annotation,
             initializer=None,
             kind=ARG_NAMED_OPT if force_optional or self.has_default else ARG_NAMED,
         )
 
-    def expand_type(self, current_info: TypeInfo) -> Type | None:
+    def expand_type(self, current_info: TypeInfo, api: SemanticAnalyzerPluginInterface) -> Type | None:
         """Based on mypy.plugins.dataclasses.DataclassAttribute.expand_type."""
         # The getattr in the next line is used to prevent errors in legacy versions of mypy without this attribute
         if self.type is not None and getattr(self.info, 'self_type', None) is not None:
             # In general, it is not safe to call `expand_type()` during semantic analyzis,
             # however this plugin is called very late, so all types should be fully ready.
             # Also, it is tricky to avoid eager expansion of Self types here (e.g. because
             # we serialize attributes).
             expanded_type = expand_type(self.type, {self.info.self_type.id: fill_typevars(current_info)})
             if isinstance(self.type, UnionType) and not isinstance(expanded_type, UnionType):
-                raise _DeferAnalysis()
+                if not api.final_iteration:
+                    raise _DeferAnalysis()
             return expanded_type
         return self.type
 
-    def to_var(self, current_info: TypeInfo, use_alias: bool) -> Var:
+    def to_var(self, current_info: TypeInfo, api: SemanticAnalyzerPluginInterface, use_alias: bool) -> Var:
         """Based on mypy.plugins.dataclasses.DataclassAttribute.to_var."""
         if use_alias and self.alias is not None:
             name = self.alias
         else:
             name = self.name
 
-        return Var(name, self.expand_type(current_info))
+        return Var(name, self.expand_type(current_info, api))
 
     def serialize(self) -> JsonDict:
         """Based on mypy.plugins.dataclasses.DataclassAttribute.serialize."""
         assert self.type
         return {
             'name': self.name,
             'alias': self.alias,
@@ -474,15 +484,15 @@
             if field.type is None:
                 return False
 
         is_settings = any(base.fullname == BASESETTINGS_FULLNAME for base in info.mro[:-1])
         try:
             self.add_initializer(fields, config, is_settings, is_root_model)
             self.add_model_construct_method(fields, config, is_settings)
-            self.set_frozen(fields, frozen=config.frozen is True)
+            self.set_frozen(fields, self._api, frozen=config.frozen is True)
         except _DeferAnalysis:
             if not self._api.final_iteration:
                 self._api.defer()
 
         self.adjust_decorator_signatures()
 
         info.metadata[METADATA_KEY] = {
@@ -911,15 +921,15 @@
             self._cls,
             'model_construct',
             args=args,
             return_type=fill_typevars(self._cls.info),
             is_classmethod=True,
         )
 
-    def set_frozen(self, fields: list[PydanticModelField], frozen: bool) -> None:
+    def set_frozen(self, fields: list[PydanticModelField], api: SemanticAnalyzerPluginInterface, frozen: bool) -> None:
         """Marks all fields as properties so that attempts to set them trigger mypy errors.
 
         This is the same approach used by the attrs and dataclasses plugins.
         """
         info = self._cls.info
         for field in fields:
             sym_node = info.names.get(field.name)
@@ -936,15 +946,15 @@
                         var_str = str(var)
                     except TypeError:
                         # This happens for PlaceholderNode; perhaps it will happen for other types in the future..
                         var_str = repr(var)
                     detail = f'sym_node.node: {var_str} (of type {var.__class__})'
                     error_unexpected_behavior(detail, self._api, self._cls)
             else:
-                var = field.to_var(info, use_alias=False)
+                var = field.to_var(info, api, use_alias=False)
                 var.info = info
                 var.is_property = frozen
                 var._fullname = info.fullname + '.' + var.name
                 info.names[var.name] = SymbolTableNode(MDEF, var)
 
     def get_config_update(self, name: str, arg: Expression) -> ModelConfigData | None:
         """Determines the config update due to a single kwarg in the ConfigDict definition.
@@ -1033,15 +1043,19 @@
         """Helper function used during the construction of the `__init__` and `model_construct` method signatures.
 
         Returns a list of mypy Argument instances for use in the generated signatures.
         """
         info = self._cls.info
         arguments = [
             field.to_argument(
-                info, typed=typed, force_optional=requires_dynamic_aliases or is_settings, use_alias=use_alias
+                info,
+                typed=typed,
+                force_optional=requires_dynamic_aliases or is_settings,
+                use_alias=use_alias,
+                api=self._api,
             )
             for field in fields
             if not (use_alias and field.has_dynamic_alias)
         ]
         return arguments
 
     def should_init_forbid_extra(self, fields: list[PydanticModelField], config: ModelConfigData) -> bool:
```

### Comparing `pydantic-2.6.3/pydantic/networks.py` & `pydantic-2.6.4/pydantic/networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/root_model.py` & `pydantic-2.6.4/pydantic/root_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/type_adapter.py` & `pydantic-2.6.4/pydantic/type_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,17 @@
     except TypeError:
         # type is not a class
         return False
 
 
 @final
 class TypeAdapter(Generic[T]):
-    """Type adapters provide a flexible way to perform validation and serialization based on a Python type.
+    """Usage docs: https://docs.pydantic.dev/2.6/concepts/type_adapter/
+
+    Type adapters provide a flexible way to perform validation and serialization based on a Python type.
 
     A `TypeAdapter` instance exposes some of the functionality from `BaseModel` instance methods
     for types that do not have such methods (such as dataclasses, primitive types, and more).
 
     **Note:** `TypeAdapter` instances are not types, and cannot be used as type annotations for fields.
 
     Attributes:
```

### Comparing `pydantic-2.6.3/pydantic/types.py` & `pydantic-2.6.4/pydantic/types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/validate_call_decorator.py` & `pydantic-2.6.4/pydantic/validate_call_decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/version.py` & `pydantic-2.6.4/pydantic/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The `version` module holds the version information for Pydantic."""
 from __future__ import annotations as _annotations
 
 __all__ = 'VERSION', 'version_info'
 
-VERSION = '2.6.3'
+VERSION = '2.6.4'
 """The version of Pydantic."""
 
 
 def version_short() -> str:
     """Return the `major.minor` part of Pydantic version.
 
     It returns '2.1' if Pydantic version is '2.1.1'.
```

### Comparing `pydantic-2.6.3/pydantic/warnings.py` & `pydantic-2.6.4/pydantic/warnings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_config.py` & `pydantic-2.6.4/pydantic/_internal/_config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_core_metadata.py` & `pydantic-2.6.4/pydantic/_internal/_core_metadata.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_core_utils.py` & `pydantic-2.6.4/pydantic/_internal/_core_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,14 @@
 
 _CORE_SCHEMA_FIELD_TYPES = {'typed-dict-field', 'dataclass-field', 'model-field', 'computed-field'}
 _FUNCTION_WITH_INNER_SCHEMA_TYPES = {'function-before', 'function-after', 'function-wrap'}
 _LIST_LIKE_SCHEMA_WITH_ITEMS_TYPES = {'list', 'set', 'frozenset'}
 
 _DEFINITIONS_CACHE_METADATA_KEY = 'pydantic.definitions_cache'
 
-NEEDS_APPLY_DISCRIMINATED_UNION_METADATA_KEY = 'pydantic.internal.needs_apply_discriminated_union'
-"""Used to mark a schema that has a discriminated union that needs to be checked for validity at the end of
-schema building because one of it's members refers to a definition that was not yet defined when the union
-was first encountered.
-"""
 TAGGED_UNION_TAG_KEY = 'pydantic.internal.tagged_union_tag'
 """
 Used in a `Tag` schema to specify the tag used for a discriminated union.
 """
 HAS_INVALID_SCHEMAS_METADATA_KEY = 'pydantic.internal.invalid'
 """Used to mark a schema that is invalid because it refers to a definition that was not yet defined when the
 schema was first encountered.
```

### Comparing `pydantic-2.6.3/pydantic/_internal/_dataclasses.py` & `pydantic-2.6.4/pydantic/_internal/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_decorators.py` & `pydantic-2.6.4/pydantic/_internal/_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_decorators_v1.py` & `pydantic-2.6.4/pydantic/_internal/_decorators_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_discriminated_union.py` & `pydantic-2.6.4/pydantic/_internal/_discriminated_union.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import TYPE_CHECKING, Any, Hashable, Sequence
 
 from pydantic_core import CoreSchema, core_schema
 
 from ..errors import PydanticUserError
 from . import _core_utils
 from ._core_utils import (
-    NEEDS_APPLY_DISCRIMINATED_UNION_METADATA_KEY,
     CoreSchemaField,
     collect_definitions,
     simplify_schema_references,
 )
 
 if TYPE_CHECKING:
     from ..types import Discriminator
@@ -25,45 +24,36 @@
     """
 
     def __init__(self, ref: str) -> None:
         self.ref = ref
         super().__init__(f'Missing definition for ref {self.ref!r}')
 
 
-def set_discriminator(schema: CoreSchema, discriminator: Any) -> None:
+def set_discriminator_in_metadata(schema: CoreSchema, discriminator: Any) -> None:
     schema.setdefault('metadata', {})
     metadata = schema.get('metadata')
     assert metadata is not None
     metadata[CORE_SCHEMA_METADATA_DISCRIMINATOR_PLACEHOLDER_KEY] = discriminator
 
 
 def apply_discriminators(schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
     definitions: dict[str, CoreSchema] | None = None
 
     def inner(s: core_schema.CoreSchema, recurse: _core_utils.Recurse) -> core_schema.CoreSchema:
         nonlocal definitions
-        if 'metadata' in s:
-            if s['metadata'].get(NEEDS_APPLY_DISCRIMINATED_UNION_METADATA_KEY, True) is False:
-                return s
 
         s = recurse(s, inner)
         if s['type'] == 'tagged-union':
             return s
 
         metadata = s.get('metadata', {})
-        discriminator = metadata.get(CORE_SCHEMA_METADATA_DISCRIMINATOR_PLACEHOLDER_KEY, None)
+        discriminator = metadata.pop(CORE_SCHEMA_METADATA_DISCRIMINATOR_PLACEHOLDER_KEY, None)
         if discriminator is not None:
             if definitions is None:
                 definitions = collect_definitions(schema)
-                # After we collect the definitions schemas, we must run through the discriminator
-                # application logic for each one. This step is crucial to prevent an exponential
-                # increase in complexity that occurs if schemas are left as 'union' schemas
-                # rather than 'tagged-union' schemas.
-                # For more details, see https://github.com/pydantic/pydantic/pull/8904#discussion_r1504687302
-                definitions = {k: recurse(v, inner) for k, v in definitions.items()}
             s = apply_discriminator(s, discriminator, definitions)
         return s
 
     return simplify_schema_references(_core_utils.walk_core_schema(schema, inner))
 
 
 def apply_discriminator(
@@ -270,36 +260,37 @@
 
         Here, "handling" entails:
         * Coalescing nested unions and compatible tagged-unions
         * Tracking the presence of 'none' and 'nullable' schemas occurring as choices
         * Validating that each allowed discriminator value maps to a unique choice
         * Updating the _tagged_union_choices mapping that will ultimately be used to build the TaggedUnionSchema.
         """
+        if choice['type'] == 'definition-ref':
+            if choice['schema_ref'] not in self.definitions:
+                raise MissingDefinitionForUnionRef(choice['schema_ref'])
+
         if choice['type'] == 'none':
             self._should_be_nullable = True
         elif choice['type'] == 'definitions':
             self._handle_choice(choice['schema'])
         elif choice['type'] == 'nullable':
             self._should_be_nullable = True
             self._handle_choice(choice['schema'])  # unwrap the nullable schema
         elif choice['type'] == 'union':
             # Reverse the choices list before extending the stack so that they get handled in the order they occur
             choices_schemas = [v[0] if isinstance(v, tuple) else v for v in choice['choices'][::-1]]
             self._choices_to_handle.extend(choices_schemas)
-        elif choice['type'] == 'definition-ref':
-            if choice['schema_ref'] not in self.definitions:
-                raise MissingDefinitionForUnionRef(choice['schema_ref'])
-            self._handle_choice(self.definitions[choice['schema_ref']])
         elif choice['type'] not in {
             'model',
             'typed-dict',
             'tagged-union',
             'lax-or-strict',
             'dataclass',
             'dataclass-args',
+            'definition-ref',
         } and not _core_utils.is_function_with_inner_schema(choice):
             # We should eventually handle 'definition-ref' as well
             raise TypeError(
                 f'{choice["type"]!r} is not a valid discriminated union variant;'
                 ' should be a `BaseModel` or `dataclass`'
             )
         else:
```

### Comparing `pydantic-2.6.3/pydantic/_internal/_fields.py` & `pydantic-2.6.4/pydantic/_internal/_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_forward_ref.py` & `pydantic-2.6.4/pydantic/_internal/_forward_ref.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_generate_schema.py` & `pydantic-2.6.4/pydantic/_internal/_generate_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 from ..json_schema import JsonSchemaValue
 from ..version import version_short
 from ..warnings import PydanticDeprecatedSince20
 from . import _core_utils, _decorators, _discriminated_union, _known_annotated_metadata, _typing_extra
 from ._config import ConfigWrapper, ConfigWrapperStack
 from ._core_metadata import CoreMetadataHandler, build_metadata_dict
 from ._core_utils import (
-    NEEDS_APPLY_DISCRIMINATED_UNION_METADATA_KEY,
     CoreSchemaOrField,
     collect_invalid_schemas,
     define_expected_missing_refs,
     get_ref,
     get_type_ref,
     is_function_with_inner_schema,
     is_list_like_schema_with_items_schema,
@@ -298,15 +297,14 @@
 class GenerateSchema:
     """Generate core schema for a Pydantic model, dataclass and types like `str`, `datetime`, ... ."""
 
     __slots__ = (
         '_config_wrapper_stack',
         '_types_namespace_stack',
         '_typevars_map',
-        '_needs_apply_discriminated_union',
         '_has_invalid_schema',
         'field_name_stack',
         'defs',
     )
 
     def __init__(
         self,
@@ -314,15 +312,14 @@
         types_namespace: dict[str, Any] | None,
         typevars_map: dict[Any, Any] | None = None,
     ) -> None:
         # we need a stack for recursing into child models
         self._config_wrapper_stack = ConfigWrapperStack(config_wrapper)
         self._types_namespace_stack = TypesNamespaceStack(types_namespace)
         self._typevars_map = typevars_map
-        self._needs_apply_discriminated_union = False
         self._has_invalid_schema = False
         self.field_name_stack = _FieldNameStack()
         self.defs = _Definitions()
 
     @classmethod
     def __from_parent(
         cls,
@@ -331,15 +328,14 @@
         typevars_map: dict[Any, Any] | None,
         defs: _Definitions,
     ) -> GenerateSchema:
         obj = cls.__new__(cls)
         obj._config_wrapper_stack = config_wrapper_stack
         obj._types_namespace_stack = types_namespace_stack
         obj._typevars_map = typevars_map
-        obj._needs_apply_discriminated_union = False
         obj._has_invalid_schema = False
         obj.field_name_stack = _FieldNameStack()
         obj.defs = defs
         return obj
 
     @property
     def _config_wrapper(self) -> ConfigWrapper:
@@ -412,23 +408,18 @@
         try:
             return _discriminated_union.apply_discriminator(
                 schema,
                 discriminator,
             )
         except _discriminated_union.MissingDefinitionForUnionRef:
             # defer until defs are resolved
-            _discriminated_union.set_discriminator(
+            _discriminated_union.set_discriminator_in_metadata(
                 schema,
                 discriminator,
             )
-            if 'metadata' in schema:
-                schema['metadata'][NEEDS_APPLY_DISCRIMINATED_UNION_METADATA_KEY] = True
-            else:
-                schema['metadata'] = {NEEDS_APPLY_DISCRIMINATED_UNION_METADATA_KEY: True}
-            self._needs_apply_discriminated_union = True
             return schema
 
     class CollectedInvalid(Exception):
         pass
 
     def clean_schema(self, schema: CoreSchema) -> CoreSchema:
         schema = self.collect_definitions(schema)
@@ -715,32 +706,24 @@
             return (Any, Any)
         if len(args) < 2:
             origin = get_origin(obj)
             raise TypeError(f'Expected two type arguments for {origin}, got 1')
         return args[0], args[1]
 
     def _post_process_generated_schema(self, schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
-        if 'metadata' in schema:
-            metadata = schema['metadata']
-            metadata[NEEDS_APPLY_DISCRIMINATED_UNION_METADATA_KEY] = self._needs_apply_discriminated_union
-        else:
-            schema['metadata'] = {
-                NEEDS_APPLY_DISCRIMINATED_UNION_METADATA_KEY: self._needs_apply_discriminated_union,
-            }
+        if 'metadata' not in schema:
+            schema['metadata'] = {}
         return schema
 
     def _generate_schema(self, obj: Any) -> core_schema.CoreSchema:
         """Recursively generate a pydantic-core schema for any supported python type."""
         has_invalid_schema = self._has_invalid_schema
         self._has_invalid_schema = False
-        needs_apply_discriminated_union = self._needs_apply_discriminated_union
-        self._needs_apply_discriminated_union = False
-        schema = self._post_process_generated_schema(self._generate_schema_inner(obj))
+        schema = self._generate_schema_inner(obj)
         self._has_invalid_schema = self._has_invalid_schema or has_invalid_schema
-        self._needs_apply_discriminated_union = self._needs_apply_discriminated_union or needs_apply_discriminated_union
         return schema
 
     def _generate_schema_inner(self, obj: Any) -> core_schema.CoreSchema:
         if isinstance(obj, _AnnotatedType):
             return self._annotated_schema(obj)
 
         if isinstance(obj, dict):
@@ -961,15 +944,15 @@
             alias_generator: A callable that takes a string and returns a string, or an AliasGenerator instance.
             field_info: The FieldInfo instance to which the alias_generator is (maybe) applied.
             field_name: The name of the field from which to generate the alias.
         """
         # Apply an alias_generator if
         # 1. An alias is not specified
         # 2. An alias is specified, but the priority is <= 1
-        if alias_generator and (
+        if (
             field_info.alias_priority is None
             or field_info.alias_priority <= 1
             or field_info.alias is None
             or field_info.validation_alias is None
             or field_info.serialization_alias is None
         ):
             alias, validation_alias, serialization_alias = None, None, None
@@ -997,14 +980,57 @@
             if field_info.alias is None:
                 field_info.alias = alias
             if field_info.serialization_alias is None:
                 field_info.serialization_alias = serialization_alias or alias
             if field_info.validation_alias is None:
                 field_info.validation_alias = validation_alias or alias
 
+    @staticmethod
+    def _apply_alias_generator_to_computed_field_info(
+        alias_generator: Callable[[str], str] | AliasGenerator,
+        computed_field_info: ComputedFieldInfo,
+        computed_field_name: str,
+    ):
+        """Apply an alias_generator to alias on a ComputedFieldInfo instance if appropriate.
+
+        Args:
+            alias_generator: A callable that takes a string and returns a string, or an AliasGenerator instance.
+            computed_field_info: The ComputedFieldInfo instance to which the alias_generator is (maybe) applied.
+            computed_field_name: The name of the computed field from which to generate the alias.
+        """
+        # Apply an alias_generator if
+        # 1. An alias is not specified
+        # 2. An alias is specified, but the priority is <= 1
+
+        if (
+            computed_field_info.alias_priority is None
+            or computed_field_info.alias_priority <= 1
+            or computed_field_info.alias is None
+        ):
+            alias, validation_alias, serialization_alias = None, None, None
+
+            if isinstance(alias_generator, AliasGenerator):
+                alias, validation_alias, serialization_alias = alias_generator.generate_aliases(computed_field_name)
+            elif isinstance(alias_generator, Callable):
+                alias = alias_generator(computed_field_name)
+                if not isinstance(alias, str):
+                    raise TypeError(f'alias_generator {alias_generator} must return str, not {alias.__class__}')
+
+            # if priority is not set, we set to 1
+            # which supports the case where the alias_generator from a child class is used
+            # to generate an alias for a field in a parent class
+            if computed_field_info.alias_priority is None or computed_field_info.alias_priority <= 1:
+                computed_field_info.alias_priority = 1
+
+            # if the priority is 1, then we set the aliases to the generated alias
+            # note that we use the serialization_alias with priority over alias, as computed_field
+            # aliases are used for serialization only (not validation)
+            if computed_field_info.alias_priority == 1:
+                computed_field_info.alias = serialization_alias or alias
+
     def _common_field_schema(  # C901
         self, name: str, field_info: FieldInfo, decorators: DecoratorInfos
     ) -> _CommonField:
         # Update FieldInfo annotation if appropriate:
         from .. import AliasChoices, AliasPath
         from ..fields import FieldInfo
 
@@ -1621,28 +1647,20 @@
         return_type_schema = self.generate_schema(return_type)
         # Apply serializers to computed field if there exist
         return_type_schema = self._apply_field_serializers(
             return_type_schema,
             filter_field_decorator_info_by_field(field_serializers.values(), d.cls_var_name),
             computed_field=True,
         )
-        # Handle alias_generator using similar logic to that from
-        # pydantic._internal._generate_schema.GenerateSchema._common_field_schema,
-        # with field_info -> d.info and name -> d.cls_var_name
+
         alias_generator = self._config_wrapper.alias_generator
-        if alias_generator and (d.info.alias_priority is None or d.info.alias_priority <= 1):
-            alias = None
-            if isinstance(alias_generator, AliasGenerator) and alias_generator.alias is not None:
-                alias = alias_generator.alias(d.cls_var_name)
-            elif isinstance(alias_generator, Callable):
-                alias = alias_generator(d.cls_var_name)
-            if not isinstance(alias, str):
-                raise TypeError(f'alias_generator {alias_generator} must return str, not {alias.__class__}')
-            d.info.alias = alias
-            d.info.alias_priority = 1
+        if alias_generator is not None:
+            self._apply_alias_generator_to_computed_field_info(
+                alias_generator=alias_generator, computed_field_info=d.info, computed_field_name=d.cls_var_name
+            )
 
         def set_computed_field_metadata(schema: CoreSchemaOrField, handler: GetJsonSchemaHandler) -> JsonSchemaValue:
             json_schema = handler(schema)
 
             json_schema['readOnly'] = True
 
             title = d.info.title
```

### Comparing `pydantic-2.6.3/pydantic/_internal/_generics.py` & `pydantic-2.6.4/pydantic/_internal/_generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_git.py` & `pydantic-2.6.4/pydantic/_internal/_git.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_known_annotated_metadata.py` & `pydantic-2.6.4/pydantic/_internal/_known_annotated_metadata.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_mock_val_ser.py` & `pydantic-2.6.4/pydantic/_internal/_mock_val_ser.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_model_construction.py` & `pydantic-2.6.4/pydantic/_internal/_model_construction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_repr.py` & `pydantic-2.6.4/pydantic/_internal/_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_schema_generation_shared.py` & `pydantic-2.6.4/pydantic/_internal/_schema_generation_shared.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_signature.py` & `pydantic-2.6.4/pydantic/_internal/_signature.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_std_types_schema.py` & `pydantic-2.6.4/pydantic/_internal/_std_types_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_typing_extra.py` & `pydantic-2.6.4/pydantic/_internal/_typing_extra.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_utils.py` & `pydantic-2.6.4/pydantic/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_validate_call.py` & `pydantic-2.6.4/pydantic/_internal/_validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/_internal/_validators.py` & `pydantic-2.6.4/pydantic/_internal/_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/deprecated/class_validators.py` & `pydantic-2.6.4/pydantic/deprecated/class_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/deprecated/config.py` & `pydantic-2.6.4/pydantic/deprecated/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/deprecated/copy_internals.py` & `pydantic-2.6.4/pydantic/deprecated/copy_internals.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/deprecated/decorator.py` & `pydantic-2.6.4/pydantic/deprecated/decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/deprecated/json.py` & `pydantic-2.6.4/pydantic/deprecated/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/deprecated/parse.py` & `pydantic-2.6.4/pydantic/deprecated/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/deprecated/tools.py` & `pydantic-2.6.4/pydantic/deprecated/tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/plugin/__init__.py` & `pydantic-2.6.4/pydantic/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/plugin/_loader.py` & `pydantic-2.6.4/pydantic/plugin/_loader.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/plugin/_schema_validator.py` & `pydantic-2.6.4/pydantic/plugin/_schema_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/__init__.py` & `pydantic-2.6.4/pydantic/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/_hypothesis_plugin.py` & `pydantic-2.6.4/pydantic/v1/_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/annotated_types.py` & `pydantic-2.6.4/pydantic/v1/annotated_types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/class_validators.py` & `pydantic-2.6.4/pydantic/v1/class_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/color.py` & `pydantic-2.6.4/pydantic/v1/color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/config.py` & `pydantic-2.6.4/pydantic/v1/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/dataclasses.py` & `pydantic-2.6.4/pydantic/v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/datetime_parse.py` & `pydantic-2.6.4/pydantic/v1/datetime_parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/decorator.py` & `pydantic-2.6.4/pydantic/v1/decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/env_settings.py` & `pydantic-2.6.4/pydantic/v1/env_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/error_wrappers.py` & `pydantic-2.6.4/pydantic/v1/error_wrappers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/errors.py` & `pydantic-2.6.4/pydantic/v1/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/fields.py` & `pydantic-2.6.4/pydantic/v1/fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/generics.py` & `pydantic-2.6.4/pydantic/v1/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/json.py` & `pydantic-2.6.4/pydantic/v1/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/main.py` & `pydantic-2.6.4/pydantic/v1/main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/mypy.py` & `pydantic-2.6.4/pydantic/v1/mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/networks.py` & `pydantic-2.6.4/pydantic/v1/networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/parse.py` & `pydantic-2.6.4/pydantic/v1/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/schema.py` & `pydantic-2.6.4/pydantic/v1/schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/tools.py` & `pydantic-2.6.4/pydantic/v1/tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/types.py` & `pydantic-2.6.4/pydantic/v1/types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/typing.py` & `pydantic-2.6.4/pydantic/v1/typing.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/utils.py` & `pydantic-2.6.4/pydantic/v1/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/validators.py` & `pydantic-2.6.4/pydantic/v1/validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pydantic/v1/version.py` & `pydantic-2.6.4/pydantic/v1/version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/check_usage_docs.py` & `pydantic-2.6.4/tests/check_usage_docs.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/conftest.py` & `pydantic-2.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_abc.py` & `pydantic-2.6.4/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_aliases.py` & `pydantic-2.6.4/tests/test_aliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -698,7 +698,30 @@
 
     # the same behavior we'd expect if we defined alias, validation_alias
     # and serialization_alias on the field itself
     f = Foo(a_val_alias='a')
     assert f.a == 'a'
     assert f.model_dump(by_alias=True) == {'a_ser_alias': 'a'}
     assert f.model_dump(by_alias=False) == {'a': 'a'}
+
+
+def test_alias_generator_with_computed_field_for_serialization() -> None:
+    """Tests that the alias generator is used for computed fields, with serialization_alias taking precedence over alias."""
+
+    class Rectangle(BaseModel):
+        model_config = ConfigDict(
+            alias_generator=AliasGenerator(
+                validation_alias=lambda field_name: f'{field_name}_val_alias',
+                alias=lambda field_name: f'{field_name}_alias',
+                serialization_alias=lambda field_name: f'{field_name}_ser_alias',
+            )
+        )
+
+        width: int
+        height: int
+
+        @computed_field
+        def area(self) -> int:
+            return self.width * self.height
+
+    r = Rectangle(width_val_alias=10, height_val_alias=20)
+    assert r.model_dump(by_alias=True) == {'width_ser_alias': 10, 'height_ser_alias': 20, 'area_ser_alias': 200}
```

### Comparing `pydantic-2.6.3/tests/test_annotated.py` & `pydantic-2.6.4/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_assert_in_validators.py` & `pydantic-2.6.4/tests/test_assert_in_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_callable.py` & `pydantic-2.6.4/tests/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_color.py` & `pydantic-2.6.4/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_computed_fields.py` & `pydantic-2.6.4/tests/test_computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_config.py` & `pydantic-2.6.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_construction.py` & `pydantic-2.6.4/tests/test_construction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_create_model.py` & `pydantic-2.6.4/tests/test_create_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_dataclasses.py` & `pydantic-2.6.4/tests/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_datetime.py` & `pydantic-2.6.4/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_decorators.py` & `pydantic-2.6.4/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_deprecated.py` & `pydantic-2.6.4/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_deprecated_validate_arguments.py` & `pydantic-2.6.4/tests/test_deprecated_validate_arguments.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_discriminated_union.py` & `pydantic-2.6.4/tests/test_discriminated_union.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from enum import Enum, IntEnum
 from types import SimpleNamespace
 from typing import Any, Callable, Generic, List, Optional, Sequence, TypeVar, Union
 
 import pytest
 from dirty_equals import HasRepr, IsStr
 from pydantic_core import SchemaValidator, core_schema
-from typing_extensions import Annotated, Literal
+from typing_extensions import Annotated, Literal, TypedDict
 
 from pydantic import BaseModel, ConfigDict, Discriminator, Field, TypeAdapter, ValidationError, field_validator
 from pydantic._internal._discriminated_union import apply_discriminator
+from pydantic.dataclasses import dataclass as pydantic_dataclass
 from pydantic.errors import PydanticUserError
 from pydantic.fields import FieldInfo
 from pydantic.json_schema import GenerateJsonSchema
 from pydantic.types import Tag
 
 
 def test_discriminated_union_type():
@@ -1864,15 +1865,97 @@
         state_type: Literal['loop']
         substate: 'AnyState'
 
     class LeafState(BaseModel):
         state_type: Literal['leaf']
 
     AnyState = Annotated[Union[NestedState, LoopState, LeafState], Field(..., discriminator='state_type')]
-    NestedState.model_rebuild()
-    LoopState.model_rebuild()
     adapter = TypeAdapter(AnyState)
 
     assert adapter.core_schema['schema']['type'] == 'tagged-union'
     for definition in adapter.core_schema['definitions']:
         if definition['schema']['model_name'] in ['NestedState', 'LoopState']:
             assert definition['schema']['fields']['substate']['schema']['schema']['type'] == 'tagged-union'
+
+
+def test_recursive_discriminiated_union_with_typed_dict() -> None:
+    class Foo(TypedDict):
+        type: Literal['foo']
+        x: 'Foobar'
+
+    class Bar(TypedDict):
+        type: Literal['bar']
+
+    Foobar = Annotated[Union[Foo, Bar], Field(discriminator='type')]
+    ta = TypeAdapter(Foobar)
+
+    # len of errors should be 1 for each case, bc we're using a tagged union
+    with pytest.raises(ValidationError) as e:
+        ta.validate_python({'type': 'wrong'})
+    assert len(e.value.errors()) == 1
+
+    with pytest.raises(ValidationError) as e:
+        ta.validate_python({'type': 'foo', 'x': {'type': 'wrong'}})
+    assert len(e.value.errors()) == 1
+
+    core_schema = ta.core_schema
+    assert core_schema['schema']['type'] == 'tagged-union'
+    for definition in core_schema['definitions']:
+        if 'Foo' in definition['ref']:
+            assert definition['fields']['x']['schema']['type'] == 'tagged-union'
+
+
+def test_recursive_discriminiated_union_with_base_model() -> None:
+    class Foo(BaseModel):
+        type: Literal['foo']
+        x: 'Foobar'
+
+    class Bar(BaseModel):
+        type: Literal['bar']
+
+    Foobar = Annotated[Union[Foo, Bar], Field(discriminator='type')]
+    ta = TypeAdapter(Foobar)
+
+    # len of errors should be 1 for each case, bc we're using a tagged union
+    with pytest.raises(ValidationError) as e:
+        ta.validate_python({'type': 'wrong'})
+    assert len(e.value.errors()) == 1
+
+    with pytest.raises(ValidationError) as e:
+        ta.validate_python({'type': 'foo', 'x': {'type': 'wrong'}})
+    assert len(e.value.errors()) == 1
+
+    core_schema = ta.core_schema
+    assert core_schema['schema']['type'] == 'tagged-union'
+    for definition in core_schema['definitions']:
+        if 'Foo' in definition['ref']:
+            assert definition['schema']['fields']['x']['schema']['type'] == 'tagged-union'
+
+
+def test_recursive_discriminated_union_with_pydantic_dataclass() -> None:
+    @pydantic_dataclass
+    class Foo:
+        type: Literal['foo']
+        x: 'Foobar'
+
+    @pydantic_dataclass
+    class Bar:
+        type: Literal['bar']
+
+    Foobar = Annotated[Union[Foo, Bar], Field(discriminator='type')]
+    ta = TypeAdapter(Foobar)
+
+    # len of errors should be 1 for each case, bc we're using a tagged union
+    with pytest.raises(ValidationError) as e:
+        ta.validate_python({'type': 'wrong'})
+    assert len(e.value.errors()) == 1
+
+    with pytest.raises(ValidationError) as e:
+        ta.validate_python({'type': 'foo', 'x': {'type': 'wrong'}})
+    assert len(e.value.errors()) == 1
+
+    core_schema = ta.core_schema
+    assert core_schema['schema']['type'] == 'tagged-union'
+    for definition in core_schema['definitions']:
+        if 'Foo' in definition['ref']:
+            for field in definition['schema']['fields']:
+                assert field['schema']['type'] == 'tagged-union' if field['name'] == 'x' else True
```

### Comparing `pydantic-2.6.3/tests/test_docs.py` & `pydantic-2.6.4/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_edge_cases.py` & `pydantic-2.6.4/tests/test_edge_cases.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_errors.py` & `pydantic-2.6.4/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_exports.py` & `pydantic-2.6.4/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_fastapi.sh` & `pydantic-2.6.4/tests/test_fastapi.sh`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_fastapi_json_schema.py` & `pydantic-2.6.4/tests/test_fastapi_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_fields.py` & `pydantic-2.6.4/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_forward_ref.py` & `pydantic-2.6.4/tests/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_generics.py` & `pydantic-2.6.4/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_internal.py` & `pydantic-2.6.4/tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_json.py` & `pydantic-2.6.4/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_json_schema.py` & `pydantic-2.6.4/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_main.py` & `pydantic-2.6.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_migration.py` & `pydantic-2.6.4/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_model_signature.py` & `pydantic-2.6.4/tests/test_model_signature.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_model_validator.py` & `pydantic-2.6.4/tests/test_model_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_networks.py` & `pydantic-2.6.4/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_networks_ipaddress.py` & `pydantic-2.6.4/tests/test_networks_ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_parse.py` & `pydantic-2.6.4/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_pickle.py` & `pydantic-2.6.4/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_plugins.py` & `pydantic-2.6.4/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_private_attributes.py` & `pydantic-2.6.4/tests/test_private_attributes.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_rich_repr.py` & `pydantic-2.6.4/tests/test_rich_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_root_model.py` & `pydantic-2.6.4/tests/test_root_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_serialize.py` & `pydantic-2.6.4/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_strict.py` & `pydantic-2.6.4/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_structural_pattern_matching.py` & `pydantic-2.6.4/tests/test_structural_pattern_matching.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_tools.py` & `pydantic-2.6.4/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_type_adapter.py` & `pydantic-2.6.4/tests/test_type_adapter.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_type_alias_type.py` & `pydantic-2.6.4/tests/test_type_alias_type.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_types.py` & `pydantic-2.6.4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_types_namedtuple.py` & `pydantic-2.6.4/tests/test_types_namedtuple.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_types_payment_card_number.py` & `pydantic-2.6.4/tests/test_types_payment_card_number.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_types_typeddict.py` & `pydantic-2.6.4/tests/test_types_typeddict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_typing.py` & `pydantic-2.6.4/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_utils.py` & `pydantic-2.6.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_v1.py` & `pydantic-2.6.4/tests/test_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_validate_call.py` & `pydantic-2.6.4/tests/test_validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_validators.py` & `pydantic-2.6.4/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_validators_dataclass.py` & `pydantic-2.6.4/tests/test_validators_dataclass.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_version.py` & `pydantic-2.6.4/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/test_warnings.py` & `pydantic-2.6.4/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/benchmarks/basemodel_eq_performance.py` & `pydantic-2.6.4/tests/benchmarks/basemodel_eq_performance.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/benchmarks/generate_north_star_data.py` & `pydantic-2.6.4/tests/benchmarks/generate_north_star_data.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/benchmarks/test_fastapi_startup_generics.py` & `pydantic-2.6.4/tests/benchmarks/test_fastapi_startup_generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/benchmarks/test_fastapi_startup_simple.py` & `pydantic-2.6.4/tests/benchmarks/test_fastapi_startup_simple.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/benchmarks/test_north_star.py` & `pydantic-2.6.4/tests/benchmarks/test_north_star.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/test_mypy.py` & `pydantic-2.6.4/tests/mypy/test_mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/configs/mypy-plugin-strict-no-any.ini` & `pydantic-2.6.4/tests/mypy/configs/mypy-plugin-strict-no-any.ini`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/configs/pyproject-default.toml` & `pydantic-2.6.4/tests/mypy/configs/pyproject-default.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/configs/pyproject-plugin-bad-param.toml` & `pydantic-2.6.4/tests/mypy/configs/pyproject-plugin-bad-param.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/configs/pyproject-plugin-no-strict-optional.toml` & `pydantic-2.6.4/tests/mypy/configs/pyproject-plugin-no-strict-optional.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/configs/pyproject-plugin-strict.toml` & `pydantic-2.6.4/tests/mypy/configs/pyproject-plugin-strict.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/configs/pyproject-plugin.toml` & `pydantic-2.6.4/tests/mypy/configs/pyproject-plugin.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/modules/computed_fields.py` & `pydantic-2.6.4/tests/mypy/modules/computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/modules/fail4.py` & `pydantic-2.6.4/tests/mypy/modules/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/modules/generics.py` & `pydantic-2.6.4/tests/mypy/modules/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/modules/metaclass_args.py` & `pydantic-2.6.4/tests/mypy/modules/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/modules/plugin_default_factory.py` & `pydantic-2.6.4/tests/mypy/modules/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/modules/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/modules/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/modules/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/modules/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/modules/plugin_success.py` & `pydantic-2.6.4/tests/mypy/modules/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/modules/plugin_success_baseConfig.py` & `pydantic-2.6.4/tests/mypy/modules/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/modules/success.py` & `pydantic-2.6.4/tests/mypy/modules/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py` & `pydantic-2.6.4/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py` & `pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py` & `pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py` & `pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py` & `pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py` & `pydantic-2.6.4/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py` & `pydantic-2.6.4/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py` & `pydantic-2.6.4/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py` & `pydantic-2.6.4/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py` & `pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py` & `pydantic-2.6.4/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/plugin/example_plugin.py` & `pydantic-2.6.4/tests/plugin/example_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/plugin/test_plugin.py` & `pydantic-2.6.4/tests/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/tests/pyright/pyright_example.py` & `pydantic-2.6.4/tests/pyright/pyright_example.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/.gitignore` & `pydantic-2.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/LICENSE` & `pydantic-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/pyproject.toml` & `pydantic-2.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.6.3/PKG-INFO` & `pydantic-2.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic
-Version: 2.6.3
+Version: 2.6.4
 Summary: Data validation using Python type hints
 Project-URL: Homepage, https://github.com/pydantic/pydantic
 Project-URL: Documentation, https://docs.pydantic.dev
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic
 Project-URL: Changelog, https://docs.pydantic.dev/latest/changelog/
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>, Adrian Garcia Badaracco <1755071+adriangb@users.noreply.github.com>, Terrence Dorsey <terry@pydantic.dev>, David Montague <david@pydantic.dev>, Serge Matveenko <lig@countzero.co>, Marcelo Trylesinski <marcelotryle@gmail.com>, Sydney Runkle <sydneymarierunkle@gmail.com>, David Hewitt <mail@davidhewitt.io>
@@ -109,14 +109,27 @@
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/pydantic/security/policy).
 
 ## Changelog
 
+## v2.6.4 (2024-03-08)
+
+[GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.6.4)
+
+### What's Changed
+
+#### Fixes
+
+* Fix usage of `AliasGenerator` with `computed_field` decorator by [@sydney-runkle](https://github.com/sydney-runkle) in [#8806](https://github.com/pydantic/pydantic/pull/8806)
+* Fix nested discriminated union schema gen, pt 2 by [@sydney-runkle](https://github.com/sydney-runkle) in [#8932](https://github.com/pydantic/pydantic/pull/8932)
+* Fix bug with no_strict_optional=True caused by API deferral by [@dmontagu](https://github.com/dmontagu) in [#8826](https://github.com/pydantic/pydantic/pull/8826)
+
+
 ## v2.6.3 (2024-02-27)
 
 [GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.6.3)
 
 ### What's Changed
 
 #### Packaging
```

