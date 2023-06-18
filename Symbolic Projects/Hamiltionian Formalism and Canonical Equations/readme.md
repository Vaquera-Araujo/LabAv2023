# Hamiltonian and Canonical Equations

The Canonical equations describe the dynamics of a system in terms of its Hamiltonian function.  They involve the canonical variables, 
which comprise the generalized coordinates $q_i$ and their canonical momenta $p_i = \frac{\partial L}{\partial \dot{q}_i}$, where $L$ is the Lagrangian of the system.

The Hamiltonian function $H(q_i, p_i, t)$ is obtained by a Legendre transformation of the Lagrangian:

$H(q_i, p_i, t) = \sum_{i=1}^{n} p_i \dot{q}_i - L(q_i, \dot{q}_i, t)$

and describes the total energy of the system as a function of generalized coordinates $q_i$ and momenta $p_i$.

The canonical equations of motion are given by:

$\dot{q}_i = \frac{\partial H}{\partial p_i} \quad \text{and} \quad \dot{p}_i = -\frac{\partial H}{\partial q_i}$

where $\dot{q}_i$ and $\dot{q}_i$ represent the time derivatives of the canonical variables.

The canonical equations provide an equivalent description of the system's dynamics and constitute a significant improvement, since they are a system of first order equations instead of second order, and they are written in a more symmetric set of variables. 
