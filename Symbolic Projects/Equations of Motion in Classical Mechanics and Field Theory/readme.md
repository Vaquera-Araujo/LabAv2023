# Lagrangian Mechanics and Euler-Lagrange Equations

## Introduction

Lagrangian mechanics is a powerful formulation of classical mechanics that provides a concise and elegant description of the dynamics of physical systems. It was developed by Joseph-Louis Lagrange in the late 18th century and has since become an essential tool in many areas of physics.

## Lagrangian Function
The cornerstone of Lagrangian mechanics is the Lagrangian function, denoted by $L$. The Lagrangian is defined as the difference between the kinetic energy $T$ and the potential energy $V$ of a system: $L = T - V$. It is a function of the generalized coordinates $q_i$, their time derivatives $\dot{q}_i$, and time $t$. The generalized coordinates $q_i$ are the independent degrees of freedom needed to describe the configuration of the system.

## Principle of Least Action
The central idea in Lagrangian mechanics is the principle of least action. According to this principle, the motion of a physical system between two points in time is such that the action integral is minimized. The action $S$ is defined as the integral of the Lagrangian over time:  $S = \int_{t_1}^{t_2}  dt \mathcal{L}(q_i, \dot{q}_i, t)$.

## Euler-Lagrange Equations
The Euler-Lagrange equations are a set of second-order differential equations that describe the equations of motion of a system derived from the principle of least action. They are obtained by varying the action with respect to each generalized coordinate $q_i$ while keeping the other coordinates fixed. The Euler-Lagrange equations have the form:

$\frac{d}{dt} \left( \frac{\partial \mathcal{L}}{\partial \dot{q}_i} \right) - \frac{\partial \mathcal{L}}{\partial q_i} = 0$

These equations provide a systematic and elegant way to determine the equations of motion for a wide range of physical systems. Solving the Euler-Lagrange equations yields the trajectories of the system's degrees of freedom as functions of time.

Lagrangian mechanics, based on the Lagrangian function and the principle of least action, provides a powerful framework for analyzing the classical dynamics of physical systems. The Euler-Lagrange equations serve as the fundamental equations of motion, allowing us to derive the trajectories of the system's generalized coordinates. This formalism has proven to be a valuable tool in various fields of physics , enabling the study and understanding of complex mechanical systems.

## Classical Field Theory
Classical field theory provides a mathematical framework to describe the behavior of fields, such as the electromagnetic field or the gravitational field. The Euler-Lagrange equations play a fundamental role in this theory, allowing us to derive the equations of motion for these fields based on the principle of least action.

## The Action Principle in Field Theory
The starting point of classical field theory is the action principle. The action $S$, is defined as the integral of the Lagrangian density, $\mathcal{L}$, over the space-time volume:

$S=\int d^4x \mathcal{L}$

where $d^4x$ represents the infinitesimal volume element in 4-dimensional Minkowski spacetime, and $x^{\mu}$, $\mu=1,\dots,4$ are the space-time coordinates.

## Variational Principle
The key idea behind the Euler-Lagrange equations is the variational principle. According to this principle, the actual path taken by the field is the one that minimizes the action, which is equivalent to saying that the action is stationary under infinitesimal variations of the field configurations.

Mathematically, we consider a variation of the field $\phi$ as $\phi \rightarrow \phi + \delta \phi$, where $\delta \phi$ is an infinitesimal change in the field. The variation of the action $\delta S$ is given by:

$\delta S=\int d^4x \left[ \frac{\partial \mathcal{L}}{\partial \phi} \delta \phi + \frac{\partial \mathcal{L}}{\partial (\partial_{\mu} \phi)} \delta (\partial_{\mu} \phi) \right]$

where $\partial_{\mu}$ represents the partial derivative with respect to the space-time coordinate $x^{\mu}$. 

## Derivation of Euler-Lagrange Equations
To derive the Euler-Lagrange equations, we impose the condition that the action is stationary, i.e., $\delta S = 0$, for arbitrary variations $\delta \phi$. Using the principle of least action, we obtain:

$\frac{\partial\mathcal{L}}{\partial\phi}-\partial_{\mu}\left[ \frac{\partial\mathcal{L}}{\partial(\partial_{\mu} \phi)}\right]=0$

These are the Euler-Lagrange equations for the field $\phi$ in classical field theory. They represent a set of second-order partial differential equations that govern the dynamics of the field.

## Conclusion
The Euler-Lagrange equations are a powerful tool in classical field theory, allowing us to determine the equations of motion for fields based on the principle of least action. By solving these equations, we can study the behavior of various fields and make predictions about their interactions in the physical world.

## Examples
Coplanar double pendulum:
![Diagram](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20Projects/Equations%20of%20Motion%20in%20Classical%20Mechanics%20and%20Field%20Theory/coplanar_double_pendulum.png) 
[coplanar_double_pendulum.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20Projects/Equations%20of%20Motion%20in%20Classical%20Mechanics%20and%20Field%20Theory/coplanar_double_pendulum.ipynb)




Klein-Gordon field equation of motion
[klein_gordon.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20Projects/Equations%20of%20Motion%20in%20Classical%20Mechanics%20and%20Field%20Theory/klein_gordon.ipynb)




