# Analytical_Solution_Linear_Regression

Short Jupyter Notebook demonstrating the analytical solution for linear regression.

Given a family of regression models, the least squares solution is the model that minimises the mean squared error on our training dataset. Consider the folowing **multiple linear model**:

$\begin{equation}
f(x) = w_0 + w_1 x_1 + ... + w_K x_K
\end{equation}$

where $x_1, ..., x_K$ are the predictors and $w_0, ..., w_K$ are the model's parameters. If we have a dataset consisting of $N$ samples, we can obtain the parameters of the least squares solution using the **normal equations** 

$\begin{equation}
\mathbf{w} = (\mathbf{X}^T\mathbf{X})^{-1}\mathbf{X}^T\mathbf{y}
\end{equation}$

where $\mathbf{w}=[w_1, ... , w_K]^T$ are the parameters of the model, $\mathbf{y}=[y_0, ..., y_N]^T$ are the true labels in the dataset and $\mathbf{X}$ is the design matrix. The least squares solution for **simple polynomial regression** can be obtained following an identical approach. Given a polynomial model

$\begin{equation}
f(x) = w_0 + w_1 x + ... + w_K x^K
\end{equation}$

we can treat $x, x^2, ..., x^K$ as separate predictors, build the corresponding design matrix $\mathbf{X}$ and use the normal equation.
