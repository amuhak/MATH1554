# An example
We have a unit sphere $1=x_1^2+x_2^2+x_3^2=||x||^2$. We wish to optimize $Q=9x_1^2+4x_2^2+3x_3^2$. To find the largest and smallest value of $Q$. It can be graphed as follows: 
![[Constrained Optimization.png|300]]
We wish to maximize $Q$. 
$Q=9x_1^2+4x_2^2+3x_3^2=\vec{x}^T \begin{bmatrix} 9 &0 &0 \\ 0 &4&0 \\ 0&0&3 \end{bmatrix} \vec{x}$ .
$$
\begin{aligned}
&\le 9x_1^2+9x_2^2+9x_3^2 \\
&= 9(x_1^2+x_2^2+x_3^2) \\
&= 9 ||\vec{x}||^2 \\
&= 9
\end{aligned}
$$
Note: $||\vec{x}||^2=1$ because that is what we stated in the problem.
So the max value of $Q$ is