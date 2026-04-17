# Task 1: Credit Scoring Model - CodeAlpha

## 📋 Project Overview
This project focuses on building a robust **Credit Scoring Model** to predict the likelihood of an applicant defaulting on a loan. By analyzing historical financial data, the model helps financial institutions make data-driven decisions, reducing risk and improving loan approval processes.

## 🎯 Objectives
* Perform comprehensive **Exploratory Data Analysis (EDA)** to understand the features.
* Preprocess the data by handling missing values and scaling numerical features.
* Compare multiple classification algorithms to find the most accurate model.
* Evaluate performance using metrics beyond simple accuracy (Precision, Recall, F1-Score).

## 🛠️ Tech Stack
* **Python 3.x**
* **Pandas & NumPy:** For data manipulation and cleaning.
* **Scikit-Learn:** For model building and evaluation.
* **Matplotlib & Seaborn:** For generating analytical graphs.

## 📊 Models Implemented
The following models were trained and compared:
1.  **Logistic Regression:** Baseline statistical model.
2.  **Decision Tree Classifier:** To capture non-linear relationships.
3.  **Random Forest Classifier:** An ensemble method used to improve accuracy and reduce overfitting.

## 📉 Visualizations Included
* **Correlation Heatmap:** To identify relationships between financial variables.
* **Model Comparison Bar Chart:** A side-by-side view of accuracy across different algorithms.
* **Confusion Matrix:** To visualize True Positives and False Positives.
* **ROC-AUC Curve:** To measure the diagnostic ability of the classifier.

## 🚀 Results
The **Random Forest Classifier** achieved the highest performance with:
* **Accuracy:** > 90%
* **ROC-AUC Score:** High discriminatory power between default and non-default cases.

## 📂 File Description
* `credit_scoring.ipynb`: The main Jupyter Notebook containing the code.
* `cs-training.csv`: The dataset used for training and testing.
* `credit_model.pkl`: The serialized version of the best-performing model.

---
**Author:** Raghav Tawri  
**Internship:** Machine Learning at CodeAlpha




# Task 2: Emotion Recognition from Speech - CodeAlpha

## 📋 Project Overview
This project involves developing a Machine Learning system capable of recognizing human emotions from speech audio signals. By analyzing vocal features such as pitch, intensity, and frequency, the model can categorize audio clips into specific emotional states like Happy, Sad, Angry, or Neutral.

## 🎯 Objectives
* Extract meaningful features from raw audio files using Signal Processing techniques.
* Build and compare multiple classifiers to identify the most effective architecture for audio data.
* Implement a robust preprocessing pipeline including resampling and normalization.
* Deploy the final model as a portable file for real-world inference.

## 🛠️ Tech Stack
* **Python 3.x**
* **Librosa:** For audio analysis and feature extraction.
* **Soundfile:** To read and write audio files.
* **Scikit-Learn:** For training the MLP, SVM, and Random Forest models.
* **Matplotlib & Seaborn:** For visualizing model performance and confusion matrices.

## 🎙️ Dataset & Feature Engineering
The model uses the **RAVDESS** (Ryerson Audio-Visual Database of Emotional Speech and Song) dataset. 
* **Feature Used:** Mel-frequency cepstral coefficients (MFCCs).
* **Process:** Audio files are loaded, resampled to 22050Hz, and converted into a 40-dimensional MFCC feature vector representing the "shape" of the sound.

## 📊 Models & Evaluation
We compared the following architectures:
1. **Multi-layer Perceptron (MLP):** A neural network approach that captures complex patterns in MFCC data.
2. **Support Vector Machine (SVM):** Effective for high-dimensional feature spaces.
3. **Random Forest:** An ensemble method for robust classification.

**Performance Metrics:** Accuracy, Precision, Recall, and F1-Score.

## 📉 Visualizations
* **Model Accuracy Comparison:** A bar chart showcasing which algorithm performed best.
* **Confusion Matrix Heatmap:** Detailing exactly which emotions were correctly identified and which were confused (e.g., Sad vs. Neutral).
* **Emotion Distribution Pie Chart:** Showing the balance of the dataset.

## 🚀 Results
The **MLP Classifier** provided the best balance of speed and accuracy, achieving a significant success rate in distinguishing between high-energy (Angry/Happy) and low-energy (Sad/Calm) emotions.

## 📂 File Description
* `emotion_recognition.ipynb`: Full implementation from extraction to evaluation.
* `emotion_recognition_model.pkl`: The serialized best-performing model.
* `README.md`: This documentation.

---
**Author:** Raghav Tawri  
**Internship:** Machine Learning at CodeAlpha



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
