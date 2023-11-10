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
1. Construct [[QR Factorization]]
2. Solve $R\hat{x}=Q^T\vec{b}$

