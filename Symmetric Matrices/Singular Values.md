The singular values of any $m \times n$ real matrix $A$ are the square roots of the eigenvalues of $A^TA$.
***
Say we want to find a $v$ that maximizes $||A\vec{v}||$ Where $||\vec{v}||=1$ 
This is the same thing as maximizing $||A\vec{v}||^2$, so we have
$$
\begin{aligned}
||A\vec{v}||^2 &= \vec{v}^TA^TA\vec{v}\\

\end{aligned}
$$
$A^TA$ is always [[Symmetric Matrices|symmetric]]. After acknowledging that we can realizes that is a [[Constrained Optimization]] problem. $||\vec{v}||=1$ being the constraint. 
We will simply use the largest eigenvalue of $A^TA$ to find the largest value for $||A\vec{v}||^2$. The location of this will simply be the corresponding normalized eigenvector. 

The min value can be found using a similar method. 

Calling singular values $\sigma_1 \ge \sigma_2 \ge \dots \ge \sigma_n$ we can say that the $\sigma_1$ is the max value of $||A\vec{v}||$ and $\sigma_n$ is the min value.

>[!Theorem]+ Non-Negative Eigenvalues
>The eigenvalues of $A^TA$ are non-negative.
>>[!important]- Proof
>>![[Singular Values.png]]

From the above Proof we can see, $$||A\vec{v}||^2=\lambda_i$$ And hence, $$||A\vec{v}||=\sigma_i$$
