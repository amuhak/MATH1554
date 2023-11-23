>[!Theorem]+ 
>Suppose $\vec{v}_i$ are the $n$ orthogonal eigenvectors of $A^TA$, ordered so that their corresponding eigenvalues satisfy $\lambda_1 \ge \lambda_2 \dots \ge \lambda_n$. Suppose also that $A$ has $r$ non-zero singular values, $r \le n$. Then the set of vectors,
>$$\{ \vec{v}_{r+1},\vec{v}_{r+2},\dots,\vec{v}_{n} \}$$
>is an orthogonal basis for $\text{Nul}A$, and the set
>$$\{ \vec{v_1},\vec{v_2},\dots,\vec{v_r} \}$$
>is an orthogonal basis for $\text{Row}A$, and $\text{Rank}A = r$.
>>[!important]- Proof
>>![[Singular Vectors.png]]
>>
>>![[Singular Vectors-1.png]]

Using the same assumptions as above, it can be shown that,
$$\{ A\vec{v_1},A\vec{v_2},\dots,A\vec{v_r} \}$$
is an orthogonal basis for $\text{Col}A.$
>[!important]- Proof
>![[Singular Vectors-2.png]]


![[Singular Vectors-3.png]]![[Singular Vectors-4.png]]
- Right Singular Vectors are the eigenvectors of $A^TA$ 
- Left Singular Vectors are the basis for $\text{Col}A$
