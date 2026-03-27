# Workshop: Gradient Descent in Single- and Multi-Layer Neural Networks

## Team Information
**Group 2**
- Ali Cihan Ozdemir (ID: 9091405)
- Lohith Reddy Danda (ID: 9054470)
*(Note: Rosetta/Roshan did not attend class and made no contributions to the project)*

## Summary of Completed Work
This repository contains the completed Jupyter Notebook for the Gradient Descent workshop. In this assignment, we:
1. **PyTorch Implementation:** Successfully implemented a manual gradient descent training loop in PyTorch, utilizing `autograd` and updating parameters properly using `torch.no_grad()`.
2. **TensorFlow Implementation:** Wrote a customized `tf.GradientTape` training loop from scratch, computing and applying gradients manually. Furthermore, we extended the baseline code to utilize mini-batch training using `tf.data.Dataset` and introduced noise to the dataset. We then plotted the loss curve over epochs to analyze optimization trajectories under stochasticity.
3. **Keras Implementations:** Trained a Sequential neural network by both compiling/fitting the model using Keras' high-level API and by defining a custom training step iteratively mapping `tape.gradient()`.
4. **Reflection Answers:** Addressed 15 conceptual and practical questions exploring learning rate characteristics, backpropagation mechanics, optimizer comparisons (SGD), and differences across three major AI frameworks: PyTorch, TensorFlow, and Keras.
