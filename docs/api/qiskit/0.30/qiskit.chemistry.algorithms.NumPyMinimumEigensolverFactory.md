# NumPyMinimumEigensolverFactory

<span id="undefined" />

`NumPyMinimumEigensolverFactory(filter_criterion=None, use_default_filter_criterion=False)`

Bases: `qiskit.chemistry.algorithms.ground_state_solvers.minimum_eigensolver_factories.minimum_eigensolver_factory.MinimumEigensolverFactory`

A factory to construct a NumPyMinimumEigensolver.

**Parameters**

*   **filter\_criterion** (`Optional`\[`Callable`\[\[`Union`\[`List`, `ndarray`], `float`, `Optional`\[`List`\[`float`]]], `bool`]]) – callable that allows to filter eigenvalues/eigenstates. The minimum eigensolver is only searching over feasible states and returns an eigenstate that has the smallest eigenvalue among feasible states. The callable has the signature filter(eigenstate, eigenvalue, aux\_values) and must return a boolean to indicate whether to consider this value or not. If there is no feasible element, the result can even be empty.
*   **use\_default\_filter\_criterion** (`bool`) – whether to use the transformation’s default filter criterion if `filter_criterion` is `None`.

## Methods

|                                                                                                                                                                                                                                                                                     |                                                                                                                      |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| [`get_solver`](qiskit.chemistry.algorithms.NumPyMinimumEigensolverFactory.get_solver#qiskit.chemistry.algorithms.NumPyMinimumEigensolverFactory.get_solver "qiskit.chemistry.algorithms.NumPyMinimumEigensolverFactory.get_solver")                                                 | Returns a NumPyMinimumEigensolver which possibly uses the default filter criterion provided by the `transformation`. |
| [`supports_aux_operators`](qiskit.chemistry.algorithms.NumPyMinimumEigensolverFactory.supports_aux_operators#qiskit.chemistry.algorithms.NumPyMinimumEigensolverFactory.supports_aux_operators "qiskit.chemistry.algorithms.NumPyMinimumEigensolverFactory.supports_aux_operators") | Returns whether the eigensolver generated by this factory supports auxiliary operators.                              |

## Attributes

<span id="undefined" />

### filter\_criterion

returns filter criterion

**Return type**

`Callable`\[\[`Union`\[`List`, `ndarray`], `float`, `Optional`\[`List`\[`float`]]], `bool`]

<span id="undefined" />

### use\_default\_filter\_criterion

returns whether to use the default filter criterion

**Return type**

`bool`