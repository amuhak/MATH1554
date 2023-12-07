A Leontif Input-Output Model is a model that describes a economy whos' parts need resources to provide resources. 

$C$ is the consumption matrix. 
Entries of $C$ are $C_{i,j}$, with $C_{i,j} \in [0, 1]$ , and
$C \vec{x} =$ units consumed
$\vec{x}-C\vec{x}=$ units left after internal consumption

$\vec{d}$ is the external demand.
$\vec{x}$ is the produced quantity.

So for an economy we can derive the formula,

$$\textcolor{green}{\text{Total production}} - \textcolor{blue}{\text{Total internal usage}} = \textcolor{red}{\text{Total external demand}}$$
$$\textcolor{green}{\vec{x}} - \textcolor{blue}{C\vec{x}} = \textcolor{red}{\vec{d}}$$

Supposes we have a economy that looks like so,
![[Leontif Input-Output Model.png|500]]
E, W, M all produce something but D only consumes.

So we know that D is our$\textcolor{red}{\text{ external demand}}$
Our $\textcolor{blue}{\text{internal usage}}$ usages are all the black arrows in the diagram.
So we need to find $\textcolor{green}{\text{total production}}$

First define $\vec{x}=\begin{bmatrix} x_e \\ x_w \\ x_m \end{bmatrix}$ 
We can construct $\textcolor{blue}{C\vec{x}}$ 

$$\textcolor{blue}{
\begin{align*}
C\vec{x}&=x_e\begin{bmatrix} 20\% \\ 10\% \\ 10\%  \end{bmatrix}+x_w\begin{bmatrix} 0\% \\ 20\% \\ 10\% \end{bmatrix}+x_m\begin{bmatrix} 0\% \\ 0\% \\ 20\% \end{bmatrix}\\
C\vec{x}&=x_e\begin{bmatrix} .2 \\ .1 \\ .1  \end{bmatrix}+x_w\begin{bmatrix} 0 \\ .2 \\ .1 \end{bmatrix}+x_m\begin{bmatrix} 0 \\ 0\\ .2 \end{bmatrix}\\
C&=\begin{bmatrix} .2 &0&0 \\ .1 &.2&0\\ .1 &.1&.2\end{bmatrix}
\end{align*}
}$$

We can construct $\textcolor{red}{\text{ external demand},\vec{d}.}$ 
$$\textcolor{red}{
\begin{bmatrix} 80 \\ 70 \\ 160 \end{bmatrix}
}
$$
Now we can put this in our formula to get $\textcolor{green}{\vec{x}}$ 

$$
\begin{align*}
\textcolor{green}{\vec{x}} - \textcolor{blue}{C\vec{x}} &= \textcolor{red}{\vec{d}}\\
(I - \textcolor{blue}{C})\textcolor{green}{\vec{x}} &= \textcolor{red}{\vec{d}}\\
\left(\begin{bmatrix} 1 &0&0\\0&1&0\\0&0&1 \end{bmatrix}-\textcolor{blue}{\begin{bmatrix} .2 &0&0 \\ .1 &.2&0\\ .1 &.1&.2\end{bmatrix}}\right) \textcolor{green}{\vec{x}} &= \textcolor{red}{\begin{bmatrix} 80 \\ 70 \\ 160 \end{bmatrix}}\\
\textcolor{green}{\vec{x}} &= \textcolor{green}{\begin{bmatrix} 100 \\ 100 \\ 225 \end{bmatrix} }
\end{align*}
$$
