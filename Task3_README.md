# Task 3: Handwritten Character Recognition - CodeAlpha

## 📋 Project Overview
This project implements a **Handwritten Character Recognition** system using Deep Learning. Specifically, it focuses on identifying handwritten digits (0-9) from the globally recognized **MNIST** dataset. By utilizing Convolutional Neural Networks (CNNs), the model learns to identify patterns, strokes, and shapes to classify images with high precision.

## 🎯 Objectives
* Design and implement a Deep Learning architecture optimized for image recognition.
* Preprocess and normalize image data for faster convergence during training.
* Utilize **Convolutional Neural Networks (CNN)** to capture spatial hierarchies in pixel data.
* Evaluate the model using loss/accuracy curves and classification reports.
* Package the model for deployment using serialization techniques.

## 🛠️ Tech Stack
* **Python 3.x**
* **TensorFlow & Keras:** For building and training the Deep Learning model.
* **NumPy:** For high-performance matrix operations on image data.
* **Matplotlib & Seaborn:** For plotting training history and error analysis.

## 🧠 Model Architecture (CNN)
The model follows a structured CNN pipeline designed to minimize error:
1.  **Input Layer:** Accepts 28x28 grayscale images.
2.  **Convolutional Layers:** 32 and 64 filters to extract edges, corners, and textures.
3.  **Max-Pooling Layers:** Reduces spatial dimensions while retaining critical features.
4.  **Flatten Layer:** Converts 2D feature maps into a 1D vector.
5.  **Dense (Fully Connected) Layers:** Interprets features to make the final classification.
6.  **Dropout Layer:** Set to 0.2 to prevent overfitting and improve generalization.
7.  **Output Layer:** Softmax activation with 10 nodes (representing digits 0-9).

## 📊 Visualizations
* **Training History:** Line charts showing the decrease in Loss and increase in Accuracy over epochs.
* **Confusion Matrix Heatmap:** A detailed look at which digits the model classifies perfectly and which it occasionally confuses (e.g., 4 vs 9).
* **Per-Digit Accuracy Bar Chart:** Displays the performance consistency across all 10 classes.
* **Dataset Distribution Pie Chart:** Verifies the balance of training samples for each digit.

## 🚀 Results
The CNN model achieved an exceptional **test accuracy of over 99%**, showcasing its robustness in handling variations in handwriting styles.

## 📂 File Description
* `handwritten_recognition.ipynb`: Complete code for data loading, training, and evaluation.
* `handwritten_character_model.keras`: The saved high-performance model.
* `mnist_cnn_deployment.pkl`: Deployment package containing model architecture and weights.

---
**Author:** Raghav Tawri  
**Internship:** Machine Learning at CodeAlpha
