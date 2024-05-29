# Action Detection for Sign Language

![Sign Language Action Detection](docs/Images/sign_language_detection.jpg)

## Overview

The "Action Detection for Sign Language" project aims to detect sign language actions using a machine learning model based on LSTM (Long Short-Term Memory) neural networks. The implementation utilizes Python, TensorFlow, OpenCV, MediaPipe, and other libraries to preprocess data, train the model, and make predictions.

## Features

- **Video Capture**: OpenCV is used to capture video frames, enabling real-time sign language action detection from webcam or video streams.
- **LSTM Model**: The core of the project is an LSTM neural network model trained on sign language action sequences to recognize and classify different gestures and movements.
- **Preprocessing**: Data preprocessing techniques are applied to extract relevant features from video frames, such as hand gestures and movements, before feeding them into the LSTM model.
- **Real-time Prediction**: The trained model is used to make real-time predictions on incoming video streams, providing instant feedback on detected sign language actions.

## Benefits

- **Accessibility**: The project enhances accessibility for the deaf and hard of hearing community by providing a tool for real-time sign language action recognition and interpretation.
- **Education**: It can be used as an educational tool to teach sign language and raise awareness about sign language communication.
- **Communication**: Enables better communication between individuals proficient in sign language and those who are not, bridging the communication gap.
- **Research**: Contributes to research in the field of computer vision and gesture recognition, with potential applications beyond sign language, such as human-computer interaction and robotics.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/SahanNimantha99/action_detection_for_sign_language-
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Evaluation of Models

### Model Comparison

We evaluated three different models for sign language action detection: CNN (Convolutional Neural Network), RNN (Recurrent Neural Network), and LSTM (Long Short-Term Memory) networks. Each model was assessed using the following metrics: MSE (Mean Squared Error), RMSE (Root Mean Squared Error), and R values.

### Results

The LSTM model outperformed the CNN and RNN models with lower MSE and RMSE values and higher R values, indicating better accuracy and predictive performance.

## ML DevOps Integration

We integrated ML DevOps practices into our project pipeline to streamline model development, deployment, and monitoring processes. The following practices were incorporated:

- **Continuous Integration/Continuous Deployment (CI/CD)**: Automated pipelines were set up to build, test, and deploy models, ensuring rapid iteration and deployment cycles.
- **Model Monitoring**: We implemented monitoring solutions to track model performance metrics in real-time and trigger alerts for any deviations from expected behavior.
- **Version Control**: All model artifacts and code changes are version-controlled using Git, facilitating collaboration and reproducibility.
