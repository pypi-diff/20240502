# Comparing `tmp/quil-0.9.1.tar.gz` & `tmp/quil-0.9.1rc0.tar.gz`

## Comparing `quil-0.9.1.tar` & `quil-0.9.1rc0.tar`

### file list

```diff
@@ -1,209 +1,209 @@
--rw-r--r--   0     1001      127     1414 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/Cargo.toml
--rw-r--r--   0     1001      127    44490 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/CHANGELOG.md
--rw-r--r--   0     1001      127      954 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/README.md
--rw-r--r--   0     1001      127     1692 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/benches/corpus.rs
--rw-r--r--   0     1001      127      941 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/benches/get_frames_for_instruction.rs
--rw-r--r--   0     1001      127      985 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/benches/parser.rs
--rw-r--r--   0     1001      127   803952 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/benches/sample-calibrations.quil
--rw-r--r--   0     1001      127     1478 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/benches/scheduled_program_from_program.rs
--rw-r--r--   0     1001      127      969 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/benches/simplification.rs
--rw-r--r--   0     1001      127    12979 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/benches/test_expressions.txt
--rw-r--r--   0     1001      127     6316 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/examples/generate_test_expressions.rs
--rw-r--r--   0     1001      127    38082 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/expression/mod.rs
--rw-r--r--   0     1001      127    34338 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/expression/simplification/by_hand.rs
--rw-r--r--   0     1001      127    12745 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/expression/simplification/mod.rs
--rw-r--r--   0     1001      127     1002 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/hash.rs
--rw-r--r--   0     1001      127     5302 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/calibration.rs
--rw-r--r--   0     1001      127     6478 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/circuit.rs
--rw-r--r--   0     1001      127     9937 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/classical.rs
--rw-r--r--   0     1001      127     5260 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/control_flow.rs
--rw-r--r--   0     1001      127     6939 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/declaration.rs
--rw-r--r--   0     1001      127     9842 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/frame.rs
--rw-r--r--   0     1001      127    43954 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/gate.rs
--rw-r--r--   0     1001      127      771 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/measurement.rs
--rw-r--r--   0     1001      127    39443 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/mod.rs
--rw-r--r--   0     1001      127     1798 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/pragma.rs
--rw-r--r--   0     1001      127     3425 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/qubit.rs
--rw-r--r--   0     1001      127      654 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/reset.rs
--rw-r--r--   0     1001      127      133 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Fixed Qubit.snap
--rw-r--r--   0     1001      127      133 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Variable Qubit.snap
--rw-r--r--   0     1001      127      124 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition No Params.snap
--rw-r--r--   0     1001      127      167 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Params.snap
--rw-r--r--   0     1001      127      160 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Single Param.snap
--rw-r--r--   0     1001      127      109 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Basic Declaration.snap
--rw-r--r--   0     1001      127      141 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration with Offsets.snap
--rw-r--r--   0     1001      127      125 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration.snap
--rw-r--r--   0     1001      127      191 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Parameterized GateDefinition.snap
--rw-r--r--   0     1001      127      178 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Pauli Sum GateDefinition.snap
--rw-r--r--   0     1001      127      139 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Permutation GateDefinition.snap
--rw-r--r--   0     1001      127      143 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/snapshots/quil_rs__instruction__waveform__test_waveform_definition__display@Simple WaveformDefinition.snap
--rw-r--r--   0     1001      127     1528 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/timing.rs
--rw-r--r--   0     1001      127     3666 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/instruction/waveform.rs
--rw-r--r--   0     1001      127     1910 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/lib.rs
--rw-r--r--   0     1001      127     1013 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/macros.rs
--rw-r--r--   0     1001      127    36217 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/command.rs
--rw-r--r--   0     1001      127    23080 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/common.rs
--rw-r--r--   0     1001      127     5970 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/error/error.rs
--rw-r--r--   0     1001      127     2519 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/error/input.rs
--rw-r--r--   0     1001      127     3242 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/error/internal.rs
--rw-r--r--   0     1001      127     1004 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/error/kind.rs
--rw-r--r--   0     1001      127     2685 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/error/mod.rs
--rw-r--r--   0     1001      127    17487 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/expression.rs
--rw-r--r--   0     1001      127     2212 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/gate.rs
--rw-r--r--   0     1001      127    40974 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/instruction.rs
--rw-r--r--   0     1001      127     1380 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/lexer/error.rs
--rw-r--r--   0     1001      127    17439 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/lexer/mod.rs
--rw-r--r--   0     1001      127     4222 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/lexer/quoted_strings.rs
--rw-r--r--   0     1001      127     3357 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/lexer/wrapped_parsers.rs
--rw-r--r--   0     1001      127     4162 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/macros.rs
--rw-r--r--   0     1001      127     2446 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/mod.rs
--rw-r--r--   0     1001      127     5841 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/parser/token.rs
--rw-r--r--   0     1001      127    25985 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/analysis/control_flow_graph.rs
--rw-r--r--   0     1001      127      974 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/analysis/mod.rs
--rw-r--r--   0     1001      127     9591 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/analysis/qubit_graph.rs
--rw-r--r--   0     1001      127      889 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap
--rw-r--r--   0     1001      127     1329 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/analysis/test_programs.rs
--rw-r--r--   0     1001      127    23626 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/calibration.rs
--rw-r--r--   0     1001      127     7227 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/calibration_set.rs
--rw-r--r--   0     1001      127     2283 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/error/leftover.rs
--rw-r--r--   0     1001      127     3068 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/error/mod.rs
--rw-r--r--   0     1001      127     2252 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/error/result.rs
--rw-r--r--   0     1001      127     2725 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/error/syntax.rs
--rw-r--r--   0     1001      127     8742 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/frame.rs
--rw-r--r--   0     1001      127    17109 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/memory.rs
--rw-r--r--   0     1001      127    51116 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/mod.rs
--rw-r--r--   0     1001      127    26031 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/graph.rs
--rw-r--r--   0     1001      127    20046 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/graphviz_dot.rs
--rw-r--r--   0     1001      127      456 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/mod.rs
--rw-r--r--   0     1001      127    16670 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/schedule.rs
--rw-r--r--   0     1001      127     2678 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap
--rw-r--r--   0     1001      127     1560 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap
--rw-r--r--   0     1001      127     1166 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap
--rw-r--r--   0     1001      127     1732 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap
--rw-r--r--   0     1001      127     1112 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap
--rw-r--r--   0     1001      127     1195 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap
--rw-r--r--   0     1001      127     1780 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap
--rw-r--r--   0     1001      127     1653 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap
--rw-r--r--   0     1001      127     1003 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap
--rw-r--r--   0     1001      127     1032 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap
--rw-r--r--   0     1001      127      552 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap
--rw-r--r--   0     1001      127     1540 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap
--rw-r--r--   0     1001      127     1073 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap
--rw-r--r--   0     1001      127     1338 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap
--rw-r--r--   0     1001      127     1866 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap
--rw-r--r--   0     1001      127      854 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap
--rw-r--r--   0     1001      127      867 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap
--rw-r--r--   0     1001      127      887 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap
--rw-r--r--   0     1001      127     1892 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap
--rw-r--r--   0     1001      127      839 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap
--rw-r--r--   0     1001      127      768 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap
--rw-r--r--   0     1001      127      591 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap
--rw-r--r--   0     1001      127      793 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap
--rw-r--r--   0     1001      127      852 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap
--rw-r--r--   0     1001      127      585 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap
--rw-r--r--   0     1001      127      227 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Instruction-Match.snap
--rw-r--r--   0     1001      127      136 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Literal-Parameter.snap
--rw-r--r--   0     1001      127      215 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Multiple-Qubits.snap
--rw-r--r--   0     1001      127      476 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Param-Precedence.snap
--rw-r--r--   0     1001      127      210 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Simple.snap
--rw-r--r--   0     1001      127      141 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Variable-Qubit.snap
--rw-r--r--   0     1001      127      159 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@FenceVariableQubit.snap
--rw-r--r--   0     1001      127      309 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Measure-Calibration.snap
--rw-r--r--   0     1001      127      261 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Fixed-Match.snap
--rw-r--r--   0     1001      127      155 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-No-Qubit-Match.snap
--rw-r--r--   0     1001      127      254 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Variable-Match.snap
--rw-r--r--   0     1001      127      174 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@ShiftPhase.snap
--rw-r--r--   0     1001      127      167 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__tests__filter_instructions.snap
--rw-r--r--   0     1001      127     3755 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap
--rw-r--r--   0     1001      127      425 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__tests__wrap_in_loop.snap
--rw-r--r--   0     1001      127    35001 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/program/type_check.rs
--rw-r--r--   0     1001      127     2422 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/quil.rs
--rw-r--r--   0     1001      127     2749 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/reserved.rs
--rw-r--r--   0     1001      127     2109 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/validation/identifier.rs
--rw-r--r--   0     1001      127       20 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/src/validation/mod.rs
--rw-r--r--   0     1001      127      724 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/calibration_test.rs
--rw-r--r--   0     1001      127      742 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/programs/calibration_cz.quil
--rw-r--r--   0     1001      127     1888 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/programs/calibration_cz_phase.quil
--rw-r--r--   0     1001      127     3266 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/programs/calibration_measure.quil
--rw-r--r--   0     1001      127     1588 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/programs/calibration_rx.quil
--rw-r--r--   0     1001      127     1786 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/programs/calibration_xy.quil
--rw-r--r--   0     1001      127      747 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap
--rw-r--r--   0     1001      127     1797 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap
--rw-r--r--   0     1001      127     3187 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap
--rw-r--r--   0     1001      127     1519 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap
--rw-r--r--   0     1001      127     1719 2024-04-17 20:38:44.000000 quil-0.9.1/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap
--rw-r--r--   0        0        0     1218 1970-01-01 00:00:00.000000 quil-0.9.1/quil-py/Cargo.toml
--rw-r--r--   0     1001      127      203 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/.flake8
--rw-r--r--   0     1001      127       10 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/.stubtest-allowlist
--rw-r--r--   0     1001      127    20924 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/CHANGELOG.md
--rw-r--r--   0     1001      127     1258 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/Makefile.toml
--rw-r--r--   0     1001      127      777 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/README-py.md
--rw-r--r--   0     1001      127      337 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/README.md
--rw-r--r--   0     1001      127       71 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/build.rs
--rw-r--r--   0     1001      127      403 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/make_docs.py
--rw-r--r--   0     1001      127      135 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/out/index.html
--rw-r--r--   0     1001      127    34673 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/out/quil/quil.html
--rw-r--r--   0     1001      127    34581 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/out/quil.html
--rw-r--r--   0     1001      127    20706 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/out/search.js
--rw-r--r--   0     1001      127    32817 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/poetry.lock
--rw-r--r--   0     1001      127      283 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/__init__.pyi
--rw-r--r--   0     1001      127       30 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/expression/__init__.py
--rw-r--r--   0     1001      127     7528 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/expression/__init__.pyi
--rw-r--r--   0     1001      127      123 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/instructions/__init__.py
--rw-r--r--   0     1001      127    91194 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/instructions/__init__.pyi
--rw-r--r--   0     1001      127      127 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/program/__init__.py
--rw-r--r--   0     1001      127    17967 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/program/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/py.typed
--rw-r--r--   0     1001      127      160 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/validation/__init__.py
--rw-r--r--   0     1001      127       39 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/validation/__init__.pyi
--rw-r--r--   0     1001      127       41 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/validation/identifier.py
--rw-r--r--   0     1001      127      419 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil/validation/identifier.pyi
--rw-r--r--   0     1001      127    34593 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/quil.html
--rw-r--r--   0     1001      127     6656 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/expression.rs
--rw-r--r--   0     1001      127     2838 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/calibration.rs
--rw-r--r--   0     1001      127     1251 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/circuit.rs
--rw-r--r--   0     1001      127    11440 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/classical.rs
--rw-r--r--   0     1001      127     4295 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/control_flow.rs
--rw-r--r--   0     1001      127     5561 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/declaration.rs
--rw-r--r--   0     1001      127     9507 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/frame.rs
--rw-r--r--   0     1001      127     8394 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/gate.rs
--rw-r--r--   0     1001      127     1056 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/measurement.rs
--rw-r--r--   0     1001      127     8741 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/mod.rs
--rw-r--r--   0     1001      127     1852 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/pragma.rs
--rw-r--r--   0     1001      127      978 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/qubit.rs
--rw-r--r--   0     1001      127      738 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/reset.rs
--rw-r--r--   0     1001      127     1591 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/timing.rs
--rw-r--r--   0     1001      127     2443 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/instruction/waveform.rs
--rw-r--r--   0     1001      127     1967 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/lib.rs
--rw-r--r--   0     1001      127     2982 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/program/analysis.rs
--rw-r--r--   0     1001      127     4156 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/program/calibration.rs
--rw-r--r--   0     1001      127     2774 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/program/frame.rs
--rw-r--r--   0     1001      127      897 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/program/memory.rs
--rw-r--r--   0     1001      127    12676 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/program/mod.rs
--rw-r--r--   0     1001      127     1970 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/program/scheduling.rs
--rw-r--r--   0     1001      127     1136 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/validation/identifier.rs
--rw-r--r--   0     1001      127      151 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/src/validation/mod.rs
--rw-r--r--   0     1001      127     1617 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/test/instructions/test_copy.py
--rw-r--r--   0     1001      127      351 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/test/instructions/test_gate.py
--rw-r--r--   0     1001      127      137 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/test/program/__snapshots__/test_program.ambr
--rw-r--r--   0     1001      127     4596 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/test/program/test_program.py
--rw-r--r--   0     1001      127     1025 2024-04-17 20:38:44.000000 quil-0.9.1/quil-py/test/test_eq.py
--rw-r--r--   0     1001      127    50466 2024-04-17 20:38:52.000000 quil-0.9.1/Cargo.lock
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 quil-0.9.1/Cargo.toml
--rw-r--r--   0        0        0     3107 1970-01-01 00:00:00.000000 quil-0.9.1/pyproject.toml
--rw-r--r--   0     1001      127      127 2024-04-17 20:38:44.000000 quil-0.9.1/quil/program/__init__.py
--rw-r--r--   0     1001      127    17967 2024-04-17 20:38:44.000000 quil-0.9.1/quil/program/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-04-17 20:38:44.000000 quil-0.9.1/quil/py.typed
--rw-r--r--   0     1001      127      123 2024-04-17 20:38:44.000000 quil-0.9.1/quil/instructions/__init__.py
--rw-r--r--   0     1001      127    91194 2024-04-17 20:38:44.000000 quil-0.9.1/quil/instructions/__init__.pyi
--rw-r--r--   0     1001      127       30 2024-04-17 20:38:44.000000 quil-0.9.1/quil/expression/__init__.py
--rw-r--r--   0     1001      127     7528 2024-04-17 20:38:44.000000 quil-0.9.1/quil/expression/__init__.pyi
--rw-r--r--   0     1001      127      283 2024-04-17 20:38:44.000000 quil-0.9.1/quil/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-17 20:38:44.000000 quil-0.9.1/quil/__init__.pyi
--rw-r--r--   0     1001      127       41 2024-04-17 20:38:44.000000 quil-0.9.1/quil/validation/identifier.py
--rw-r--r--   0     1001      127      160 2024-04-17 20:38:44.000000 quil-0.9.1/quil/validation/__init__.py
--rw-r--r--   0     1001      127       39 2024-04-17 20:38:44.000000 quil-0.9.1/quil/validation/__init__.pyi
--rw-r--r--   0     1001      127      419 2024-04-17 20:38:44.000000 quil-0.9.1/quil/validation/identifier.pyi
--rw-r--r--   0     1001      127      777 2024-04-17 20:38:44.000000 quil-0.9.1/README-py.md
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 quil-0.9.1/PKG-INFO
+-rw-r--r--   0     1001      127     1419 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/Cargo.toml
+-rw-r--r--   0     1001      127    44400 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/CHANGELOG.md
+-rw-r--r--   0     1001      127      954 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/README.md
+-rw-r--r--   0     1001      127     1692 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/corpus.rs
+-rw-r--r--   0     1001      127      941 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/get_frames_for_instruction.rs
+-rw-r--r--   0     1001      127      985 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/parser.rs
+-rw-r--r--   0     1001      127   803952 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/sample-calibrations.quil
+-rw-r--r--   0     1001      127     1478 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/scheduled_program_from_program.rs
+-rw-r--r--   0     1001      127      969 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/simplification.rs
+-rw-r--r--   0     1001      127    12979 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/test_expressions.txt
+-rw-r--r--   0     1001      127     6316 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/examples/generate_test_expressions.rs
+-rw-r--r--   0     1001      127    38082 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/expression/mod.rs
+-rw-r--r--   0     1001      127    34338 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/expression/simplification/by_hand.rs
+-rw-r--r--   0     1001      127    12745 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/expression/simplification/mod.rs
+-rw-r--r--   0     1001      127     1002 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/hash.rs
+-rw-r--r--   0     1001      127     5302 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/calibration.rs
+-rw-r--r--   0     1001      127     6478 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/circuit.rs
+-rw-r--r--   0     1001      127     9937 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/classical.rs
+-rw-r--r--   0     1001      127     5260 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/control_flow.rs
+-rw-r--r--   0     1001      127     6939 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/declaration.rs
+-rw-r--r--   0     1001      127     9842 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/frame.rs
+-rw-r--r--   0     1001      127    43954 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/gate.rs
+-rw-r--r--   0     1001      127      771 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/measurement.rs
+-rw-r--r--   0     1001      127    39443 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/mod.rs
+-rw-r--r--   0     1001      127     1798 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/pragma.rs
+-rw-r--r--   0     1001      127     3425 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/qubit.rs
+-rw-r--r--   0     1001      127      654 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/reset.rs
+-rw-r--r--   0     1001      127      133 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Fixed Qubit.snap
+-rw-r--r--   0     1001      127      133 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Variable Qubit.snap
+-rw-r--r--   0     1001      127      124 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition No Params.snap
+-rw-r--r--   0     1001      127      167 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Params.snap
+-rw-r--r--   0     1001      127      160 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Single Param.snap
+-rw-r--r--   0     1001      127      109 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Basic Declaration.snap
+-rw-r--r--   0     1001      127      141 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration with Offsets.snap
+-rw-r--r--   0     1001      127      125 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration.snap
+-rw-r--r--   0     1001      127      191 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Parameterized GateDefinition.snap
+-rw-r--r--   0     1001      127      178 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Pauli Sum GateDefinition.snap
+-rw-r--r--   0     1001      127      139 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Permutation GateDefinition.snap
+-rw-r--r--   0     1001      127      143 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__waveform__test_waveform_definition__display@Simple WaveformDefinition.snap
+-rw-r--r--   0     1001      127     1528 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/timing.rs
+-rw-r--r--   0     1001      127     3666 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/waveform.rs
+-rw-r--r--   0     1001      127     1910 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/lib.rs
+-rw-r--r--   0     1001      127     1013 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/macros.rs
+-rw-r--r--   0     1001      127    36217 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/command.rs
+-rw-r--r--   0     1001      127    23080 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/common.rs
+-rw-r--r--   0     1001      127     5970 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/error/error.rs
+-rw-r--r--   0     1001      127     2519 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/error/input.rs
+-rw-r--r--   0     1001      127     3242 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/error/internal.rs
+-rw-r--r--   0     1001      127     1004 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/error/kind.rs
+-rw-r--r--   0     1001      127     2685 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/error/mod.rs
+-rw-r--r--   0     1001      127    17487 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/expression.rs
+-rw-r--r--   0     1001      127     2212 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/gate.rs
+-rw-r--r--   0     1001      127    40974 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/instruction.rs
+-rw-r--r--   0     1001      127     1380 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/lexer/error.rs
+-rw-r--r--   0     1001      127    17439 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/lexer/mod.rs
+-rw-r--r--   0     1001      127     4222 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/lexer/quoted_strings.rs
+-rw-r--r--   0     1001      127     3357 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/lexer/wrapped_parsers.rs
+-rw-r--r--   0     1001      127     4162 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/macros.rs
+-rw-r--r--   0     1001      127     2446 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/mod.rs
+-rw-r--r--   0     1001      127     5841 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/token.rs
+-rw-r--r--   0     1001      127    25985 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/analysis/control_flow_graph.rs
+-rw-r--r--   0     1001      127      974 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/analysis/mod.rs
+-rw-r--r--   0     1001      127     9591 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/analysis/qubit_graph.rs
+-rw-r--r--   0     1001      127      889 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap
+-rw-r--r--   0     1001      127     1329 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/analysis/test_programs.rs
+-rw-r--r--   0     1001      127    23626 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/calibration.rs
+-rw-r--r--   0     1001      127     7227 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/calibration_set.rs
+-rw-r--r--   0     1001      127     2283 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/error/leftover.rs
+-rw-r--r--   0     1001      127     3068 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/error/mod.rs
+-rw-r--r--   0     1001      127     2252 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/error/result.rs
+-rw-r--r--   0     1001      127     2725 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/error/syntax.rs
+-rw-r--r--   0     1001      127     8742 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/frame.rs
+-rw-r--r--   0     1001      127    17109 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/memory.rs
+-rw-r--r--   0     1001      127    51116 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/mod.rs
+-rw-r--r--   0     1001      127    26031 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/graph.rs
+-rw-r--r--   0     1001      127    20046 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/graphviz_dot.rs
+-rw-r--r--   0     1001      127      456 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/mod.rs
+-rw-r--r--   0     1001      127    16670 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/schedule.rs
+-rw-r--r--   0     1001      127     2678 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap
+-rw-r--r--   0     1001      127     1560 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap
+-rw-r--r--   0     1001      127     1166 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap
+-rw-r--r--   0     1001      127     1732 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap
+-rw-r--r--   0     1001      127     1112 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap
+-rw-r--r--   0     1001      127     1195 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap
+-rw-r--r--   0     1001      127     1780 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap
+-rw-r--r--   0     1001      127     1653 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap
+-rw-r--r--   0     1001      127     1003 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap
+-rw-r--r--   0     1001      127     1032 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap
+-rw-r--r--   0     1001      127      552 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap
+-rw-r--r--   0     1001      127     1540 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap
+-rw-r--r--   0     1001      127     1073 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap
+-rw-r--r--   0     1001      127     1338 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap
+-rw-r--r--   0     1001      127     1866 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap
+-rw-r--r--   0     1001      127      854 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap
+-rw-r--r--   0     1001      127      867 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap
+-rw-r--r--   0     1001      127      887 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap
+-rw-r--r--   0     1001      127     1892 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap
+-rw-r--r--   0     1001      127      839 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap
+-rw-r--r--   0     1001      127      768 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap
+-rw-r--r--   0     1001      127      591 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap
+-rw-r--r--   0     1001      127      793 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap
+-rw-r--r--   0     1001      127      852 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap
+-rw-r--r--   0     1001      127      585 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap
+-rw-r--r--   0     1001      127      227 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Instruction-Match.snap
+-rw-r--r--   0     1001      127      136 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Literal-Parameter.snap
+-rw-r--r--   0     1001      127      215 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Multiple-Qubits.snap
+-rw-r--r--   0     1001      127      476 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Param-Precedence.snap
+-rw-r--r--   0     1001      127      210 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Simple.snap
+-rw-r--r--   0     1001      127      141 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Variable-Qubit.snap
+-rw-r--r--   0     1001      127      159 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@FenceVariableQubit.snap
+-rw-r--r--   0     1001      127      309 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Measure-Calibration.snap
+-rw-r--r--   0     1001      127      261 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Fixed-Match.snap
+-rw-r--r--   0     1001      127      155 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-No-Qubit-Match.snap
+-rw-r--r--   0     1001      127      254 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Variable-Match.snap
+-rw-r--r--   0     1001      127      174 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@ShiftPhase.snap
+-rw-r--r--   0     1001      127      167 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__filter_instructions.snap
+-rw-r--r--   0     1001      127     3755 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap
+-rw-r--r--   0     1001      127      425 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__wrap_in_loop.snap
+-rw-r--r--   0     1001      127    35001 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/type_check.rs
+-rw-r--r--   0     1001      127     2422 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/quil.rs
+-rw-r--r--   0     1001      127     2749 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/reserved.rs
+-rw-r--r--   0     1001      127     2109 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/validation/identifier.rs
+-rw-r--r--   0     1001      127       20 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/validation/mod.rs
+-rw-r--r--   0     1001      127      724 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/calibration_test.rs
+-rw-r--r--   0     1001      127      742 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/programs/calibration_cz.quil
+-rw-r--r--   0     1001      127     1888 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/programs/calibration_cz_phase.quil
+-rw-r--r--   0     1001      127     3266 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/programs/calibration_measure.quil
+-rw-r--r--   0     1001      127     1588 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/programs/calibration_rx.quil
+-rw-r--r--   0     1001      127     1786 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/programs/calibration_xy.quil
+-rw-r--r--   0     1001      127      747 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap
+-rw-r--r--   0     1001      127     1797 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap
+-rw-r--r--   0     1001      127     3187 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap
+-rw-r--r--   0     1001      127     1519 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap
+-rw-r--r--   0     1001      127     1719 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 quil-0.9.1rc0/quil-py/Cargo.toml
+-rw-r--r--   0     1001      127      203 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/.flake8
+-rw-r--r--   0     1001      127       10 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/.stubtest-allowlist
+-rw-r--r--   0     1001      127    20835 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/CHANGELOG.md
+-rw-r--r--   0     1001      127     1258 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/Makefile.toml
+-rw-r--r--   0     1001      127      777 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/README-py.md
+-rw-r--r--   0     1001      127      337 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/README.md
+-rw-r--r--   0     1001      127       71 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/build.rs
+-rw-r--r--   0     1001      127      403 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/make_docs.py
+-rw-r--r--   0     1001      127      135 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/out/index.html
+-rw-r--r--   0     1001      127    34673 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/out/quil/quil.html
+-rw-r--r--   0     1001      127    34581 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/out/quil.html
+-rw-r--r--   0     1001      127    20706 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/out/search.js
+-rw-r--r--   0     1001      127    32817 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/poetry.lock
+-rw-r--r--   0     1001      127      283 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/__init__.pyi
+-rw-r--r--   0     1001      127       30 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/expression/__init__.py
+-rw-r--r--   0     1001      127     7528 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/expression/__init__.pyi
+-rw-r--r--   0     1001      127      123 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/instructions/__init__.py
+-rw-r--r--   0     1001      127    91194 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/instructions/__init__.pyi
+-rw-r--r--   0     1001      127      127 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/program/__init__.py
+-rw-r--r--   0     1001      127    17967 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/program/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/py.typed
+-rw-r--r--   0     1001      127      160 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/validation/__init__.py
+-rw-r--r--   0     1001      127       39 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/validation/__init__.pyi
+-rw-r--r--   0     1001      127       41 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/validation/identifier.py
+-rw-r--r--   0     1001      127      419 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/validation/identifier.pyi
+-rw-r--r--   0     1001      127    34593 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil.html
+-rw-r--r--   0     1001      127     6656 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/expression.rs
+-rw-r--r--   0     1001      127     2838 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/calibration.rs
+-rw-r--r--   0     1001      127     1251 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/circuit.rs
+-rw-r--r--   0     1001      127    11440 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/classical.rs
+-rw-r--r--   0     1001      127     4295 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/control_flow.rs
+-rw-r--r--   0     1001      127     5561 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/declaration.rs
+-rw-r--r--   0     1001      127     9507 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/frame.rs
+-rw-r--r--   0     1001      127     8394 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/gate.rs
+-rw-r--r--   0     1001      127     1056 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/measurement.rs
+-rw-r--r--   0     1001      127     8741 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/mod.rs
+-rw-r--r--   0     1001      127     1852 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/pragma.rs
+-rw-r--r--   0     1001      127      978 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/qubit.rs
+-rw-r--r--   0     1001      127      738 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/reset.rs
+-rw-r--r--   0     1001      127     1591 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/timing.rs
+-rw-r--r--   0     1001      127     2443 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/waveform.rs
+-rw-r--r--   0     1001      127     1967 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/lib.rs
+-rw-r--r--   0     1001      127     2982 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/analysis.rs
+-rw-r--r--   0     1001      127     4156 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/calibration.rs
+-rw-r--r--   0     1001      127     2774 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/frame.rs
+-rw-r--r--   0     1001      127      897 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/memory.rs
+-rw-r--r--   0     1001      127    12676 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/mod.rs
+-rw-r--r--   0     1001      127     1970 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/scheduling.rs
+-rw-r--r--   0     1001      127     1136 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/validation/identifier.rs
+-rw-r--r--   0     1001      127      151 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/validation/mod.rs
+-rw-r--r--   0     1001      127     1617 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/test/instructions/test_copy.py
+-rw-r--r--   0     1001      127      351 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/test/instructions/test_gate.py
+-rw-r--r--   0     1001      127      137 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/test/program/__snapshots__/test_program.ambr
+-rw-r--r--   0     1001      127     4596 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/test/program/test_program.py
+-rw-r--r--   0     1001      127     1025 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/test/test_eq.py
+-rw-r--r--   0     1001      127    50481 2024-04-17 20:38:08.000000 quil-0.9.1rc0/Cargo.lock
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 quil-0.9.1rc0/Cargo.toml
+-rw-r--r--   0        0        0     3112 1970-01-01 00:00:00.000000 quil-0.9.1rc0/pyproject.toml
+-rw-r--r--   0     1001      127      127 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/program/__init__.py
+-rw-r--r--   0     1001      127    17967 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/program/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/py.typed
+-rw-r--r--   0     1001      127      123 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/instructions/__init__.py
+-rw-r--r--   0     1001      127    91194 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/instructions/__init__.pyi
+-rw-r--r--   0     1001      127       30 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/expression/__init__.py
+-rw-r--r--   0     1001      127     7528 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/expression/__init__.pyi
+-rw-r--r--   0     1001      127      283 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/__init__.pyi
+-rw-r--r--   0     1001      127       41 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/validation/identifier.py
+-rw-r--r--   0     1001      127      160 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/validation/__init__.py
+-rw-r--r--   0     1001      127       39 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/validation/__init__.pyi
+-rw-r--r--   0     1001      127      419 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/validation/identifier.pyi
+-rw-r--r--   0     1001      127      777 2024-04-17 20:38:00.000000 quil-0.9.1rc0/README-py.md
+-rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 quil-0.9.1rc0/PKG-INFO
```

### Comparing `quil-0.9.1/quil-rs/Cargo.toml` & `quil-0.9.1rc0/quil-rs/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "quil-rs"
 description = "Rust tooling for Quil (Quantum Instruction Language)"
-version = "0.25.1"
+version = "0.25.1-rc.0"
 edition = "2021"
 rust-version = "1.70"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/quil-rust"
 keywords = ["Quil", "Quantum", "Rigetti"]
 categories = ["parser-implementations", "science", "compilers", "emulators"]
```

### Comparing `quil-0.9.1/quil-rs/CHANGELOG.md` & `quil-0.9.1rc0/quil-rs/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-## 0.25.1
-
-### Features
-
-- Support constructing ControlFlowGraph and BasicBlocks. (#359)
-
 ## 0.25.1-rc.0
 
 ### Features
 
 - Support constructing ControlFlowGraph and BasicBlocks. (#359)
 
 ## 0.25.0
```

### Comparing `quil-0.9.1/quil-rs/README.md` & `quil-0.9.1rc0/quil-rs/README.md`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/benches/corpus.rs` & `quil-0.9.1rc0/quil-rs/benches/corpus.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/benches/get_frames_for_instruction.rs` & `quil-0.9.1rc0/quil-rs/benches/get_frames_for_instruction.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/benches/parser.rs` & `quil-0.9.1rc0/quil-rs/benches/parser.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/benches/sample-calibrations.quil` & `quil-0.9.1rc0/quil-rs/benches/sample-calibrations.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/benches/scheduled_program_from_program.rs` & `quil-0.9.1rc0/quil-rs/benches/scheduled_program_from_program.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/benches/simplification.rs` & `quil-0.9.1rc0/quil-rs/benches/simplification.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/benches/test_expressions.txt` & `quil-0.9.1rc0/quil-rs/benches/test_expressions.txt`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/examples/generate_test_expressions.rs` & `quil-0.9.1rc0/quil-rs/examples/generate_test_expressions.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/expression/mod.rs` & `quil-0.9.1rc0/quil-rs/src/expression/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/expression/simplification/by_hand.rs` & `quil-0.9.1rc0/quil-rs/src/expression/simplification/by_hand.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/expression/simplification/mod.rs` & `quil-0.9.1rc0/quil-rs/src/expression/simplification/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/hash.rs` & `quil-0.9.1rc0/quil-rs/src/hash.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/calibration.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/circuit.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/circuit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/classical.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/classical.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/control_flow.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/control_flow.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/declaration.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/declaration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/frame.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/gate.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/measurement.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/measurement.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/mod.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/pragma.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/pragma.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/qubit.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/qubit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/reset.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/reset.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/timing.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/timing.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/instruction/waveform.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/waveform.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/lib.rs` & `quil-0.9.1rc0/quil-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/macros.rs` & `quil-0.9.1rc0/quil-rs/src/macros.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/command.rs` & `quil-0.9.1rc0/quil-rs/src/parser/command.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/common.rs` & `quil-0.9.1rc0/quil-rs/src/parser/common.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/error/error.rs` & `quil-0.9.1rc0/quil-rs/src/parser/error/error.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/error/input.rs` & `quil-0.9.1rc0/quil-rs/src/parser/error/input.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/error/internal.rs` & `quil-0.9.1rc0/quil-rs/src/parser/error/internal.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/error/kind.rs` & `quil-0.9.1rc0/quil-rs/src/parser/error/kind.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/error/mod.rs` & `quil-0.9.1rc0/quil-rs/src/parser/error/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/expression.rs` & `quil-0.9.1rc0/quil-rs/src/parser/expression.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/gate.rs` & `quil-0.9.1rc0/quil-rs/src/parser/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/instruction.rs` & `quil-0.9.1rc0/quil-rs/src/parser/instruction.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/lexer/error.rs` & `quil-0.9.1rc0/quil-rs/src/parser/lexer/error.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/lexer/mod.rs` & `quil-0.9.1rc0/quil-rs/src/parser/lexer/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/lexer/quoted_strings.rs` & `quil-0.9.1rc0/quil-rs/src/parser/lexer/quoted_strings.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/lexer/wrapped_parsers.rs` & `quil-0.9.1rc0/quil-rs/src/parser/lexer/wrapped_parsers.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/macros.rs` & `quil-0.9.1rc0/quil-rs/src/parser/macros.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/mod.rs` & `quil-0.9.1rc0/quil-rs/src/parser/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/parser/token.rs` & `quil-0.9.1rc0/quil-rs/src/parser/token.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/analysis/control_flow_graph.rs` & `quil-0.9.1rc0/quil-rs/src/program/analysis/control_flow_graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/analysis/mod.rs` & `quil-0.9.1rc0/quil-rs/src/program/analysis/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/analysis/qubit_graph.rs` & `quil-0.9.1rc0/quil-rs/src/program/analysis/qubit_graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap` & `quil-0.9.1rc0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/analysis/test_programs.rs` & `quil-0.9.1rc0/quil-rs/src/program/analysis/test_programs.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/calibration.rs` & `quil-0.9.1rc0/quil-rs/src/program/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/calibration_set.rs` & `quil-0.9.1rc0/quil-rs/src/program/calibration_set.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/error/leftover.rs` & `quil-0.9.1rc0/quil-rs/src/program/error/leftover.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/error/mod.rs` & `quil-0.9.1rc0/quil-rs/src/program/error/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/error/result.rs` & `quil-0.9.1rc0/quil-rs/src/program/error/result.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/error/syntax.rs` & `quil-0.9.1rc0/quil-rs/src/program/error/syntax.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/frame.rs` & `quil-0.9.1rc0/quil-rs/src/program/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/memory.rs` & `quil-0.9.1rc0/quil-rs/src/program/memory.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/mod.rs` & `quil-0.9.1rc0/quil-rs/src/program/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/graph.rs` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/graphviz_dot.rs` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/graphviz_dot.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/schedule.rs` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/schedule.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap` & `quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/program/type_check.rs` & `quil-0.9.1rc0/quil-rs/src/program/type_check.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/quil.rs` & `quil-0.9.1rc0/quil-rs/src/quil.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/reserved.rs` & `quil-0.9.1rc0/quil-rs/src/reserved.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/src/validation/identifier.rs` & `quil-0.9.1rc0/quil-rs/src/validation/identifier.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/calibration_test.rs` & `quil-0.9.1rc0/quil-rs/tests/calibration_test.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/programs/calibration_cz.quil` & `quil-0.9.1rc0/quil-rs/tests/programs/calibration_cz.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/programs/calibration_cz_phase.quil` & `quil-0.9.1rc0/quil-rs/tests/programs/calibration_cz_phase.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/programs/calibration_measure.quil` & `quil-0.9.1rc0/quil-rs/tests/programs/calibration_measure.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/programs/calibration_rx.quil` & `quil-0.9.1rc0/quil-rs/tests/programs/calibration_rx.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/programs/calibration_xy.quil` & `quil-0.9.1rc0/quil-rs/tests/programs/calibration_xy.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap` & `quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap` & `quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap` & `quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap` & `quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap` & `quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/Cargo.toml` & `quil-0.9.1rc0/quil-py/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "quil-py"
 description = "Python bindings for quil-rs"
-version = "0.9.1"
+version = "0.9.1-rc.0"
 edition = "2021"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/quil-rs"
 keywords = ["pyquil", "SDK", "Rigetti", "Quil", "Quantum"]
 categories = ["api-bindings", "parsers", "science", "emulators"]
 readme = "./README.md"
 
@@ -18,15 +18,15 @@
 #
 # Downstream Rust code (including code in `bin/`, `examples/`, and `tests/`) will not be able
 # to `use quil;` unless the "lib" and "rlib" crate type is also included:
 crate-type = ["cdylib", "rlib"]
 
 [dependencies]
 ndarray.workspace = true
-quil-rs = { path = "../quil-rs", version = "0.25.1" }
+quil-rs = { path = "../quil-rs", version = "0.25.1-rc.0" }
 strum.workspace = true
 # pyo3 dependencies should be updated together
 numpy = "0.20.0"
 pyo3 = { version = "0.20.3", features = ["indexmap"] }
 rigetti-pyo3 = {version = "0.3.4", features = ["indexmap"]}
 indexmap.workspace = true
```

### Comparing `quil-0.9.1/quil-py/CHANGELOG.md` & `quil-0.9.1rc0/quil-py/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-## 0.9.1
-
-### Features
-
-- Support constructing ControlFlowGraph and BasicBlocks. (#359)
-
 ## 0.9.1-rc.0
 
 ### Features
 
 - Support constructing ControlFlowGraph and BasicBlocks. (#359)
 
 ## 0.9.0
```

### Comparing `quil-0.9.1/quil-py/Makefile.toml` & `quil-0.9.1rc0/quil-py/Makefile.toml`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/README-py.md` & `quil-0.9.1rc0/quil-py/README-py.md`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/out/quil/quil.html` & `quil-0.9.1rc0/quil-py/out/quil/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/out/quil.html` & `quil-0.9.1rc0/quil-py/out/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/out/search.js` & `quil-0.9.1rc0/quil-py/out/search.js`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/poetry.lock` & `quil-0.9.1rc0/quil-py/poetry.lock`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/quil/expression/__init__.pyi` & `quil-0.9.1rc0/quil-py/quil/expression/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/quil/instructions/__init__.pyi` & `quil-0.9.1rc0/quil-py/quil/instructions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/quil/program/__init__.pyi` & `quil-0.9.1rc0/quil-py/quil/program/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/quil.html` & `quil-0.9.1rc0/quil-py/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/expression.rs` & `quil-0.9.1rc0/quil-py/src/expression.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/calibration.rs` & `quil-0.9.1rc0/quil-py/src/instruction/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/circuit.rs` & `quil-0.9.1rc0/quil-py/src/instruction/circuit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/classical.rs` & `quil-0.9.1rc0/quil-py/src/instruction/classical.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/control_flow.rs` & `quil-0.9.1rc0/quil-py/src/instruction/control_flow.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/declaration.rs` & `quil-0.9.1rc0/quil-py/src/instruction/declaration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/frame.rs` & `quil-0.9.1rc0/quil-py/src/instruction/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/gate.rs` & `quil-0.9.1rc0/quil-py/src/instruction/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/measurement.rs` & `quil-0.9.1rc0/quil-py/src/instruction/measurement.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/mod.rs` & `quil-0.9.1rc0/quil-py/src/instruction/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/pragma.rs` & `quil-0.9.1rc0/quil-py/src/instruction/pragma.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/qubit.rs` & `quil-0.9.1rc0/quil-py/src/instruction/qubit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/reset.rs` & `quil-0.9.1rc0/quil-py/src/instruction/reset.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/timing.rs` & `quil-0.9.1rc0/quil-py/src/instruction/timing.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/instruction/waveform.rs` & `quil-0.9.1rc0/quil-py/src/instruction/waveform.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/lib.rs` & `quil-0.9.1rc0/quil-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/program/analysis.rs` & `quil-0.9.1rc0/quil-py/src/program/analysis.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/program/calibration.rs` & `quil-0.9.1rc0/quil-py/src/program/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/program/frame.rs` & `quil-0.9.1rc0/quil-py/src/program/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/program/memory.rs` & `quil-0.9.1rc0/quil-py/src/program/memory.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/program/mod.rs` & `quil-0.9.1rc0/quil-py/src/program/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/program/scheduling.rs` & `quil-0.9.1rc0/quil-py/src/program/scheduling.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/src/validation/identifier.rs` & `quil-0.9.1rc0/quil-py/src/validation/identifier.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/test/instructions/test_copy.py` & `quil-0.9.1rc0/quil-py/test/instructions/test_copy.py`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/test/program/test_program.py` & `quil-0.9.1rc0/quil-py/test/program/test_program.py`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil-py/test/test_eq.py` & `quil-0.9.1rc0/quil-py/test/test_eq.py`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/Cargo.lock` & `quil-0.9.1rc0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1082,38 +1082,38 @@
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quil-cli"
-version = "0.2.1"
+version = "0.2.1-rc.0"
 dependencies = [
  "anyhow",
  "clap",
  "quil-rs",
 ]
 
 [[package]]
 name = "quil-py"
-version = "0.9.1"
+version = "0.9.1-rc.0"
 dependencies = [
  "indexmap",
  "ndarray",
  "numpy",
  "pyo3",
  "pyo3-build-config",
  "quil-rs",
  "rigetti-pyo3",
  "strum",
 ]
 
 [[package]]
 name = "quil-rs"
-version = "0.25.1"
+version = "0.25.1-rc.0"
 dependencies = [
  "approx",
  "clap",
  "criterion",
  "dot-writer",
  "indexmap",
  "insta",
```

### Comparing `quil-0.9.1/pyproject.toml` & `quil-0.9.1rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   "Operating System :: OS Independent",
 ]
 
 # PEP 621 specifies the [project] table as the source for project metadata. However, Poetry only supports [tool.poetry]
 # We can remove this table once this issue is resolved: https://github.com/python-poetry/poetry/issues/3332
 [tool.poetry]
 name = "quil"
-version = "0.9.1"
+version = "0.9.1-rc.0"
 description = "A Python package for building and parsing Quil programs."
 readme = "README-py.md"
 authors = ["Rigetti Computing <softapps@rigetti.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.21"
```

### Comparing `quil-0.9.1/quil/program/__init__.pyi` & `quil-0.9.1rc0/quil/program/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil/instructions/__init__.pyi` & `quil-0.9.1rc0/quil/instructions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/quil/expression/__init__.pyi` & `quil-0.9.1rc0/quil/expression/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/README-py.md` & `quil-0.9.1rc0/README-py.md`

 * *Files identical despite different names*

### Comparing `quil-0.9.1/PKG-INFO` & `quil-0.9.1rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: quil
-Version: 0.9.1
+Version: 0.9.1rc0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Summary: A Python package for building and parsing Quil programs.
```

