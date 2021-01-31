# Cost Function Intuition II

A contour plot is a graph that contains many contour lines. A contour line of a two variable function has a constant value at all points of the same line. An example of such a graph is the one to the right below.
![cost function contour plot](./assets/6.png)

Taking any color and going along the 'circle', one would expect to get the same value of the cost function. For example, the three green points found on the green line above have the same value for J(&theta;<sub>0</sub>,&theta;<sub>1</sub>) and as a result, they are found along the same line. The circled x displays the value of the cost function for the graph on the left when &theta;<sub>0</sub> = 800, &theta;<sub>1</sub> = -0.15

Taking another h(x) and plotting its contour plot, one gets the following graphs:
![contour plot 2](./assets/7.png)

### Best fit

When &theta;<sub>0</sub> = 360 and &theta;<sub>1</sub> = 0. The value of J(&theta;<sub>0</sub>,&theta;<sub>1</sub>) in the contour plot gets closer to the center thus reducing the cost function error. Now giving our hypothesis function a slightly positive slope results in a better fit of the data.
![best fit contour plot 3](./assets/8.png)

The graph above minimizes the cost function as much as possible and consequently, the result of &theta;<sub>1</sub> and &theta;<sub>0</sub> tend to be around 0.12 and 250 respectively. Plotting those values on our graph to the right seems to put our point in the center of the inner most 'circle'.

---
#### [<< previous](./02_part1_cost_function.md)  |  [Next >>](./02_part1_cost_function.md)