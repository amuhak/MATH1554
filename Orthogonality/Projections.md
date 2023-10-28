We have a subspace $W$ (the span of $\vec{u}$), and we want to find the vector ($\hat{y}$) closest to $\vec{y}$ in $W$.
We also want to find $\vec{z} \in W^\perp$ such that $\vec{y}=\hat{y}+\vec{z}$. 
Diagrammatically, 
![[Projections.png]]
We know $\vec{z} \in W^\perp$, so:
$$\vec{z} \cdot \vec{u}=0$$
We also know $\vec{y}=\hat{y}+\vec{z}$ and $\hat{y}=k\vec{u}$ ($k\in \mathbb{R}$), so:
$$
\begin{aligned} 
\vec{z}&=\vec{y}-k\vec{u}\\
0 &=(\vec{y}-k\vec{u}) \cdot \vec{u}\\
&=\vec{y}\cdot \vec{u}-k\vec{u} \cdot \vec{u}\\
k&=\frac{\vec{y}\cdot\vec{u}}{\vec{u} \cdot \vec{u}},& \vec{u} \ne\vec{0}\\
\end{aligned}
$$
So finely, $\hat{y}=\frac{\vec{y}\cdot\vec{u}}{\vec{u} \cdot \vec{u}}\vec{u}$ 
>[!Theorem] Orthogonal Projection
>Let non-zero $\vec{u} \in \mathbb{R}^n$, and $\vec{y} \in \mathbb{R}^n$. The orthogonal projection of $\vec{y}$ onto $\vec{u}$ is the vector in the span of $\vec{u}$ that is closest to $\vec{y}$.
>$$
>\text{proj}_\vec{u}\vec{y}=\frac{\vec{y}\cdot\vec{u}}{\vec{u} \cdot \vec{u}}\vec{u}
>$$

