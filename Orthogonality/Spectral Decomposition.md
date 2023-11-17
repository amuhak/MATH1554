If $A$ can be decomposed like so ([[Orthogonal Diagonalization#Example $PDP T$|PDP^T]]),
$$
\begin{aligned}
A&=PDP^{T}\\
A&=\begin{bmatrix} v_1&v_2\dots&v_n \end{bmatrix} \begin{bmatrix} \lambda_1\\ &\lambda_2\\ &&\ddots\\ &&&\lambda_n \end{bmatrix} \begin{bmatrix} v_1\\v_2\\\vdots\\v_n \end{bmatrix}
\end{aligned}
$$
Then, $A$ has the following decomposition:
$$
A= 
\lambda_1\vec{u_1}\vec{u_1}^T+\dots+\lambda_n\vec{u_n}\vec{u_n}^T=\sum_{i=1}^n{\lambda_i\vec{u_i}\vec{u_i}^T}
$$
We must notice that $\vec{u_i}\vec{u_i}^T$ is an $n \times n$ matrix, assuming that $\vec{u_i}$ is $n \times 1$.
> [!Important]- Proof
> We see that $PD = \begin{bmatrix} Pd_1 & Pd_2 & \dots & Pd_i \end{bmatrix}$
> $d_i$ are columns of $D$
> We need to realize that that, $Pd_i= P\begin{bmatrix} 0 \\ \vdots \\ 0 \\ \lambda_i \\ 0 \\ \vdots \\ 0 \end{bmatrix}= 0+ \dots + 0 + p_i\lambda_i + 0 \dots + 0 =p_i\lambda_i$. 
> Hence $PD = \begin{bmatrix} p_1\lambda_1 & p_2\lambda_2 & \dots &  p_1\lambda_1 \end{bmatrix}$
> So, $PDP^T = \begin{bmatrix} p_1\lambda_1 & p_2\lambda_2 & \dots & p_1\lambda_1 \end{bmatrix} \begin{bmatrix} u_1^T \\ u_2^T \\ \vdots \\ u_i^T \end{bmatrix} =A$
> Using math we can conclude, 
> $$\boxed{A=\lambda_1\vec{u_1}\vec{u_1}^T+\lambda_2\vec{u_2}\vec{u_2}^T+\dots+\lambda_n\vec{u_n}\vec{u_n}^T=\sum_{i=1}^n{\lambda_i\vec{u_i}\vec{u_i}^T}} $$

# Example
![[Spectral Decomposition.png]]

# Properties
- $\lambda_n\vec{u_n}\vec{u_n}^T$ will be $n \times n$ and have a Rank of 1.
>[!extra] Aproximation
>![[Spectral Decomposition-1.png]]

