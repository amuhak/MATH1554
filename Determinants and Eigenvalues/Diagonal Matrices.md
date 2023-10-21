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

