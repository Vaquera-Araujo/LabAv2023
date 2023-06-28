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

$$\delta_1 E_n=\bra{n^{(0)}}\delta_1 H\ket{n^{(0)}}.$$

and

$$\ket{\delta_1 n}=\sum_{l\neq n}\frac{\bra{l^{(0)}}\delta_1 H\ket{n^{(0)}}}{E_n^{(0)}-E_l^{(0)}}\ket{l^{(0)}}.$$

At second order, we have

$$\delta_2E_n=\sum_{l\neq n}\frac{|\bra{l^{(0)}}\delta_1 H\ket{n^{(0)}}|^2}{E_n^{(0)}-E_l^{(0)}}+\bra{ n^{(0)}}\delta_2H\ket{ n^{(0)}}.$$

and

$$\ket{\delta_2 n}=\sum_{l\neq n}\frac{\ket{l^{(0)}}}{E_n^{(0)}-E_l^{(0)}}\bigg[\sum_{j\neq n}
\frac{\bra{l^{(0)}}\delta_1 H\ket{j^{(0)}}\bra{j^{(0)}}\delta_1 H\ket{n^{(0)}}}{E_n^{(0)}-E_{j}^{(0)}}-\delta_1 E_n\frac{\bra{l^{(0)}}\delta_1 H\ket{n^{(0)}}}{E_n^{(0)}-E_l^{(0)}}+\bra{l^{(0)}}\delta_2H\ket{ n^{(0)}}\bigg]-\frac{1}{2}\sum_{l\neq n}\left|\frac{\bra{l^{(0)}}\delta_1 H\ket{n^{(0)}}}{E_n^{(0)}-E_l^{(0)}}\right|^2\ket{n^{(0)}}.
$$

Perturbation theory provides increasingly accurate approximations as higher-order corrections are included. However, the convergence of the series depends on the strength of the perturbation and the energy differences between eigenstates. In cases where the perturbation is strong or the energy denominators are small, other methods such as variational approaches or numerical techniques may be more suitable.

## Examples

Relativistic Corrections to the  1-D Simple Harmonic Oscillator

[relativistic_corrections_sho.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20and%20Numerical%20Projects/Time%20Independent%20Perturbation%20Theory/relativistic_corrections_sho.ipynb)

## Challenges

Find the first and second order shifts in energy and in states of a simple harmonic oscillator perturbed by a cubic term in the potential of the form $\epsilon x^3$
