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

# Row Operations
## Replacement/Addition
Add a multiple of one row to another.
This does $\boxed{\textbf{NOT}}$ effect the determinant.
$\boxed{\det{A}=\det{B}}$
## Interchange
Interchange two rows to make B.
One swap means, $\boxed{\det{B}=-\det{A}}$.
Two One swap means, $\boxed{\det{B}=\det{A}}$.
We can continue this pattern
## Scaling
Multiply a row by a non-zero scalar to make B.
$\boxed{\det{B}=k\det{A}}$

# [[Inverse of a Matrix|Invertibility]]
![[Determinants.png]]

# Properties
1. $\det A = \det A^T$ ([[Matrix Transpose and Powers|Transpose]]).
2. A is [[Inverse of a Matrix|invertible]] if and only if $\det A \ne 0$.
3. $\det(AB)=\det A \cdot \det B$.
4. If A is [[Inverse of a Matrix|invertible]], then $\det A^{-1} = \frac{1}{\det A}$.
# Geometric interpretation
[Watch 3b1b](https://youtu.be/Ip3X9LOh2dk?si=VfZBRWRHh1SilWGf)
<iframe width="728" height="410" src="https://www.youtube-nocookie.com/embed/Ip3X9LOh2dk?si=MQIM8sWBvjtwk2zu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
## TLDR
Area of parallelogram spanned by the columns columns of an $n \times n$ matrix $A$ is $\det \left( \begin{bmatrix} a &c\\b&d \end{bmatrix} \right)=$$ad-bc$.

The volume of the parallelepiped spanned by the columns of an $n \times n$ matrix $A$ is $|{\det A}|$.

# [[Linear Transformations]]

If we have $T: \mathbb{R}^n \rightarrow \mathbb{R}^n$, and $S$ is a parallelogram in $\mathbb{R}^n$, then:
$$
\text{volume}(T(S)) = |\det{A}| \cdot \text{volume}(S)
$$
This can be extended to higher dimentiond