# Formulas and Theorem
***
>[!Theorem] Expansion in Orthogonal Basis
> If we have an Orthogonal Basis $\{ \vec{u}_1, \dots ,\vec{v}_n \}$  in $\mathbb{R}^n$ then for any $\vec{w} \in \mathbb{R}^n$,
> $$
> \vec{w} = c_1 \vec{u}_1+ \dots + c_n \vec{v}_n
> $$
> $C_q$ can be found using,
> $$c_q=\frac{\vec{w}\cdot\vec{u}_q}{\vec{u}_q\cdot\vec{u}_q}$$

***
>[!Theorem] Orthogonal Projection
>Let non-zero $\vec{u} \in \mathbb{R}^n$, and $\vec{y} \in \mathbb{R}^n$. The orthogonal projection of $\vec{y}$ onto $\vec{u}$ is the vector in the span of $\vec{u}$ that is closest to $\vec{y}$.
>$$
>\text{proj}_\vec{u}\vec{y}=\frac{\vec{y}\cdot\vec{u}}{\vec{u} \cdot \vec{u}}\vec{u}
>$$
>Also, $\vec{y}=\hat{y}+\vec{z}$ and, $\vec{z} \in W^\perp$

***
>[!Theorem] Best Approximation Theorem
>Let $W$ be a subspace of $\mathbb{R}^n, \vec{y}\in\mathbb{R}^n$, and $\hat{y}$ is the orthogonal projection of $\vec{y}$ onto $W$. Then for any $\vec{v}\ne\hat{y}, \vec{v} \in W$, we have 
>$$
>||\vec{y}-\hat{y}||<||\vec{y}-\vec{v}||
>$$

***
>[!Theorem] Orthogonal Decomposition Theorem
>Let $W$ be a subspace of $\mathbb{R}^n$. Then, each $\vec{y} \in \mathbb{R}^n$ has a unique decomposition.
>$$
>\vec{y}=\hat{y}+z,\quad  \hat{y}\in W ,\quad z \in W^\perp
>$$
>If $\vec{u_1}, \dots , \vec{u_n}$ is the orthogonal basis for $W$,
>$$
>\hat{y}=
>\frac{\vec{y}\cdot\vec{u_1}}{\vec{u_1}\cdot\vec{u_1}}\vec{u_1}+ \dots + \frac{\vec{y}\cdot\vec{u_n}}{\vec{u_n}\cdot\vec{u_n}}\vec{u_n}
>$$
>$\hat{y}$ is the orthogonal projection of $\vec{y}$ onto $W$

***
>[!Theorem] QR Factorization
>For a $m\times n$ matrix $A$ linearly independent columns,
>$$
>A=
>QR
>$$
>$Q$ is an $m\times n$, with columns are an orthonormal basis for $\text{Col} A$.
>$R$ is $n \times n$, upper triangular, with positive entries on its diagonal.

***
