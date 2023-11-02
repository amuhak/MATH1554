# Orthonormal Basis
If vectors have unit lengths they are orthonormal. 

To find the orthonormal basis of $\vec{v}$, $\hat{v}$ 
$$
\hat{v} =
\frac{1}{{||\vec{v}||}} \vec{v}
$$
***
>[!Theorem] QR Factorization
>For a $m\times n$ matrix $A$ linearly independent columns,
>$$
>A=
>QR
>$$
>$Q$ is an $m\times n$, with columns are an orthonormal basis for $\text{Col} A$.
>$R$ is $n \times n$, upper triangular, with positive entries on its diagonal.


We can get $Q$ using the Gram-Schmidt process.
To find $R$, we can us $R=Q^TA$ due to $Q^TQ=I$

# Properties 
$\text{ Length of the } j^{th} \text{ column of }R = \text{ length of the } j^{th} \text{ column of } A$
