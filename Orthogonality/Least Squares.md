We want to find a line/curve that minimizes the sum of the square of the error caused due to deviation.

>[!Definition]+ Least squares
>The least squares for $Ax=b$ is $\hat{x}$ for which,
>$$
>||b-A\hat{x}|| \le ||b-Ax||
>$$
>for all ${x}$

We can use the normal equation to solve for $\hat{x}$
>[!Theorem]+ Normal Equation
>$$
>A^TA\hat{x}=A^T\vec{b}
>$$
>Manipulating this we can get this,
>$$
>\hat{x}=(A^TA)^{-1}A^T\vec{b}
>$$
>>[!IMPORTANT]+ Proof
>>![[Least Squares-1.png]]


>[!Theorem]+ Using [[QR Factorization]]
>$$
>R\hat{x}=Q^T\vec{b}
>$$
>>[!IMPORTANT]+ Proof
>>$$
>>\begin{aligned}
>>A^TA\hat{x}&=A^T \vec{b} \\
>>(QR)^TQR\hat{x}&=(QR)^T \vec{b}\\
>>R^TQ^TQR\hat{x}&=R^TQ^T\vec{b}\\
>>R^TR\hat{x}&=R^TQ^T\vec{b}\\
>>R\hat{x}&=Q^T\vec{b}
>>\end{aligned}
>>$$

## How to solve
### Method 1
1. Construct [[QR Factorization]]
2. Solve $R\hat{x}=Q^T\vec{b}$
### Method 2
1. Solve the normal equation for $\hat{x}$.

### Method 3
1. [[Mean-Deviation Form|Use Mean Deviation]]

# Line
Say we want to find a line $y=mx+b$ that is the best fit for the following points:

| x | -2 | -1 | 1 | 1 | 2 | 
| -- | -- | -- | -- | -- | -- |
| y | -2 | -1 | 1 | 2 | 2 |  

![[Least Squares.png|200]]
We can create a list of linear equations using this:
$$
\begin{aligned}
m(-2)+b&=-2\\
m(-1)+b&=-1\\
m(1)+b&=1\\
m(1)+b&=2\\
m(2)+b&=2
\end{aligned}
$$
We can turn this in to a matrix equation like so,
$$A\vec{x}=\vec{b}$$
$$
\begin{bmatrix}
1&-2\\
1&-1\\
1&1\\
1&1\\
1&2
\end{bmatrix}
\begin{bmatrix}
b \\
m
\end{bmatrix}
=
\begin{bmatrix}
-2 \\ -1 \\ 1 \\ 2 \\ 2
\end{bmatrix}
$$
Compute QR, 
$$
\begin{bmatrix}
\frac{1}{\sqrt{5}} & -\frac{2}{\sqrt{10}} \\
\frac{1}{\sqrt{5}} & -\frac{1}{\sqrt{10}} \\
\frac{1}{\sqrt{5}} & 0 \\
\frac{1}{\sqrt{5}} & \frac{1}{\sqrt{10}} \\
\frac{1}{\sqrt{5}} & \frac{2}{\sqrt{10}} \\
\end{bmatrix}
\begin{bmatrix}
\frac{5}{\sqrt{5}} & 0\\
0 & \frac{10}{\sqrt{10}}
\end{bmatrix}
$$
Now compute $Q^T\vec{b}$,
$$Q^T\vec{b}=\begin{bmatrix} \frac{2}{\sqrt{5}}\\\frac{11}{\sqrt{10}} \end{bmatrix}$$
Finally solve $R\hat{x}=Q^T\vec{b}$,
$$
\begin{bmatrix}
\frac{5}{\sqrt{5}} & 0\\
0 & \frac{10}{\sqrt{10}}
\end{bmatrix} \hat{x} = 
\begin{bmatrix} \frac{2}{\sqrt{5}}\\\frac{11}{\sqrt{10}} \end{bmatrix}
$$
$$
\hat{x} = \boxed{
\begin{bmatrix}
\frac{2}{5} \\
\frac{11}{10} 
\end{bmatrix}
}
$$
So we get $\boxed{y=\dfrac{2}{5}+\dfrac{11}{10}x}$

# Curves
We can use this method to fit data to a curve using the function,
$$
y=c_0+c_1f_1(x)+c_2f_2(x)+\dots+c_nf_n(x)
$$
Lets take an example, 
Say we want to modal:

| x | -1 | 0 | 0 | 1 | 
| -- | -- | -- | -- | -- |
| y | 2 | 1 | 0 | 6 |

Using $y=c_1x+c_2x^2$
$$
\begin{aligned}
-c_1+c_2&=2\\
0c_1+0c_2&=1\\
0c_1+0c_2&=0\\
c_1+c_2&=6
\end{aligned}
$$
Now we can use [[Least Squares#How to solve|one of the methods]] to solve for $c_1\text{ and } c_2$ 