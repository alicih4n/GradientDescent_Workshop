# Gradient Descent Workshop: Foundations of Neural Networks

## Overview

This workshop introduces students to **Gradient Descent**, a core
optimization algorithm used in training neural networks. Students will
explore how models learn by iteratively updating parameters to minimize
a loss function.

The workshop combines: - Mathematical intuition - Hands-on coding with
PyTorch - Implementation challenges using TensorFlow and Keras -
Reflective analysis across frameworks

------------------------------------------------------------------------

## Learning Objectives

By the end of this workshop, students will be able to:

1.  **Understand Gradient Descent**
    -   Explain gradient descent as an optimization algorithm
    -   Interpret gradients as directions of steepest ascent/descent
    -   Describe how learning rate affects convergence
2.  **Connect Math to Neural Networks**
    -   Relate loss functions to model performance
    -   Compute gradients conceptually for simple models
    -   Understand parameter updates in single- and multi-layer networks
3.  **Apply Gradient Descent in Practice**
    -   Use PyTorch to implement training loops
    -   Understand automatic differentiation (`autograd`)
    -   Visualize loss reduction over iterations
4.  **Implement Across Frameworks**
    -   Apply gradient descent using TensorFlow (`GradientTape`)
    -   Use Keras high-level APIs and custom training loops
    -   Compare abstraction levels across frameworks
5.  **Critically Reflect on ML Frameworks**
    -   Identify similarities and differences between PyTorch,
        TensorFlow, and Keras
    -   Discuss trade-offs in usability, flexibility, and control

------------------------------------------------------------------------

## Workshop Structure

### 1. Mathematical Foundations

-   Loss functions and optimization objectives

-   Gradient as slope and direction

-   Update rule:

    \[ `\theta `{=tex}:= `\theta `{=tex}-
    `\eta `{=tex}`\nabla`{=tex}\_`\theta `{=tex}L(`\theta`{=tex}) \]

-   Extension to multi-layer networks via backpropagation

------------------------------------------------------------------------

### 2. PyTorch Implementation (Guided)

Students will: - Build a simple neural network - Define a loss
function - Use PyTorch's `autograd` to compute gradients - Implement a
training loop - Observe loss decreasing over iterations

------------------------------------------------------------------------

### 3. TensorFlow & Keras Challenges (Hands-On)

Students will: - Re-implement gradient descent using TensorFlow's
`GradientTape` - Train a model using Keras `fit()` - Implement a custom
training loop in Keras - Compare implementation complexity and
flexibility

------------------------------------------------------------------------

### 4. Reflection & Discussion

Students will analyze: - How gradient descent behaves in practice - The
role of automatic differentiation - Differences between frameworks -
Trade-offs in abstraction vs control

------------------------------------------------------------------------

## Expected Student Work

Students are expected to:

-   Follow and understand provided PyTorch examples
-   Complete partially implemented TensorFlow and Keras code
-   Debug and experiment with hyperparameters (learning rate, epochs)
-   Write short reflections addressing conceptual and practical insights

------------------------------------------------------------------------

## Deliverables

Students should submit: - Completed notebook with working code - Answers
to challenge tasks - Written reflection section

------------------------------------------------------------------------

## Suggested Extensions (Optional)

-   Experiment with different optimizers (SGD vs Adam)
-   Visualize loss landscapes
-   Apply gradient descent to deeper networks

------------------------------------------------------------------------

## References

-   PyTorch Documentation: https://docs.pytorch.org
-   TensorFlow Documentation: https://www.tensorflow.org
-   CS231n (Stanford): http://cs231n.stanford.edu
-   Deep Learning Book (Goodfellow et al.)

------------------------------------------------------------------------

### ✅ 5. How to Correctly Install PyTorch

The correct installation depends on your OS, Python version, and whether you want GPU support.

Below are the **official, recommended** commands.

***

#### ✅ **1. CPU‑Only Installation (simplest)**

If you do **not** need GPU support:

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
```

***

#### ✅ **2. GPU Installation (NVIDIA CUDA)**

### First, check your CUDA version:

```bash
nvidia-smi
```

Then install the matching version, e.g.:

#### ✅ For CUDA 12.1:

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
```

#### ✅ For CUDA 11.8:

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

***

#### ✅ **3. Generic Install (lets pip choose CPU/GPU)**

```bash
pip install torch torchvision torchaudio
```

⚠️ This may be slower and sometimes fails on Windows, so prefer the index‑url commands above.

***

#### ✅ Verify Installation

Run:

```bash
python -c "import torch; print(torch.__version__, torch.cuda.is_available())"
```


