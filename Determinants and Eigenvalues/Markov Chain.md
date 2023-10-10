Say, $A$ and $B$ are libraries with $1000$ books. 
![[Markov Chains.png]]

In the beginning, $x_0 = \begin{bmatrix} 0.5\\0.5 \end{bmatrix}$
Now, after $1$ month, $x_1=\begin{bmatrix} 0.8 \cdot 0.5+0.3 \cdot 0.5\\0.2 \cdot 0.5+0.7 \cdot 0.5 \end{bmatrix} =\begin{bmatrix} 0.8&0.3\\0.2&0.7  \end{bmatrix} \begin{bmatrix} 0.5\\0.5 \end{bmatrix}=Px_1$

$$
\boxed{
P=
\begin{bmatrix} 0.8&0.3\\0.2&0.7  \end{bmatrix}
}
$$
Now, after $2$ month, $x_2=Px_1= Px_0 = P^2x_0$
$\vdots$
Now, after $k$ months, $x_k=P^kx_0$

# Steady State
Find the steady state of $P=\begin{bmatrix} 0.8&0.3\\0.2&0.7  \end{bmatrix}$.
$$
\begin{aligned}
P\vec{q}&=\vec{q}\\
P\vec{q}-\vec{q}&=0\\
P\vec{q}-I_n\vec{q}&=0\\
(P-I_n)\vec{q}&=0\\
\left( \begin{bmatrix} 0.8&0.3\\0.2&0.7  \end{bmatrix} - \begin{bmatrix} 1&0\\0&1  \end{bmatrix}\right)\vec{q}&=0\\
\begin{bmatrix} 0.2&-0.3\\-0.2&0.3  \end{bmatrix}\vec{q}&=0\\
\begin{cases}
2x_1&-3x_2&=0\\
-2x_1&+3x_2&=0\\
\end{cases}\\
\{x_1=3,x_2&=2\}\\
\frac{1}{3+2}\begin{bmatrix} 3 \\2 \end{bmatrix}&=\vec{q}\\
\vec{q}&=\boxed{\begin{bmatrix} \frac{3}{5} \\ \frac{2}{5} \end{bmatrix}}
\end{aligned}
$$
# Convergence
We have $x_1, x_2,x_3,\dots x_k$. We want to know if while $k \rightarrow \infty$ $x_k$ will converge to a steady state.

If $P$ is a regular stochastic matrix ([[Vocabulary|vocabulary]]), then $P$ has a unique steady-state vector $\vec{q}$, and $\vec{x}_{k+1}=P\vec{x}_k$ converges to $\vec{q}$ as $k \rightarrow \infty$  