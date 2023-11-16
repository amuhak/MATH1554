>[!Theorem]+ Eigenvectors orthogonality 
>If $A$ is a symmetric matrix, with eigenvectors $\vec{v_1}$ and $\vec{v_2}$ corresponding to two distinct eigenvalues, then $\vec{v_1}$ and $\vec{v_2}$ are orthogonal.
>>[!important]- Proof
>>![[Orthogonal Diagonalization-1.png]]

# Example $PDP^T$
![[Orthogonal Diagonalization-2.png]]
We need to find the [[Eigen Things#Eigenspaces|Eigenvectors]] of $A$.
Skipping the computation, we get,
$$
\begin{aligned}
\vec{v_1}&=\begin{bmatrix} 1 \\ 0 \\ -1 \end{bmatrix}, \lambda=-1\\
\vec{v_2}&=\begin{bmatrix} 0 \\ 1 \\ 0  \end{bmatrix}, \lambda=1\\
\vec{v_3}&=\begin{bmatrix} 1 \\ 0 \\ 1 \end{bmatrix},  \lambda=1
\end{aligned}
$$
Now we must find $PDP^T$,
The columns of $P$ are the **orthonormalized** Eigenvectors, and $D$ is the eigenvalue.
$$
\begin{aligned}
P&=\begin{bmatrix} 
\frac{1}{\sqrt{2}}&0&\frac{1}{\sqrt{2}}\\
0&1&0\\
\frac{-1}{\sqrt{2}}&0&\frac{1}{\sqrt{2}}
\end{bmatrix}\\
D&=\begin{bmatrix} 
-1&0&0\\
0&1&0\\
0&0&1
\end{bmatrix}\\
\end{aligned}
$$
Finding $P^T$ is trivial and left to the reader. 