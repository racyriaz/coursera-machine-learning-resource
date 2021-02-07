# Multiple Features

- Linear regression with multiple feature is called *Multivariate Linear Regression*.
- so the notations for multiple feature will be given by,

> x<sub>*j*</sub><sup>(*i*)</sup>= value of the feature *j* in the i<sup>th</sup> column <br />
x<sup>(*i*)</sup> = the input feature of the i<sup>th</sup> training example <br />
*m* = number of  training examples <br />
*n* = number of features

- previously we know the hyperparameter, *h<sub>&theta;</sub>(x)* = &theta;<sub>0</sub> + &theta;<sub>1</sub>*X*, where we had only a single parameter, x.

- But now the hyperparameter is given by, *h<sub>&theta;</sub>(x)* = [ &theta;<sub>0</sub> &theta;<sub>1</sub> . . .  &theta;<sub>*n*</sub> ] <!-- $\begin{align*}h_\theta(x) =\begin{bmatrix}\theta_0 \hspace{2em} \theta_1 \hspace{2em} ... \hspace{2em} \theta_n\end{bmatrix}\begin{bmatrix}x_0 \newline x_1 \newline \vdots \newline x_n\end{bmatrix}= \theta^T x\end{align*}$ --> <img style="transform: translateY(0.1em); background: white;" src="..\svg\uYiZEfOKAo.svg">

i.e *hθ<sub>​(x)</sub>=θ<sub>0​</sub>+θ<sub>1​</sub>x1​+θ<sub>2</sub>​x<sub>2</sub>​+θ<sub>3</sub>​x<sub>3</sub>​+⋯+θ<sub>n</sub>​x<sub>n</sub>​*

Remark: Note that for convenience reasons in this course we assume  <br /><!-- $x_{0} (i)  =1 for (i∈1,…,m).$ --> <img style="transform: translateY(0.1em); background: white;" src="..\svg\c4Fa9Ws4G3.svg">