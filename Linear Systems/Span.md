Given vectors $\mathbf{v_1},\mathbf{v_2}, . . . , \mathbf{v_p} \in \mathbb{R}^n$. The set of all linear combinations of $\mathbf{v_1},\mathbf{v_2}, . . . , \mathbf{v_p}$ is called the **span** of $\mathbf{v_1},\mathbf{v_2}, . . . , \mathbf{v_p}$.

Thus, $span\{\mathbf{v_1},\mathbf{v_2}, \dots, \mathbf{v_p}\}$ can be represented like this:
$$c_1\mathbf{v_1},c_2\mathbf{v_2}, . . . , c_p\mathbf{v_p}$$
Where $c_1, c_2, . . . , c_p$ are scalars.

![[Span.png]]

$$c_1  \begin{bmatrix} 1 \\ -2 \\ -3 \end{bmatrix}  + c_2  \begin{bmatrix} 2 \\ 5 \\ 6 \end{bmatrix} = \begin{bmatrix} 7 \\ 4 \\ 15 \end{bmatrix}$$
$$\begin{bmatrix} c_1   \\ -2c_1   \\ -3c_1   \end{bmatrix}  +   \begin{bmatrix} 2c_2 \\ 5c_2 \\ 6c_2 \end{bmatrix} = \begin{bmatrix} 7 \\ 4 \\ 15 \end{bmatrix}$$
$$\left[ \begin{array}{cc|c} 1 & 2 & 7 \\ -2 & 5 & 4 \\ -3 & 6 & 15 \\ \end{array} \right]$$
$$\left[ \begin{array}{cc|c} 1 & 2 & 7 \\ -2 & 5 & 4 \\ -1 & 2 & 5 \\ \end{array} \right]$$
$$\left[ \begin{array}{cc|c} 1 & 2 & 7 \\ 0 & 1 & -6 \\ -1 & 2 & 5 \\ \end{array} \right]$$
$$\left[ \begin{array}{cc|c} 1 & 2 & 7 \\ 0 & 1 & -6 \\ 0 & 1 & 3 \\ \end{array} \right]$$
$$\left[ \begin{array}{cc|c} 1 & 0 & 19 \\ 0 & 1 & -6 \\ 0 & 1 & 3 \\ \end{array} \right]$$
$$\left[ \begin{array}{cc|c} 1 & 0 & 19 \\ 0 & 1 & -6 \\ 0 & 0 & 9 \\ \end{array} \right]$$
<p style="text-align: center;">
Row<sub>3</sub>
/
9
</p>

$$\left[ \begin{array}{cc|c} 1 & 0 & 19 \\ 0 & 1 & -6 \\ 0 & 0 & 1 \\ \end{array} \right]$$

So $y$ is not in span $\{ \mathbf{v_1}, \mathbf{v_2}\}$ 
Look at [[Row Operations]]
