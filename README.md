# TensorFlow: Handwritten Digit Recognition

Neural network training for handwritten digit classification (0–9).

---

## 🎯 Project Objective

The aim of this project is to train **Deep Neural Networks (DNNs)** for the classification of handwritten digits (0–9).  

---

## ⚙️ Implementation

- The **MNIST dataset** was loaded using TensorFlow.  
- Images of size **28x28 pixels** were flattened into vectors of length 784, while labels were encoded using **one-hot encoding**.  
- The initial network architecture included:  
  - An input layer with **784 neurons**  
  - Two hidden layers with **256 neurons each**, using the **tanh** activation function  
  - An output layer with **10 neurons**, using **softmax** activation  
- Training used **Stochastic Gradient Descent (SGD)** with a learning rate of `0.001`.  
- The model was trained for **10 epochs**.  
- Performance optimization was explored by varying:  
  - Number of layers  
  - Number of neurons per layer  
  - Number of epochs  
  - Learning rate  
  - Activation function  
- A dropout rate of **0.3** was applied to the hidden layers, although this did not lead to accuracy improvements.  
- For each model, both **accuracy** and **loss** were recorded during training and validation.  

---

## 📊 Results

The final model achieved an accuracy of **over 95% on the test dataset**, indicating that the neural network is highly effective for handwritten digit recognition.  

---
