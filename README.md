# 🧠 Simple Neural Network with NumPy

This project demonstrates how to build **basic feedforward neural networks from scratch** using only NumPy — no machine learning libraries like TensorFlow or PyTorch involved.

It includes **two parts**:

1. A **2-layer neural network** (input → hidden → output)
2. A **1-layer neural network** (input → output)

These examples are perfect for educational purposes to understand how neural networks work under the hood.

---

## 📦 Requirements

Only one dependency is required:

```txt
numpy
```

Install with:

```bash
pip install numpy
```

---

## 📁 File Overview

```python
import numpy as np
```

* ### 🔹 Part 1: Two-Layer Neural Network

```python
X = np.array([[0, 0, 1],
              [1, 1, 1],
              [1, 0, 1],
              [0, 1, 1]])
y = np.array([[0, 1, 1, 0]]).T
```

* Input: 4 samples, each with 3 binary features
* Output: XOR-like pattern

The network architecture:

* **Input layer:** 3 neurons
* **Hidden layer:** 4 neurons
* **Output layer:** 1 neuron
* **Activation Function:** Sigmoid

Training loop runs for 6,000 iterations using basic forward and backward propagation.

---

* ### 🔹 Part 2: One-Layer Neural Network

```python
X = np.array([[0, 0, 1],
              [1, 1, 1],
              [1, 0, 1],
              [0, 1, 1]])
y = np.array([[0, 0, 1, 1]]).T
```

This version simplifies the network to just:

* **Input layer:** 3 neurons
* **Output layer:** 1 neuron
* **Activation Function:** Sigmoid

Training loop runs for 10,000 iterations.

---

## 🧮 Concepts Covered

* Forward propagation
* Sigmoid activation function and its derivative
* Backpropagation (gradient descent)
* Weight updates using error deltas
* Manual weight initialization

---

## 📤 Output

At the end of training, the model prints the output predictions for the dataset:

```bash
Output after training
[[0.00966449]
 [0.00786506]
 [0.99358911]
 [0.99337711]]
```

These values approach the target outputs `[0, 0, 1, 1]`, showing the network has learned the task.

---

## 🔧 How to Run

1. Save the script as `neural_network.py`
2. Run it with:

```bash
python neural_network.py
```

---

## 📚 Learning Resource

This project is inspired by early neural network tutorials, particularly from:

* Andrew Trask’s blog: [“A Neural Network in 11 Lines of Python”](https://iamtrask.github.io/2015/07/12/basic-python-network/)

---

## 📝 License

MIT License — feel free to modify and use for your own learning or projects.

