$$
\begin{equation} T: R^n \to R^m \text{ is linear if } \begin{cases} T(u + v) &= T(u) + T(v) \\ T(cv) &= cT(v) \end{cases} \end{equation}
$$

Create a $2\times2$ matrix $A$ that applies a linear transformation that rotates by an angle $\theta$ counterclockwise 

$$
\begin{align*}
A &=[\vec{a_1},\vec{a_2}] \\
T(\vec{e_1}) &= \vec{a_1} \\
T(\vec{e_1}) &= \begin{bmatrix} a \\ b \end{bmatrix} &= \begin{bmatrix}\cos{ \theta} \\ \sin{ \theta} \end{bmatrix} \\
\vec{a_1} &= \begin{bmatrix}\cos{ \theta} \\ \sin{ \theta} \end{bmatrix} \\
T(\vec{e_2}) &= \vec{a_2} \\
T(\vec{e_2}) &= \begin{bmatrix} a \\ b \end{bmatrix} &= \begin{bmatrix} -\sin{ \theta} \\ \cos{ \theta}\end{bmatrix} \\
\vec{a_2} &= \begin{bmatrix} -\sin{ \theta} \\ \cos{ \theta}\end{bmatrix} \\
\end{align*}
$$
$$
\boxed 
{A = \begin{bmatrix} \cos{ \theta} & -\sin{ \theta} \\ \sin{ \theta}  & \cos{ \theta} \end{bmatrix}}
$$

