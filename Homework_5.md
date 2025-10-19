# Homework 5

decompose the regular rep. of $S_3$ group into irreducible rep.

The symmetric group $S_3$ has order $|S_3| = 6$. Its regular representation is a 6-dimensional representation.

The **regular representation** of a finite group $G$ decomposes as a direct sum of all its irreducible representations, each appearing with multiplicity equal to its dimension:

$$
\mathbb{C}[G] \cong \bigoplus_{\rho \in \widehat{G}} (\dim \rho) \cdot \rho,
$$

where $\widehat{G}$ denotes the set of (isomorphism classes of) irreducible complex representations of $G$.

Recall that, the group $S_3$ has three conjugacy classes:

1. Identity: $\{e\}$
2. Transpositions: $\{(12), (13), (23)\}$
3. 3-cycles: $\{(123), (132)\}$

Hence, there are **three** irreducible complex representations.

Let their dimensions be $d_1, d_2, d_3$. Then by the dimension formula:

$$
d_1^2 + d_2^2 + d_3^2 = |S_3| = 6.
$$

The only integer solution (up to ordering) with positive integers is:

$$
1^2 + 1^2 + 2^2 = 1 + 1 + 4 = 6.
$$

So $S_3$ has:

- Two 1-dimensional irreps,
- One 2-dimensional irrep.

These are well known:

1. **Trivial representation** $\mathbf{1}$: every group element acts as $+1$.
2. **Sign representation** $\mathbf{1}'$: even permutations act as $+1$, odd permutations (transpositions) as $-1$.
3. **Standard (2-dimensional) representation** $\mathbf{2}$: obtained by the natural action of $S_3$ on the subspace $\{(x_1,x_2,x_3) \in \mathbb{C}^3 : x_1 + x_2 + x_3 = 0\}$, which is 2-dimensional.

The 2D rep $\mathbf{2}$ (dim = 2) appears **twice** (since its multiplicity equals its dimension).

Thus, the decomposition is:

$$
\mathbb{C}[S_3] \cong \mathbf{1} \oplus \mathbf{1}' \oplus \mathbf{2} \oplus \mathbf{2}.
$$

So, this accounts for total dimension: $1 + 1 + 2 + 2 = 6$, as required.

The character $\chi_{\text{reg}}$ of the regular representation is:

$$
\chi_{\text{reg}}(g) = 
\begin{cases}
|G| = 6, & \text{if } g = e, \\
0, & \text{if } g \ne e.
\end{cases}
$$

Now compute the character of the proposed decomposition:

| Class          | Size | $\chi_{\mathbf{1}}$ | $\chi_{\mathbf{1}'}$ | $\chi_{\mathbf{2}}$ | Total $\chi$        |
| -------------- | ---- | --------------------- | ---------------------- | --------------------- | --------------------- |
| e         | 1    | 1                     | 1                      | 2                     | 1 + 1 + 2 + 2 = 6 |
| transpositions | 3    | 1                     | -1                     | 0                     | 1 -1 + 0 + 0 = 0  |
| 3-cycles       | 2    | 1                     | 1                      | -1                    | 1 + 1 -1 -1 = 0   |




