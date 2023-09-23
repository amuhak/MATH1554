Imagine a matrix A,
$$A=\begin{bmatrix} 1&0&0&5\\0&1&0&6\\0&0&1&6\\7&9&1&6\end{bmatrix}$$
Partitioned it could look like this,
$$\begin{aligned}
A&= \begin{bmatrix} \begin{bmatrix} 1&0&0\\0&1&0\\0&0&1 \end{bmatrix} &\begin{bmatrix} 5\\6\\6 \end{bmatrix} \\\begin{bmatrix} 7&9&1 \end{bmatrix} & \begin{bmatrix} 6 \end{bmatrix} \end{bmatrix} \\
&=\begin{bmatrix}  I_3 & U \\ V & X \end{bmatrix}
\end{aligned}
$$
We can even perform [[Matrix Multiplication|matrix multiplication]],
$$\begin{bmatrix} 1&0&1\\0&1&1 \end{bmatrix} \begin{bmatrix} 2&-1\\0&-1\\0&1 \end{bmatrix}$$
$$
\begin{aligned}
&=\begin{bmatrix}  I_2 &X \end{bmatrix}\begin{bmatrix} U \\ V \end{bmatrix} \\
&=I_2U+XY\\
&=\begin{bmatrix} 2 & -1 \\0&-1 \end{bmatrix} + \begin{bmatrix} 1 \\1 \end{bmatrix} \begin{bmatrix} 0&1 \end{bmatrix}\\
&=\begin{bmatrix} 2 & -1 \\0&-1 \end{bmatrix} +\begin{bmatrix} 0&1\\0&1 \end{bmatrix}\\
&=\begin{bmatrix} 2 & 0 \\ 0 & 0 \end{bmatrix}
\end{aligned}
$$

# [[Inverse of a Matrix|Find the Inverse]]
Compute equations the inverse $\begin{bmatrix} A & B \\ 0 & C \end{bmatrix}$.

$$
\begin{bmatrix} A & B \\ 0 & C \end{bmatrix}\begin{bmatrix} W & X \\ Y & Z \end{bmatrix}=I=\begin{bmatrix} I_n & 0 \\ 0 & I_n \end{bmatrix}
$$
$$
\begin{equation*} 
\begin{split}
0W+CY&=0 \\
CY&=0 \\
C^{-1}CY&=C^{-1}0 \\
Y&=0
\end{split}
\end{equation*}
$$
$$
\begin{equation*} 
\begin{split}
0X+CZ&=I_n\\
C^{-1}CZ&=C^{-1}I_n\\
Z&=C^{-1}
\end{split}
\end{equation*}
$$
$\text{We know } Y=0 \text{ as it was calculated above}$
$$
\begin{equation*} 
\begin{split}
AW+BY&=I_n\\
AW+B0&=I_n \\
A^{-1}AW&=A^{-1}I_n\\
W&=A^{-1}
\end{split}
\end{equation*}
$$
$$
\begin{equation*} 
\begin{split}
AX+BZ&=0\\
A^{-1}AX&=-A^{-1}BZ\\
X&=-A^{-1}BZ\\
X&=-A^{-1}BC^{-1}
\end{split}
\end{equation*}
$$
So, putting this back into a matrix:
$$
\begin{bmatrix} A & B \\ 0 & C \end{bmatrix}^{-1}=
\boxed
{
\begin{bmatrix}
A^{-1}&-A^{-1}BC^{-1}\\
0&C^{-1}
\end{bmatrix}
}
$$

