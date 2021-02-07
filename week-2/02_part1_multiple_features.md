# Multiple Features

### Linear regression with multiple feature is called *Multivariate Linear Regression*.
- so the notations for multiple feature will be given by,

> x<sub>*j*</sub><sup>(*i*)</sup>= value of the feature *j* in the i<sup>th</sup> column <br />
x<sup>(*i*)</sup> = the input feature of the i<sup>th</sup> training example <br />
*m* = number of  training examples <br />
*n* = number of features

- previously we know the hyperparameter, *h<sub>&theta;</sub>(x)* = &theta;<sub>0</sub> + &theta;<sub>1</sub>*X*, where we had only a single parameter, x.

- But now the hyperparameter is given by, *h<sub>&theta;</sub>(x)* = [ &theta;<sub>0</sub> &theta;<sub>1</sub> . . .  &theta;<sub>*n*</sub> ] <!-- $\begin{align*}h_\theta(x) =\begin{bmatrix}\theta_0 \hspace{2em} \theta_1 \hspace{2em} ... \hspace{2em} \theta_n\end{bmatrix}\begin{bmatrix}x_0 \newline x_1 \newline \vdots \newline x_n\end{bmatrix}= \theta^T x\end{align*}$ --> <img style="transform: translateY(0.1em); background: white;" src="..\svg\uYiZEfOKAo.svg">

i.e *hθ<sub>​(x)</sub>=θ<sub>0​</sub>+θ<sub>1​</sub>x1​+θ<sub>2</sub>​x<sub>2</sub>​+θ<sub>3</sub>​x<sub>3</sub>​+⋯+θ<sub>n</sub>​x<sub>n</sub>​*

Remark: Note that for convenience reasons in this course we assume  <br /><!-- $x_{0} (i)  =1 for (i∈1,…,m).$ --> <img style="transform: translateY(0.1em); background: white;" src="..\svg\c4Fa9Ws4G3.svg">

### Gradient Descent for Multiple Variables

- the GD for multiple variable will be the same as single variable except that it will be repeated for n features.
![Gradient Descent for multiple variables](./assets/1.png)


## Parameters to fine tune gradient descent

#### 1. Feature Scaling

- If you have multiple features in Linear Regression and they are said to be in same/similar scale. Then Gradient Descent will make *J*(&theta;), Cost Function will converge quickly. Else they will take a huge time to converge because of complex trajectories.

Lets have look on contour plots with and without Feature Scaling

##### Conture plot *without* Feature Scaling

![without feature scaling](./assets/2.png)

- Takes a huge time to get converge i.e. finding its way to global minimum
- plot is more skinnier/thin and tall.
- complicated trajectory.
- skew and elliptical shape

##### Conture plot *with* Feature Scaling

![with Feature Scaling](./assets/3.png)

- with Feature scaling implemented, the plots are more round.
- takes less time to converge, i.e. to reach global minimum (yellow point).

### Feature scaling with example.
Lets consider a house price prediction where
 - **x1** = Size(0-2000 feet <sup>2</sup>)
 - **x2** = number of bedrooms (1-5)

 the contour plot for this cost Function will look elliptical.

whereas lets implement a **simple cost Function**
where,
 - x1 = <!-- $\frac{size(feet^2)}{2000}$ --> <img style="transform: translateY(0.1em); background: white;" src="..\svg\owWwDfZPBy.svg">
 - x2 = <!-- $\frac{number of bedrooms}{5}$ --> <img style="transform: translateY(0.5em); background: white;" src="..\svg\voifrUT9m1.svg">

the contour plot will look more circular for this, since the feature are scaled between <br />*0 <= x1 <= 1*, *0 <= x2 <= 1*

# Feature Scaling

- Generally in Feature Scaling we have values ranging from <br /> -1 <= x<sub>*i*</sub> <= 1
- good ranges for Feature Scaling
  - range in 0 to 1
  - range of -1 to 1
  - range of -3 to 3
  - range of -0.01 to 0.001
  - range of -2 to 0.5
- bad ranges for Feature Scaling
  - range of -100 to 100
  - range of 0.0001 to -0.0001
  - very long range
  - very small range
- Most commonly scientists use **Mean Normalization** to scale features

### Mean Normalization
- for Mean Normalization we take a feature subtract it with the average value in the feature by the max value in the feature

SYNTAX:
  - x<sub>*i*</sub> = <!-- $\frac{Feature - Avg. value(Feature)}{Max. value - Min. value of the Feature}$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=%5Cfrac%7BFeature%20-%20Avg.%20value(Feature)%7D%7BMax.%20value%20-%20Min.%20value%20of%20the%20Feature%7D">
  - x<sub>1</sub> = (x<sub>1</sub> - &mu;<sub>1</sub>)/s

  where

  - x is Feature value
  - &mu; is Average value of feature
  - s is range of values &rarr; (max - min) / Standard Deviation


EXAMPLE:
  - x<sub>1</sub> = <!-- $\frac{size-1000}{2000}$ --> <img style="transform: translateY(0.4em); background: white;" src="https://render.githubusercontent.com/render/math?math=%5Cfrac%7Bsize-1000%7D%7B2000%7D">
  - x<sub>2</sub> = <!-- $\frac{size-2}{5}$ --> <img style="transform: translateY(0.4em); background: white;" src="https://render.githubusercontent.com/render/math?math=%5Cfrac%7Bsize-2%7D%7B5%7D">

---
#### [<< previous](./01_part1_matlab_setup.md)  |  [Next >>](./03_optimizing_GD.md)
