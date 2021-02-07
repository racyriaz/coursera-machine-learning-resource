# Cost Function

## Cost Function / Squared error function / Mean Squared error

Cost functions are used **find the best possible fit of straight line to our data.** We can measure the accuracy of our hypothesis function by using a cost function.

  i.e. to minimize &theta;<sub>0</sub> and &theta;<sub>1</sub> such that (h<sub>&theta;</sub>(x)-y)<sup>2</sup> is very minimum. *Note: punishes large errors*

#### Squared error function

<!-- $J(\theta_{0},\theta_{1}) = \sum_{i=1}^{m} (h_{\theta}(x^i)-y^i)^2$ --> <img style="transform: translateY(0.1em); background: white;" src="..\svg\yqXe4yIfRG.svg">

* i.e. sum of (prediction - output $)^2$ should be minimum.
 $\therefore$ the cost function is given by **J(&theta;<sub>0</sub>,&theta;<sub>1</sub>)**

#### Mean Squared error

<!-- $J(\theta_{0},\theta_{1}) = \frac1{2m}\sum_{i=1}^{m} (h_{\theta}(x^i)-y^i)^2$ --> <img style="transform: translateY(0.1em); background: white;" src="..\svg\R8f2u2EsEZ.svg">

 where

* <!-- $\frac1{2m}$ --> <img style="transform: translateY(0.1em); background: white;" src="..\svg\REhairWRHd.svg"> is (half the mean) as a convenience for the computation of the gradient descent.
* mean is ( <sup>sum of all numbers</sup>/<sub>n</sub> )

---
### VISUALIZING COST FUNCTION

| In 2d plot with single parametric function &theta;<sub>1</sub> | In 3d plot with two parameters &theta;<sub>0</sub> and &theta;<sub>1</sub> |
|---------------------------------------------------------|--------------------------------------------------------------|
| <img src="./assets/4.png" width=auto height="250" />    | <img src="./assets/3.png" width=auto height="250">           |

* In general, we will use **contour plots** to visualize 3d plots into 2d plots.

| *(the simple working of contour plot is represented below)*        |
|--------------------------------------------------------------------|
| <img align="right" src="./assets/5.png" width=auto height="350" /> |

---
#### [<< previous](./01_part2_model_representation.md)  |  [Next >>](./02_part2_cost_function.md)
