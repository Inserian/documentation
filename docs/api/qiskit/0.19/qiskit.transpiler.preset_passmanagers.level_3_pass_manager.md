---
title: level_3_pass_manager
description: API reference for qiskit.transpiler.preset_passmanagers.level_3_pass_manager
in_page_toc_min_heading_level: 1
python_api_type: function
python_api_name: qiskit.transpiler.preset_passmanagers.level_3_pass_manager
---

# level\_3\_pass\_manager

<span id="qiskit.transpiler.preset_passmanagers.level_3_pass_manager" />

`level_3_pass_manager(pass_manager_config)`

Level 3 pass manager: heavy optimization by noise adaptive qubit mapping and gate cancellation using commutativity rules and unitary synthesis.

This pass manager applies the user-given initial layout. If none is given, a search for a perfect layout (i.e. one that satisfies all 2-qubit interactions) is conducted. If no such layout is found, and device calibration information is available, the circuit is mapped to the qubits with best readouts and to CX gates with highest fidelity.

The pass manager then transforms the circuit to match the coupling constraints. It is then unrolled to the basis, and any flipped cx directions are fixed. Finally, optimizations in the form of commutative gate cancellation, resynthesis of two-qubit unitary blocks, and redundant reset removal are performed.

<Admonition title="Note" type="note">
  In simulators where `coupling_map=None`, only the unrolling and optimization stages are done.
</Admonition>

**Parameters**

**pass\_manager\_config** ([`PassManagerConfig`](qiskit.transpiler.PassManagerConfig "qiskit.transpiler.passmanager_config.PassManagerConfig")) – configuration of the pass manager.

**Return type**

[`PassManager`](qiskit.transpiler.PassManager "qiskit.transpiler.passmanager.PassManager")

**Returns**

a level 3 pass manager.

**Raises**

[**TranspilerError**](qiskit.transpiler.TranspilerError "qiskit.transpiler.TranspilerError") – if the passmanager config is invalid.
