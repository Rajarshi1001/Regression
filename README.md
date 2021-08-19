# Regression Notebooks

This repo has 2 notebooks based on Linear Regression which uses two different loss function for evaluating the total loss of the model.The fit is pretty good.

The loss functions involves the predicted value from the model <code>x<sub>i</sub></code> and the actual value <code>x</code> . The loss function actually describes the amout of error between the two values and the model optimizes the loss function using the `Gradient Descent` Algorithm.

-__Linear Regression__

Equation: <code>y = mx + c</code>

1. Loss function: <code>|x - x<sub>i</sub>|<sup>1</sup></code>
```python
Iterations: 2000
Learning rate: 0.0001
The final loss for this model: -0.043649895876628514
```
2. Loss function: <code>|x - x<sub>i</sub>|<sup>3</sup></code>
```python
Iterations: 2000
Learning rate: 0.0001
The final loss for this model: -0.00038246939204274676
```

Thus the second loss function <code>|x - x<sub>i</sub>|<sup>3</sup></code> seems to perform better on the dataset generated.

-__Polynomial Regression__

Equation: <code>y = ax<sup>2</sup> + bx + c</code>

1. Loss function: <code>|x - x<sub>i</sub>|<sup>4</sup></code>
```python
Iterations: 5000
Learning rate: 0.001
The final loss for this model: 0.00043381989579868225
```
2. Loss function: <code>|x - x<sub>i</sub>|<sup>7</sup></code>
```python
Iterations: 5000
Learning rate: 0.00001
The final loss for this model: -2.1841120256905214e-07
```
Although the loss for the second model is less than the first the first model seems to fit better to the dataset.

The comparison graphs are present in the notebooks along with the loss values during each iteration in the training process.
