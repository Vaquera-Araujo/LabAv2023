# The Time-Dependent and Time-Independent Schrödinger Equations

## Time-Dependent Schrödinger Equation

The time-dependent Schrödinger equation is given by:

$$i\hbar \frac{\partial \Psi}{\partial t} = \hat{H} \Psi$$

where $\Psi$ represents the wave function of the quantum system, $\hat{H}$ is the Hamiltonian operator and $\hbar$ is the reduced Planck's constant.

This equation describes the wave function $\Psi$ dynamics. The left-hand side represents the rate of change of the wave function, while the right-hand side represents the action of the Hamiltonian operator on the wave function.

## Time-Independent Schrödinger Equation

The time-independent Schrödinger equation is an eigenvalue equation that allows us to determine the stationary states and corresponding energies of a quantum system. It is given by:

$$\hat{H} \psi = E \psi$$

where $\psi$ represents the stationary state wave function, $\hat{H}$ is the Hamiltonian operator, $E$ is the energy of the stationary state, and $\psi$ is the eigenfunction.

Solving this equation involves finding the eigenvalues $E$ and the corresponding eigenfunctions $\psi$ of the Hamiltonian operator. The eigenvalues represent the possible energies of the system, while the eigenfunctions represent the corresponding wave functions.

## Examples

Numerical Solution to the Time Independent Schrödinger equation: Anharmonic Oscillator

[numerical_time_independent_schrodinger_equation.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20and%20Numerical%20Projects/Schr%C3%B6dinger%20Equation%20in%20One%20Dimension/numerical_time_independent_schrodinger_equation.ipynb)

Numerical Solution to the Time Dependent Schrödinger Equation: Harmonic Oscillator

[numerical_time_dependent_quantum_harmonic_oscillator.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20and%20Numerical%20Projects/Schr%C3%B6dinger%20Equation%20in%20One%20Dimension/numerical_time_dependent_quantum_harmonic_oscillator.ipynb)


# Time Independent Perturbation Theory

Quantum mechanics provides a powerful framework for understanding the behavior of microscopic particles. However, many quantum systems are analytically intractable and require approximations. Perturbation theory is a valuable tool in such cases, allowing us to study the effects of small perturbations on known solutions.

Consider a quantum system described by the Hamiltonian $H_0$, which has known eigenstates and eigenvalues

$$H_0\ket{n^{0)}}=E_n^{(0)}\ket{n^{(0)}},\qquad\bra{n^{(0)}}\ket{m^{(0)}}=\delta_{nm}.$$

We introduce a perturbation $\delta H$ to the system, causing the Hamiltonian to become $H=H_0+\delta H$. Our goal is to find the corrected eigenstates and eigenvalues of this perturbed system

$$(H_0+\delta H)\ket{n}=E_n\ket{n}.$$

We expect then a shift in eigenvalues and eigenkets given by

$$E_n=E_n^{(0)}+\delta E_n \qquad \ket{n}=\ket{n^{(0)}}+\ket{\delta n}.$$

Assuming that the perturbation is characterized by a small parameter $\epsilon$, we can write a power expansion of the form

$$\delta H=\delta_1 H+\delta_2 H+\cdots,$$

and one can attempt to  determine the corresponding $\delta E_n$ and $\ket{\delta n}$ as powers of $\epsilon$ by matching the solution to the Schrödinger equation order by order

$$\delta E_n=\delta_1 E_n+\delta_2 E_n+\cdots, \qquad \ket{\delta n}=\ket{\delta_1 n}+\ket{\delta_2 n}+\cdots.$$

In absence of degeneracy, the shifts at first order are

$$\delta_1 E_n=\bra{n^{(0)}}\delta H\ket{n^{(0)}}.$$

and

$$\ket{\delta_1 n}=\sum_{l\neq n}\frac{\bra{l^{(0)}}\delta H\ket{n^{(0)}}}{E_n^{(0)}-E_l^{(0)}}\ket{l^{(0)}}.$$

At second order, we have

$$\delta_2E_n=\sum_{l\neq n}\frac{|\bra{l^{(0)}}\delta_1 H\ket{n^{(0)}}|^2}{E_n^{(0)}-E_l^{(0)}}+\bra{ n^{(0)}}\delta_2H\ket{ n^{(0)}}.$$

and

$$\ket{\delta_2 n}=\sum_{l\neq n}\frac{\ket{l^{(0)}}}{E_n^{(0)}-E_l^{(0)}}\bigg[\sum_{j\neq n}
\frac{\bra{l^{(0)}}\delta_1 H\ket{j^{(0)}}\bra{j^{(0)}}\delta_1 H\ket{n^{(0)}}}{E_n^{(0)}-E_{j}^{(0)}}-\delta_1 E_n\frac{\bra{l^{(0)}}\delta_1 H\ket{n^{(0)}}}{E_n^{(0)}-E_l^{(0)}}+\bra{l^{(0)}}\delta_2H\ket{ n^{(0)}}\bigg]-\frac{1}{2}\sum_{l\neq n}\left|\frac{\bra{l^{(0)}}\delta_1 H\ket{n^{(0)}}}{E_n^{(0)}-E_l^{(0)}}\right|^2\ket{n^{(0)}}.
$$

Perturbation theory provides increasingly accurate approximations as higher-order corrections are included. However, the convergence of the series depends on the strength of the perturbation and the energy differences between eigenstates. In cases where the perturbation is strong or the energy denominators are small, other methods such as variational approaches or numerical techniques may be more suitable.

