## Qiskit implementation of https://arxiv.org/abs/2404.02819

## Efficient Quantum Circuits for Non-Unitary and Unitary Diagonal Operators with Space-Time-Accuracy trade-offs
### Authors: 
Julien Zylberman, Ugo Nzongani, Andrea Simonetto, Fabrice Debbasch

### Abstract:

Unitary and non-unitary diagonal operators are fundamental building blocks in quantum algorithms with applications in the resolution of partial differential equations, Hamiltonian simulations, the loading of classical data on quantum computers (quantum state preparation) and many others. In this paper, we introduce a general approach to implement unitary and non-unitary diagonal operators with efficient-adjustable-depth quantum circuits. The depth, i.e., the number of layers of quantum gates of the quantum circuit, is reducible with respect either to the width, i.e, the number of ancilla qubits, or to the accuracy between the implemented operator and the target one. While exact methods have an optimal exponential scaling either in terms of size, i.e., the total number of primitive quantum gates, or width, approximate methods prove to be efficient for the class of diagonal operators depending on smooth, at least differentiable, functions. Our approach is general enough to allow any method for diagonal operators to become adjustable-depth or approximate, decreasing the depth of the circuit by increasing its width or its approximation level. This feature offers flexibility and can match with the hardware limitations in coherence time or cumulative gate error. We illustrate these methods by performing quantum state preparation and non-unitary-real-space simulation of the diffusion equation. This simulation paves the way to efficient implementations of stochastic models useful in physics, chemistry, biology, image processing and finance.

### Versions:
qiskit: 0.24.1 <br> 
qiskit-terra: 0.24.1

### Description:

The python files in the "code" folder contain all the code needed to generate the quantum circuits.

The notebook diagonal_unitary_example presents ajustable-depth quantum circuits for the implementation of a diagonal unitary using a Walsh series approximation.

The notebook diagonal_non_unitary_and_quantum_state_preparation_example presents ajustable-depth quantum circuits for the block-encoding of a non-unitary diagonal operator and its application to Quantum State Preparation.
