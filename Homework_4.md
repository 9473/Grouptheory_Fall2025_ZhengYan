# Homework 4

Prove that the regular representation must be reducible.

Let $G$ be a finite group with $|G| > 1$ (e.g., $G = S_3$).  Consider the vector  

$$
v = \sum_{g \in G} e_g \in \mathbb{C}[G]
$$

in the regular representation. For any $h\in G$,  

$$
h \cdot v = \sum_{g \in G} e_{hg} = \sum_{g' \in G} e_{g'} = v,
$$

since left multiplication by $h$ permutes the group elements.

Thus, the 1-dimensional subspace $\mathbb{C} v$ is **invariant** under the action of $G$.  The 1-dimensional subspace $\mathbb{C}v$ is $G$​-invariant and carries the trivial representation.  

Since $\dim \mathbb{C}[G] = |G| \geq 2$, this is a proper, nontrivial invariant subspace.  Hence, the regular representation is reducible. 

(If  $|G| = 1$ (the trivial group), then the regular representation is 1-dimensional and irreducible. But for any **nontrivial** finite group (including $S_3$), the regular representation is reducible.)

