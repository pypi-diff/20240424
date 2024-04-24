# Comparing `tmp/qcs_sdk_python_grpc_web-0.17.7rc0.tar.gz` & `tmp/qcs_sdk_python_grpc_web-0.17.8rc0.tar.gz`

## Comparing `qcs_sdk_python_grpc_web-0.17.7rc0.tar` & `qcs_sdk_python_grpc_web-0.17.8rc0.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0     1001      127     2496 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/Cargo.toml
--rw-r--r--   0     1001      127    44902 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/CHANGELOG.md
--rw-r--r--   0     1001      127      752 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/Makefile.toml
--rw-r--r--   0     1001      127     2186 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/README.md
--rw-r--r--   0     1001      127       95 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/build.rs
--rw-r--r--   0     1001      127      931 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/delayed_job_retrieval.rs
--rw-r--r--   0     1001      127     1770 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/execute.rs
--rw-r--r--   0     1001      127      674 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/libquil.rs
--rw-r--r--   0     1001      127      767 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/local.rs
--rw-r--r--   0     1001      127     2154 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/parametric_compilation.rs
--rw-r--r--   0     1001      127     1277 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/quil_t.rs
--rw-r--r--   0     1001      127      126 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/bin/diagnostics.rs
--rw-r--r--   0     1001      127     5479 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/client.rs
--rw-r--r--   0     1001      127     8277 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/isa/edge.rs
--rw-r--r--   0     1001      127     6791 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/isa/mod.rs
--rw-r--r--   0     1001      127     8320 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/isa/operator.rs
--rw-r--r--   0     1001      127    13686 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/isa/qubit.rs
--rw-r--r--   0     1001      127    11548 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/libquil.rs
--rw-r--r--   0     1001      127      198 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/mod.rs
--rw-r--r--   0     1001      127    16466 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/quilc.rs
--rw-r--r--   0     1001      127    11529 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/rpcq.rs
--rw-r--r--   0     1001      127     8271 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/diagnostics.rs
--rw-r--r--   0     1001      127    36127 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/executable.rs
--rw-r--r--   0     1001      127    23212 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/execution_data.rs
--rw-r--r--   0     1001      127     1984 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/lib.rs
--rw-r--r--   0     1001      127    25522 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/api.rs
--rw-r--r--   0     1001      127    12027 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/execution.rs
--rw-r--r--   0     1001      127     3187 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/mod.rs
--rw-r--r--   0     1001      127     6058 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/result_data.rs
--rw-r--r--   0     1001      127    17418 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/rewrite_arithmetic.rs
--rw-r--r--   0     1001      127      137 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_allocates_for_multiple_expressions-2.snap
--rw-r--r--   0     1001      127      131 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_allocates_for_multiple_expressions.snap
--rw-r--r--   0     1001      127      112 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_frequency_expressions-2.snap
--rw-r--r--   0     1001      127      119 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_frequency_expressions.snap
--rw-r--r--   0     1001      127      127 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_phases.snap
--rw-r--r--   0     1001      127      111 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_set_scale_units.snap
--rw-r--r--   0     1001      127      134 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_substitutes_and_reuses_gate_expressions.snap
--rw-r--r--   0     1001      127      127 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_substitutes_gate_parameters.snap
--rw-r--r--   0     1001      127     9322 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/translation.rs
--rw-r--r--   0     1001      127     4292 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qvm/execution.rs
--rw-r--r--   0     1001      127    13970 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qvm/http.rs
--rw-r--r--   0     1001      127     6966 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qvm/libquil.rs
--rw-r--r--   0     1001      127    11138 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qvm/mod.rs
--rw-r--r--   0     1001      127      154 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qvm/snapshots/qcs__qvm__test__apply_valid_parameters_to_program.snap
--rw-r--r--   0     1001      127     1938 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/register_data.rs
--rw-r--r--   0     1001      127   104426 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/aspen_9_isa.json
--rw-r--r--   0     1001      127     1921 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/basic_qvm.rs
--rw-r--r--   0     1001      127      558 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/bell_state_response_data.hex
--rw-r--r--   0     1001      127    81629 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/compiler-isa-Aspen-8.json
--rw-r--r--   0     1001      127    14144 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/mocked_qpu.rs
--rw-r--r--   0     1001      127     2071 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/parametric_compilation.rs
--rw-r--r--   0     1001      127    71490 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/qcs-isa-Aspen-8.json
--rw-r--r--   0     1001      127     3933 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/qvm_api.rs
--rw-r--r--   0     1001      127     2275 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/qvm_isa.json
--rw-r--r--   0     1001      127      148 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/secrets.toml
--rw-r--r--   0     1001      127      298 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/settings.toml
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/Cargo.toml
--rw-r--r--   0     1001      127      203 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/.flake8
--rw-r--r--   0     1001      127       64 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/.stubtest-allowlist
--rw-r--r--   0     1001      127    46496 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/CHANGELOG.md
--rw-r--r--   0     1001      127     1332 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/Makefile.toml
--rw-r--r--   0     1001      127     3674 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/README.md
--rw-r--r--   0     1001      127       71 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/build.rs
--rw-r--r--   0     1001      127    34757 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/poetry.lock
--rw-r--r--   0     1001      127      257 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/__init__.py
--rw-r--r--   0     1001      127    17080 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/__init__.pyi
--rw-r--r--   0     1001      127       29 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/client.py
--rw-r--r--   0     1001      127     4116 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/client.pyi
--rw-r--r--   0     1001      127      100 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/compiler/__init__.py
--rw-r--r--   0     1001      127      299 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/compiler/__init__.pyi
--rw-r--r--   0     1001      127    11882 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/compiler/quilc.pyi
--rw-r--r--   0     1001      127      736 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/diagnostics.py
--rw-r--r--   0     1001      127        0 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/py.typed
--rw-r--r--   0     1001      127       85 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/__init__.py
--rw-r--r--   0     1001      127     7954 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/__init__.pyi
--rw-r--r--   0     1001      127    21174 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/api.pyi
--rw-r--r--   0     1001      127    12322 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/isa.pyi
--rw-r--r--   0     1001      127     1884 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/rewrite_arithmetic.pyi
--rw-r--r--   0     1001      127     5935 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/translation.pyi
--rw-r--r--   0     1001      127       85 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qvm/__init__.py
--rw-r--r--   0     1001      127     5671 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qvm/__init__.pyi
--rw-r--r--   0     1001      127     9537 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qvm/api.pyi
--rw-r--r--   0     1001      127     1113 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/scripts/patch_grpc_web.py
--rw-r--r--   0     1001      127     6001 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/client.rs
--rw-r--r--   0     1001      127      149 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/compiler/mod.rs
--rw-r--r--   0     1001      127    12242 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/compiler/quilc.rs
--rw-r--r--   0     1001      127    10280 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/executable.rs
--rw-r--r--   0     1001      127    10202 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/execution_data.rs
--rw-r--r--   0     1001      127      637 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/from_py.rs
--rw-r--r--   0     1001      127       16 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/grpc/mod.rs
--rw-r--r--   0     1001      127     1988 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/grpc/models/controller.rs
--rw-r--r--   0     1001      127       20 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/grpc/models/mod.rs
--rw-r--r--   0     1001      127     2064 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/lib.rs
--rw-r--r--   0     1001      127     4303 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/py_sync.rs
--rw-r--r--   0     1001      127    17827 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/api.rs
--rw-r--r--   0     1001      127     4501 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/isa.rs
--rw-r--r--   0     1001      127     1762 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/mod.rs
--rw-r--r--   0     1001      127     4554 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/result_data.rs
--rw-r--r--   0     1001      127     4560 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/rewrite_arithmetic.rs
--rw-r--r--   0     1001      127     6203 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/translation.rs
--rw-r--r--   0     1001      127     8832 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qvm/api.rs
--rw-r--r--   0     1001      127     8478 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qvm/mod.rs
--rw-r--r--   0     1001      127     1248 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/register_data.rs
--rw-r--r--   0     1001      127   410675 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/_fixtures/aspen-m-3.json
--rw-r--r--   0     1001      127     7302 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/_fixtures/device-2q.json
--rw-r--r--   0     1001      127      190 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/_qcs_config/secrets.toml
--rw-r--r--   0     1001      127      605 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/_qcs_config/settings.toml
--rw-r--r--   0     1001      127     1212 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/compiler/__snapshots__/test_quilc.ambr
--rw-r--r--   0     1001      127     4818 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/compiler/test_quilc.py
--rw-r--r--   0     1001      127     3233 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/conftest.py
--rw-r--r--   0     1001      127     5219 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/execution_data/test_execution_data.py
--rw-r--r--   0     1001      127     1384 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qpu/test_api.py
--rw-r--r--   0     1001      127     1096 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qpu/test_isa.py
--rw-r--r--   0     1001      127     2124 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qpu/test_qpu.py
--rw-r--r--   0     1001      127      823 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qpu/test_rewrite_arithmetic.py
--rw-r--r--   0     1001      127     1704 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qpu/test_translation.py
--rw-r--r--   0     1001      127      301 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qvm/test_qvm.py
--rw-r--r--   0     1001      127     2410 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/test_client.py
--rw-r--r--   0     1001      127      154 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/test_diagnostics.py
--rw-r--r--   0     1001      127     1637 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/test_executable.py
--rw-r--r--   0     1001      127      162 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/test_logging.py
--rw-r--r--   0     1001      127   100371 2024-04-17 22:41:28.000000 qcs_sdk_python_grpc_web-0.17.7rc0/Cargo.lock
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.7rc0/Cargo.toml
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.7rc0/pyproject.toml
--rw-r--r--   0     1001      127       85 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qvm/__init__.py
--rw-r--r--   0     1001      127     9537 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qvm/api.pyi
--rw-r--r--   0     1001      127     5671 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qvm/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/py.typed
--rw-r--r--   0     1001      127      736 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/diagnostics.py
--rw-r--r--   0     1001      127       29 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/client.py
--rw-r--r--   0     1001      127      100 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/compiler/__init__.py
--rw-r--r--   0     1001      127      299 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/compiler/__init__.pyi
--rw-r--r--   0     1001      127    11882 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/compiler/quilc.pyi
--rw-r--r--   0     1001      127      257 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/__init__.py
--rw-r--r--   0     1001      127     5935 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/translation.pyi
--rw-r--r--   0     1001      127    12322 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/isa.pyi
--rw-r--r--   0     1001      127       85 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/__init__.py
--rw-r--r--   0     1001      127    21174 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/api.pyi
--rw-r--r--   0     1001      127     7954 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/__init__.pyi
--rw-r--r--   0     1001      127     1884 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/rewrite_arithmetic.pyi
--rw-r--r--   0     1001      127    17080 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/__init__.pyi
--rw-r--r--   0     1001      127     4116 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/client.pyi
--rw-r--r--   0     1001      127     3674 2024-04-17 22:41:15.000000 qcs_sdk_python_grpc_web-0.17.7rc0/README.md
--rw-r--r--   0        0        0     4549 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.7rc0/PKG-INFO
+-rw-r--r--   0     1001      127     2496 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/Cargo.toml
+-rw-r--r--   0     1001      127    44997 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/CHANGELOG.md
+-rw-r--r--   0     1001      127      752 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/Makefile.toml
+-rw-r--r--   0     1001      127     2186 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/README.md
+-rw-r--r--   0     1001      127       95 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/build.rs
+-rw-r--r--   0     1001      127      931 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/delayed_job_retrieval.rs
+-rw-r--r--   0     1001      127     1770 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/execute.rs
+-rw-r--r--   0     1001      127      674 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/libquil.rs
+-rw-r--r--   0     1001      127      767 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/local.rs
+-rw-r--r--   0     1001      127     2154 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/parametric_compilation.rs
+-rw-r--r--   0     1001      127     1277 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/quil_t.rs
+-rw-r--r--   0     1001      127      126 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/bin/diagnostics.rs
+-rw-r--r--   0     1001      127     5479 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/client.rs
+-rw-r--r--   0     1001      127     8277 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/edge.rs
+-rw-r--r--   0     1001      127     6791 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/mod.rs
+-rw-r--r--   0     1001      127     8320 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/operator.rs
+-rw-r--r--   0     1001      127    13686 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/qubit.rs
+-rw-r--r--   0     1001      127    11548 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/libquil.rs
+-rw-r--r--   0     1001      127      198 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/mod.rs
+-rw-r--r--   0     1001      127    16466 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/quilc.rs
+-rw-r--r--   0     1001      127    11529 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/rpcq.rs
+-rw-r--r--   0     1001      127     8271 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/diagnostics.rs
+-rw-r--r--   0     1001      127    36127 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/executable.rs
+-rw-r--r--   0     1001      127    23212 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/execution_data.rs
+-rw-r--r--   0     1001      127     1984 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/lib.rs
+-rw-r--r--   0     1001      127    25522 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/api.rs
+-rw-r--r--   0     1001      127    12027 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/execution.rs
+-rw-r--r--   0     1001      127     3187 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/mod.rs
+-rw-r--r--   0     1001      127     6058 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/result_data.rs
+-rw-r--r--   0     1001      127    17418 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/rewrite_arithmetic.rs
+-rw-r--r--   0     1001      127      137 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_allocates_for_multiple_expressions-2.snap
+-rw-r--r--   0     1001      127      131 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_allocates_for_multiple_expressions.snap
+-rw-r--r--   0     1001      127      112 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_frequency_expressions-2.snap
+-rw-r--r--   0     1001      127      119 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_frequency_expressions.snap
+-rw-r--r--   0     1001      127      127 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_phases.snap
+-rw-r--r--   0     1001      127      111 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_set_scale_units.snap
+-rw-r--r--   0     1001      127      134 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_substitutes_and_reuses_gate_expressions.snap
+-rw-r--r--   0     1001      127      127 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_substitutes_gate_parameters.snap
+-rw-r--r--   0     1001      127     9322 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/translation.rs
+-rw-r--r--   0     1001      127     4292 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/execution.rs
+-rw-r--r--   0     1001      127    13970 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/http.rs
+-rw-r--r--   0     1001      127     6966 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/libquil.rs
+-rw-r--r--   0     1001      127    11138 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/mod.rs
+-rw-r--r--   0     1001      127      154 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/snapshots/qcs__qvm__test__apply_valid_parameters_to_program.snap
+-rw-r--r--   0     1001      127     1938 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/register_data.rs
+-rw-r--r--   0     1001      127   104426 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/aspen_9_isa.json
+-rw-r--r--   0     1001      127     1921 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/basic_qvm.rs
+-rw-r--r--   0     1001      127      558 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/bell_state_response_data.hex
+-rw-r--r--   0     1001      127    81629 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/compiler-isa-Aspen-8.json
+-rw-r--r--   0     1001      127    14144 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/mocked_qpu.rs
+-rw-r--r--   0     1001      127     2071 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/parametric_compilation.rs
+-rw-r--r--   0     1001      127    71490 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qcs-isa-Aspen-8.json
+-rw-r--r--   0     1001      127     3933 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qvm_api.rs
+-rw-r--r--   0     1001      127     2275 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qvm_isa.json
+-rw-r--r--   0     1001      127      148 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/secrets.toml
+-rw-r--r--   0     1001      127      298 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/settings.toml
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/Cargo.toml
+-rw-r--r--   0     1001      127      203 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/.flake8
+-rw-r--r--   0     1001      127       64 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/.stubtest-allowlist
+-rw-r--r--   0     1001      127    46591 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/CHANGELOG.md
+-rw-r--r--   0     1001      127     1332 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/Makefile.toml
+-rw-r--r--   0     1001      127     3674 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/README.md
+-rw-r--r--   0     1001      127       71 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/build.rs
+-rw-r--r--   0     1001      127    34757 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/poetry.lock
+-rw-r--r--   0     1001      127      257 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/__init__.py
+-rw-r--r--   0     1001      127    17080 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/__init__.pyi
+-rw-r--r--   0     1001      127       29 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/client.py
+-rw-r--r--   0     1001      127     4116 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/client.pyi
+-rw-r--r--   0     1001      127      100 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/compiler/__init__.py
+-rw-r--r--   0     1001      127      299 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/compiler/__init__.pyi
+-rw-r--r--   0     1001      127    11882 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/compiler/quilc.pyi
+-rw-r--r--   0     1001      127      736 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/diagnostics.py
+-rw-r--r--   0     1001      127        0 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/py.typed
+-rw-r--r--   0     1001      127       85 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/__init__.py
+-rw-r--r--   0     1001      127     7954 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/__init__.pyi
+-rw-r--r--   0     1001      127    21174 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/api.pyi
+-rw-r--r--   0     1001      127    12322 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/isa.pyi
+-rw-r--r--   0     1001      127     1884 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/rewrite_arithmetic.pyi
+-rw-r--r--   0     1001      127     5935 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/translation.pyi
+-rw-r--r--   0     1001      127       85 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qvm/__init__.py
+-rw-r--r--   0     1001      127     5671 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qvm/__init__.pyi
+-rw-r--r--   0     1001      127     9537 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qvm/api.pyi
+-rw-r--r--   0     1001      127     1113 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/scripts/patch_grpc_web.py
+-rw-r--r--   0     1001      127     6001 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/client.rs
+-rw-r--r--   0     1001      127      149 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/compiler/mod.rs
+-rw-r--r--   0     1001      127    12242 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/compiler/quilc.rs
+-rw-r--r--   0     1001      127    10280 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/executable.rs
+-rw-r--r--   0     1001      127    10202 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/execution_data.rs
+-rw-r--r--   0     1001      127      637 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/from_py.rs
+-rw-r--r--   0     1001      127       16 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     1988 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/grpc/models/controller.rs
+-rw-r--r--   0     1001      127       20 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/grpc/models/mod.rs
+-rw-r--r--   0     1001      127     2064 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/lib.rs
+-rw-r--r--   0     1001      127     4303 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/py_sync.rs
+-rw-r--r--   0     1001      127    17827 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/api.rs
+-rw-r--r--   0     1001      127     4501 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/isa.rs
+-rw-r--r--   0     1001      127     1762 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/mod.rs
+-rw-r--r--   0     1001      127     4554 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/result_data.rs
+-rw-r--r--   0     1001      127     4560 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/rewrite_arithmetic.rs
+-rw-r--r--   0     1001      127     6203 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/translation.rs
+-rw-r--r--   0     1001      127     8832 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qvm/api.rs
+-rw-r--r--   0     1001      127     8478 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qvm/mod.rs
+-rw-r--r--   0     1001      127     1248 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/register_data.rs
+-rw-r--r--   0     1001      127   410675 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_fixtures/aspen-m-3.json
+-rw-r--r--   0     1001      127     7302 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_fixtures/device-2q.json
+-rw-r--r--   0     1001      127      190 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_qcs_config/secrets.toml
+-rw-r--r--   0     1001      127      605 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_qcs_config/settings.toml
+-rw-r--r--   0     1001      127     1212 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/compiler/__snapshots__/test_quilc.ambr
+-rw-r--r--   0     1001      127     4818 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/compiler/test_quilc.py
+-rw-r--r--   0     1001      127     3233 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/conftest.py
+-rw-r--r--   0     1001      127     5219 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/execution_data/test_execution_data.py
+-rw-r--r--   0     1001      127     1384 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_api.py
+-rw-r--r--   0     1001      127     1096 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_isa.py
+-rw-r--r--   0     1001      127     2124 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_qpu.py
+-rw-r--r--   0     1001      127      823 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_rewrite_arithmetic.py
+-rw-r--r--   0     1001      127     1704 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_translation.py
+-rw-r--r--   0     1001      127      301 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qvm/test_qvm.py
+-rw-r--r--   0     1001      127     2410 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_client.py
+-rw-r--r--   0     1001      127      154 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_diagnostics.py
+-rw-r--r--   0     1001      127     1637 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_executable.py
+-rw-r--r--   0     1001      127      162 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_logging.py
+-rw-r--r--   0     1001      127   100372 2024-04-24 19:33:43.000000 qcs_sdk_python_grpc_web-0.17.8rc0/Cargo.lock
+-rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.8rc0/Cargo.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.8rc0/pyproject.toml
+-rw-r--r--   0     1001      127       85 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qvm/__init__.py
+-rw-r--r--   0     1001      127     9537 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qvm/api.pyi
+-rw-r--r--   0     1001      127     5671 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qvm/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/py.typed
+-rw-r--r--   0     1001      127      736 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/diagnostics.py
+-rw-r--r--   0     1001      127       29 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/client.py
+-rw-r--r--   0     1001      127      100 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/compiler/__init__.py
+-rw-r--r--   0     1001      127      299 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/compiler/__init__.pyi
+-rw-r--r--   0     1001      127    11882 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/compiler/quilc.pyi
+-rw-r--r--   0     1001      127      257 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/__init__.py
+-rw-r--r--   0     1001      127     5935 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/translation.pyi
+-rw-r--r--   0     1001      127    12322 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/isa.pyi
+-rw-r--r--   0     1001      127       85 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/__init__.py
+-rw-r--r--   0     1001      127    21174 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/api.pyi
+-rw-r--r--   0     1001      127     7954 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/__init__.pyi
+-rw-r--r--   0     1001      127     1884 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/rewrite_arithmetic.pyi
+-rw-r--r--   0     1001      127    17080 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/__init__.pyi
+-rw-r--r--   0     1001      127     4116 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/client.pyi
+-rw-r--r--   0     1001      127     3674 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/README.md
+-rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.8rc0/PKG-INFO
```

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/Cargo.toml` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "qcs"
 description = "High level interface for running Quil on a QPU"
-version = "0.21.7-rc.0"
+version = "0.21.8-rc.0"
 edition = "2018"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/qcs-sdk-rust"
 keywords = ["pyquil", "SDK", "Rigetti", "Quil", "Quantum"]
 categories = ["api-bindings", "compilers", "science", "emulators"]
 readme = "./README.md"
```

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/CHANGELOG.md` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 0.21.8-rc.0
+
+### Features
+
+- Update quil-rs (#464)
+
+## 0.21.7
+
+### Features
+
+- Update quil
+
 ## 0.21.7-rc.0
 
 ### Features
 
 - Update quil
 
 ## 0.21.6
```

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/Makefile.toml` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/Makefile.toml`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/README.md` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/README.md`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/delayed_job_retrieval.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/delayed_job_retrieval.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/execute.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/execute.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/libquil.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/libquil.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/local.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/local.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/parametric_compilation.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/parametric_compilation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/examples/quil_t.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/quil_t.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/client.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/client.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/isa/edge.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/edge.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/isa/mod.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/isa/operator.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/operator.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/isa/qubit.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/qubit.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/libquil.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/libquil.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/quilc.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/quilc.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/compiler/rpcq.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/rpcq.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/diagnostics.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/diagnostics.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/executable.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/executable.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/execution_data.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/execution_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/lib.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/api.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/api.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/execution.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/execution.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/mod.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/result_data.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/result_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/rewrite_arithmetic.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/rewrite_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qpu/translation.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/translation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qvm/execution.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/execution.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qvm/http.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/http.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qvm/libquil.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/libquil.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/qvm/mod.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/src/register_data.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/register_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/aspen_9_isa.json` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/aspen_9_isa.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/basic_qvm.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/basic_qvm.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/bell_state_response_data.hex` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/bell_state_response_data.hex`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/compiler-isa-Aspen-8.json` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/compiler-isa-Aspen-8.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/mocked_qpu.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/mocked_qpu.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/parametric_compilation.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/parametric_compilation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/qcs-isa-Aspen-8.json` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qcs-isa-Aspen-8.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/qvm_api.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qvm_api.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/lib/tests/qvm_isa.json` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qvm_isa.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/Cargo.toml` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "qcs-sdk-python-grpc-web"
 description = "Python bindings to qcs-sdk-rust"
-version = "0.17.7-rc.0"
+version = "0.17.8-rc.0"
 edition = "2021"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/qcs-sdk-rust"
 keywords = [ "pyquil", "SDK", "Rigetti", "Quil", "Quantum",]
 categories = [ "api-bindings", "compilers", "science", "emulators",]
 readme = "./README.md"
```

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/CHANGELOG.md` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 0.17.8-rc.0
+
+### Features
+
+- Update quil-rs (#464)
+
+## 0.17.7
+
+### Features
+
+- Update quil
+
 ## 0.17.7-rc.0
 
 ### Features
 
 - Update quil
 
 ## 0.17.6
```

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/Makefile.toml` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/Makefile.toml`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/README.md` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/README.md`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/poetry.lock` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/client.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/client.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/compiler/quilc.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/compiler/quilc.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/diagnostics.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/diagnostics.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/api.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/api.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/isa.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/isa.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/rewrite_arithmetic.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/rewrite_arithmetic.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qpu/translation.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/translation.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qvm/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/qcs_sdk/qvm/api.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qvm/api.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/scripts/patch_grpc_web.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/scripts/patch_grpc_web.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/client.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/client.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/compiler/quilc.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/compiler/quilc.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/executable.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/executable.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/execution_data.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/execution_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/from_py.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/grpc/models/controller.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/grpc/models/controller.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/lib.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/py_sync.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/py_sync.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/api.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/api.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/isa.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/isa.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/mod.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/result_data.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/result_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/rewrite_arithmetic.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/rewrite_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qpu/translation.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/translation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qvm/api.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qvm/api.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/qvm/mod.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qvm/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/src/register_data.rs` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/register_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/_fixtures/aspen-m-3.json` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_fixtures/aspen-m-3.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/_fixtures/device-2q.json` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_fixtures/device-2q.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/_qcs_config/settings.toml` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_qcs_config/settings.toml`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/compiler/__snapshots__/test_quilc.ambr` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/compiler/__snapshots__/test_quilc.ambr`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/compiler/test_quilc.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/compiler/test_quilc.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/conftest.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/execution_data/test_execution_data.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/execution_data/test_execution_data.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qpu/test_api.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_api.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qpu/test_isa.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_isa.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qpu/test_qpu.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_qpu.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qpu/test_rewrite_arithmetic.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_rewrite_arithmetic.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/qpu/test_translation.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_translation.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/test_client.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/crates/python/tests/test_executable.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_executable.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/Cargo.lock` & `qcs_sdk_python_grpc_web-0.17.8rc0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1085,15 +1085,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
 dependencies = [
  "futures-util",
  "http",
  "hyper",
  "log",
- "rustls 0.21.10",
+ "rustls 0.21.11",
  "rustls-native-certs 0.6.3",
  "tokio",
  "tokio-rustls 0.24.1",
 ]
 
 [[package]]
 name = "hyper-socks2"
@@ -2089,15 +2089,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.53",
 ]
 
 [[package]]
 name = "qcs"
-version = "0.21.7-rc.0"
+version = "0.21.8-rc.0"
 dependencies = [
  "assert2",
  "async-trait",
  "built",
  "cached",
  "derive_builder",
  "enum-as-inner",
@@ -2225,15 +2225,15 @@
  "tracing",
  "url",
  "urlpattern",
 ]
 
 [[package]]
 name = "qcs-sdk-python-grpc-web"
-version = "0.17.7-rc.0"
+version = "0.17.8-rc.0"
 dependencies = [
  "async-trait",
  "numpy",
  "once_cell",
  "paste",
  "pyo3",
  "pyo3-asyncio",
@@ -2255,16 +2255,16 @@
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quil-rs"
-version = "0.25.1"
-source = "git+https://github.com/rigetti/quil-rs?tag=quil-py/v0.9.1#4179fb03feff6b83edfb7a0448b0b3967ed28212"
+version = "0.26.0"
+source = "git+https://github.com/rigetti/quil-rs?tag=quil-py/v0.10.0#25966563850ed151fad0cdab3f6931bdd90be8f8"
 dependencies = [
  "approx",
  "indexmap 2.2.6",
  "itertools 0.12.1",
  "lexical",
  "ndarray",
  "nom 7.1.3",
@@ -2401,15 +2401,15 @@
  "js-sys",
  "log",
  "mime",
  "mime_guess",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls 0.21.10",
+ "rustls 0.21.11",
  "rustls-native-certs 0.6.3",
  "rustls-pemfile 1.0.4",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
  "system-configuration",
@@ -2565,29 +2565,29 @@
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.21.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "7fecbfb7b1444f477b345853b1fce097a2c6fb637b2bfb87e6bc5db0f043fae4"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki 0.101.7",
  "sct",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.22.2"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e87c9956bd9807afa1f77e0f7594af32566e830e088a5576d27c5b6f30f49d41"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
  "ring",
  "rustls-pki-types",
  "rustls-webpki 0.102.2",
  "subtle",
  "zeroize",
@@ -3188,25 +3188,25 @@
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
- "rustls 0.21.10",
+ "rustls 0.21.11",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "775e0c0f0adb3a2f22a00c4745d728b479985fc15ee7ca6a2608388c5569860f"
 dependencies = [
- "rustls 0.22.2",
+ "rustls 0.22.4",
  "rustls-pki-types",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-socks"
 version = "0.5.1"
```

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/Cargo.toml` & `qcs_sdk_python_grpc_web-0.17.8rc0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 [profile.release]
 strip = true
 lto = true
 codegen-units = 1
 
 [workspace.dependencies.quil-rs]
-version = "0.25.1"
+version = "0.26.0"
 git = "https://github.com/rigetti/quil-rs"
-tag = "quil-py/v0.9.1"
+tag = "quil-py/v0.10.0"
 
 [workspace.dependencies.ndarray]
 version = "0.15.6"
 features = [ "serde",]
 
 [workspace.dependencies.pyo3]
 version = "0.20.0"
```

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/pyproject.toml` & `qcs_sdk_python_grpc_web-0.17.8rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "qcs-sdk-python-grpc-web"
-version = "0.17.7-rc.0"
+version = "0.17.8-rc.0"
 description = "Python interface for the QCS Rust SDK"
 readme = "README.md"
 classifiers = [ "Development Status :: 3 - Alpha", "License :: OSI Approved :: Apache Software License", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10", "Programming Language :: Python :: 3.11", "Operating System :: OS Independent",]
-dependencies = [ "quil==0.9.1",]
+dependencies = [ "quil==0.10.0",]
 [[project.authors]]
 name = "Rigetti Computing"
 email = "softapps@rigetti.com"
 
 [[project.authors]]
 name = "Mark Skilbeck"
 email = "mark.skilbeck@rigetti.com"
@@ -26,15 +26,15 @@
 build-backend = "maturin"
 
 [project.license]
 text = "Apache-2.0"
 
 [tool.poetry]
 name = "qcs-sdk-python"
-version = "0.17.7-rc.0"
+version = "0.17.8-rc.0"
 description = "Python interface for the QCS Rust SDK"
 readme = "README.md"
 authors = [ "Rigetti Computing <softapps@rigetti.com>", "Mark Skilbeck <mark.skilbeck@rigetti.com>", "Marquess Valdez <mvaldez@rigetti.com>", "Randall Fulton <rfulton@rigetti.com>",]
 
 [tool.maturin]
 features = [ "pyo3/extension-module",]
 bindings = "pyo3"
```

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qvm/api.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qvm/api.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qvm/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/diagnostics.py` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/diagnostics.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/compiler/quilc.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/compiler/quilc.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/translation.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/translation.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/isa.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/isa.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/api.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/api.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/qpu/rewrite_arithmetic.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/rewrite_arithmetic.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/qcs_sdk/client.pyi` & `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/client.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/README.md` & `qcs_sdk_python_grpc_web-0.17.8rc0/README.md`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.7rc0/PKG-INFO` & `qcs_sdk_python_grpc_web-0.17.8rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: qcs-sdk-python-grpc-web
-Version: 0.17.7rc0
+Version: 0.17.8rc0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Dist: quil ==0.9.1
+Requires-Dist: quil ==0.10.0
 Summary: Python interface for the QCS Rust SDK
 Keywords: pyquil,SDK,Rigetti,Quil,Quantum
 Author-email: Rigetti Computing <softapps@rigetti.com>, Mark Skilbeck <mark.skilbeck@rigetti.com>, Marquess Valdez <mvaldez@rigetti.com>, Randall Fulton <rfulton@rigetti.com>
 License: Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/rigetti/qcs-sdk-rust
```

