# Features and Polynomial Regression

- We can improve our features and the form of our hypothesis function in a couple different ways.
- We can combine multiple features into one. For example, we can combine x<sub>1</sub> ​and x<sub>2</sub> ​ into a new feature x<sub>3</sub>​ by taking x<sub>1</sub>​∙ x<sub>2</sub>

### Polynomial Regression

- Our hypothesis function need not be linear (a straight line) if that does not fit the data well.
- We can change the behavior or curve of our hypothesis function by making it a quadratic, cubic or square root function (or any other form).
- For example, if our hypothesis function is <!-- $h_\theta(x) = \theta_0 + \theta_1 x_1$ --> <img style="transform: translateY(0.2em); background: white;" src="https://render.githubusercontent.com/render/math?math=h_%5Ctheta(x)%20%3D%20%5Ctheta_0%20%2B%20%5Ctheta_1%20x_1"> then we can create additional features based on x<sub>1</sub>​
  - To get the **quadratic function** <!-- $h_\theta(x) = \theta_0 + \theta_1 x_1 + \theta_2 x_1^2h$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=h_%5Ctheta(x)%20%3D%20%5Ctheta_0%20%2B%20%5Ctheta_1%20x_1%20%2B%20%5Ctheta_2%20x_1%5E2h">
  - or the **cubic function** <!-- $h_\theta(x) = \theta_0 + \theta_1 x_1 + \theta_2 x_1^2 + \theta_3 x_1^3h$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=h_%5Ctheta(x)%20%3D%20%5Ctheta_0%20%2B%20%5Ctheta_1%20x_1%20%2B%20%5Ctheta_2%20x_1%5E2%20%2B%20%5Ctheta_3%20x_1%5E3h">

- In the cubic version, we have created new features x<sub>2</sub>​ and x<sub>3</sub>​​ where <!-- $x_2 = x_1^2$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=x_2%20%3D%20x_1%5E2"> ​ and <!-- $x_3 = x_1^3$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=x_3%20%3D%20x_1%5E3">.
- To make it a square root function, we could do: <!-- $h_\theta(x) = \theta_0 + \theta_1 x_1 + \theta_2 \sqrt{x_1}$ --> <img style="transform: translateY(0.5em); background: white;" src="https://render.githubusercontent.com/render/math?math=h_%5Ctheta(x)%20%3D%20%5Ctheta_0%20%2B%20%5Ctheta_1%20x_1%20%2B%20%5Ctheta_2%20%5Csqrt%7Bx_1%7D">
- One important thing to keep in mind is, if you choose your features this way then feature scaling becomes very important. eg. if x<sub>1</sub> has range 1 - 1000 then range of <!-- $x_1^2$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=x_1%5E2">​ becomes 1 - 1000000 and that of <!-- $x_1^3$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=x_1%5E3">​ becomes 1 - 1000000000

---