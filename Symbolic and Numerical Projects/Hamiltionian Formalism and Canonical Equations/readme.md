# Hamiltonian and Canonical Equations

The Canonical equations describe the dynamics of a system in terms of its Hamiltonian function.  They involve the canonical variables, 
which comprise the generalized coordinates $q_i$ and their canonical momenta $p_i = \frac{\partial L}{\partial \dot{q}_i}$, where $L$ is the Lagrangian of the system.

The Hamiltonian function $H(q_i, p_i, t)$ is obtained by a Legendre transformation of the Lagrangian:

$$H(q_i, p_i, t) = p_i \dot{q}_i - L(q_i, \dot{q}_i, t),$$

and describes the total energy of the system as a function of generalized coordinates $q_i$ and momenta $p_i$.

The canonical equations of motion are given by:

$$\dot{q}_i = \frac{\partial H}{\partial p_i} \quad \text{and} \quad \dot{p}_i = -\frac{\partial H}{\partial q_i},$$

where $\dot{q}_i$ and $\dot{q}_i$ represent the time derivatives of the canonical variables.

The canonical equations provide an equivalent description of the system's dynamics and constitute a significant improvement, since they are a system of first order equations instead of second order, and they are written in a more symmetric set of variables. 

## Examples:

### Doble pendulum Hamiltonian, Equations of motion and Numerical Solution

[double_pendulum_hamiltonian.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20and%20Numerical%20Projects/Hamiltionian%20Formalism%20and%20Canonical%20Equations/double_pendulum_hamiltonian.ipynb)

### Poisson Brackets Jacobi Identity

[jacobi_identity.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20and%20Numerical%20Projects/Hamiltionian%20Formalism%20and%20Canonical%20Equations/jacobi_identity.ipynb)

### Simple Pendulum Phase Space Diagram

[simple_pendulum_phase_space.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20and%20Numerical%20Projects/Hamiltionian%20Formalism%20and%20Canonical%20Equations/simple_pendulum_phase_space.ipynb)

## Challenges:

Obtain the canonical equations and obtain the numerical solution for problems 2, 3 and 4 in page 11 of Mechanics, Third Edition: Volume 1 (Course of Theoretical Physics) L. Landau, and E. Lifshitz. Butterworth-Heinemann, 3 edition, (Jan 15, 1976).
