# qiskit.ignis.mitigation.complete\_meas\_cal

<span id="undefined" />

`complete_meas_cal(qubit_list=None, qr=None, cr=None, circlabel='')`

Return a list of measurement calibration circuits for the full Hilbert space.

If the circuit contains $n$ qubits, then $2^n$ calibration circuits are created, each of which creates a basis state.

**Parameters**

*   **qubit\_list** (`Optional`\[`List`\[`int`]]) – A list of qubits to perform the measurement correction on. If None, and qr is given then assumed to be performed over the entire qr. The calibration states will be labelled according to this ordering (default None).
*   **qr** (`Union`\[`int`, `List`\[`QuantumRegister`], `None`]) – Quantum registers (or their size).
*   **None** (*If*) –
*   **is created** (*one*) –
*   **cr** (`Union`\[`int`, `List`\[`ClassicalRegister`], `None`]) – Classical registers (or their size).
*   **None** –
*   **is created** –
*   **circlabel** (`str`) – A string to add to the front of circuit names for unique identification(default ‘ ‘).

**Return type**

`Tuple`\[`List`\[`QuantumCircuit`], `List`\[`str`]]

**Returns**

A list of QuantumCircuit objects containing the calibration circuits.

A list of calibration state labels.

## Additional Information:

The returned circuits are named circlabel+cal\_XXX where XXX is the basis state, e.g., cal\_1001.

Pass the results of these circuits to the CompleteMeasurementFitter constructor.

**Raises**

**QiskitError** – if both qubit\_list and qr are None.