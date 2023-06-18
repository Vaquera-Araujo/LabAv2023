# Small Oscillations

## Free oscillations in one dimension

A very common form of motion of mechanical systems is what are called small oscillations of a system about a position of stable equilibrium. We shall consider first of all the simplest case, that of a system with only one degree of freedom.
Stable equilibrium corresponds to a position $q_0$ of the system in which its potential energy $U(q)$ is a minimum  $dU(q_0)/dq=0$, and  $d^2U(q_0)/dq^2>0$. A movement away from this position results in the setting up of a force $-dU/dq$ which tends to return the system to equilibrium. For small deviations from the equilibrium position, it is sufficient to retain the first non vanishing term in the expansion of the difference

$U(q)\approx U(q_0)+\frac{1}{2}\left.\frac{d^2U}{dq^2}\right|_{q_0}(q-q_0)^2$

The constant term $U(q_0)$ does not modify the equations of motion, thus we can remove it by measuring the potential energy from its minimum value, \emph{i.e.} setting $U(q_0) = 0$, and use the symbol $x=q-q_0$ for the deviation of the coordinate from its equilibrium value. Thus

$U(x)\approx \frac{1}{2}\left.\frac{d^2U}{dq^2}\right|_{q_0}x^2\equiv \frac{1}{2}kx^2$.

The kinetic energy of a system with one degree of freedom is in general
of the form $T=a(q)\dot{q}^2/2=a(q)\dot{x}^2/2$.  In the same approximation, it is sufficient to replace the function $a(q)$ by its value at $q = q_0$. Putting for brevity $a(q_0)\equiv m$, the Lagrangian of a system executing small oscillations in one dimension is equivalent to the simple harmonic oscillator

$L=\frac{1}{2}m \dot{x}^2-\frac{1}{2}k x^2$.

The corresponding equation of motion is

$\ddot{x}+\omega^2x=0$

with angular frequency $\omega=\sqrt{\frac{k}{m}}$, and solution

$x(t)= C\cos(\omega t+\delta)$

where the constants $C$ and $\delta$ are real and determined by the initial conditions.

## Linearized equations of motion
Now, consider a system with $n$ degrees of freedom characterized by the generalized coordinates $q_i$, with a time independent scalar potential $U(q_i)$ displaying a strict local minimum at $q^0_i$ and rescaled such that $U(q_i^0)=0$. Using a standard particle Lagrangian, the kinetic energy is a quadratic function of the velocities, provided that the generalized coordinates are time-independent functions of the Cartesian coordinates. Then, generalizing the  previous results, the Lagrangian can be approximated to second order in the perturbation expansion around equilibrium by

$L=\frac{1}{2}\bra{\dot{x}}M\ket{\dot{x}}-\frac{1}{2}\bra{x}K\ket{x}$

where $x_i=q_i-q^{0}_i$ are the components of $\ket{x}$, and the matrix elements of $M$ are 
