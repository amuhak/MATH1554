>[!Theorem]+ Principle Axes Theorem
>If $A$ is a symmetric matrix then there exists an orthogonal change of variable $\vec{x}=P\vec{y}$ that transforms $\vec{x}^TA\vec{x}$ to $\vec{y}^TD\vec{y}$ with no cross-product terms.
>>[!important]- Proof
>>![[Change of Variable.png]]

To express this (the theorem) more clearly, what we are doing is changing variables from $x_1,x_2,\dots,x_n$ to $y_1,y_2,\dots,y_n$. We will define this using equations discussed later. Our motivation to do this is to remove the cross product term, so that equation is easier to understand. 
Here is the equation relating $\vec{x}$ and $\vec{y}$ that I promised earlier, 
$$
\vec{x} = P\vec{y} \quad \quad \quad\quad  \quad \quad \quad \vec{y} = P^{-1} \vec{x}
$$
Now remember that we are apply this to matrix $Q$ which is the [[Quadratic Forms|quadratic form]] of an equation. Also recall that $Q=\vec{x}^TA\vec{x}$, where matrix $A$ is [[Symmetric Matrices|symmetric]]. Because of this property of $A$ we can create an [[Orthogonal Diagonalization|orthogonal diagonalization]] of $A$ where $A=PDP^T$, $D$ is [[Diagonal Matrices|diagonal]], and $P$ is an [[Orthogonal Matrices|orthonormal matrix]], so $P^{-1}=P^T$ Now we can do some math,
$$
\begin{align*}
Q&=\vec{x}^TA\vec{x}\\
Q&=\vec{x}^TPDP^T\vec{x}\\
Q&=\vec{x}^TPD\vec{y}\\
Q&=\vec{x}^T(P^T)^TD\vec{y}\\
Q&=(P^T\vec{x})^TD\vec{y}\\
Q&=(P^{-1}\vec{x})^TD\vec{y}\\
Q&={(\vec{y})^TD\vec{y}}\\
Q&=\vec{y}^TD\vec{y}
\end{align*}
$$
Now we have successful expressed $Q$ in terms of $\vec{y}$ instead of $\vec{x}$, and more importantly the middle matrix is $D$. Remember $D$ is a diagonal matrix, hence $\vec{y}^TD\vec{y}$ will **not** have any no cross product terms. Don't believe me? Well just multiply any diagonal matrix $D$ with a correspondingly sized $\vec{y}$.


