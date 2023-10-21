Finding powers of a diagonal matrix, is very simple.
$$
\begin{bmatrix} a&0\\0&b \end{bmatrix}^k = \begin{bmatrix} a^k&0\\0&b^k \end{bmatrix}
$$
# Diagonalizable
If $A$ is similar to diagonal matrix $D$ ($A=PDP^{-1}$) then A is diagonalizable.

$$
\begin{aligned}
A&=PDP^{-1}\\
A&=\begin{bmatrix} v_1&v_2\dots&v_n \end{bmatrix} \begin{bmatrix} \lambda_1\\ &\lambda_2\\ &&\ddots\\ &&&\lambda_4 \end{bmatrix} \begin{bmatrix} v_1&v_2\dots&v_n \end{bmatrix}^{-1}
\end{aligned}
$$
> [!IMPORTANT] 
> $v_1 \dots v_n$ are eigenvectors
> $\lambda_1 \dots \lambda_n$ are eigenvalue

>[!NOTE|] Proof
![[Pasted image 20231020130535.png|450]]

$A$ is diagonalizable if and only if $A$ has $n$ linearly independent eigenvectors.

# Example

Diagonalize $A=\begin{bmatrix} 2&6\\0&-1 \end{bmatrix}$
Eigenvalue $= 2,-1$ 
Eigenvectors $= \begin{bmatrix} 1\\0 \end{bmatrix},\begin{bmatrix} 2\\-1 \end{bmatrix}$
$$
\begin{aligned}
A&=PDP^{-1}\\
&=\begin{bmatrix} 1&2\\0&-1 \end{bmatrix} \begin{bmatrix} 2&0\\0&-1 \end{bmatrix} \begin{bmatrix} 1&2\\0&-1 \end{bmatrix}^{-1}\\
&=\begin{bmatrix} 1&2\\0&-1 \end{bmatrix} \begin{bmatrix} 2&0\\0&-1 \end{bmatrix} \begin{bmatrix} 1&2\\0&-1 \end{bmatrix}\\
\end{aligned}
$$

> [!note]
> This is a special case and is not always true,  
> $$\begin{bmatrix} 1&2\\0&-1 \end{bmatrix}^{-1}=\begin{bmatrix} 1&2\\0&-1 \end{bmatrix}$$

If $A$ is $n \times n$ and has $n$ distinct eigenvalues, then $A$ is diagonalizable.
$A$ does not **have to** have $n$ distinct eigenvalues for $A$ to be diagonalizable.
![[Diagonal Matrices.png]]

# Repeated Eigenvalue
(I didn't feel like typing)
![[Diagonal Matrices-1.png]]
![[Diagonal Matrices-2.png]]
![[Diagonal Matrices-3.png]]
![[Diagonal Matrices-4.png]]
![[Diagonal Matrices-5.png]]