# Rotations

In mathematics and physics, groups play a fundamental role in describing symmetries and transformations. Here, we provide a brief description of three important Lie groups: SO(2), SO(3), and SU(2). These groups find applications in various areas, including classical mechanics, quantum mechanics, and field theory.

## SO(2)

The group SO(2) represents the special orthogonal transformations in two-dimensional Euclidean space. These transformations preserve distances, angles, and orientation. An element of SO(2) is represented by a $2 \times 2$ real orthogonal matrix with determinant $1$. The general form of an SO(2) matrix is given by:


```math
R_{\mathrm{SO(2)}}(\theta)=\begin{pmatrix}
\cos\theta &-\sin\theta\\
\sin\theta &\cos\theta
\end{pmatrix}
```

where $\theta$ is the rotation angle. SO(2) is an Abelian group isomorphic to the unit circle $S^1$ and can be viewed as the group of rotations about the origin in the plane.

## SO(3)

The group SO(3) represents the special orthogonal transformations in three-dimensional Euclidean space. These transformations preserve distances, angles, and orientation. An element of SO(3) is represented by a $3 \times 3$ real orthogonal matrix with determinant $1$. The general form of an SO(3) matrix is given by:

$$R(\theta, \mathbf{n}) = \exp(-i \theta \mathbf{n}\cdot\mathbf{J}),$$


where $\theta$ is the rotation angle, $\mathbf{n}$ is a unit vector specifying the rotation axis, and the components of $\mathbf{J}$ are
the generators that satisfy the so(3) algebra $[J_i,J_j]=i\epsilon_{ijk}J_k$. SO(3) is locally isomorphic to the SU(2) group.

## SU(2)

The group SU(2) represents the special unitary transformations in two complex dimensions. These transformations preserve the Hermitian inner product and have determinant $1$. An element of SU(2) is represented by a $2 \times 2$ complex unitary matrix with determinant $1$. The general form of an SU(2) matrix is given by:

$$U(\theta, \mathbf{n}) = \exp(-i \theta \mathbf{n}\cdot\mathbf{j})\equiv\exp(-i \theta \mathbf{n}\cdot\boldsymbol{\sigma}/2)=\cos\frac{\theta}{2}\mathbb{1}-i\sin\frac{\theta}{2}\mathbf{\hat{n}}\cdot\boldsymbol{\sigma},$$

where the components of $\boldsymbol{\sigma}$ are the Pauli matrices. One can rotate a 3-D vector $\mathbf{r}$ using SU(2) matrices according to

$$(\mathbf{j}\cdot\mathbf{r}')=U(\mathbf{j}\cdot\mathbf{r})U^{\dagger},$$

with $\mathbf{r}'=R\mathbf{r}$. This transformation reveals the map between SU(2) and SO(3) matrices, that can be written as

$$R_{ik}(U)=2\mathrm{Tr}(j_i U j_k U^{\dagger}).$$

## Quaternions
Notice that the $SU(2)$ realization of rotations is a 2-dimensional representation of the quaternion algebra given by

$$\mathbf{i}=-i\sigma^1,\quad\mathbf{j}=-i\sigma^2,\quad\mathbf{k}=-i\sigma^3,$$

```math
\begin{gather}
\mathbf{i}^2=\mathbf{j}^2=\mathbf{k}^2=\mathbf{i}\mathbf{j}\mathbf{k}=-1,\\
\mathbf{i}\mathbf{j}=-\mathbf{j}\mathbf{i}=\mathbf{k},\\
\mathbf{j}\mathbf{k}=-\mathbf{k}\mathbf{j}=\mathbf{i},\\
\mathbf{k}\mathbf{i}=-\mathbf{i}\mathbf{k}=\mathbf{j},
\end{gather}
```
which was the first successful description of rotations, conceived by Hamilton himself. In this framework we can 
perform rotations by packing the components of  $\mathbf{r}$ in a purely imaginary quaternion

$$q=x_1\mathbf{i}+x_2\mathbf{j}+x_3\mathbf{k},$$

which is rotated by the corresponding quaternion (also known as rotor)

$$u(\theta,\mathbf{\hat{n}})=\cos\frac{\theta}{2}+\sin\frac{\theta}{2}[n_1 \mathbf{i}+n_2 \mathbf{j}+n_3 \mathbf{k}],$$

and its conjugate (inverse)

$$u^{*}(\theta,\mathbf{\hat{n}})=\cos\frac{\theta}{2}-\sin\frac{\theta}{2}[n_1 \mathbf{i}+n_2 \mathbf{j}+n_3 \mathbf{k}],$$

through

$$q'=u(\theta,\mathbf{\hat{n}})q u^{*}(\theta,\mathbf{\hat{n}})$$

where the product of two quaternions $q_a=w_a+x_a\mathbf{i}+y_a\mathbf{j}+z_a\mathbf{k}$, $a=1,2$, is determined by the quaternion algebra to be

```math
\begin{split}
q_1 q_2=&w_1 w_2 - x_1 x_2 - y_1  y_2 - z_1 z_2\\
& +(w_1 x_2 + x_1 w_2 + y_1 z_2 - z_1 y_2)\mathbf{i}\\
& +(w_1 y_2 + y_1 w_2 + z_1 x_2 - x_1z_2)\mathbf{j}\\
& +(w_1 z_2 + z_1 w_2 + x_1 y_2 - y_1x_2)\mathbf{k}.
\end{split}
```

## Euler-Rodrigues Formula
It can be shown that the general rotation of a vector $\mathbf{r}$ through an angle $\theta$ around the axis $\widehat{\mathbf{n}}$ is given by the Euler-Rodrigues formula

$$\mathbf{r}'=\mathbf{r} \cos\theta+\widehat{\mathbf{n}}\times \mathbf{r}\sin\theta+(\widehat{\mathbf{n}}\cdot \mathbf{r})\widehat{\mathbf{n}}(1-\cos\theta)$$

## Examples

SO(2): Group of Proper Rotations on the Plane
[SO(2).ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20and%20Numerical%20Projects/Rotations/SO(2).ipynb)

SO(3) and SU(2) Local Isomorphism
[SO(3)_and_SU(2).ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20and%20Numerical%20Projects/Rotations/SO(3)_and_SU(2).ipynb)

Quaternion Rotation and Euler-Rodrigues Formula
[quaternion_rotation_rodrigues_formula.ipynb](https://github.com/Vaquera-Araujo/LabAv2023/blob/main/Symbolic%20and%20Numerical%20Projects/Rotations/quaternion_rotation_rodrigues_formula.ipynb)


## Challenges

Write a Jupyter Notebook for the Determination of the $su(3)$ and $so(4)$ Lie Algebras

Implement a Numerical Version of the Quaternion Rotation





