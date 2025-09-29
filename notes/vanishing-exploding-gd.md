# Vanishing and Exploding Gradients

This document summarizes the key concepts from `vanishing-exploding-gd.txt` regarding vanishing and exploding gradients in deep learning.

## Vanishing Gradients
- Occur when gradients become very small during backpropagation.
- Lead to slow learning or inability to update weights in earlier layers.
- Common in deep neural networks with sigmoid or tanh activation functions.
- Solutions:
  - Use ReLU or variants.
  - Proper weight initialization (e.g., Xavier, He).
  - Batch normalization.

## Exploding Gradients
- Occur when gradients become very large during backpropagation.
- Cause unstable training and large weight updates.
- Often seen in deep or recurrent neural networks.
- Solutions:
  - Gradient clipping.
  - Careful weight initialization.
  - Use of normalization techniques.

## References
- See `xavier.md` for details on Xavier initialization.
- Further reading: Deep Learning textbooks, research papers on gradient issues.

---
*This markdown file was auto-generated from the notes in `vanishing-exploding-gd.txt`.*
