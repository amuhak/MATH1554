Say, $A$ and $B$ are libraries with $1000$ books. 
![[Markov Chains.png]]

In the beginning, $x_0 = \begin{bmatrix} 0.5\\0.5 \end{bmatrix}$
Now, after $1$ month, $x_1=\begin{bmatrix} 0.8 \cdot 0.5+0.3 \cdot 0.5\\0.2 \cdot 0.5+0.7 \cdot 0.5 \end{bmatrix} =\begin{bmatrix} 0.8&0.3\\0.2&0.7  \end{bmatrix} \begin{bmatrix} 0.5\\0.5 \end{bmatrix}=Px_1$

Now, after $2$ month, $x_2=Px_1= Px_0 = P^2x_0$
$\vdots$
Now, after $k$ months, $x_k=P^kx_0$
