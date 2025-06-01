# 🤖 Sigmoid Function and Derivative of ReLU – Deep Learning Insights & Visualization

This project explores two foundational components in neural networks:

- **Sigmoid Activation Function**
- **Derivative of ReLU (Rectified Linear Unit)**

These concepts are key to understanding how deep learning models activate neurons and learn through backpropagation.

---

## 📘 Sigmoid Function

### 📌 Formula

\[
\sigma(x) = \frac{1}{1 + e^{-x}}
\]

### 🔍 Properties

- **Range**: (0, 1)
- **Shape**: S-shaped (sigmoid curve)
- **Use**: Outputs probabilities for binary classification
- **Smooth** and differentiable at all points

---

## 📈 Derivative of Sigmoid

### Formula

\[
\sigma'(x) = \sigma(x)(1 - \sigma(x))
\]

### Characteristics

- Peaks at \( x = 0 \)
- Gradient vanishes as \( |x| \to \infty \)
- May cause **vanishing gradients** in deep networks

---

## ⚡ ReLU Activation Function

### 📌 Formula

\[
f(x) = \max(0, x)
\]

- Introduced to address slow training due to vanishing gradients in sigmoid/tanh
- Allows fast, sparse, and effective activation

---

## 🔁 Derivative of ReLU

### Formula

\[
f'(x) =
\begin{cases}
1 & \text{if } x > 0 \\
0 & \text{if } x \leq 0
\end{cases}
\]

### Characteristics

- **Simple and efficient**
- **Discontinuous at 0**, but manageable in practice
- **No learning** for \( x \leq 0 \) (can cause dead neurons)

---

## 🔬 Comparison Summary

| Feature                  | Sigmoid Function          | Derivative of ReLU           |
|--------------------------|---------------------------|-------------------------------|
| Output Range             | (0, 1)                    | Binary gradient (0 or 1)      |
| Use Case                 | Output layer (binary)     | Hidden layers (deep networks) |
| Gradient Issue           | Vanishing at edges        | Dead neurons for \( x \leq 0 \) |
| Smoothness               | Fully smooth              | Not differentiable at 0       |
| Computation              | Slightly expensive        | Very efficient                |

---
