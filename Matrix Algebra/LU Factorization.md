# Triangular Matrices
## Upper Triangular
If $a_{i,j} = 0$ for $i>j$ 
In other words the elements below the main diagonal are 0.
Examples:
![[LU Factorization.png]]

## Lower Triangular
If $a_{i,j} = 0$ for $i<j$ 
In other words the elements above the main diagonal are 0.
Examples:
![[LU Factorization-1.png]]
***
# LU Factorization
If $A$ is an $m \times n$ matrix that can be row reduced to echelon form without row exchanges, then $A = LU$. $L$ is a lower triangular $m \times m$ matrix with 1's on the diagonal, $U$ is an echelon form of $A$.

For example the $LU$ factorization of $A \in \mathbb{R}^{3\times 2}$  would look like:

$$
A
=
LU
=
\begin{bmatrix}
1&0&0 \\ *&1&0 \\ * & * & 1
\end{bmatrix}
\begin{bmatrix}
*&* \\ 0&* \\ 0&0 
\end{bmatrix}
$$
## Algorithm
To solve $A\vec{x}=\vec{b}$  for $\vec{x}$:
1. Construct the $LU$ decomposition of $A$ to obtain $L$ and $U$.
2. Set $U\vec{x}=\vec{y}$. Forward solve for $\vec{x}$ in $L\vec{y}=\vec{b}$.
3. Backwards solve for $\vec{x}$ in $U\vec{x}=\vec{y}$.

In other words:
Get [[LU Factorization#Computing LU|LU]]
Then solve $L\vec{y}=\vec{b}$ for $\vec{y}$ 
Finally use that $\vec{y}$ to solve for $\vec{x}$ in $U\vec{x}=\vec{y}$

# Computing LU
**You are not allowed to swap rows.**
Also [[Matrix Addition and Scalar Multiplication|Scalar Multiplication]] is not needed. 
$$E_p \cdots E_1A = U$$
$E_j$ are matrices that perform elementary row operations. Because we did not swap rows, each $E_j$ happens to be lower triangular and invertible

$$
\begin{equation*} 
\begin{split}
E_p \cdots E_1A &= U \\
L E_p \cdots E_1A&= LU \\
L L^{-1} A&= LU\\
A&= LU
\end{split}
\end{equation*}
$$
$$\boxed{E_p \cdots E_1 = L^{-1} }$$
To compute the $LU$ decomposition:
1. Reduce $A$ to an echelon form $U$ by a sequence of row replacement operations, if possible.
2. Place entries in $L$ such that the same sequence of row operations reduces $L$ to $I$.

## Example
Compute the $LU$ factorization of:
$$
A=
\begin{bmatrix}
4&-3&-1&5\\
-16&12&2&-17\\
8&-6&-12&22
\end{bmatrix}
$$
Reducing it to [[Echelon Form|echelon form]] we get:
$$\boxed
{U=
\begin{bmatrix}
4&-3&-1&5\\
0&0&-2&3\\
0&0&0&-3
\end{bmatrix}}
$$
To reduce it we use the following row operations:
$$
\begin{equation*} 
\begin{split}
R_2&+\textcolor{red}{4}R_1 \\
R_3&-\textcolor{blue}{2}R_1 \\
R_3&-\textcolor{green}{5}R_2
\end{split}
\end{equation*}
$$
So $L$ will be such that the same sequence of row operations reduces $L$ to $I$.
$$\boxed
{L=
\begin{bmatrix}
1&0&0\\
\textcolor{red}{-4}&1&0\\
\textcolor{blue}{2}&\textcolor{green}{5}&1
\end{bmatrix}}
$$
