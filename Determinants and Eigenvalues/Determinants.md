A general way to compute it is,
If If $A$ is an $n \times n$ matrix where $n=1$,
$$\det(A) = a_{1,1}$$
If $A$ is an $n \times n$ matrix where $n>1$,
$$\det(A) = a_{1,1}\det \left(A_{1,1}\right) - a_{1,2}\det \left(A_{1,2}\right) + \dots + \left( -1\right)^{n+1}a_{1,n}\det \left(A_{1,n}\right)$$
$a_{i,j}$ means the element at the $i^{\text{th}}$ row and the $j^{\text{th}}$ column.
$A_{i,j}$ means the Matrix if you drop (get rid of) the $i^{\text{th}}$ row and the $j^{\text{th}}$ column.

Deriving it for a $2 \times 2$
Say we have $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$ 

$$
\begin{aligned}
\det(A)&=(a_{1,1})(\det \left(A_{1,1}\right)) - (a_{1,2})(\det \left(A_{1,2}\right))\\
\det(A)&=(a)\left(d\right) - (b)\left(c\right)\\
\det(A)&=ad-bc
\end{aligned}$$

# Using a [[Cofactors|Cofactor]]
The determinant of a matrix $A$ can be computed down any row or column of the matrix.

For example, down the $j^{\text{th}}$ column the determinant is:
$$
\det(A)=a_{1,j}\det \left(A_{1,j}\right) - a_{2,j}\det \left(A_{2,j}\right) + \dots + \left( -1\right)^{n+1}a_{n,j}\det \left(A_{n,j}\right)
$$
This would be useful for a matrix with a few 0's.
Say $A=\begin{bmatrix}5&4&3&2\\0&1&2&0\\0&-1&1&0\\0&1&1&3\end{bmatrix}$ find $\det(A)$ 
$$
\begin{aligned}
A&=
\begin{bmatrix}
5&4&3&2\\
0&1&2&0\\
0&-1&1&0\\
0&1&1&3
\end{bmatrix}
\end{aligned}
$$![[Determinants.png]]