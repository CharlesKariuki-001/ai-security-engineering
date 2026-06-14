# Week 2 Notes – Training Loops, Neural Networks, and Gradients

## Objective

The goal of this week was to understand how Artificial Intelligence models learn from data. I learned how to build a complete training loop, train a model using gradients, create my first neural network, and understand the relationship between learning and AI security.

---

## What I Learned

### 1. How AI Learns

In Week 1, I learned that AI models operate on tensors and perform mathematical operations such as matrix multiplication.

This week answered a more important question:

**How does an AI model improve itself over time?**

The answer is through a process called **training**.

Training is the repeated process of:

1. Making predictions
2. Measuring mistakes
3. Calculating gradients
4. Updating model parameters
5. Repeating until the model improves

This cycle is the foundation of all modern machine learning and deep learning systems.

---

### 2. Understanding the Training Loop

I built a complete training loop manually using PyTorch.

The training process followed five steps:

#### Step 1: Forward Pass

The model receives input data and generates predictions.

Example:

House Size → Model → Predicted Price

At the beginning, predictions are poor because the model's parameters are random.

---

#### Step 2: Calculate Loss

Loss measures how wrong the model's predictions are.

A high loss means the model is making large mistakes.

A low loss means the model's predictions are close to the correct answers.

The goal of training is to reduce loss as much as possible.

---

#### Step 3: Backward Pass

Using:

```python
loss.backward()
```

PyTorch automatically computes gradients.

Gradients tell the model:

> "Which direction should I move my parameters to reduce the error?"

This process is called automatic differentiation (Autograd).

---

#### Step 4: Update Parameters

The model adjusts its weights and bias using the gradients.

```python
weight -= learning_rate * weight.grad
```

This moves the model slightly closer to a better solution.

---

#### Step 5: Repeat

The process repeats hundreds or thousands of times.

As training continues:

* Loss decreases
* Predictions improve
* The model learns patterns in the data

---

### 3. Weights and Bias

I learned that every AI model contains internal numbers called parameters.

The two simplest parameters are:

#### Weight

Controls how strongly an input affects the output.

#### Bias

Allows the model to shift predictions up or down.

Example:

```text
Prediction = Weight × Input + Bias
```

Training is simply the process of finding better values for these parameters.

---

### 4. Building My First Neural Network

I built my first real neural network using:

```python
class SimpleNet(nn.Module)
```

The network contained multiple layers:

```text
Input
 ↓
Layer 1 (16 neurons)
 ↓
ReLU Activation
 ↓
Layer 2 (8 neurons)
 ↓
ReLU Activation
 ↓
Output Layer
```

Unlike the simple linear model, the neural network can learn more complex patterns.

This is the same fundamental concept used in:

* ChatGPT
* Fraud detection systems
* Recommendation engines
* Computer vision systems
* Cybersecurity AI tools

The difference is that real-world systems use millions or billions of parameters.

---

### 5. Activation Functions (ReLU)

I learned about ReLU:

```python
nn.ReLU()
```

ReLU stands for:

**Rectified Linear Unit**

It introduces non-linearity into the network.

Without activation functions:

* Neural networks would behave like simple calculators.
* Deep learning would not work effectively.

ReLU allows models to learn complex relationships and patterns.

---

### 6. The Optimizer

I used the Adam optimizer:

```python
torch.optim.Adam()
```

The optimizer automates the process of updating model parameters.

Instead of manually changing weights and biases, Adam calculates efficient updates that help the model learn faster and more reliably.

The optimizer is essentially the model's learning strategy.

---

### 7. Understanding Loss Curves

I visualized training progress using a loss curve.

The loss curve shows:

```text
Training Progress
      ↓
Loss Decreases
      ↓
Model Improves
```

A decreasing loss curve is evidence that learning is occurring.

It provides a way to monitor whether training is successful.

---

### 8. Gradients and AI Security

The most important concept this week was understanding gradients.

A gradient answers the question:

> "If I change this value slightly, how will the output change?"

For training:

* Gradients help models learn.

For security:

* Gradients can help attackers manipulate model behavior.

This is the bridge between machine learning and AI security.

---

### 9. Gradient with Respect to Inputs

I calculated:

```python
x_test.grad
```

Instead of measuring how weights affect outputs, I measured how inputs affect outputs.

This revealed:

> "What input changes would most influence the model's decision?"

This concept is the foundation of:

* Adversarial attacks
* Prompt manipulation
* Input perturbation attacks
* Model evasion techniques

Future red-team exercises will build directly on this concept.

---

### 10. Saving and Loading Models

I learned how to save a trained model:

```python
torch.save()
```

and load it again:

```python
load_state_dict()
```

This is important because real AI systems must:

* Save trained models
* Deploy models
* Share models
* Restore models later

Model storage and deployment will become important security topics in later blocks.

---

## Key Takeaways

* Training is the process of reducing prediction errors.
* Loss measures how wrong a model is.
* Gradients tell the model how to improve.
* Weights and biases are the numbers a model learns.
* Neural networks are collections of layers that learn patterns from data.
* ReLU allows networks to learn complex relationships.
* Optimizers automate the learning process.
* Loss curves help visualize learning progress.
* Gradients can be used for both learning and attacking.
* Saving and loading models is essential for real-world AI deployment.

---

## Personal Reflection

Week 1 taught me what AI systems are made of.

Week 2 taught me how AI systems learn.

Before this week, training felt like a mysterious process hidden inside machine learning libraries.

Now I understand that training is simply a repeated cycle of prediction, error measurement, gradient calculation, and parameter updates.

I built a complete training loop from scratch, trained a neural network, visualized its learning process, and explored how gradients can influence both learning and security.

For the first time, I can see how a model starts with random knowledge and gradually learns patterns from data.

This week transformed my understanding of AI from static mathematical operations into a dynamic learning system.

It also introduced the first direct connection between machine learning and offensive AI security, which will become increasingly important throughout the rest of this roadmap.
