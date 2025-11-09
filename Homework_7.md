# Homework 7

> Give the generators in SO(4)?  What are the rotation matrices? 


### (a) Generators of SO(4)

By definition,

$$
SO(4)={R\in \mathbb{R}^{4\times4}\mid R^{\mathsf T}R=\mathbb{I}_4,\ \det R=1}.
$$

The Lie algebra is

$$
\mathfrak{so}(4)={A\in \mathbb{R}^{4\times4}\mid A^{\mathsf T}=-A},
$$

the space of real antisymmetric $4\times 4$ matrices.

An antisymmetric $n\times n$ matrix has free entries only above the diagonal, i.e.  $\binom{n}{2}=n(n-1)/2$  parameters. For (n=4),

$$
\dim \mathfrak{so}(4)=\frac{4\cdot 3}{2}=6.
$$

A standard basis of generators

For  $1\le i<j\le 4$ , define  $L_{ij}\in\mathfrak{so}(4)$  by

$$
(L_{ij})*{kl}=\delta*{ik}\delta_{jl}-\delta_{il}\delta_{jk}.
$$

Equivalently, $L_{ij}$ has a +1 at (i,j)), a -1) at (j,i), and zeros elsewhere.

The six basis elements are

$$
L_{12},;L_{13},;L_{14},;L_{23},;L_{24},;L_{34}.
$$

For example, explicitly:

$$
L_{12}=
\begin{pmatrix}
0 & 1 & 0 & 0 \\
-1 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0
\end{pmatrix},\quad
L_{13}=
\begin{pmatrix}
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 \\
-1 & 0 & 0 & 0 \\
0 & 0 & 0 & 0
\end{pmatrix},\quad
L_{14}=
\begin{pmatrix}
0 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
-1 & 0 & 0 & 0
\end{pmatrix}
$$




$$
L_{23}=
\begin{pmatrix}
0 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & -1 & 0 & 0 \\
0 & 0 & 0 & 0
\end{pmatrix},\quad
L_{24}=
\begin{pmatrix}
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 \\
0 & -1 & 0 & 0
\end{pmatrix},\quad
L_{34}=
\begin{pmatrix}
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & -1 & 0
\end{pmatrix}.
$$


They obey the $\mathfrak{so}(4)$ commutation relations

$$
[L_{ij},L_{kl}]
=\delta_{jk}L_{il}-\delta_{ik}L_{jl}-\delta_{jl}L_{ik}+\delta_{il}L_{jk}.
$$


---

### (b) Rotation matrices in SO(4)

General finite rotation. Any rotation is obtained by exponentiating an antisymmetric matrix:

$$
R(\theta)= \exp \sum _{i<j} \theta_{ij} L_{ij}  \in SO(4) 
$$

Geometrically, a simple rotation in the (ij)-plane by angle $\theta$ is

$$
R_{ij}(\theta)=\exp(\theta, L_{ij}).
$$

In a basis where the (ij)-plane is $(e_i,e_j)$, this is a $2\times 2$ rotation block acting on (i,j) and identity on the orthogonal directions.

**One explicit rotation.** Rotation by angle $\theta$ in the (1,2)-plane:

$$
R_{12}(\theta)=\exp(\theta L_{12}) =
\begin{pmatrix}
\cos\theta & \sin\theta & 0 & 0 \\
-\sin\theta & \cos\theta & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{pmatrix}.
$$


Then one can analogously write $R_{13}(\theta), R_{14}(\theta), R_{23}(\theta), R_{24}(\theta), R_{34}(\theta)$ by placing the $2\times2$ rotation block in the appropriate rows/columns.

**Checks:**

1.  $R_{12}(\theta)^{\mathsf T}R_{12}(\theta)=\mathbb{I}_4$  
2.  $\det R_{12}(\theta)=1$ 
3.  

$$
{\frac{d}{d \theta} R_{12}(\theta)|_{\theta=0} = L_{12}}
$$

matching the generator.

