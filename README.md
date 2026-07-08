# Regression-optimization-problem
understanding the main optimization methods
1.Ordinary least squares (OLS) regression learns the weights by minimizing MSE on training data:

2.Gradient Descent
Let f : R
k → R be a convex function and we want to find its global
minimum. This optimization algorithm is based on the fact that the fastest
decreasing direction of the function is the opposite direction of gradient:

xn+1 = xn − α∇f (xn)

and x0 ∈ R
k
is a arbitrary point.


3.Stochastic Gradient Descent
Note that in each case we can represent the loss function by the following
form:

L (w) = 1/n * sum(Li (w))

SGD algorithm is the following:
Choose an initial vector of parameters w and learning rate α.
Repeat until an approximate minimum is obtained.
Randomly shuffle examples in the training set.
For i = 1, 2, ..., n, do w ← w − α∇Li (w).
