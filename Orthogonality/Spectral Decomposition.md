If $A$ can be decomposed like so ([[Orthogonal Diagonalization#Example $PDP T$|PDP^T]]),
$$
\begin{aligned}
A&=PDP^{T}\\
A&=\begin{bmatrix} v_1&v_2\dots&v_n \end{bmatrix} \begin{bmatrix} \lambda_1\\ &\lambda_2\\ &&\ddots\\ &&&\lambda_n \end{bmatrix} \begin{bmatrix} v_1\\v_2\\\vdots\\v_n \end{bmatrix}
\end{aligned}
$$Then, $A$ has the following decomposition:
$$
A= 
\lambda_1\vec{u_1}\vec{u_1}^T+\dots+\lambda_n\vec{u_n}\vec{u_n}^T=\sum_{i=1}^n{\lambda_i\vec{u_i}\vec{u_i}^T}
$$
We must notice that $\vec{u_i}\vec{u_i}^T$ is an $n \times n$ matrix, assuming that $\vec{u_i}$ is $n \times 1$.
> [!Important]+ Proof
> We see that $PD = \begin{bmatrix} Pd_1 & Pd_2 & \dots & Pd_1 \end{bmatrix}$

