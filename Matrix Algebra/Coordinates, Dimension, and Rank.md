![[Coordinates, Dimension, and Rank.png]]

In [[Row Reduction Algorithm|RREF]]
$$
\left[
\begin{array}{cc|c}
1&0&2\\
0&1&3\\
0&0&0
\end{array}
\right]
$$
So, $\vec{x}$ is in the span of $B$ and $[x]_B=\begin{bmatrix} 2 \\3 \end{bmatrix}$.

# Dimension 
$\text{dim} (\mathbb{R}^n) = n$
$\text{dim}(\text{Null} (A) ) = \text{no of free variables}$
$\text{dim}(\text{Col} (A) ) = \text{no of pivot columns}$

# Rank
$\text{Rank} (A)=\text{dim}(\text{Col} (A) ) = \text{no of pivot columns}$
$\text{Rank} (A) + \text{dim}(\text{Null} (A)) = \text{dim}(\text{Col} (A)) + \text{dim}(\text{Null} (A)) = \text{no of columns}$ 
# Invertibility
If $A$ is an $n \times n$ matrix. These conditions are equivalent.
1. $A$ is invertible.
2. The columns of $A$ are a basis for $\mathbb{R}^n$
3. Col $A = \mathbb{R}^n$.
4. Rank $A = \text{dim}(\text{Col } A) = n$.
5. Null $A = \{ \vec{0} \}$ 