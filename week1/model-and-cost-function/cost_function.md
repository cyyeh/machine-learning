# Cost Function

We can measure the accuracy of our hypothesis function by using a cost function. This takes an average difference (actually a fancier version of an average) of all the results of the hypothesis with inputs from x's and the actual output y's.

```math
J\left(\theta_{0}, \theta_{1}\right)=\frac{1}{2 m} \sum_{i=1}^{m}\left(\hat{y}_{i}-y_{i}\right)^{2}=\frac{1}{2 m} \sum_{i=1}^{m}\left(h_{\theta}\left(x_{i}\right)-y_{i}\right)^{2}
```

To break it apart, it is \frac{1}{2} x¯ where x¯ is the mean of the squares of h_\theta (x_{i}) - y_{i}, or the difference between the predicted value and the actual value.

This function is otherwise called the "Squared error function", or "Mean squared error". The mean is halved (\frac{1}{2}) as a convenience for the computation of the gradient descent, as the derivative term of the square function will cancel out the \frac{1}{2} term. The following image summarizes what the cost function does:

![cost function](../images/cost_function.png)