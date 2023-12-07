We can compute the average, $\bar{x}$, of the $x$-values, and introduce a new variable ${x}_*=x-\bar{x}$.

|x|2|5|7|8|
|-|-|-|-|-|
|y|1|1|4|3|

We can set $y=c_0-c_1x_*$ 
$$
\begin{bmatrix}
1&-3.5\\
1&-0.5\\
1&1.5\\
1&2.5\\
\end{bmatrix}
\begin{bmatrix}
c_0\\c_1
\end{bmatrix}=
\begin{bmatrix}
1\\1\\4\\3
\end{bmatrix}
$$
Notice that the columns are Orthogonal. Hence, $A^TA$ is diagonal.
Now we can solve this normal using the normal equation.
