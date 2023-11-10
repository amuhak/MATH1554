This is closely related to [[Least Squares]]
![[Deviation.png]]
The red lines are the deviation/error/residuals in approximation.

We were finding an $\hat{x}$ to minimize $||A\hat{x}-b||$.
This is the same thing as minimizing $||A\hat{x}-b||^2$.
Now, over all $\hat{x}$,
$$
||A\hat{x}-b||^2= ||r||^2= \sum_{i=1}^{n}{r_i^2}
$$
So basically we are trying to minimize the square of the residual. 
