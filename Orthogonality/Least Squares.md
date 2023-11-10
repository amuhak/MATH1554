We want to find a line/curve that minimizes the sum of the square of the error caused due to deviation.

# Line
Say we want to find a line $y=mx+b$ that is the best fit for the following points:

| x | -1.5 | -1 | 1 | 1.5 | 2 | 
| -- | -- | -- | -- | -- | -- |
| y | -2 | -1 | 1 | 2 | 2 |  

![[Least Squares.png|200]]
We can create a list of linear equations using this:
$$
\begin{aligned}
m(-1.5)+b&=-2\\
m(-1)+b&=-1\\
m(1)+b&=1\\
m(1.5)+b&=2\\
m(2)+b&=2
\end{aligned}
$$
We can turn this in to a matrix equation like so,
$$
\begin{bmatrix}
-1.5&1\\
-1&1\\
1&1\\
1.5&1\\
2&1
\end{bmatrix}
\begin{bmatrix}
m \\
b
\end{bmatrix}
=
\begin{bmatrix}
-2 \\ -1 \\ 1 \\ 2 \\ 2
\end{bmatrix}
$$

>[!Definition] Least squares
>The least squares for $Ax=b$ is $\hat{x}$ for h=which,
>$$
>||b-A\hat{x}|| \le ||b-Ax||
>$$
>for all $x$


>[!Theorem] Normal Equation
>$$
>A^TA\hat{x}=A^T\vec{b}
>$$

