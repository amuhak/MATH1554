Refer to [[Vocabulary]] for definitions.

Say we wish to find the basis for $H=\left\{ \vec{x} \in \mathbb{R}^4 | x_1 - 3x_2 - 5x_3 + 7x_4 = 0 \right\}$ (Note: this is [[Subsets and Subspaces#Set Builder Notation|set builder notation]])

We must:
1. Convert this into a $A \vec{x}=0$ form
2. Convert this into [[Parametric Vector Form]]
3. Profit???
$$
\begin{aligned}
A \vec{x}&=0\\
\begin{bmatrix} 1 & -3 & -5 & 7 \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \\ x_3 \\ x_4 \end{bmatrix}&=0\\
\begin{bmatrix} 3x_2+5x_3-7x_4\\x_2\\x_3\\x_4 \end{bmatrix}&=0\\
x_2\begin{bmatrix} 3 \\ 1 \\ 0 \\ 0 \end{bmatrix}+x_3\begin{bmatrix} 5 \\ 0 \\ 1 \\ 0 \end{bmatrix}+x_4\begin{bmatrix} -7 \\ 0 \\ 0 \\ 1 \end{bmatrix} &= 0 \\
\text{The basis for the null space of }H &= \boxed{\left\{ \begin{bmatrix} 3 \\ 1 \\ 0 \\ 0 \end{bmatrix},\begin{bmatrix} 5 \\ 0 \\ 1 \\ 0 \end{bmatrix},\begin{bmatrix} -7 \\ 0 \\ 0 \\ 1 \end{bmatrix} \right\}}
\end{aligned}
$$
This is the basis of the null space of $H$ due to the equation being $x_1 - 3x_2 - 5x_3 + 7x_4 = \boxed{0}$.

# Basis of the Null Space

Now say we wish to find the basis of the null space of $A$ 
We can:
1. Convert it into a $A \vec{x}=0$ form.
2. Convert that into [[Parametric Vector Form]]
3. The set of the vectors in parametric vector form is the basis of the null space.

# Basis of the Column Space

Say we wish to find the basis of the column space of $A$
We could:
1. Find the pivot columns of $A$.
2. The set of the pivot columns of $A$ is the basis of the column space.