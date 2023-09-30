Refer to [[Vocabulary]] for definitions.

A subspace **MUST** include the zero vector.

# Set Builder Notation
Say you want to create a set with matrixes in $\mathbb{R}^2$ such that the top element $\times$ the bottom element $= 0$.
Writing out each element is not only impractical, but impossible.
Hence we use set builder notation,

$$
\left\{ \text{matrix in } \mathbb{R}^2 \text{ such that the top element }\times \text{ the bottom element } = 0  \right\}$$
$$
\left\{ \text{matrix} \in \mathbb{R}^2 \text{ } | \text{ } \text{ the top element }\times \text{ the bottom element } = 0  \right\}$$
$$
\boxed{
\left\{ \begin{bmatrix} a \\b \end{bmatrix} \in \mathbb{R}^2 \text{ } | \text{ } a\times b = 0  \right\}
}
$$

Is $v=\left\{ \begin{bmatrix} a \\b \end{bmatrix} \in \mathbb{R}^2 \text{ } | \text{ } a\times b = 0  \right\}$ a subspace?

$\begin{bmatrix} 0 \\ 1 \end{bmatrix},\begin{bmatrix} 1 \\ 0 \end{bmatrix} \in v$ but $\begin{bmatrix} 0 \\ 1 \end{bmatrix}+\begin{bmatrix} 1 \\ 0 \end{bmatrix} \notin  v$ So $v$ is **not** a subspace.