# Variational Quantum Eigensolver

Problem: Find the expectation value of the Hamiltonian Z ⊗ Z, with respect to an arbitrarily constructed trial state using parametrize quantum circuit in Qiskit. Where Z = z-component of Pauli vector.

# Diagrammatic Explanation of VQE:

<img width="664" alt="VQEIllustration" src="https://user-images.githubusercontent.com/77266161/125802057-9de1e1ab-be92-485d-a808-0d4de3d2a836.png">

# VQE Subroutines

The Variational quantum eigensolver consists a total of three subroutines:

1) Trial State Preparation: This can be done by choosing an arbitrary quantum gate sequence (ansatz), depending on some parameters i.e. angles.

2) Finding the Energy: After preparing the initial state one need to find the expectation value of Hamiltonian (i.e. energy) on the basis of the prepared trial state.

3) Minimize the Energy: This step can be efficiently done by using a completely classical process, and by choosing an optimization method from the scipy.optimize documentation of Python.

# How to solve this Problem

This project can be completed by using only first two subroutines of VQE process. Hence your task will be to:

Construct a trial wave function using an arbitrary parametrized quantum circuit i.e. ansatz based on single qubit gates and two qubit rotating gates.

Find the expectation value of Z ⊗ Z, in the basis of the trial wave function i.e. Expectation Value = ⟨trial state|Z ⊗ Z|trial state⟩

The Trial state can be obtained by using the Statevector Simulator after running the parametrized quantum circuit mentioned in the first step 1 project elaboration.

# References Used

Michał Stęchły's blogpost: https://www.mustythoughts.com/variational-quantum-eigensolver-explained

Frank Zickert's Article: https://towardsdatascience.com/the-variational-quantum-eigensolver-explained-adcbc9659c3a

JavaFXpert's article: https://medium.com/qiskit/the-variational-quantum-eigensolver-43f7718c2747

Prof. K.L. Sebastian's lecture on Variational Methods(the backbone of VQE): https://www.youtube.com/watch?v=T-wXwgS7MuI

Qiskit Textbook https://qiskit.org/textbook/ch-applications/vqe-molecules.html
