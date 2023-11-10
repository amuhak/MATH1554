Finding powers of a diagonal matrix, is very simple.
$$
\begin{bmatrix} a&0\\0&b \end{bmatrix}^k = \begin{bmatrix} a^k&0\\0&b^k \end{bmatrix}
$$
# Diagonalizable
If $A$ is similar to diagonal matrix $D$ ($A=PDP^{-1}$) then A is diagonalizable.

$$
\begin{aligned}
A&=PDP^{-1}\\
A&=\begin{bmatrix} v_1&v_2\dots&v_n \end{bmatrix} \begin{bmatrix} \lambda_1\\ &\lambda_2\\ &&\ddots\\ &&&\lambda_n \end{bmatrix} \begin{bmatrix} v_1&v_2\dots&v_n \end{bmatrix}^{-1}
\end{aligned}
$$
> [!IMPORTANT]+ 
> $v_1 \dots v_n$ are eigenvectors
> $\lambda_1 \dots \lambda_n$ are eigenvalue
> $A$ is diagonalizable if and only if $A$ has $n$ linearly independent eigenvectors.
> [[Inverse of a Matrix|Invertibility]] has no effect on diagonalizability 

>[!NOTE|]+ Proof
![[Diagonal Matrices-6.png|450]]

***
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

> [!note]+
> This is a special case and is not always true,  
> $$\begin{bmatrix} 1&2\\0&-1 \end{bmatrix}^{-1}=\begin{bmatrix} 1&2\\0&-1 \end{bmatrix}$$

If $A$ is $n \times n$ and has $n$ distinct eigenvalues, then $A$ is diagonalizable.
$A$ does not **have to** have $n$ distinct eigenvalues for $A$ to be diagonalizable.
![[Diagonal Matrices.png]]

# Properties
- $A$ is diagonalizable if and only if $A$ has $n$ linearly independent eigenvectors.
- [[Inverse of a Matrix|Invertibility]] has no effect on diagonalizability.
- If A has $n$ distinct eigenvalues, then $A$ is diagonalizable. (The converse is not necessarily true)
# Find Diagonalizability
$$A=PDP^{-1}$$
Finding $D$ is straight forward. It is simply the eigenvalue of $A$.
$P$ **MUST** be [[Inverse of a Matrix|Invertible]].

- If $\sum g_i = n$, $A$ is diagonalizable.
- If $g_i = a_i$ for all $i$, $A$ is diagonalizable.
- If the eigenvectors of $A$ form a basis in $\mathbb{R}^n$, $A$ is diagonalizable.

# Repeated Eigenvalue

Diagonalize $A = \begin{bmatrix} 7 & 4 & 16 \\ 2 & 5 & 8 \\ -2 & -2 & -5 \end{bmatrix}$ with eigenvalues $\lambda_1 = 1 , \lambda_2 = \lambda_3 =3$. 
## Find eigenvectors of $\lambda_1 = 1$:
$$\text{Null}(A-\lambda_1 I)=\begin{bmatrix} 2 \\ 1 \\ -1 \end{bmatrix}$$
## Find eigenvectors of $\lambda_2 = \lambda_3 =3$:
$$\text{Null}(A-\lambda_2 I)= \left\{ \begin{bmatrix} -1 \\ 1 \\ 0 \end{bmatrix}  , \begin{bmatrix} -4 \\ 0 \\ 1 \end{bmatrix} \right\}$$ 
## Find $P$ 
$$
\begin{aligned}
P &= \begin{bmatrix} \vec{v_1} & \vec{v_2} & \vec{v_3} \end{bmatrix}\\
&= \begin{bmatrix} 2 & -1 & -4 \\ 1 & 1 & 0 \\ -2 & 0 & 1 \end{bmatrix}
\end{aligned}
$$
## Find $D$
$$
\begin{aligned}
D &= \begin{bmatrix} \lambda_1\\ &\lambda_2\\ &&\ddots\\ &&&\lambda_4 \end{bmatrix} \\
&= \begin{bmatrix} 1 & 0 & 0 \\ 0 & 3 & 0 \\ 0 & 0 & 3 \end{bmatrix}
\end{aligned}
$$

***
