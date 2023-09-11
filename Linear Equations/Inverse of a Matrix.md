$A \in \mathbb{R}^{n \times n}$ is invertible if there is a $C \in \mathbb{R}^{n \times n}$ so that:

$$AC=CA=I_n$$
If so we write, $C=A^{-1}$
# For a $2 \times 2$ 
## Compute
$$ \begin{bmatrix} a &b \\ c&d \end{bmatrix}^{-1} = \frac{1}{ad-bc} \begin{bmatrix} d &-b \\ -c&a \end{bmatrix} $$
## Use it to solve a Linear systems
$$
\begin{aligned}
A\vec{x}&=b \\ 
A^{-1}A\vec{x}&=A^{-1}b \\
I\vec{x}&=A^{-1}b \\
\vec{x}&=A^{-1}b
\end{aligned}
$$

