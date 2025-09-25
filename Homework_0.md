# Homework 0

Reference: Vvedensky D. Group theory in physics (2001)


1. For a finite group with three elements e, a, and b, the multiplication table can be represented as:

Example

The group must satisfy the following properties:

1. **Closure**: The product of any two elements in the group must also be an element of the group.
2. **Associativity**: The multiplication operation must be associative, meaning $(xy)z = x(yz)$ for any $x, y, z \in G$.
3. **Identity Element**: There must be an identity element $e$ such that $e \cdot x = x \cdot e = x$ for every $x \in G$.
4. **Inverse Element**: Every element $x$ in the group must have an inverse $x^{-1}$, such that $x \cdot x^{-1} = x^{-1} \cdot x = e$.



##### Step 1: The Identity Element

By the identity property of the group, we know that multiplying the identity element $e$ by any element in the group will leave the other element unchanged. Therefore, we have the following simple results:

$$
e \cdot e = e, \quad e \cdot a = a, \quad e \cdot b = b
$$

$$
a \cdot e = a, \quad b \cdot e = b
$$

##### Step 2: Closure Property

Now we need to check $a \cdot a=?, a \cdot b = ?, b \cdot b = ?$.

1. Assume the following results:

* $a \cdot a = b$
* $a \cdot b = b\cdot a= e$
* $b \cdot b = a$

2. **Failure of the Assumption $a \cdot a = e$**

​	If we **assume** that $a \cdot a = e$, we run into a **problem**. Here's why:

* If $a \cdot a = e$, then by the inverse property, $a$ would be its own inverse:  $a = a^{-1}$.
* However, for the group to remain consistent, the result of $a \cdot b$ must still belong to the group $G$.    If $a \cdot a = e$,    $a\cdot b$ must be $a$ or $b$, but for $a\cdot e =a, e\cdot b = b$, it is impossible
* This inconsistency would break the group's closure property. Therefore, assuming $a \cdot a = e$ **leads to a contradiction** and thus **fails**.

##### Step 3: Construct the Multiplication Table

So, we can now construct the multiplication table:

$$
\begin{array}{c|ccc}
  & e & a & b \\
\hline
e & e & a & b \\
a & a & b & e \\
b & b & e & a \\
\end{array}
$$

Now, this table satisfies the closure, identity, and inverse properties of the group.

---


2. For the symmetric group $S_3$, the multiplication table is as follows (page 25)

$$
\begin{array}{c|cccccc}
  & e & a & b & c & d & f \\
\hline
e & e & a & b & c & d & f \\
a & a & e & d & f & b & c \\
b & b & f & e & d & c & a \\
c & c & d & f & e & a & b \\
d & d & c & a & b & f & e \\
f & f & b & c & a & e & d \\
\end{array}
$$


