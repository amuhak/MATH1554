Translations of points in $\mathbb{R}^n$ does not correspond directly to a linear transform. Homogeneous coordinates are used to model translations using matrix multiplication. 

### Homogeneous Coordinates in $\mathbb{R}^2$
Each point $(x, y)$ in $\mathbb{R}^2$ can be identified with the point $(x, y, H)$, $H \neq 0$, on the plane in $\mathbb{R}3$ that lies $H$ units above the $xy$-plane.

$(x,y) \rightarrow (x+h,y+k)$ can be represented by, 
![[Homogeneous Coordinates.png|500]]

Now rotate a triangle ($(1,1),(2,4),(3,1)$) by $\frac{\pi}{2}$ radians counterclockwise about the point $(0,1)$.
$$
\begin{aligned}
d&=
\begin{bmatrix}
1&2&3\\
1&4&1\\
1&1&1
\end{bmatrix}\\
\text{Shift up by 1},\\
\begin{bmatrix}
1&0&0\\
0&1&-1\\
0&0&1
\end{bmatrix}d&=
\begin{bmatrix}
1&2&3\\
0&3&0\\
1&1&1
\end{bmatrix}\\

\end{aligned}
$$
