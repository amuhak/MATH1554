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
We will use the first column due to the 3 zeros.
$$
\begin{aligned}
\det(A)&=5C_{1,1}+0C_{2,1}+0C_{3,1}+0C_{4,1}\\
&=5\cdot(-1)^{1+1}\cdot \det \left(
\begin{bmatrix}
1&2&0\\
-1&1&0\\
1&1&3
\end{bmatrix}
\right)\\
3^{\text{rd}}\text{ column}\\
&=5\cdot
\left(
0C_{1,3}+0C_{2,3}+3C_{3,3}
\right)\\
&=5\cdot
\left(
3\cdot(-1)^{3+3}
\det
\left(
\begin{bmatrix}
1&2\\-1&1
\end{bmatrix}
\right)
\right)\\
\text{Formula}\\
&=5(3(1\times1-2\times-1))\\
&=\boxed{45}
\end{aligned} 
$$
# Triangular Matrices
The determinant of a triangular matrix is the product of the entries on the main diagonal.

