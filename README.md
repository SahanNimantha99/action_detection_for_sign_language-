# Action Detection for Sign Language

This project aims to detect sign language actions using a machine learning model based on an LSTM neural network. The implementation utilizes Python, TensorFlow, OpenCV, MediaPipe, and other libraries to preprocess data, train the model, and make predictions.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
  - [Data Collection](#data-collection)
  - [Model Training](#model-training)
  - [Making Predictions](#making-predictions)
- [Project Structure](#project-structure)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Installation

To set up the project, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/sign-language-detection.git
    cd sign-language-detection
    ```

2. Create and activate a virtual environment (optional but recommended):
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows, use `env\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Data Collection

To collect data for training, use OpenCV and MediaPipe to capture video and extract keypoints from the sign language actions. Follow these steps:

1. **Set up the data collection script**: Modify the script `data_collection.py` to specify the actions you want to collect data for and the number of sequences.
2. **Run the script**: Execute the script to start capturing video and extracting keypoints.
    ```bash
    python data_collection.py
    ```

### Model Training

Once you have collected the data, proceed to train the LSTM model:

1. **Preprocess the data**: Ensure the data is in the correct format and split into training and validation sets. Modify and run the script `preprocess_data.py` if needed.
    ```bash
    python preprocess_data.py
    ```

2. **Train the model**: Use the script `train_model.py` to train the LSTM model on the preprocessed data.
    ```bash
    python train_model.py
    ```

3. **Evaluate the model**: After training, evaluate the model's performance using the validation set.
    ```bash
    python evaluate_model.py
    ```

### Making Predictions

Use the trained model to make predictions on new sign language actions:

1. **Load the trained model**: Use the script `predict.py` to load the model and make predictions.
    ```bash
    python predict.py
    ```

2. **Real-time predictions**: Integrate the model with a live video feed for real-time action detection.
    ```bash
    python real_time_prediction.py
    ```

## Project Structure

The project is organized as follows:

