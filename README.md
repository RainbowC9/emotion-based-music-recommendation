# 🎵 Emotion-Based Music Recommendation using Speech Emotion Recognition

An AI-powered Flutter mobile application that detects a user's emotion from speech using a TensorFlow Lite model and recommends songs from predefined playlists based on the detected emotion.

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Python](https://img.shields.io/badge/Python-3.10-blue)
![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00)
![TensorFlow Lite](https://img.shields.io/badge/TensorFlow-Lite-orange)
![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00)


## 📖 Overview

Emotion-Based Music Recommendation is an AI-powered Android application that analyzes a user's speech to identify their emotional state and recommends songs from predefined playlists.

The speech emotion recognition model was trained using the **RAVDESS** and **CREMA-D** datasets in Google Colab. The trained model was converted to **TensorFlow Lite** and integrated into a Flutter mobile application, allowing emotion prediction to run directly on the device without requiring a server connection.

This project demonstrates the complete machine learning deployment pipeline, from data preprocessing and model training to mobile application integration and real-time inference.


## 🎥 Demo
https://youtube.com/shorts/RWsWnFfwoRY?feature=share


## ✨ Features

-  Record speech directly from the mobile application
-  Audio preprocessing for speech analysis
-  Speech emotion recognition using TensorFlow Lite
-  Predict user emotions in real time
-  Recommend songs from predefined playlists
-  Offline inference without requiring an internet connection
-  Fast on-device prediction


## 🔄 System Workflow

```text
User Speaks
      │
      ▼
Flutter Mobile Application
      │
      ▼
Record Audio
      │
      ▼
Audio Preprocessing
      │
      ▼
MFCC Feature Extraction
      │
      ▼
TensorFlow Lite Model
      │
      ▼
Emotion Prediction
      │
      ▼
Recommend Songs
```


## 🏗 System Architecture

The application consists of two major components:

### Model Development
- Dataset Collection
- Audio Preprocessing
- Feature Extraction
- CNN-BiLSTM Training
- Model Evaluation
- TensorFlow Lite Conversion

### Mobile Application
- Voice Recording
- Audio Processing
- TensorFlow Lite Inference
- Emotion Prediction
- Song Recommendation


## Technologies Used
| Category           | Technology            |
| ------------------ | --------------------- |
| Mobile Development | Flutter, Dart         |
| Machine Learning   | TensorFlow, Keras     |
| Deployment         | TensorFlow Lite       |
| Audio Processing   | Librosa               |
| Development        | Google Colab, VS Code |
| Dataset            | RAVDESS, CREMA-D      |
| Version Control    | Git, GitHub           |


## 📂 Dataset
This project uses two public speech emotion datasets:

### RAVDESS
Ryerson Audio-Visual Database of Emotional Speech and Song
https://zenodo.org/record/1188976

### CREMA-D
Crowd-sourced Emotional Multimodal Actors Dataset
https://github.com/CheyneyComputerScience/CREMA-D


The datasets are not included in this repository due to licensing restrictions and repository size.
Please download them from their official sources before running the project.


## 📊 Model Evaluation

### Confusion Matrix
The confusion matrix illustrates the model's classification performance across the supported emotion classes.

![Confusion Matrix](images/confusion-matrix.png)

### Classification Report
The classification report summarizes the model's Precision, Recall, F1-score, and overall Accuracy for each emotion category.

![Classification Report](images/classification-report.png)

### Training Performance
Training and validation accuracy/loss during model training using the combined RAVDESS and CREMA-D datasets.

![Training vs Validation](images/training-validation.png)

## 🧠 Model Architecture
The Speech Emotion Recognition model uses a CNN-BiLSTM architecture to learn both spatial and temporal features from extracted MFCC representations.

![CNN-BiLSTM Summary](images/cnn-bilstm-summary.png)


## 📱 Mobile Application

The home screen allows users to start the speech emotion recognition process by recording their voice.
After processing the recorded speech, the application predicts the user's emotion and recommends songs from a predefined playlist associated with the detected emotion.

| Home Screen | Emotion Prediction |
|-------------|--------------------|
| <img src="images/app-home.jpg" width="300"> | <img src="images/app-result.png" width="300"> |


## 🚀 Future Improvements

- Integrate Spotify API or other music streaming services.
- Support multilingual speech emotion recognition.
- Improve model performance using larger and more diverse datasets.
- Personalize recommendations based on user preferences.
- Add support for iOS devices.


## 🙏 Acknowledgements

This project uses the following public datasets:
- RAVDESS
- CREMA-D

Special thanks to the researchers and contributors who made these datasets publicly available.


## 📄 License
This project is licensed under the MIT License.
