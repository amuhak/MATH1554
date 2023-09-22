Imagine a matrix A,
$$A=\begin{bmatrix} 1&0&0&5\\0&1&0&6\\0&0&1&6\\7&9&1&6\end{bmatrix}$$
Partitioned it could look like this,
$$\begin{aligned}
A&= \begin{bmatrix} \begin{bmatrix} 1&0&0\\0&1&0\\0&0&1 \end{bmatrix} &\begin{bmatrix} 5\\6\\6 \end{bmatrix} \\\begin{bmatrix} 7&9&1 \end{bmatrix} & \begin{bmatrix} 6 \end{bmatrix} \end{bmatrix} \\
&=\begin{bmatrix}  I_3 & U \\ V & X \end{bmatrix}
\end{aligned}
$$
We can even perform matrix multiplication,
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

