# An example when $||x||=1$
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
So the max value of $Q$ is 1.
More accurately, $\text{max}\{Q(\vec{c}) : ||\vec{x}|| = 1 \} = 9,$ and max occurs at $\vec{x} = \begin{bmatrix} \pm 1 \\ 0 \\ 0 \end{bmatrix}$.
If we minimize $Q$, $\text{min}\{Q(\vec{c}) : ||\vec{x}|| = 1 \} = 3,$ and min occurs at $\vec{x} = \begin{bmatrix} 0 \\ 0 \\ \pm 1 \end{bmatrix}$.
Notice that the minimum and maximum values of $Q$ were the eigenvalues of $A$, and the corresponding eigenvectors gave their locations.

>[!Theorem]+ Constrained Optimization
>If $Q=x^TAx$, $A$ is a real $n \times n$ symmetric matrix, with eigenvalues
>$$\lambda_1 \ge \lambda_2 \dots \ge \lambda_n $$
>and associated normalized eigenvectors
>$$ u_1,u_2,\dots,u_n$$
>Also, $||x||=1$
>Then max value of $Q(x)=\lambda_1$ attained at $\pm u_1$
>Then min value of $Q(x)=\lambda_n$ attained at $\pm u_n$
>>[!important]- Proof
>>![[Constrained Optimization-1.png]]


# Repeated Eigenvalue
If we have repeated eigenvalues then, the min and max values are found using the same prosses. The locations are the span of all the eigenvectors of the corresponding min or max eigenvalue.


