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

