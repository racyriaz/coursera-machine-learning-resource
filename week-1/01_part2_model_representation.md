# Model Representation

1. To establish notations we will make use of  $x^{(i)}$ to denote the **input variable** a.k.a *input features* and $y^{(i)}$ to denote the **output** or *target variable.*
2. A pair ($x^{(i)}$ , $y^{(i)}$ ) is called a **training example**.

* where $i = 1,2, ..., m$ and $m$ is called as **training set**
  * Also please note that the superscript  $“(i)”$ in the notation is simply an index into the training set a.k.a number of training set, and has nothing to do with exponentiation.

3. Let us consider a function $h$, such that it takes input X and returns output, Y. <br /> i.e. $h$ = X ⮕ Y
historically  this function was named as **Hypothesis**, ($h$)  for some reason.
![hypothesis function](week-1\assets\2.PNG)

* its given by the equation:

### $h_{\theta}(x) = \theta_{0} + \theta_{1}x$

  where,

* $h_{\theta}$  is called *Hypothesis function* - **Function**
  * $\theta_{i}$ is called *Theta* - **Parameters**
  * $i$ is 1,2,3, ... ,$m$ ⭢ number of training set
  * $\theta_{0}$ is called **intercept**, i.e. the value at which the line crosses the $y$ axis
* Inorder for better results we want the difference *(gap between the data points and st. line)* to be small.

# Cost Function / Squared error function / Mean Squared error

Cost functions are used **find the best possible fit of straight line to our data.** We can measure the accuracy of our hypothesis function by using a cost function.

  i.e. to minimize $\theta_{0}$ and $\theta_{1}$ such that $(h_{\theta}(x)-y)^2$ is very minimum. *Note: punishes large errors*

### Squared error function

### $J(\theta_{0},\theta_{1})$ = $\sum_{i=1}^{m} (h_{\theta}(x^i)-y^i)^2$

* i.e. sum of (prediction - output $)^2$ should be minimum.
 $\therefore$ the cost function is given by **$J(\theta_{0},\theta_{1})$**

### Mean Squared error

### $J(\theta_{0},\theta_{1})$ = $\frac1{2m}\sum_{i=1}^{m} (h_{\theta}(x^i)-y^i)^2$

 where

* $\frac1{2m}$ is *(half the mean)* as a convenience for the computation of the gradient descent.
* mean is $\frac {sum of all numbers}{n}$

#### [<< previous](./01_part1_model_representation.md)  |  [Next >>]()
