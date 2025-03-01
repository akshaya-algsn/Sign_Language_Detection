

## Sign Language Detection

### Overview
This project implements a real-time sign language detection system using machine learning models. The system captures hand gestures via a webcam, processes them using MediaPipe, and classifies them into meaningful sign language gestures.

### Features
- Real-time sign language recognition
- Three different models for improved accuracy
- Supports video-based gesture recognition
- Optimized using TensorFlow Lite for efficient deployment
- Application in assistive technology and accessibility solutions

---

## Installation

### Prerequisites
- Python 3.x
- OpenCV
- TensorFlow
- MediaPipe
- NumPy
- Scikit-learn
- Matplotlib

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/sign-language-detection.git
   cd sign-language-detection
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

### 1. Data Collection
- Run `collect_imgs.py` to capture hand gesture images and store them in class directories.
- Extract hand keypoints using `create_dataset.py`.

### 2. Model Training
#### Model 1: SVM
- Train the SVM model using `train_classifier.py`.
- Perform inference using `inference_classifier.py`.

#### Model 2: LSTM
- Train an LSTM model with `train_lstm.py` using extracted keypoints.
- Convert the model to TensorFlow Lite for optimized deployment.

#### Model 3: LSTM for Video Sequences
- Capture and extract holistic keypoints (pose, face, hand) using `extract_keypoints.py`.
- Train an LSTM model on video sequences with `train_lstm_video.py`.
- Run real-time predictions.

---

## Results
- Achieved high accuracy in real-time sign detection.
- Successfully implemented three models with different approaches.
- Optimized model size using TensorFlow Lite.

---

## Future Enhancements
- Expand dataset to include more sign language gestures.
- Implement multilingual sign language recognition.
- Deploy as a mobile or web application for accessibility.

---



This project aims to enhance accessibility for the Deaf and hard-of-hearing community through advanced sign language recognition technology. 🚀
