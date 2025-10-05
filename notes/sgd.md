# Stochastic Gradient Descent (SGD)

Stochastic Gradient Descent (SGD) is an essential optimization algorithm in machine learning used to train models efficiently, especially when dealing with large datasets. It is a variant of the standard Gradient Descent method and operates by iteratively updating model parameters (such as weights and biases) using only one randomly chosen data point or a small batch at each step instead of the entire dataset.

## How SGD Works

In each iteration, SGD computes the gradient of the loss function for a single training example or a mini-batch, and updates parameters to minimize the loss.

This randomness introduces “stochasticity,” making the algorithm faster, more scalable, and enabling it to escape poor local minima due to noisy updates.

### Basic update rule

The basic parameter update rule for SGD is:

$$
\theta = \theta - \eta \nabla_{\theta} J(\theta; x_i, y_i)
$$

where:
- $\theta$ are the model parameters,
- $\eta$ is the learning rate,
- $J$ is the loss function,
- $(x_i, y_i)$ is the current training example (or mini-batch) used to compute the gradient.

## Usage and Benefits

- Widely used for training deep neural networks and other models with large datasets.
- Efficiency comes from updating after each individual sample or mini-batch, enabling it to handle massive data and keep memory requirements low.
- Its stochastic updates help the optimizer escape shallow/local minima by introducing noise into the optimization trajectory.
- SGD forms the basis for many advanced optimizers like Adam and RMSProp, which add momentum and adaptive techniques for improved convergence.

## Applications

- Deep learning (CNNs, RNNs, transformers)
- Natural language processing
- Computer vision
- Large-scale machine learning tasks

## Summary

Stochastic Gradient Descent’s ability to scale, adapt to streaming or large datasets, and work efficiently with high-dimensional parameter spaces has made it a backbone algorithm in modern machine learning.
