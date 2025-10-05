# Xavier Initialization in Machine Learning

Xavier initialization (Glorot initialization) is a technique for initializing neural network weights to prevent vanishing and exploding gradients. It keeps the variance of activations and gradients stable across layers, enabling efficient and stable training.

---

## How Xavier Initialization Works

Xavier initialization sets initial weights based on the number of input ($n_{in}$) and output ($n_{out}$) units in a layer:

- **Uniform Xavier initialization:**
  - Weights are sampled uniformly from the range $[-x, x]$, where:
    $$
    x = \sqrt{\frac{6}{n_{in} + n_{out}}}
    $$

- **Normal Xavier initialization:**
  - Weights are sampled from a normal distribution with mean 0 and standard deviation:
    $$
    \sigma = \sqrt{\frac{2}{n_{in} + n_{out}}}
    $$

---

## Why It Matters
- Maintains the variance of activations through layers, avoiding vanishing or exploding gradients.
- Effective for activation functions like sigmoid and tanh.
- Helps gradients propagate smoothly during backpropagation, improving convergence and stability.

---

## Practical Use
- Widely used in neural network frameworks (TensorFlow, PyTorch).
- Known as Glorot Uniform (uniform) or Glorot Normal (normal) initialization in libraries.

---

## Summary
Xavier initialization is a foundational technique that balances activation and gradient variance across layers, significantly improving deep neural network training stability and efficiency.
