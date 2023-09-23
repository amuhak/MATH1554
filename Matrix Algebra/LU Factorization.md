# Triangular Matrices
## Upper Triangular
If $a_{i,j} = 0$ for $i>j$ 
In other words the elements below the main diagonal are 0.
Examples:
![[LU Factorization.png]]

## Lower Triangular
If $a_{i,j} = 0$ for $i<j$ 
In other words the elements above the main diagonal are 0.
Examples:
![[LU Factorization-1.png]]
***
# LU Factorization
If $A$ is an $m \times n$ matrix that can be row reduced to echelon form without row exchanges, then $A = LU$. $L$ is a lower triangular $m \times m$ matrix with 1's on the diagonal, $U$ is an echelon form of $A$.

For example the $LU$ factorization of $A \in \mathbb{R}^{3\times 2}$  would look like:

$$
\begin{bmatrix}
1&0&0 \\ *&1&0 \\ * & * & 1
\end{bmatrix}
$$