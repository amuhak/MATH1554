>[!Theorem]+ Principle Axes Theorem
>If $A$ is a symmetric matrix then there exists an orthogonal change of variable $\vec{x}=P\vec{y}$ that transforms $\vec{x}^TA\vec{x}$ to $\vec{y}^TD\vec{y}$ with no cross-product terms.
>>[!important]- Proof
>>![[Change of Variable.png]]

To express this idea more clearly, what we are doing is changing variables from $x_1,x_2,\dots,x_n$ to $y_1,y_2,\dots,y_n$. We will define this using equations discussed later. Our motivation to do this is to remove the cross product term, so that equation is easier to understand. 
Here is the equation relating $\vec{x}$ and $\vec{y}$, 
$$
\vec{x} = P\vec{y} \quad \quad \quad\quad  \quad \quad \quad \vec{y} = P^{-1} \vec{x}
$$
Now remember that we are apply this to matrix $Q$ which is the [[Quadratic Forms|quadratic form]] of an equation. Also recall that $Q=\vec{x}^TA\vec{x}$, where matrix $A$ is [[Symmetric Matrices|symmetric]]. 