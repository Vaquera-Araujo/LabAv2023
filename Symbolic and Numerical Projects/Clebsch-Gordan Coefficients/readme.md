# Sum of Angular Momentum in Quantum Mechanics and Clebsch-Gordan Coefficients

In quantum mechanics, the concept of angular momentum plays a crucial role in understanding the behavior of particles. Angular momentum is associated with rotational motion and can have both magnitude and direction. When dealing with composite systems, such as atoms or nuclei, it becomes necessary to consider the total angular momentum resulting from the combination of individual angular momenta.

## Total Angular Momentum

The total angular momentum operator, denoted as $J$, is defined as the sum of the individual angular momentum operators for each particle in the system. Mathematically, this can be expressed as:


$$\mathbf{J} = \mathbf{J}_1\otimes \mathbb{1}_2 + \mathbb{1}_1\otimes\mathbf{J}_2 $$

Here, $\mathbf{J}$ represents the total angular momentum, $\mathbf{J}_1$, $\mathbf{J}_2$ correspond to the angular momentum operators for the individual particles, and $\otimes$ stands for the direct product. The direct product of two matrices is a fundamental operation that allows us to construct a new matrix by combining the elements of the original matrices. Given two matrices $A$ and $B$, their direct product $A\otimes B$ results in a larger matrix with dimensions equal to the product of the dimensions of $A$ and $B$.

The direct product is defined element-wise, meaning that each element of $A\otimes B$ is obtained by multiplying the corresponding elements of $A$ and $B$. Mathematically, if $A$ is an $m \times n$ matrix and $B$ is a $p \times q$ matrix, then the resulting matrix $A\otimes B$  is an $(mp) \times (nq)$ matrix given by:

```math
A\otimes B=\left(\begin{array}{cccc}
a_{11} B&a_{12} B&\cdots a_{1m} B\\
a_{21} B&a_{22} B&\cdots a_{2m} B\\
\vdots&\vdots&\ddots&\vdots\\
a_{m1} B&a_{m2} B&\cdots a_{mm} B
\end{array}\right).
```

Here, each element $a_{ij}$ of $A$ is multiplied by the entire matrix $B$ to obtain the corresponding block $a_{ij}B$ in the resulting direct product matrix.

## Eigenstates of Total Angular Momentum

The total angular momentum operator, $\mathbf{J}$, has associated eigenstates that describe the allowed values of the total angular momentum magnitude and its projection along a specific axis. These eigenstates are denoted by $|J, M⟩$, where $j$ represents the total angular momentum quantum number and $m$ represents the magnetic quantum number.

The total angular momentum eigenstates can be obtained by combining the individual angular momentum states using the Clebsch-Gordan coefficients. These coefficients provide the probability amplitudes for the coupling of two angular momenta to form a total angular momentum.

## Clebsch-Gordan Coefficients

The Clebsch-Gordan coefficients, denoted as $C(j_1, m_1; j_2, m_2 | J, M)$, relate the individual angular momentum quantum numbers $(j_1,j_2)$ and their corresponding magnetic quantum numbers $(m_1,m_2)$  to the total angular momentum quantum numbers (J, M).

These coefficients can be used to express the total angular momentum eigenstates in terms of the individual angular momentum states. Mathematically, this relationship is given by:


$$|J, m⟩ = \sum_{m_1, m_2} C(j_1, m_1; j_2, m_2 | J, M) |j_1, m_1⟩ \otimes |j_2, m_2⟩.$$

## Examples

### Symbolic Calculation of a Table of Clebsch-Gordan Coefficients in the Sum of any Pair of Spins

[clebsch.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20and%20Numerical%20Projects/Clebsch-Gordan%20Coefficients/clebsch.ipynb)

## Challenges

Write a Numeric Version of the Example.
