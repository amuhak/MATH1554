>[!Theorem]+ SVD
>Suppose $A$ is an $m \times n$ matrix with singular values $\sigma_1 \ge \sigma_2 \ge \dots \ge \sigma_n$ and $m \ge n$. Then $A$ has the decomposition $A=U\Sigma V^T$ where,
>$$\b{D\\0_{m-n,n}} \quad \quad D=\b{\sigma_1 &0 & \dots &0 \\ 0 & \sigma_2 & \dots & 0 \\ \vdots & \vdots & \ddots & \vdots \\ 0 &0&\dots & \sigma_n}$$
>$U$ is a $m \times m$ orthogonal matrix, and $V$ is a $n \times n$ orthogonal matrix.
>If $m < n$ then $\Sigma= \b{D & 0_{m,n-m}}$ with everything else being the same.
>>[!important]- Proof
>>![[SVD.png]]
>
>>[!question]- Geometric Interpretation
>>![[SVD-1.png]]

# Computing 
Suppose $A$ is $m \times n$ and has rank $r$.
1. Compute the squared singular values of $A^TA,\sigma_i^2$, and construct $\Sigma$.
2. Compute the unit [[Singular Vectors|singular vectors]] of $A^TA, \vec{v}_i$, use them to form $V$.
3. Compute an orthonormal basis for $\text{Col}A$ using,
$$\vec{u_i}=\frac{1}{\sigma_i}A\vec{v_i}, \quad \quad i=1,2,\dots,r$$
If necessary, extend the set $\{ \vec{u_i} \}$ to form an orthonormal basis for $\mathbb{R}^m$ and use the basis to form $U$.

# Example
