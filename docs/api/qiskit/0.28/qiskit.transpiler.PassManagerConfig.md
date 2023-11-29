# qiskit.transpiler.PassManagerConfig

<span id="undefined" />

`PassManagerConfig(initial_layout=None, basis_gates=None, coupling_map=None, layout_method=None, routing_method=None, translation_method=None, scheduling_method=None, instruction_durations=None, backend_properties=None, approximation_degree=None, seed_transpiler=None, timing_constraints=None)`

Pass Manager Configuration.

Initialize a PassManagerConfig object

**Parameters**

*   **initial\_layout** ([*Layout*](qiskit.transpiler.Layout#qiskit.transpiler.Layout "qiskit.transpiler.Layout")) – Initial position of virtual qubits on physical qubits.
*   **basis\_gates** (*list*) – List of basis gate names to unroll to.
*   **coupling\_map** ([*CouplingMap*](qiskit.transpiler.CouplingMap#qiskit.transpiler.CouplingMap "qiskit.transpiler.CouplingMap")) – Directed graph represented a coupling map.
*   **layout\_method** (*str*) – the pass to use for choosing initial qubit placement.
*   **routing\_method** (*str*) – the pass to use for routing qubits on the architecture.
*   **translation\_method** (*str*) – the pass to use for translating gates to basis\_gates.
*   **scheduling\_method** (*str*) – the pass to use for scheduling instructions.
*   **instruction\_durations** ([*InstructionDurations*](qiskit.transpiler.InstructionDurations#qiskit.transpiler.InstructionDurations "qiskit.transpiler.InstructionDurations")) – Dictionary of duration (in dt) for each instruction.
*   **backend\_properties** ([*BackendProperties*](qiskit.providers.models.BackendProperties#qiskit.providers.models.BackendProperties "qiskit.providers.models.BackendProperties")) – Properties returned by a backend, including information on gate errors, readout errors, qubit coherence times, etc.
*   **approximation\_degree** (*float*) – heuristic dial used for circuit approximation (1.0=no approximation, 0.0=maximal approximation)
*   **seed\_transpiler** (*int*) – Sets random seed for the stochastic parts of the transpiler.
*   **timing\_constraints** (*TimingConstraints*) – Hardware time alignment restrictions.

<span id="undefined" />

`__init__(initial_layout=None, basis_gates=None, coupling_map=None, layout_method=None, routing_method=None, translation_method=None, scheduling_method=None, instruction_durations=None, backend_properties=None, approximation_degree=None, seed_transpiler=None, timing_constraints=None)`

Initialize a PassManagerConfig object

**Parameters**

*   **initial\_layout** ([*Layout*](qiskit.transpiler.Layout#qiskit.transpiler.Layout "qiskit.transpiler.Layout")) – Initial position of virtual qubits on physical qubits.
*   **basis\_gates** (*list*) – List of basis gate names to unroll to.
*   **coupling\_map** ([*CouplingMap*](qiskit.transpiler.CouplingMap#qiskit.transpiler.CouplingMap "qiskit.transpiler.CouplingMap")) – Directed graph represented a coupling map.
*   **layout\_method** (*str*) – the pass to use for choosing initial qubit placement.
*   **routing\_method** (*str*) – the pass to use for routing qubits on the architecture.
*   **translation\_method** (*str*) – the pass to use for translating gates to basis\_gates.
*   **scheduling\_method** (*str*) – the pass to use for scheduling instructions.
*   **instruction\_durations** ([*InstructionDurations*](qiskit.transpiler.InstructionDurations#qiskit.transpiler.InstructionDurations "qiskit.transpiler.InstructionDurations")) – Dictionary of duration (in dt) for each instruction.
*   **backend\_properties** ([*BackendProperties*](qiskit.providers.models.BackendProperties#qiskit.providers.models.BackendProperties "qiskit.providers.models.BackendProperties")) – Properties returned by a backend, including information on gate errors, readout errors, qubit coherence times, etc.
*   **approximation\_degree** (*float*) – heuristic dial used for circuit approximation (1.0=no approximation, 0.0=maximal approximation)
*   **seed\_transpiler** (*int*) – Sets random seed for the stochastic parts of the transpiler.
*   **timing\_constraints** (*TimingConstraints*) – Hardware time alignment restrictions.

## Methods

|                                                                                                                                                 |                                       |
| ----------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
| [`__init__`](#qiskit.transpiler.PassManagerConfig.__init__ "qiskit.transpiler.PassManagerConfig.__init__")(\[initial\_layout, basis\_gates, …]) | Initialize a PassManagerConfig object |