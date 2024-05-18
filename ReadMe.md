# Gradient Descent Implementation 

This repository contains an implementation of the Gradient Descent algorithm using Python. It is designed to optimize functions using various configurations of learning rates, stopping criteria, and maximum iterations. The implementation leverages autograd for automatic differentiation.

## Instalation
* pip install -r requirements.txt

## Usage
* Objective function

The **objective_function** is designed to take a numpy array x and an integer alpha as inputs and return a scalar value. It ensures that the input x is at least a 2-dimensional vector and then computes a weighted sum of squares based on the alpha parameter.

* Solver

The **solver** function performs the gradient descent optimization. It takes the following parameters:

-func: The objective function to be minimized.

-x0: The initial point as a numpy array.

-params: An instance of optim_params containing the learning rate, maximum iterations, and tolerance.

-condition_toggle: A boolean to toggle the stopping condition.

-stop_toggle: A boolean to indicate if the function reached the maximum iteration limit.

The solver function returns an instance of optim_result containing the history of function values, iterations, and stopping information.

* Comparison Function

The **comparision function** sets up and runs a comparison between different configurations of the optimizer using the cec2017 benchmark functions. It prints the output of the optimization process for review.

