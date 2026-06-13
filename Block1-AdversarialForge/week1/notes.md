# Week 1 Notes – Tensors Fundamentals

## Objective

The goal of this week was to understand tensors, the fundamental building blocks of modern Artificial Intelligence systems, and learn how AI models use mathematical operations to process information and learn from data.

---

## What I Learned

### 1. What a Tensor Is

A tensor is a collection of numbers organized in one or more dimensions. Tensors are used to represent and store data inside AI systems.

Examples:

* **Scalar (0D):** A single number such as `7`
* **Vector (1D):** A list of numbers such as `[1, 2, 3, 4]`
* **Matrix (2D):** A table of numbers with rows and columns
* **3D+ Tensor:** Multiple matrices stacked together

Everything an AI model processes eventually becomes a tensor.

---

### 2. How AI Sees the World

Computers do not understand words, images, audio, or videos directly. They only understand numbers.

Examples:

* Text → Converted into numerical representations called embeddings
* Images → Converted into pixel values
* Audio → Converted into numerical waveforms
* Model parameters and weights → Stored as tensors

This means that every AI system is essentially processing tensors.

---

### 3. Tensor Operations

I learned how to perform basic operations using PyTorch:

* Creating tensors
* Viewing tensor shapes
* Reshaping tensors
* Adding tensors
* Multiplying tensors
* Matrix multiplication

These operations form the foundation of machine learning and deep learning.

---

### 4. Matrix Multiplication

Matrix multiplication is one of the most important operations in AI.

Neural networks perform matrix multiplications continuously to transform input data into useful predictions.

Examples include:

* Predicting fraud
* Recommending products
* Generating text
* Recognizing images
* Detecting cyber threats

I also implemented matrix multiplication manually to understand what happens behind the scenes instead of relying only on PyTorch.

---

### 5. Gradients and Learning

A gradient measures how much the output changes when the input changes.

Using PyTorch's automatic differentiation system (`.backward()`), I learned how gradients are calculated automatically.

Gradients are important because they allow AI models to:

* Learn from mistakes
* Update their weights
* Improve predictions over time

Without gradients, modern AI training would not be possible.

---

### 6. Connection to AI Security

Understanding tensors and gradients is essential for AI Security Engineering.

Future topics will build directly on these concepts, including:

* Adversarial attacks
* Data poisoning
* Model manipulation
* Red teaming AI systems
* Secure model deployment

Many attacks work by understanding how tensors and gradients influence a model's behavior.

---

## Key Takeaways

* AI systems operate on tensors.
* Tensors are simply numbers organized in different dimensions.
* Matrix multiplication is the engine that powers neural networks.
* Gradients tell a model how to learn and improve.
* Understanding tensors and gradients is the first step toward becoming an AI Security Engineer.
* Every modern AI system, including chatbots, recommendation systems, fraud detectors, and computer vision models, relies on tensor operations.

---

## Personal Reflection

This week changed how I think about Artificial Intelligence.

Before this week, AI felt like a black box that magically produced answers.

Now I understand that underneath every AI model are tensors, matrix multiplications, and gradients working together to process information and learn patterns.

I can now create tensors, reshape them, perform mathematical operations, implement matrix multiplication, and compute gradients using PyTorch.

This knowledge forms the mathematical foundation for the rest of my AI Security Engineering journey.
