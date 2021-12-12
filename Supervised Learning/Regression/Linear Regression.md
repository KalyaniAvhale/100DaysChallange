<h1>Linear Regression</h1>
Linear regression is one of the easiest and most popular Machine Learning algorithms. It is a statistical method that is used for predictive analysis. Linear regression makes predictions for continuous/real or numeric variables such as sales, salary, age, product price, etc.
Linear regression algorithm shows a linear relationship between a dependent (y) and one or more independent (y) variables, hence called as linear regression. Since linear regression shows the linear relationship, which means it finds how the value of the dependent variable is changing according to the value of the independent variable.
The linear regression model provides a sloped straight line representing the relationship between the variables. Consider the below image:<b><br>
  
 ![image](https://user-images.githubusercontent.com/47108982/145704624-db150d32-a0bd-4042-98cd-a72b8d765ad5.png)

  <br>Mathematically, we can represent a linear regression as: <br>
  ![image](https://user-images.githubusercontent.com/47108982/145705030-2e356c16-a6e0-4f59-8623-5a7a9b6113c2.png)
  <br>Here,

Y = Dependent Variable (Target Variable)<br>
X = Independent Variable (predictor Variable)<br>
b = intercept of the line (Gives an additional degree of freedom)<br>
m = Linear regression coefficient (scale factor to each input value).<br>

- <h3> Types of Linear Regression<br></h3>
Linear regression can be further divided into two types of the algorithm:<br>
1. Simple Linear Regression:<br>
If a single independent variable is used to predict the value of a numerical dependent variable, then such a Linear Regression algorithm is called Simple Linear Regression.
2. Multiple Linear regression:<br>
If more than one independent variable is used to predict the value of a numerical dependent variable, then such a Linear Regression algorithm is called Multiple Linear Regression.
- Finding the best fit line:</h3><br>
When working with linear regression, our main goal is to find the best fit line that means the error between predicted values and actual values should be minimized. The best fit line will have the least error.
The different values for weights or the coefficient of lines (m,c) gives a different line of regression, so we need to calculate the best values for m and c to find the best fit line, so to calculate this we use cost function.
<br><br>
  <h4> Cost function </h4>
  The different values for weights or coefficient of lines (m,c) gives the different line of regression, and the cost function is used to estimate the values of the coefficient for the best fit line.
Cost function optimizes the regression coefficients or weights. It measures how a linear regression model is performing.
We can use the cost function to find the accuracy of the mapping function, which maps the input variable to the output variable. This mapping function is also known as Hypothesis function.
For Linear Regression, we use the Mean Squared Error (MSE) cost function, which is the average of squared error occurred between the predicted values and actual values. It can be written as:
  
  ![image](https://user-images.githubusercontent.com/47108982/145704907-2b67923e-d77a-4386-b28c-64344d387577.png)
  
Where,

N=Total number of observation
Yi = Actual value
(a1xi+a0)= Predicted value.

<b>Residuals:</b> The distance between the actual value and predicted values is called residual. If the observed points are far from the regression line, then the residual will be high, and so cost function will high. If the scatter points are close to the regression line, then the residual will be small and hence the cost function.

- <h3>Gradient Descent:</h3><br>
Gradient descent is a method of updating a0 and a1 to minimize the cost function (MSE). A regression model uses gradient descent to update the coefficients of the line (a0, a1 => xi, b) by reducing the cost function by a random selection of coefficient values and then iteratively update the values to reach the minimum cost function.
<br>
![image](https://user-images.githubusercontent.com/47108982/145705223-ddc2a34f-aa55-49db-a2ba-6d04da5a919f.png)
<br>
Imagine a pit in the shape of U. You are standing at the topmost point in the pit, and your objective is to reach the bottom of the pit. There is a treasure, and you can only take a discrete number of steps to reach the bottom. If you decide to take one footstep at a time, you would eventually get to the bottom of the pit but, this would take a longer time. If you choose to take longer steps each time, you may get to sooner but, there is a chance that you could overshoot the bottom of the pit and not near the bottom. In the gradient descent algorithm, the number of steps you take is the learning rate, and this decides how fast the algorithm converges to the minima.
<br>
![image](https://user-images.githubusercontent.com/47108982/145705254-4222030c-bda9-4fac-b646-a3dc7f8d10e0.png)



- <h3>Summary</h3>
In Regression, we plot a graph between the variables which best fit the given data points. Linear regression shows the linear relationship between the independent variable (X-axis) and the dependent variable (Y-axis).To calculate best-fit line linear regression uses a traditional slope-intercept form. A regression line can be a Positive Linear Relationship or a Negative Linear Relationship.

 The goal of the linear regression algorithm is to get the best values for a0 and a1 to find the best fit line and the best fit line should have the least error. In Linear Regression, Mean Squared Error (MSE) cost function is used, which helps to figure out the best possible values for a0 and a1, which provides the best fit line for the data points. Using the MSE function, we will change the values of a0 and a1 such that the MSE value settles at the minima. Gradient descent is a method of updating a0 and a1 to minimize the cost function (MSE)
