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
