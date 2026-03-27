# Workshop: Gradient Descent in Single- and Multi-Layer Neural Networks

## Workshop Description
This repository serves as a profound technical exploration into the mechanics of **Gradient Descent** across modern machine learning frameworks. The primary objective of this workshop is to demystify how neural networks optimize their weights recursively by descending across a loss landscape. 

By taking a comparative approach, this workshop explores standard dataset optimization utilizing isolated math equations, and implements these structures natively across three distinct levels of API abstraction:
1. **Low-Level Native Gradients (PyTorch):** Tracking gradients with direct variable autograd tracking.
2. **Intermediate Tape Execution (TensorFlow):** Managing manual computation graphs via `tf.GradientTape`.
3. **High-Level Abstraction (Keras):** Packaging pipelines within standard API configurations (`model.fit`) alongside customized training overrides.

## Team Information
**Group 2**
- **Ali Cihan Ozdemir** (Student ID: 9091405)
- **Lohith Reddy Danda** (Student ID: 9054470)
*(Note: Roshan did not attend class and made no contributions to the project and is excluded from this document and the final submission.)*

## Summary of Completed Work
This repository contains the completed code challenges evaluating gradient workflows. Throughout this assignment, we:
1. **PyTorch Validation:** Implemented a robust computational loop utilizing autograd, successfully running isolated parameter updates directly within a `torch.no_grad()` matrix boundary.
2. **TensorFlow & Extensibility:** Computed analytical gradients recursively via `tf.GradientTape()` while extending the core logic to accommodate raw noise variations and isolated mini-batching using standard `tf.data.Dataset` pipelines. We successfully output the dynamically plotted loss curve across localized epochs.
3. **Keras Compilation:** Orchestrated predictive behavior efficiently via `keras.Sequential()` high-level compilations natively alongside building an iterative manual equivalent mapping `tape.gradient()`.
4. **Comprehensive Reflections:** Thoroughly assessed and addressed 15 distinct critical questions comparing framework tradeoffs, mathematical behavior for local linear approximations, and the tangible differences bridging single node SGD iterations.
