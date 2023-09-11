$A \in \mathbb{R}^{n \times n}$ is invertible if there is a $C \in \mathbb{R}^{n \times n}$ so that:

$$AC=CA=I_n$$
If so we write, $C=A^{-1}$
***
$A$ has an inverse if and only if there is a pivot on every row and column.  
# For a $2 \times 2$ 
## Compute
$$ \begin{bmatrix} a &b \\ c&d \end{bmatrix}^{-1} = \frac{1}{ad-bc} \begin{bmatrix} d &-b \\ -c&a \end{bmatrix} $$
## Use it to solve a Linear systems
$$
\begin{aligned}
A\vec{x}&=b \\ 
A^{-1}A\vec{x}&=A^{-1}b \\
I\vec{x}&=A^{-1}b \\
\vec{x}&=A^{-1}b
\end{aligned}
$$

# Computing $A^{-1}$
1. Row reduce the augmented matrix $\left( A\ |\ I_n \right)$ to [[Row Reduction Algorithm|RREF]] 
2. If the reduction is in the form, $(I_n\ |\ B)$ then $A$ is invertible and $B=A^{-1}$. Else, $A$ is not invertible.

For example to find $\left[ \begin{array} \\ 0 &1&2\\1&0&3\\0&0&1 \end{array} \right]^{-1}:$
$$
\begin{aligned}
&=\left[ \begin{array}{ccc|ccc} 0 &1&2&1&0&0\\1&0&3&0&1&0\\0&0&1&0&0&1 \end{array} \right] \\
&=\left[ \begin{array}{ccc|ccc} 1 &0&0&0&1&-3\\0&1&0&1&0&-2\\0&0&1&0&0&1 \end{array} \right] \\
&=(I_3\ |\ A^{-1})\\
A^{-1} &= \left[ \begin{array}{ccc} 0&1&-3\\1&0&-2\\0&0&1 \end{array} \right]
\end{aligned}
$$
Some properties:
![[Inverse of a Matrix.png]]