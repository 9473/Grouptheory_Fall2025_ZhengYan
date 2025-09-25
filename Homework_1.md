# Homework 1



### 1: Find a Self-Conjugate Subgroup of $S_4$

A **self-conjugate subgroup** (or **normal subgroup**) $H$ of a group $G$ is a subgroup that satisfies the condition:

$$
gHg^{-1} = H \quad \text{for every} \quad g \in G
$$

In other words, conjugating any element of the subgroup by any element of the group results in another element of the subgroup.

One well-known self-conjugate subgroup of $S_4$ is the **Klein four-group** $V_4$. The elements of $V_4$ are:

$$
V_4 = \{ e, (12)(34), (13)(24), (14)(23) \}
$$

you can check if $V_4$ satisfies $gV_4g^{-1} = V_4$, i.e.,  check if $g \cdot h \cdot g^{-1} \in V_4$ for every $h \in V_4$ and for every $g \in S_4$.

For example,

$$
(13) \cdot (12)(34) \cdot (13)^{-1} = (14)(23) \in V_4
$$



### 2: Quotient group

Then, We constructed the quotient group $S_4 / V_4$, which contains 24/4=6 cosets. (S4: 4!=24)

S4={1,(12),(13),(14),(23),(24),(34),

​	(12)(34),(13)(24),(14)(23),

​	(123),(132),(124),(134),(143),(234),(243),

​	(1234),(1243),(1324),(1423),(1432)}

The cosets are formed by multiplying each element of $S_4$ by the subgroup $V_4$.

The cosets of $V_4$ in $S_4$ are as follows:



1. $C_0 = V_4 \cdot e = V_4$:

$$
C_0 = \{ e, (12)(34), (13)(24), (14)(23) \}
$$

2. $C_1 = V_4 \cdot (12) = (12)V_4$

$$
C_1 = \{ (12), (34), (1324), (1423) \}
$$

3. $C_2 = V_4 \cdot (13) = (13)V_4$

$$
C_2 = \{ (13), (24), (1234), (1432) \}
$$

4. $C_3 = V_4 \cdot (23) = (23)V_4$

$$
C_3 = \{ (23), (14), (1243), (1342) \}
$$

5. $C_4 = V_4 \cdot (123) = (123)V_4$

$$
C_4 = \{ (123), (134), (142), (243) \}
$$

6. $C_5 = V_4 \cdot (132) = (132)V_4$

$$
C_5 = \{ (132), (124), (143), (234) \}
$$



Consider $e,12,13,23,123,132$,  it reminds us $S_4/V_4$ is isomorphic to $S_3$. So their multiplication table should be similar.




### 3. Multiplication table

For example: $C_5 \cdot C_5 = (132)(132)V_4 = (123)V_4$.

$$
\begin{array}{c|cccccc}
 & C_0 & C_1 & C_2 & C_3 & C_4 & C_5 \\
\hline
C_0 & C_0 & C_1 & C_2 & C_3 & C_4 & C_5 \\
C_1 & C_1 & C_0 & C_5 & C_4 & C_3 & C_2 \\
C_2 & C_2 & C_4 & C_0 & C_5 & C_1 & C_3 \\
C_3 & C_3 & C_5 & C_4 & C_0 & C_2 & C_1 \\
C_4 & C_4 & C_2 & C_3 & C_1 & C_5 & C_0 \\
C_5 & C_5 & C_3 & C_1 & C_2 & C_0 & C_4 \\
\end{array}
$$


