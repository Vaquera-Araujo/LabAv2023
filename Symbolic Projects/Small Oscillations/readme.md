# Small Oscillations

## Free oscillations in one dimension

A very common form of motion of mechanical systems is what are called small oscillations of a system about a position of stable equilibrium. We shall consider first of all the simplest case, that of a system with only one degree of freedom.
Stable equilibrium corresponds to a position $q_0$ of the system in which its potential energy $U(q)$ is a minimum  $dU(q_0)/dq=0$, and  $d^2U(q_0)/dq^2>0$. A movement away from this position results in the setting up of a force $-dU/dq$ which tends to return the system to equilibrium. For small deviations from the equilibrium position, it is sufficient to retain the first non vanishing term in the expansion of the difference

$U(q)\approx U(q_0)+\frac{1}{2}\left.\frac{d^2U}{dq^2}\right|_{q_0}(q-q_0)^2$.

The constant term $U(q_0)$ does not modify the equations of motion, thus we can remove it by measuring the potential energy from its minimum value, \emph{i.e.} setting $U(q_0) = 0$, and use the symbol $x=q-q_0$ for the deviation of the coordinate from its equilibrium value. Thus

$U(x)\approx \frac{1}{2}\left.\frac{d^2U}{dq^2}\right|_{q_0}x^2\equiv \frac{1}{2}kx^2$.

The kinetic energy of a system with one degree of freedom is in general
of the form $T=a(q)\dot{q}^2/2=a(q)\dot{x}^2/2$.  In the same approximation, it is sufficient to replace the function $a(q)$ by its value at $q = q_0$. Putting for brevity $a(q_0)\equiv m$, the Lagrangian of a system executing small oscillations in one dimension is equivalent to the simple harmonic oscillator

$L=\frac{1}{2}m \dot{x}^2-\frac{1}{2}k x^2$.

The corresponding equation of motion is

$\ddot{x}+\omega^2x=0$,

with angular frequency $\omega=\sqrt{\frac{k}{m}}$, and solution

$x(t)= C\cos(\omega t+\delta)$,

where the constants $C$ and $\delta$ are real and determined by the initial conditions.

## Linearized equations of motion
Now, consider a system with $n$ degrees of freedom characterized by the generalized coordinates $q_i$, with a time independent scalar potential $U(q_i)$ displaying a strict local minimum at $q^0_i$ and rescaled such that $U(q_i^0)=0$. Using a standard particle Lagrangian, the kinetic energy is a quadratic function of the velocities, provided that the generalized coordinates are time-independent functions of the Cartesian coordinates. Then, generalizing the  previous results, the Lagrangian can be approximated to second order in the perturbation expansion around equilibrium by

$L\approx\frac{1}{2}\bra{\dot{x}}M\ket{\dot{x}}-\frac{1}{2}\bra{x}K\ket{x}$,

where $x_i=q_i-q^0_i$ are the components of $\ket{x}$, and we have defined the  
matrix elements $M_{ij}= a_{ij}(q^0_l)$, and $k_{ij}=\left.\frac{\partial^2U}{\partial q_i\partial q_j}\right|_{q^0_l}$.

The matrices $M$ and $K$ can be diagonalized simultaneously through the following algoritm:

1.- Diagonalize the symmetric Matrix $M$ with an ortogonal transformation

$O^T_M M O_M=\sum_{i}m_i\ket{e_i}\bra{e_i}\equiv M_D $,

and perform the same transformation on $K$ to obtain $K_M\equiv O^T_M K O_M$.

2.- Apply a scale transformation, converting the inertial matrix to the identity matrix with $M_D^{-1/2}\equiv\sum_{i}m^{-1/2}_i\ket{e_i}\bra{e_i}$, according to

$M_D^{-1/2}M_DM_D^{-1/2}=\mathbb{1}$,

and do the same transformation to $K_M$ to obtain $W=M_D^{-1/2}K_M M_D^{-1/2}$.

3.- Finally, diagonalize the symmetric matrix through an ortogonal transformation 

$O^T_W W O_W=\sum_{i}\omega^2_i\ket{e_i}\bra{e_i}\equiv W_D $.

This last orthogonal transformation has no effect on the identity matrix, so the goal of simultaneous diagonalization of two symmetric matrices has been achieved.

After this procedure, the lagrangian becomes

$L=\frac{1}{2}\bra{\dot{\zeta}}\mathbb{1}\ket{\dot{\zeta}}-\frac{1}{2}\bra{\zeta}W_{D}\ket{\zeta}=\frac{1}{2}\sum\left[\dot{\zeta}_i^2-\omega^2_i \zeta^2_i\right]$,

with decoupled equations of motion

$\ddot{\zeta}_i+\omega^2\zeta_i=0$,

for the normal coordinates $\ket{\zeta}=O_W^TM_D^{1/2}O_M^T\ket{x}\equiv S^{-1}\ket{x}$, such that $\ket{x}=O_M M_D^{-1/2} O_W \ket{\zeta}\equiv S\ket{\zeta}=S\sum_i[\zeta_i(t)]\ket{e_i}$, where 

$\zeta_i(t)=C_i\cos(\omega_i t+\delta_i)$ for $\omega_i>0$, and $\zeta_i(t)=c_i+v_i t$ for the zero frequency modes with $\omega_i=0$.
